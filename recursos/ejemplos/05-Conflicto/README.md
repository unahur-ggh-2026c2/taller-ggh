# Ejemplo 05 — Conflicto

Ejemplo pequeño para provocar un conflicto durante un `merge` y resolverlo manualmente.

---

## Objetivo

Mostrar este recorrido:

```text
rama A
  ↓
cambio

rama B
  ↓
cambio sobre las mismas líneas

        ↓

merge
  ↓
conflicto
  ↓
resolución
  ↓
commit
```

---

## 1. Crear el repositorio

```bash
mkdir 05-Conflicto
cd 05-Conflicto
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
git switch -c feature-a
```

Modificar `mensaje.txt`:

```text
Versión modificada por feature A.
```

Registrar:

```bash
git add mensaje.txt
git commit -m "Modifica mensaje desde feature A"
```

---

## 3. Volver a `main`

```bash
git switch main
```

Crear otra rama desde el estado original:

```bash
git switch -c feature-b
```

Modificar la misma línea de `mensaje.txt`:

```text
Versión modificada por feature B.
```

Registrar:

```bash
git add mensaje.txt
git commit -m "Modifica mensaje desde feature B"
```

---

## 4. Integrar `feature-a`

Volver a `main`:

```bash
git switch main
```

Integrar:

```bash
git merge feature-a
```

Ahora `main` contiene el cambio de `feature-a`.

---

## 5. Intentar integrar `feature-b`

```bash
git merge feature-b
```

Git no puede decidir automáticamente qué versión conservar porque ambas ramas modificaron la misma línea.

Se producirá un conflicto.

---

## 6. Revisar el estado

```bash
git status
```

Git indicará los archivos afectados por el conflicto.

---

## 7. Abrir el archivo

`mensaje.txt` tendrá marcas similares a:

```text
<<<<<<< HEAD
Versión modificada por feature A.
=======
Versión modificada por feature B.
>>>>>>> feature-b
```

Las marcas indican las dos versiones involucradas.

---

## 8. Resolver

Decidí qué contenido debe conservar el proyecto.

Por ejemplo:

```text
Versión modificada por A y B.
```

El archivo debe quedar sin las marcas de conflicto:

```text
Versión modificada por A y B.
```

---

## 9. Revisar

Comprobar:

```bash
git status
```

Revisar el archivo y probar el proyecto.

La resolución no termina simplemente porque desaparecieron las marcas.

---

## 10. Registrar la resolución

Preparar el archivo:

```bash
git add mensaje.txt
```

Completar el merge:

```bash
git commit -m "Resuelve conflicto entre feature A y feature B"
```

---

## 11. Revisar el historial

```bash
git log --oneline --graph --all
```

La historia mostrará las dos líneas de trabajo y su integración.

---

## Resultado

El flujo fue:

```text
main
 ├── feature-a
 │      ↓
 │    cambio A
 │      ↓
 │    merge
 │
 └── feature-b
        ↓
      cambio B
        ↓
      merge
        ↓
    conflicto
        ↓
    resolución
        ↓
      commit
```

La resolución de un conflicto requiere una decisión sobre el resultado correcto del proyecto.

> **Un conflicto no es un error de Git: significa que Git necesita que una persona decida cómo combinar cambios que no puede integrar automáticamente.**

