# Ejemplo 01 — Repositorio Mínimo

Ejemplo de un repositorio Git básico, creado desde cero.

---

## Estructura

```text
01-Repositorio-Minimo/
├── README.md
├── .gitignore
└── src/
    └── hola.txt
```

---

## 1. Crear el proyecto

Crear la carpeta:

```bash
mkdir 01-Repositorio-Minimo
cd 01-Repositorio-Minimo
```

---

## 2. Inicializar Git

```bash
git init
```

Verificar:

```bash
git status
```

---

## 3. Crear la estructura

Crear:

```text
README.md
.gitignore
src/hola.txt
```

Contenido de `src/hola.txt`:

```text
Hola, Git.
```

---

## 4. Revisar los cambios

```bash
git status
```

Los archivos nuevos aparecerán como archivos sin seguimiento.

---

## 5. Preparar los archivos

```bash
git add .
```

Comprobar:

```bash
git status
```

---

## 6. Crear el primer commit

```bash
git commit -m "Inicializa repositorio mínimo"
```

---

## 7. Verificar

Consultar el estado:

```bash
git status
```

Consultar el historial:

```bash
git log --oneline
```

Resultado esperado:

```text
<id> Inicializa repositorio mínimo
```

---

## Resultado

El proyecto ahora tiene:

```text
archivos
   ↓
repositorio Git
   ↓
primer commit
```

Todavía no hay repositorio remoto ni trabajo con GitHub.

Eso forma parte de los siguientes ejemplos.
