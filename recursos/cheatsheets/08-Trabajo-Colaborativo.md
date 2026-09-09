# Cheatsheet — Trabajo Colaborativo

> Referencia rápida para organizar, revisar e integrar trabajo realizado por varias personas.

---

## Flujo colaborativo

```text
Issue
  ↓
rama
  ↓
commits
  ↓
push
  ↓
Pull Request
  ↓
revisión
  ↓
correcciones
  ↓
merge
```

---

## Antes de empezar

Actualizar la rama principal:

```bash
git switch main
git pull
```

Crear una rama para la tarea:

```bash
git switch -c feature-nombre
```

---

## Issue

Usá una Issue para registrar:

```text
tarea
problema
mejora
idea
```

Una Issue debería permitir entender:

```text
qué hay que hacer
por qué
qué resultado se espera
```

---

## Una tarea, una rama

Como regla práctica:

```text
Issue
  ↓
rama específica
  ↓
trabajo relacionado
```

Ejemplos:

```text
feature-login
feature-busqueda
fix-validacion
docs-readme
```

Evitá mezclar tareas independientes en una misma rama.

---

## Commits

Registrá unidades de trabajo coherentes:

```bash
git add .
git commit -m "Implementa búsqueda de usuarios"
```

Preferí mensajes descriptivos:

```text
Agrega validación de entrada
Corrige cálculo de totales
Actualiza documentación
```

---

## Publicar el trabajo

Primera publicación:

```bash
git push -u origin feature-nombre
```

Siguientes:

```bash
git push
```

---

## Pull Request

La Pull Request permite proponer los cambios para su integración.

Debe explicar, como mínimo:

```md
## Qué hice

...

## Por qué

...

## Cómo lo probé

...
```

---

## Revisión

Antes de aprobar, comprobar:

```text
[ ] Resuelve la tarea.
[ ] El cambio es coherente.
[ ] Fue probado.
[ ] No incluye información sensible.
[ ] La documentación corresponde.
[ ] No hay problemas evidentes.
```

---

## Feedback

Un comentario útil debería explicar:

```text
qué observaste
+
por qué importa
+
qué debería revisarse
```

### Evitar

```text
Está mal.
```

### Preferir

```text
Esta validación no contempla entradas vacías.
Conviene verificarlas antes de procesar el valor.
```

---

## Solicitar cambios

Si la revisión encuentra problemas:

```text
Pull Request
     ↓
feedback
     ↓
corrección
     ↓
commit
     ↓
push
     ↓
nueva revisión
```

No hace falta crear otra Pull Request para cada corrección.

---

## Integrar

Cuando la Pull Request está aprobada:

```text
Pull Request
     ↓
merge
     ↓
main
```

Después de la integración:

```bash
git switch main
git pull
```

---

## Conflictos

Un conflicto puede aparecer cuando Git no puede integrar automáticamente cambios incompatibles.

Primero:

```bash
git status
```

Después:

```text
identificar archivos
        ↓
comprender ambos cambios
        ↓
resolver
        ↓
revisar
        ↓
probar
        ↓
continuar
```

No elijas automáticamente una versión sin analizarla.

---

## Después de resolver un conflicto

Revisá:

```bash
git status
```

Y probá el proyecto.

La resolución correcta no es solamente:

```text
"desaparecieron las marcas de conflicto"
```

También debe conservar el comportamiento esperado.

---

## Sincronización

Antes de comenzar una tarea:

```bash
git switch main
git pull
```

Después de que otra persona integre cambios, actualizá tu rama principal antes de comenzar un nuevo trabajo.

---

## Evitar trabajar directamente sobre `main`

Como regla de trabajo:

```text
main
 ↓
rama de tarea
 ↓
Pull Request
 ↓
revisión
 ↓
merge
```

Esto permite revisar los cambios antes de incorporarlos a la línea principal.

---

## No mezclar tareas

Evitá una rama como:

```text
feature-login-y-readme-y-correccion-y-diseño
```

Preferí separar:

```text
feature-login
docs-readme
fix-validacion
```

Cada una representa un propósito claro.

---

## Colaboración real

No se trata de producir:

```text
muchos commits
muchas ramas
muchas Issues
```

Se trata de organizar trabajo real.

La evidencia debería estar relacionada con:

```text
tareas
cambios
revisiones
decisiones
integraciones
```

---

## Roles durante una revisión

Quien desarrolla debe poder:

```text
explicar el cambio
```

Quien revisa debe poder:

```text
comprender el objetivo
analizar el cambio
hacer observaciones
```

La revisión es parte del trabajo, no un trámite.

---

## Checklist antes del merge

```text
[ ] Issue identificada.
[ ] Rama correcta.
[ ] Cambios completos.
[ ] Commits claros.
[ ] Pull Request descriptiva.
[ ] Revisión realizada.
[ ] Observaciones resueltas.
[ ] Proyecto probado.
[ ] Sin información sensible.
```

---

## Flujo completo

```text
                 ┌──────────────┐
                 │    Issue     │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │     Rama     │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │   Commits    │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │     Push     │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │ Pull Request │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │   Revisión   │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │    Merge     │
                 └──────┬───────┘
                        ↓
                      main
```

---

## Comandos esenciales

| Necesidad                | Comando                   |
| ------------------------ | ------------------------- |
| Actualizar `main`        | `git pull`                |
| Crear rama               | `git switch -c rama`      |
| Cambiar rama             | `git switch rama`         |
| Ver estado               | `git status`              |
| Registrar cambios        | `git add` + `git commit`  |
| Publicar rama            | `git push -u origin rama` |
| Actualizar cambios       | `git pull`                |
| Integrar rama localmente | `git merge rama`          |

---

## Regla práctica

```text
una tarea
   ↓
una rama
   ↓
cambios relacionados
   ↓
Pull Request
   ↓
revisión
   ↓
integración
```

> **Trabajar colaborativamente no significa solamente compartir un repositorio: significa hacer que el trabajo de cada persona pueda entenderse, revisarse e integrarse con el trabajo de las demás.**

