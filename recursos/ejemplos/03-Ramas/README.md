# Ejemplo 03 — Ramas

Ejemplo pequeño para crear una rama, realizar cambios y volver a integrarlos en `main`.

---

## Estructura

```text
03-Ramas/
├── README.md
└── mensaje.txt
```

---

## 1. Crear el repositorio

```bash
mkdir 03-Ramas
cd 03-Ramas
git init
```

Crear `mensaje.txt`:

```text
Versión inicial.
```

Registrar:

```bash
git add .
git commit -m "Inicializa proyecto"
```

---

## 2. Crear una rama

```bash
git switch -c feature-mensaje
```

Comprobar:

```bash
git branch
```

La rama actual aparecerá marcada con `*`.

---

## 3. Trabajar en la rama

Modificar `mensaje.txt`:

```text
Versión inicial.
Mensaje agregado desde una rama.
```

Registrar:

```bash
git add mensaje.txt
git commit -m "Agrega mensaje"
```

---

## 4. Volver a `main`

```bash
git switch main
```

En este punto, `main` todavía no contiene el cambio realizado en `feature-mensaje`.

Podés comprobarlo revisando `mensaje.txt`.

---

## 5. Integrar la rama

Desde `main`:

```bash
git merge feature-mensaje
```

Ahora el cambio de `feature-mensaje` forma parte de `main`.

---

## 6. Revisar el historial

```bash
git log --oneline --graph --all
```

La historia será similar a:

```text
* <id> Agrega mensaje
* <id> Inicializa proyecto
```

En este caso Git puede realizar un **fast-forward**, porque `main` no tuvo nuevos commits desde la creación de la rama.

---

## Resultado

El flujo realizado fue:

```text
main
  ↓
crear rama
  ↓
feature-mensaje
  ↓
realizar cambio
  ↓
commit
  ↓
volver a main
  ↓
merge
  ↓
main actualizado
```

La rama permitió desarrollar el cambio antes de integrarlo en la línea principal.
