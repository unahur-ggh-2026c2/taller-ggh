# Cheatsheet — Proyecto Final

> Referencia rápida para planificar, desarrollar, documentar y presentar el Proyecto Final.

---

## Objetivo

Demostrar que podés utilizar Git y GitHub dentro de un proceso completo de trabajo:

```text
planificar
   ↓
desarrollar
   ↓
versionar
   ↓
documentar
   ↓
revisar
   ↓
integrar
   ↓
presentar
```

---

## Definir el proyecto

Antes de comenzar:

```text
Nombre:
________________________

Problema:
________________________

Objetivo:
________________________

Usuario o destinatario:
________________________
```

---

## Definir el alcance

### Incluir

```text
- ______________________
- ______________________
- ______________________
```

### No incluir

```text
- ______________________
- ______________________
```

Definí también la **versión mínima** que permita considerar terminado el proyecto.

---

## Organizar el trabajo

Convertí el trabajo en tareas concretas.

```text
Issue
  ↓
tarea
  ↓
rama
  ↓
desarrollo
```

Una Issue debería indicar:

```text
qué problema existe
qué se quiere lograr
qué resultado se espera
```

---

## Crear el repositorio

```bash
git init
```

Agregar estructura inicial y comprobar:

```bash id="x1w2f4"
git status
```

Archivos habituales:

```text
README.md
.gitignore
src/
```

---

## Primer commit

```bash id="9o3h7d"
git add .
git commit -m "Inicializa estructura del proyecto"
```

---

## Vincular GitHub

Comprobar remoto:

```bash id="7y2v8k"
git remote -v
```

Publicar:

```bash id="m6n4pw"
git push -u origin main
```

---

## Trabajar con ramas

Para una tarea:

```bash id="q8r3ty"
git switch -c feature-nombre
```

Trabajar:

```text
cambios
  ↓
git status
  ↓
git add
  ↓
git commit
```

Publicar:

```bash id="p4x6vz"
git push -u origin feature-nombre
```

---

## Pull Request

Crear la Pull Request hacia:

```text
main
```

Descripción mínima:

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

Comprobar:

```text
[ ] Resuelve el objetivo.
[ ] El cambio es coherente.
[ ] Fue probado.
[ ] La documentación corresponde.
[ ] No contiene información sensible.
```

Si hay observaciones:

```text
revisión
  ↓
feedback
  ↓
corrección
  ↓
commit
  ↓
push
```

---

## Integración

Una vez aprobada:

```text
Pull Request
  ↓
merge
  ↓
main
```

Actualizar el repositorio local:

```bash id="v5y8kd"
git switch main
git pull
```

---

## Conflictos

Si aparece un conflicto:

```bash id="x9q3bm"
git status
```

Después:

```text
identificar
   ↓
comprender
   ↓
resolver
   ↓
revisar
   ↓
probar
```

No elijas una versión automáticamente sin comprender los cambios.

---

## README

El README final debería permitir comprender:

```text
qué es
para qué sirve
cómo instalarlo
cómo utilizarlo
qué tecnologías utiliza
```

Secciones posibles:

```text
Descripción
Objetivo
Tecnologías
Requisitos
Instalación
Uso
Ejemplo
Estructura
Estado
Próximos pasos
```

No es necesario utilizar todas.

---

## Caso de estudio

Crear:

```text
CASO-DE-ESTUDIO.md
```

Registrar:

```text
Problema
Contexto
Solución
Tecnologías
Decisiones
Dificultades
Resultado
Aprendizajes
Próximos pasos
```

---

## Documentar decisiones

Para cada decisión importante:

```text
Decisión:
________________________

Alternativas:
________________________

Elección:
________________________

Motivo:
________________________

Resultado:
________________________
```

---

## Documentar dificultades

```text
Problema:
________________________

Investigación:
________________________

Solución:
________________________

Aprendizaje:
________________________
```

Los problemas encontrados también forman parte de la historia del proyecto.

---

## Seguridad

Antes de entregar:

```text
[ ] No hay contraseñas.
[ ] No hay tokens.
[ ] No hay claves.
[ ] No hay credenciales.
[ ] No hay datos sensibles.
[ ] `.gitignore` fue revisado.
```

---

## Revisar el historial

```bash id="w7c2qs"
git log --oneline --graph --all
```

Preguntate:

```text
¿La historia permite comprender cómo evolucionó el proyecto?
¿Los commits son claros?
¿Las ramas tienen sentido?
¿Las integraciones son identificables?
```

---

## Revisar el estado

```bash id="3m5xqk"
git status
```

Antes de entregar, asegurate de conocer el estado del repositorio.

---

## Probar la documentación

Pedile a otra persona que intente utilizar el proyecto siguiendo solamente el README.

Flujo:

```text
README
  ↓
instalación
  ↓
ejecución
  ↓
resultado
```

Corregí cualquier instrucción que no permita reproducir el procedimiento.

---

## Evidencias

El proyecto debería permitir observar:

```text
trabajo
   ↓
decisiones
   ↓
cambios
   ↓
revisión
   ↓
resultado
```

Evidencias posibles:

```text
repositorio
Issues
commits
ramas
Pull Requests
README
caso de estudio
```

No se evalúa la cantidad de elementos.

Se evalúa su coherencia con el trabajo realizado.

---

## Presentación

Prepará una presentación de aproximadamente:

```text
5–10 minutos
```

Deberías poder explicar:

```text
1. Problema
2. Objetivo
3. Solución
4. Tecnologías
5. Organización
6. Git
7. GitHub
8. Dificultades
9. Resultado
10. Aprendizajes
```

---

## Checklist final

```text
[ ] Objetivo definido.
[ ] Alcance definido.
[ ] Versión mínima definida.
[ ] Repositorio disponible.
[ ] README actualizado.
[ ] .gitignore revisado.
[ ] Sin información sensible.
[ ] Tareas organizadas.
[ ] Ramas utilizadas cuando correspondía.
[ ] Commits comprensibles.
[ ] Pull Requests revisadas.
[ ] Cambios integrados.
[ ] Proyecto probado.
[ ] Documentación actualizada.
[ ] CASO-DE-ESTUDIO.md completo.
[ ] Presentación preparada.
```

---

## Flujo completo

```text
Proyecto
   ↓
Alcance
   ↓
Issue
   ↓
Rama
   ↓
Desarrollo
   ↓
Commit
   ↓
Push
   ↓
Pull Request
   ↓
Revisión
   ↓
Corrección
   ↓
Merge
   ↓
Documentación
   ↓
Prueba
   ↓
Presentación
```

---

## Comandos esenciales

| Necesidad        | Comando                           |
| ---------------- | --------------------------------- |
| Estado           | `git status`                      |
| Cambios          | `git diff`                        |
| Preparar         | `git add .`                       |
| Commit           | `git commit -m "mensaje"`         |
| Crear rama       | `git switch -c rama`              |
| Publicar rama    | `git push -u origin rama`         |
| Cambiar a `main` | `git switch main`                 |
| Actualizar       | `git pull`                        |
| Historial        | `git log --oneline --graph --all` |
| Remoto           | `git remote -v`                   |

> **El Proyecto Final no busca demostrar que sabés una lista de comandos. Busca demostrar que podés utilizar Git y GitHub para trabajar de principio a fin.**

