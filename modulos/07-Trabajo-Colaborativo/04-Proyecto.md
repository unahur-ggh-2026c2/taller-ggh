# Proyecto
## Módulo 07 — Trabajo Colaborativo

---

## 1. Propósito

En este proyecto vamos a integrar los conocimientos desarrollados durante el módulo para simular un flujo de trabajo colaborativo sobre un repositorio Git y GitHub.

La propuesta no consiste en desarrollar una aplicación compleja.

El objetivo es construir y gestionar un pequeño proyecto de manera organizada, aplicando:

```text
Issues
   ↓
ramas
   ↓
commits
   ↓
push
   ↓
Pull Requests
   ↓
revisión
   ↓
correcciones
   ↓
merge
```

El resultado más importante no será solamente el contenido producido.

Será la **historia de colaboración que quede registrada en el repositorio**.

---

# 2. Situación

Formás parte de un pequeño equipo que debe mantener y mejorar un proyecto compartido.

El equipo necesita incorporar diferentes cambios al proyecto sin trabajar directamente sobre `main`.

Cada integrante deberá asumir responsabilidades concretas y utilizar GitHub como espacio de coordinación.

El proyecto puede ser:

- un pequeño programa;
- un repositorio de documentación;
- un conjunto de ejemplos;
- material educativo;
- una colección de recursos;
- otro proyecto acordado con el docente.

No se evalúa la complejidad del software.

Se evalúa la calidad del proceso colaborativo.

---

# 3. Objetivo general

Aplicar un flujo de trabajo colaborativo completo utilizando Git y GitHub.

Al finalizar el proyecto debería poder observarse:

```text
problema
   ↓
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
corrección
   ↓
nueva revisión
   ↓
merge
   ↓
main
```

---

# 4. Modalidad

El proyecto puede realizarse:

### En equipo

Es la modalidad recomendada.

Cada integrante trabaja sobre una tarea diferente y participa también en la revisión del trabajo de otras personas.

### Individual

Puede realizarse simulando diferentes roles.

En este caso, el estudiante deberá crear diferentes ramas y reproducir el flujo colaborativo de manera controlada.

La modalidad puede adaptarse sin modificar los objetivos del proyecto.

---

# 5. Organización del equipo

Para la modalidad grupal se recomienda trabajar con:

```text
2 a 4 integrantes
```

Cada integrante deberá tener acceso al repositorio.

El equipo debe definir:

- quién participa;
- qué tarea realiza cada persona;
- cómo se nombran las ramas;
- cómo se escriben los commits;
- cómo se realizan las revisiones.

Estas decisiones deben quedar documentadas.

---

# 6. Repositorio

El proyecto debe utilizar un repositorio GitHub.

El repositorio deberá contener como mínimo:

```text
README.md
CONTRIBUTING.md
```

Opcionalmente puede incluir:

```text
CODE_OF_CONDUCT.md
```

y los archivos propios del proyecto.

---

# 7. README.md

El `README.md` debe explicar:

- qué es el proyecto;
- cuál es su objetivo;
- cómo utilizarlo;
- cómo participar;
- dónde encontrar información relevante.

No es necesario escribir una documentación extensa.

Debe ser suficiente para que una persona nueva pueda comprender el propósito general del repositorio.

---

# 8. CONTRIBUTING.md

El archivo:

```text
CONTRIBUTING.md
```

debe documentar las reglas básicas de colaboración.

Como mínimo debe indicar:

```text
cómo crear una rama
cómo nombrar una rama
cómo realizar commits
cómo publicar cambios
cómo crear una Pull Request
cómo realizar una revisión
```

También puede incluir reglas adicionales definidas por el equipo.

---

# 9. CODE_OF_CONDUCT.md

Este archivo es opcional.

Si el equipo decide incorporarlo, debe establecer pautas básicas para la participación y comunicación dentro del proyecto.

No se busca elaborar un documento jurídico.

El objetivo es comprender el papel que puede cumplir este tipo de documentación en un proyecto colaborativo.

---

# 10. Definir las tareas

Antes de comenzar el trabajo, el equipo debe identificar al menos:

```text
3 tareas
```

Las tareas deben ser suficientemente independientes para permitir el trabajo paralelo.

Ejemplo:

```text
Issue #1
Actualizar documentación

Issue #2
Agregar nuevo ejemplo

Issue #3
Mejorar instalación
```

---

# 11. Crear las Issues

Cada tarea debe convertirse en una Issue.

Cada Issue debería contener:

```text
Título
Descripción
Objetivo
Resultado esperado
```

Evitar títulos como:

```text
Cambios
Mejoras
Cosas
Arreglar
```

Las Issues deben permitir comprender qué trabajo se espera realizar.

---

# 12. Asignación

Cada tarea debe tener una persona responsable.

Por ejemplo:

```text
Issue #1 → Persona A
Issue #2 → Persona B
Issue #3 → Persona C
```

Esto evita que dos personas comiencen accidentalmente a resolver la misma tarea.

---

# 13. Crear las ramas

Cada tarea debe desarrollarse en una rama independiente.

Ejemplo:

```text
main
 ├── docs-instalacion
 ├── nuevo-ejemplo
 └── mejora-readme
```

Las ramas deben tener nombres claros y relacionados con su propósito.

---

# 14. Primera etapa — Trabajo individual

Cada integrante debe trabajar exclusivamente sobre su rama.

Para cada tarea:

```text
Issue
  ↓
rama
  ↓
modificaciones
  ↓
commit
```

No se debe modificar directamente `main`.

---

# 15. Commits

Cada integrante debe realizar como mínimo:

```text
2 commits
```

Los commits deben representar avances comprensibles.

Evitar mensajes como:

```text
cambios
cosas
fix
prueba
final
```

Preferir mensajes que indiquen qué se hizo.

Por ejemplo:

```text
Agrega instrucciones de instalación
```

o:

```text
Incorpora ejemplo de búsqueda
```

---

# 16. Revisar antes de publicar

Antes de ejecutar:

```bash
git push
```

cada integrante debe revisar:

```bash
git status
```

y:

```bash
git diff
```

El objetivo es comprobar qué cambios están siendo publicados.

---

# 17. Publicar las ramas

Cada integrante debe publicar su rama:

```bash
git push -u origin nombre-rama
```

Al finalizar, las ramas deberían estar disponibles en GitHub.

---

# 18. Segunda etapa — Pull Requests

Cada integrante debe crear una Pull Request.

El destino será:

```text
main
```

El origen será la rama correspondiente a la tarea.

Por ejemplo:

```text
nuevo-ejemplo
      ↓
Pull Request
      ↓
main
```

---

# 19. Descripción de la Pull Request

Cada Pull Request debe contener como mínimo:

```md
## Qué hice

Descripción de los cambios.

## Por qué

Explicación del problema que se quería resolver.

## Cómo lo probé

Descripción de las verificaciones realizadas.

## Issue

Referencia a la Issue correspondiente.
```

La descripción debe permitir comprender el cambio sin revisar primero todos los archivos.

---

# 20. Tercera etapa — Revisión cruzada

Ninguna persona debería revisar solamente su propio trabajo.

Cada integrante debe revisar al menos una Pull Request de otra persona.

Ejemplo:

```text
Persona A → revisa B
Persona B → revisa C
Persona C → revisa A
```

Si solamente participan dos personas:

```text
Persona A ↔ Persona B
```

---

# 21. Qué debe revisarse

Durante la revisión se debe observar:

### Objetivo

¿La Pull Request resuelve la tarea?

### Alcance

¿Modifica solamente lo necesario?

### Claridad

¿Los cambios son comprensibles?

### Documentación

¿La documentación está actualizada?

### Calidad

¿Existe algún problema evidente?

### Pruebas

¿Se verificó el resultado?

---

# 22. Comentarios de revisión

Cada integrante debe realizar al menos:

```text
1 comentario de revisión
```

El comentario debe ser concreto.

Debe explicar:

```text
qué observaste
+
por qué importa
+
qué proponés
```

No se aceptan como única evidencia comentarios como:

```text
Está bien.
```

o:

```text
No me gusta.
```

---

# 23. Cuarta etapa — Cambio solicitado

Al menos una Pull Request del proyecto deberá recibir una observación que implique una modificación.

Por ejemplo:

> "La documentación explica cómo instalar el proyecto, pero falta indicar los requisitos previos."

El autor deberá incorporar la corrección.

---

# 24. Realizar la corrección

El autor vuelve a su rama:

```bash
git switch nombre-rama
```

Realiza el cambio.

Después:

```bash
git add .
git commit -m "Completa requisitos de instalación"
```

y:

```bash
git push
```

---

# 25. La Pull Request se actualiza

No es necesario crear una nueva Pull Request.

La misma Pull Request debe incorporar el nuevo commit.

El flujo es:

```text
Pull Request
      ↓
revisión
      ↓
cambio solicitado
      ↓
commit
      ↓
push
      ↓
Pull Request actualizada
```

---

# 26. Nueva revisión

El revisor debe volver a analizar el cambio.

Debe verificar que la observación haya sido atendida.

Si está correcto:

```text
Approved
```

Si todavía existe un problema:

```text
Request changes
```

El objetivo es experimentar el ciclo real de revisión.

---

# 27. Quinta etapa — Integración

Una vez revisada y aprobada una Pull Request, debe integrarse en:

```text
main
```

El equipo puede utilizar el mecanismo de merge disponible en GitHub.

Después de integrar:

```text
rama
  ↓
main
```

---

# 28. Actualizar el repositorio local

Después de la integración, cada integrante debe actualizar su copia local.

Por ejemplo:

```bash
git switch main
git pull
```

Después comprobar:

```bash
git status
```

---

# 29. Analizar la historia

Ejecutar:

```bash
git log --oneline --graph --all
```

El equipo debe observar la historia resultante.

Intenten identificar:

```text
commits de cada tarea
ramas
integraciones
```

---

# 30. Evidencia del trabajo

El repositorio debe conservar evidencia suficiente del proceso.

Debe ser posible identificar:

```text
Issues
Pull Requests
commits
ramas
revisiones
integraciones
```

No se debe eliminar deliberadamente la evidencia necesaria para comprender cómo se desarrolló el proyecto.

---

# 31. Sexta etapa — Conflicto controlado

El equipo deberá provocar deliberadamente un conflicto.

Dos ramas deberán modificar una misma parte del proyecto.

Por ejemplo:

```text
feature-a
    \
     \ 
      main
     /
    /
feature-b
```

Ambas ramas deberán modificar una misma línea o sección.

---

# 32. Resolver el conflicto

El conflicto deberá resolverse de manera consciente.

No se debe seleccionar una versión automáticamente sin analizarla.

El equipo debe determinar:

```text
qué intentaba hacer cada rama
        ↓
qué información aporta cada cambio
        ↓
qué resultado necesita el proyecto
        ↓
qué versión final corresponde
```

---

# 33. Documentar el conflicto

El equipo debe registrar brevemente:

```text
Qué cambios entraron en conflicto.

Por qué Git no pudo resolverlos automáticamente.

Qué decisión tomó el equipo.

Por qué esa decisión fue adecuada.
```

Esta documentación puede incorporarse a la entrega final.

---

# 34. Reglas mínimas del proyecto

El equipo deberá establecer al menos estas reglas:

### Regla 1

No trabajar directamente sobre:

```text
main
```

### Regla 2

Cada tarea debe tener una rama.

### Regla 3

Los cambios deben publicarse mediante Pull Request.

### Regla 4

Las Pull Requests deben ser revisadas.

### Regla 5

Los commits deben tener mensajes claros.

---

# 35. Reglas adicionales

El equipo puede establecer otras reglas.

Por ejemplo:

```text
Las ramas deben comenzar con feature-, fix- o docs-.

Toda Pull Request debe explicar cómo se probó el cambio.

Toda Pull Request debe tener al menos una revisión.

Las Issues deben describir claramente el resultado esperado.
```

Estas reglas deben quedar documentadas en:

```text
CONTRIBUTING.md
```

---

# 36. Estructura esperada

El repositorio final debería tener una estructura similar a:

```text
proyecto/
│
├── README.md
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
│
├── ...
│
└── recursos/
```

La estructura concreta dependerá del proyecto elegido.

---

# 37. Requisitos mínimos

Para aprobar el proyecto deberían cumplirse como mínimo:

### Repositorio

- repositorio disponible en GitHub;
- README funcional;
- CONTRIBUTING.md.

### Issues

- al menos 3 Issues.

### Ramas

- al menos 3 ramas de trabajo.

### Commits

- al menos 2 commits por tarea.

### Pull Requests

- al menos 3 Pull Requests.

### Revisiones

- al menos una revisión por Pull Request;
- al menos una Pull Request con cambios solicitados.

### Integración

- Pull Requests integradas en `main`.

### Conflicto

- al menos un conflicto provocado y resuelto conscientemente.

---

# 38. Flujo esperado

El flujo general del proyecto debe ser:

```text
                 Issue
                   ↓
             crear rama
                   ↓
                trabajo
                   ↓
               commits
                   ↓
                 push
                   ↓
            Pull Request
                   ↓
                revisión
                   ↓
          ┌────────┴────────┐
          │                 │
      corrección         aprobación
          │                 │
        commit              │
          │                 │
         push               │
          │                 │
          └───────┬─────────┘
                  ↓
                merge
                  ↓
                 main
```

---

# 39. Entrega

La entrega principal es el repositorio GitHub.

Debe poder observarse el proceso completo.

Además, el equipo deberá entregar un documento breve:

```text
INFORME.md
```

---

# 40. Contenido de `INFORME.md`

El informe debe contener:

```md
# Informe del proyecto

## Integrantes

...

## Proyecto

...

## Organización del trabajo

...

## Issues realizadas

...

## Pull Requests

...

## Revisiones

...

## Conflicto resuelto

...

## Decisiones tomadas

...

## Dificultades

...

## Aprendizajes

...
```

No se busca un informe académico extenso.

Debe servir para explicar cómo trabajó el equipo.

---

# 41. Evidencias

El repositorio debe permitir verificar:

```text
Issue
 ↓
rama
 ↓
commits
 ↓
Pull Request
 ↓
review
 ↓
corrección
 ↓
merge
```

Las capturas de pantalla pueden utilizarse como complemento, pero no deberían reemplazar la evidencia existente en GitHub.

---

# 42. Presentación

Si el proyecto se realiza en modalidad presencial, el equipo puede presentar brevemente:

1. qué proyecto desarrolló;
2. cómo organizó las tareas;
3. qué flujo utilizó;
4. qué Pull Request fue revisada;
5. qué conflicto resolvió;
6. qué aprendió del proceso.

La presentación debe centrarse en las decisiones tomadas.

---

# 43. Preguntas para la presentación

El docente puede utilizar preguntas como:

> ¿Por qué eligieron esos nombres de ramas?

> ¿Qué problema representaba cada Issue?

> ¿Cómo decidieron quién revisaba cada Pull Request?

> ¿Qué cambio solicitaron durante una revisión?

> ¿Qué ocurrió con la Pull Request después de realizar la corrección?

> ¿Cómo resolvieron el conflicto?

> ¿Por qué eligieron ese resultado?

> ¿Qué cambiarían del proceso si volvieran a comenzar?

---

# 44. Evaluación

La evaluación tendrá en cuenta cuatro dimensiones.

## 1. Uso de Git

Se evaluará:

- creación de ramas;
- commits;
- publicación;
- sincronización;
- análisis del historial.

## 2. Uso de GitHub

Se evaluará:

- Issues;
- Pull Requests;
- revisiones;
- integración;
- documentación.

## 3. Trabajo colaborativo

Se evaluará:

- organización;
- comunicación;
- distribución de tareas;
- calidad de las revisiones;
- capacidad para resolver conflictos.

## 4. Comprensión

Se evaluará la capacidad para explicar:

```text
qué se hizo
por qué se hizo
cómo se hizo
qué problemas aparecieron
cómo se resolvieron
```

---

# 45. No se evalúa solamente el resultado

Un proyecto puede terminar funcionando y, sin embargo, presentar un proceso deficiente.

Por ejemplo:

```text
todo directamente sobre main
```

o:

```text
una sola Pull Request enorme
```

o:

```text
commits sin significado
```

o:

```text
ninguna revisión
```

En este proyecto importa tanto:

```text
resultado
```

como:

```text
proceso
```

---

# 46. Criterios de calidad

Un proyecto de calidad debería mostrar:

```text
Issues claras
      +
ramas con propósito
      +
commits comprensibles
      +
Pull Requests enfocadas
      +
revisiones útiles
      +
correcciones
      +
integraciones controladas
      +
historia comprensible
```

---

# 47. Reflexión individual

Cada integrante deberá responder:

### 1.

¿Qué aprendí sobre trabajar con otras personas utilizando Git?

### 2.

¿Qué diferencia encontré entre trabajar solo y trabajar en equipo?

### 3.

¿Qué problema me resultó más difícil?

### 4.

¿Qué aprendí al revisar el trabajo de otra persona?

### 5.

¿Qué aprendí al recibir una revisión?

### 6.

¿Cómo resolvimos el conflicto?

### 7.

¿Qué regla del equipo resultó más útil?

### 8.

¿Qué cambiaría del flujo utilizado?

---

# 48. Reflexión final del equipo

Como equipo, respondan:

> ¿Qué haríamos diferente si este repositorio tuviera veinte colaboradores en lugar de tres?

Consideren:

- protección de `main`;
- revisión;
- Issues;
- convenciones;
- documentación;
- automatización;
- organización del trabajo.

No es necesario implementar todas las respuestas.

El objetivo es comenzar a pensar cómo escala un proceso colaborativo.

---

# 49. Producto final esperado

Al finalizar, el repositorio debería contar una historia.

Una persona externa debería poder observar:

```text
Había una necesidad
        ↓
se creó una Issue
        ↓
alguien trabajó en una rama
        ↓
registró cambios
        ↓
publicó el trabajo
        ↓
propuso una Pull Request
        ↓
otra persona revisó
        ↓
se realizaron correcciones
        ↓
el cambio fue aprobado
        ↓
se integró
```

Esa historia es el verdadero producto del proyecto.

---

# 50. Cierre

Este proyecto representa el paso desde:

```text
"sé usar Git"
```

hacia:

```text
"sé trabajar con otras personas utilizando Git".
```

La diferencia no está solamente en conocer más comandos.

Está en comprender un proceso:

```text
organizar
   ↓
trabajar
   ↓
registrar
   ↓
publicar
   ↓
revisar
   ↓
comunicar
   ↓
corregir
   ↓
integrar
```

El objetivo final es que puedas incorporarte a un proyecto real y comprender qué se espera de vos cuando te dicen:

> **"Creá una rama, resolvé la Issue, abrí una Pull Request y pedí revisión."**

Y que puedas hacerlo sabiendo no solamente **qué comandos ejecutar**, sino **por qué ese flujo existe y qué problema resuelve cada etapa**.