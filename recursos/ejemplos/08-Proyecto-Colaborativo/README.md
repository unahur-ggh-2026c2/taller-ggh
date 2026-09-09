# Ejemplo 08 — Trabajo Colaborativo

Ejemplo del flujo completo de una tarea desarrollada mediante Issue, rama, commits y Pull Request.

---

## Objetivo

Simular el trabajo de una persona que recibe una tarea y la desarrolla sin modificar directamente `main`.

```text
Issue
  ↓
rama
  ↓
cambios
  ↓
commit
  ↓
push
  ↓
Pull Request
  ↓
revisión
  ↓
merge
```

---

## 1. Crear la Issue

En GitHub:

```text
Título:
Agrega mensaje de bienvenida
```

Descripción:

```md
## Objetivo

Agregar un mensaje de bienvenida a la aplicación.

## Criterios

- La aplicación debe mostrar el mensaje.
- El mensaje debe estar documentado.
```

Supongamos que GitHub asigna:

```text
Issue #12
```

---

## 2. Actualizar `main`

En el repositorio local:

```bash
git switch main
git pull
```

---

## 3. Crear una rama

```bash
git switch -c feature-mensaje-bienvenida
```

---

## 4. Realizar el cambio

Modificar el archivo correspondiente.

Por ejemplo:

```text
Hola. Bienvenido al proyecto.
```

Revisar:

```bash
git status
git diff
```

---

## 5. Crear el commit

```bash
git add .
git commit -m "Agrega mensaje de bienvenida"
```

---

## 6. Publicar la rama

```bash
git push -u origin feature-mensaje-bienvenida
```

---

## 7. Crear la Pull Request

En GitHub:

```text
feature-mensaje-bienvenida
            ↓
       Pull Request
            ↓
           main
```

Título:

```text
Agrega mensaje de bienvenida
```

Descripción:

```md
## Relacionado con

Issue #12

## Qué hice

Agregué el mensaje de bienvenida solicitado.

## Cómo lo probé

Ejecuté la aplicación y verifiqué que el mensaje aparezca correctamente.
```

---

## 8. Revisar

La persona que revisa puede comprobar:

```text
[ ] La Issue está resuelta.
[ ] El cambio cumple el objetivo.
[ ] El mensaje aparece correctamente.
[ ] No hay cambios innecesarios.
[ ] La descripción de la Pull Request es clara.
```

---

## 9. Simular una corrección

Supongamos que la revisión solicita:

```text
"El mensaje debería incluir el nombre del proyecto."
```

Modificar:

```text
Hola. Bienvenido al proyecto Gestor de Tareas.
```

Registrar:

```bash
git add .
git commit -m "Mejora mensaje de bienvenida"
git push
```

La Pull Request se actualiza automáticamente.

---

## 10. Integrar

Una vez aprobada:

```text
Pull Request
     ↓
merge
     ↓
main
```

---

## 11. Actualizar el repositorio local

```bash
git switch main
git pull
```

Comprobar:

```bash
git status
```

---

## Resultado

La tarea dejó trazabilidad en:

```text
Issue #12
    ↓
feature-mensaje-bienvenida
    ↓
commit
    ↓
Pull Request
    ↓
revisión
    ↓
corrección
    ↓
merge
    ↓
main
```

La Issue explica **qué había que hacer**.

Los commits muestran **qué cambios se realizaron**.

La Pull Request permite **revisar el trabajo**.

El merge incorpora el resultado a `main`.

---

## Variante con dos personas

El mismo flujo puede utilizarse cuando participan varias personas:

```text
              ┌── feature-login ─────┐
              │                       ↓
main ─────────┼───────────────────── merge
              │
              └── feature-readme ────┘
```

Cada persona puede trabajar en su propia rama y proponer sus cambios mediante una Pull Request.

> **La colaboración funciona mejor cuando cada tarea tiene un propósito claro y existe un recorrido visible desde la necesidad hasta la integración.**
