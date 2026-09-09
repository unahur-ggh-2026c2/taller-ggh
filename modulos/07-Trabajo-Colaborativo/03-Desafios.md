# Desafíos
## Módulo 07 — Trabajo Colaborativo

Los desafíos de este módulo proponen situaciones abiertas de trabajo colaborativo.

A diferencia de los ejercicios, no siempre se indica qué comando utilizar ni cuál es la secuencia exacta.

La tarea consiste en:

```text
comprender el problema
        ↓
diseñar un flujo
        ↓
elegir las herramientas
        ↓
ejecutar
        ↓
verificar
        ↓
explicar las decisiones
```

---

# Desafío 1 — El primer repositorio compartido

Tenés que iniciar un proyecto que será desarrollado por varias personas.

El repositorio debe estar disponible en GitHub y cada integrante debe poder trabajar sobre él.

### Objetivo

Diseñá el procedimiento completo para que una persona nueva pueda:

1. obtener el proyecto;
2. configurar Git;
3. crear una rama;
4. realizar un cambio;
5. publicar el trabajo.

### Entregable

Documentá el procedimiento en:

```text
CONTRIBUTING.md
```

---

# Desafío 2 — La primera tarea

El equipo recibe esta necesidad:

> "El proyecto no explica cómo instalar las dependencias necesarias."

### Objetivo

Transformá la necesidad en un flujo colaborativo completo.

Deberías decidir:

- cómo registrar la tarea;
- qué nombre darle;
- qué rama crear;
- qué cambios realizar;
- cómo registrarlos;
- cómo publicarlos;
- cómo proponer su integración.

Representá el flujo:

```text
?
 ↓
?
 ↓
?
 ↓
?
 ↓
?
```

---

# Desafío 3 — La Pull Request profesional

Creaste una rama para resolver una tarea.

Ahora debés crear una Pull Request que otra persona pueda revisar sin tener que preguntarte qué hiciste.

### Objetivo

Redactá una Pull Request que contenga:

```text
Título claro
Descripción
Problema
Solución
Pruebas realizadas
Issue relacionada
```

### Reflexión

¿Qué información necesitás como revisor para poder comprender rápidamente el cambio?

---

# Desafío 4 — Revisar el trabajo de otra persona

Una compañera crea una Pull Request.

La modificación funciona, pero:

- el código es difícil de comprender;
- falta documentación;
- el título de la Pull Request es ambiguo.

### Objetivo

Realizá una revisión.

No rechaces automáticamente el cambio.

Escribí observaciones concretas y respetuosas.

### Condición

Cada observación debe indicar:

```text
qué observaste
+
por qué importa
+
qué proponés
```

---

# Desafío 5 — Cambios solicitados

Una Pull Request recibe tres observaciones.

El autor debe responderlas y modificar su trabajo.

### Objetivo

Simulá el ciclo completo:

```text
Pull Request
      ↓
revisión
      ↓
cambios solicitados
      ↓
correcciones
      ↓
commit
      ↓
push
      ↓
nueva revisión
```

### Entregable

Documentá qué cambió después de la revisión.

---

# Desafío 6 — Dos personas, una tarea

Dos personas reciben la misma tarea:

> "Mejorar la documentación de instalación."

Ambas comienzan a trabajar por separado.

### Objetivo

Diseñá una estrategia que evite que las dos personas hagan exactamente el mismo trabajo.

Considerá:

- Issue;
- asignación;
- ramas;
- comunicación;
- Pull Request.

### Reflexión

¿Qué problema se evita mediante una buena coordinación antes de comenzar a programar?

---

# Desafío 7 — Dos tareas simultáneas

Un equipo debe realizar:

```text
A — Agregar búsqueda
B — Actualizar documentación
```

### Objetivo

Diseñá un flujo donde ambas tareas puedan desarrollarse simultáneamente.

Representalo:

```text
                tarea A
               /
main ─────────
               \
                tarea B
```

Después explicá cómo deberían llegar los cambios a `main`.

---

# Desafío 8 — La rama equivocada

Una persona comienza a trabajar directamente sobre:

```text
main
```

y realiza dos commits.

Luego se da cuenta de que el cambio debería haber sido desarrollado en:

```text
feature-busqueda
```

### Objetivo

No ejecutes comandos inmediatamente.

Primero analizá:

1. ¿Qué ocurrió?
2. ¿Dónde están los commits?
3. ¿Qué información necesitás antes de modificar la historia?
4. ¿Qué alternativas existen?

La prioridad es aprender a **diagnosticar antes de actuar**.

---

# Desafío 9 — `main` modificada

Una persona está trabajando en:

```text
feature-login
```

Mientras tanto, otra persona integra cambios en:

```text
main
```

Ahora la rama de trabajo quedó basada en una versión anterior.

### Objetivo

Analizá:

```text
main
 ↓
nuevos cambios

feature-login
 ↓
trabajo basado en estado anterior
```

Respondé:

- ¿qué problema puede aparecer?
- ¿por qué podría ser necesario actualizar la rama?
- ¿qué riesgos existen al hacerlo?
- ¿qué debería verificarse después?

---

# Desafío 10 — Sincronización

Un integrante te informa:

> "GitHub tiene cambios que yo no tengo."

### Objetivo

Explicale cómo investigar la situación.

Tu explicación debe diferenciar:

```bash
git fetch
```

de:

```bash
git pull
```

No se busca memorizar una receta.

Se busca decidir qué información necesitás obtener y qué cambios querés integrar.

---

# Desafío 11 — Conflicto entre colaboradores

Dos personas modificaron la misma sección del README.

Persona A propone:

```text
## Instalación

Instalar Git y Python.
```

Persona B propone:

```text
## Instalación

Instalar Git, Python y Visual Studio Code.
```

### Objetivo

Integrar ambos trabajos de manera que el resultado final sea útil.

No elijas una versión automáticamente.

Analizá qué información aporta cada cambio.

---

# Desafío 12 — Conflicto con información incompatible

Ahora las dos personas modifican la misma información de manera incompatible.

Persona A:

```text
Versión requerida: Python 3.11
```

Persona B:

```text
Versión requerida: Python 3.13
```

### Objetivo

No resuelvas el conflicto simplemente eligiendo una versión.

Investigá dentro del proyecto cuál debería ser el requisito correcto.

### Reflexión

¿Qué diferencia existe entre:

```text
resolver técnicamente el conflicto
```

y:

```text
resolver correctamente el problema
```

---

# Desafío 13 — Pull Request bloqueada

Una Pull Request muestra:

```text
This branch has conflicts that must be resolved.
```

### Objetivo

Explicá al autor qué debería hacer.

Tu respuesta debería contemplar:

```text
analizar
 ↓
actualizar
 ↓
resolver
 ↓
probar
 ↓
publicar
 ↓
revisar nuevamente
```

No hace falta utilizar todavía estrategias avanzadas de Git.

---

# Desafío 14 — Revisor exigente

Sos responsable de revisar una Pull Request.

Encontrás:

- cambios correctos;
- un archivo modificado innecesariamente;
- un commit con mensaje poco claro;
- documentación incompleta.

### Objetivo

Decidí:

- qué observaciones realizar;
- qué cambios solicitar;
- qué cosas no deberían bloquear la integración.

### Reflexión

No todo defecto tiene necesariamente la misma importancia.

---

# Desafío 15 — Revisor demasiado exigente

Ahora imaginá el caso contrario.

Una persona revisa una Pull Request y solicita cambios por:

- una preferencia personal;
- un detalle que no afecta el funcionamiento;
- una decisión que el proyecto ya había documentado como válida.

### Objetivo

Analizá:

> ¿Cuándo una revisión ayuda al proyecto y cuándo comienza a convertirse en una barrera innecesaria?

Proponé criterios para distinguir ambos casos.

---

# Desafío 16 — Issue mal definida

Te entregan esta Issue:

```text
Título:
Arreglar cosas

Descripción:
Hay problemas. Revisar.
```

### Objetivo

Transformala en una Issue útil.

Debe permitir que otra persona comprenda:

```text
qué ocurre
por qué importa
qué resultado se espera
```

---

# Desafío 17 — Pull Request mal definida

Te entregan:

```text
Título:
Cambios varios

Descripción:
Actualicé cosas.
```

### Objetivo

Reescribila para que una persona que no participó del desarrollo pueda comprender:

- qué cambió;
- por qué;
- cómo se probó;
- qué Issue resuelve.

---

# Desafío 18 — Diseñar convenciones

Un equipo de cinco personas comienza un proyecto.

Antes de empezar a desarrollar, quieren establecer reglas.

### Objetivo

Diseñá una propuesta para:

```text
nombres de ramas
mensajes de commit
Pull Requests
revisión
Issues
protección de main
```

Documentala en:

```text
CONTRIBUTING.md
```

---

# Desafío 19 — El proyecto sin `CONTRIBUTING.md`

Un nuevo colaborador pregunta:

> "¿Cómo tengo que trabajar sobre este repositorio?"

El proyecto no tiene ninguna documentación.

### Objetivo

Diseñá un `CONTRIBUTING.md` que permita responder esa pregunta.

Debe contemplar como mínimo:

```text
1. Cómo obtener el proyecto.
2. Cómo crear una rama.
3. Cómo nombrarla.
4. Cómo realizar commits.
5. Cómo crear una Pull Request.
6. Qué debe revisarse.
```

---

# Desafío 20 — Incorporar una persona nueva

Una persona se incorpora al equipo.

No conoce el proyecto.

### Objetivo

Diseñá un recorrido de incorporación:

```text
GitHub
  ↓
clone
  ↓
documentación
  ↓
configuración
  ↓
Issue
  ↓
rama
  ↓
trabajo
  ↓
Pull Request
```

El objetivo es que la persona pueda completar una primera tarea sin depender permanentemente de otro integrante.

---

# Desafío 21 — Trabajo no publicado

Un compañero realizó:

```text
5 commits
```

pero nunca ejecutó:

```bash
git push
```

Otra persona pregunta:

> "¿Por qué no puedo revisar su trabajo?"

### Objetivo

Explicar qué ocurrió.

Diferenciá:

```text
commit local
```

de:

```text
cambio publicado
```

---

# Desafío 22 — La Pull Request que nunca termina

Una Pull Request lleva varios días abierta.

Cada vez que el revisor solicita un cambio, el autor agrega modificaciones nuevas que no están relacionadas con la tarea original.

### Objetivo

Analizá el problema.

¿Qué riesgos aparecen?

¿Qué recomendarías para recuperar el foco de la Pull Request?

---

# Desafío 23 — Una Pull Request demasiado grande

Una persona presenta una Pull Request que modifica:

```text
35 archivos
```

y contiene:

```text
20 commits
```

La tarea original era:

> "Corregir un error en la documentación."

### Objetivo

Evaluá la situación.

Respondé:

1. ¿Qué problemas puede generar?
2. ¿Por qué dificulta la revisión?
3. ¿Qué estrategia podría haberse utilizado?
4. ¿Cómo mejorarías la Pull Request?

---

# Desafío 24 — Commits difíciles de revisar

Una rama tiene estos commits:

```text
cosas
cambios
fix
ahora si
prueba
otra cosa
final
final2
```

### Objetivo

Analizá qué problemas genera esta historia.

Proponé una estrategia para mejorar los mensajes.

No hace falta reescribir la historia.

El objetivo es comprender por qué los mensajes importan.

---

# Desafío 25 — Trabajo colaborativo y trazabilidad

Un proyecto tiene:

```text
Issue #12
Pull Request #18
Commit abc123
```

### Objetivo

Explicá qué valor tiene poder relacionar:

```text
problema
   ↓
cambio
   ↓
revisión
   ↓
integración
```

¿Por qué esta trazabilidad puede resultar útil meses después?

---

# Desafío 26 — Decidir qué revisar

Una Pull Request modifica:

```text
README.md
CONTRIBUTING.md
src/
tests/
config/
```

### Objetivo

Diseñá una estrategia de revisión.

No intentes revisar todo de la misma manera.

Decidí:

- qué mirar primero;
- qué preguntas hacer;
- qué pruebas realizar;
- qué cambios podrían bloquear la integración.

---

# Desafío 27 — Protección de `main`

Un proyecto pequeño tiene cinco colaboradores.

Actualmente cualquiera puede hacer:

```bash
git push origin main
```

### Objetivo

Analizá si conviene proteger `main`.

Proponé un flujo alternativo.

Por ejemplo:

```text
rama
 ↓
Pull Request
 ↓
revisión
 ↓
merge
```

Explicá qué riesgos intenta reducir.

---

# Desafío 28 — Colaboración sin ramas

Un equipo decide que todos trabajarán directamente sobre:

```text
main
```

### Objetivo

Simulá mentalmente una semana de trabajo.

Identificá al menos cinco problemas que podrían aparecer.

Después compará con un flujo basado en ramas y Pull Requests.

---

# Desafío 29 — Elegir el flujo adecuado

Tenés tres escenarios.

### Escenario A

Proyecto personal.

### Escenario B

Dos personas trabajando en un proyecto académico.

### Escenario C

Proyecto abierto con muchos colaboradores.

### Objetivo

Proponé un nivel de formalidad diferente para cada uno.

Considerá:

- ramas;
- Pull Requests;
- revisión;
- Issues;
- protección de `main`;
- documentación.

No existe una única solución correcta.

Justificá tus decisiones.

---

# Desafío 30 — Pull Request como conversación

Una Pull Request contiene:

```text
Autor:
"Agregué la funcionalidad."

Revisor:
"¿Por qué lo hiciste de esta manera?"

Autor:
"Porque necesitábamos mantener compatibilidad."

Revisor:
"Entiendo. ¿Podrías agregar una prueba para ese caso?"

Autor:
"Sí."

```

### Objetivo

Explicá qué representa esta conversación dentro del proceso de desarrollo.

¿Por qué puede ser valiosa para el proyecto?

---

# Desafío 31 — Resolver sin culpar

Durante una revisión alguien detecta un error.

La respuesta del autor es:

> "Pero yo lo hice así porque nadie me explicó."

### Objetivo

Reformular la situación desde una perspectiva colaborativa.

¿Qué debería hacer el equipo?

Considerá:

```text
documentación
comunicación
revisión
aprendizaje
mejora del proceso
```

---

# Desafío 32 — Mejorar el proceso

Después de varios conflictos, el equipo detecta que todos modifican frecuentemente el mismo archivo.

### Objetivo

No te limites a resolver el próximo conflicto.

Proponé cambios en el proceso que puedan reducir el problema.

Considerá:

- organización;
- división de tareas;
- ramas;
- comunicación;
- estructura del proyecto;
- documentación.

---

# Desafío 33 — Trabajo colaborativo real

Trabajando con otra persona, desarrollen una funcionalidad.

### Condiciones

Cada persona debe:

- crear su propia rama;
- realizar al menos dos commits;
- publicar su rama;
- crear una Pull Request;
- revisar la Pull Request de la otra persona.

### Objetivo

Experimentar el flujo completo con dos participantes reales.

---

# Desafío 34 — Revisión cruzada

Formen parejas.

Cada integrante desarrolla una tarea diferente.

Después:

```text
Persona A → revisa B
Persona B → revisa A
```

### Condición

Cada revisión debe contener:

- una observación positiva;
- una pregunta;
- una sugerencia de mejora.

---

# Desafío 35 — Conflicto real

En parejas, partan del mismo commit.

Modifiquen deliberadamente la misma línea de un archivo.

Cada persona debe crear su commit.

Después intenten integrar ambas ramas.

### Objetivo

Generar un conflicto real y resolverlo conjuntamente.

### Reflexión

Documenten:

```text
qué hizo A
qué hizo B
por qué hubo conflicto
cómo lo resolvieron
qué aprendieron
```

---

# Desafío 36 — Proyecto colaborativo

Utilicen un repositorio común.

Cada integrante debe elegir una tarea diferente.

Por ejemplo:

```text
Persona A → documentación
Persona B → ejemplo
Persona C → configuración
```

Cada tarea debe seguir:

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
merge
```

---

# Desafío 37 — El repositorio como evidencia

Analizá un repositorio colaborativo de GitHub.

Observá:

- commits;
- ramas;
- Pull Requests;
- Issues;
- documentación.

### Objetivo

Intentá reconstruir cómo trabajó el equipo.

Respondé:

> ¿Qué podés aprender del proceso aunque no hayas participado en él?

---

# Desafío 38 — Diseñar un flujo profesional

Diseñá un flujo de trabajo para un equipo de desarrollo de cinco personas.

Debe contemplar:

```text
main
feature branches
Issues
Pull Requests
revisión
merge
```

Podés incorporar:

```text
CONTRIBUTING.md
protección de main
CODE_OF_CONDUCT.md
```

### Entregable

Un documento:

```text
docs/flujo-de-trabajo.md
```

que explique las reglas propuestas.

---

# Desafío 39 — Analizar un flujo defectuoso

Un equipo trabaja así:

```text
Issue
 ↓
main
 ↓
muchos commits
 ↓
push directo
 ↓
problemas
 ↓
conflictos
```

### Objetivo

Rediseñá el flujo.

Explicá qué cambiarías y por qué.

---

# Desafío 40 — Integrador

Realizá un flujo colaborativo completo.

### Situación

El proyecto necesita:

```text
1. Nueva funcionalidad.
2. Corrección de un error.
3. Actualización de documentación.
```

### Condiciones

Cada tarea debe:

- tener una Issue;
- utilizar una rama;
- contener al menos un commit;
- publicarse;
- pasar por una Pull Request.

Al menos una Pull Request debe recibir una observación y ser modificada antes de integrarse.

---

# Desafío 41 — Integrador con conflicto

Repetí el desafío anterior, pero agregando una condición:

Dos ramas deben modificar deliberadamente una misma parte del proyecto.

### Objetivo

Producir y resolver un conflicto.

La resolución debe quedar documentada.

---

# Desafío 42 — Integrador de equipo

En grupos, construyan un pequeño repositorio colaborativo.

Cada integrante debe asumir un rol:

```text
autor
revisor
```

Los roles pueden intercambiarse.

### El repositorio debe contener

```text
README.md
CONTRIBUTING.md
CODE_OF_CONDUCT.md
```

y al menos:

```text
3 Issues
3 ramas
3 Pull Requests
3 revisiones
3 merges
```

No se evalúa la cantidad por sí misma.

La cantidad busca generar suficientes situaciones para experimentar el flujo.

---

# Desafío 43 — Explicarlo a otra persona

Explicale a alguien que nunca trabajó colaborativamente con Git qué diferencia existe entre:

```text
trabajar solo
```

y:

```text
trabajar en equipo
```

No utilices solamente definiciones.

Utilizá un ejemplo concreto.

---

# Desafío 44 — Explicar el flujo completo

Sin consultar documentación, explicá:

```text
Issue
 ↓
Branch
 ↓
Commit
 ↓
Push
 ↓
Pull Request
 ↓
Review
 ↓
Correction
 ↓
Merge
```

Para cada etapa indicá:

```text
qué problema resuelve
```

---

# Desafío 45 — Diseñar las reglas del equipo

Imaginá que mañana comienzan a trabajar cinco personas sobre un proyecto.

Antes de escribir una sola línea de código, deben acordar reglas.

### Objetivo

Redactá una propuesta que responda:

1. ¿Cómo se nombran las ramas?
2. ¿Cómo se escriben los commits?
3. ¿Cuándo se crea una Issue?
4. ¿Cuándo se crea una Pull Request?
5. ¿Quién revisa?
6. ¿Cuándo se integra?
7. ¿Qué pasa con los conflictos?
8. ¿Qué documentación debe mantenerse?

---

# Desafío 46 — Decidir cuándo no usar Pull Request

El flujo de Pull Requests es muy útil, pero no necesariamente debe aplicarse con la misma formalidad a todos los proyectos.

Analizá:

### A

Repositorio personal.

### B

Trabajo práctico individual.

### C

Proyecto académico de cuatro integrantes.

### D

Proyecto abierto con muchos colaboradores.

### Objetivo

Proponer un nivel de formalidad adecuado para cada caso.

---

# Desafío 47 — Diagnóstico

Un integrante informa:

> "Hice `git pull` y ahora tengo conflictos."

### Objetivo

No respondas inmediatamente con comandos.

Primero preguntá:

- ¿En qué rama estaba?
- ¿Qué cambios había realizado?
- ¿Qué cambios había en remoto?
- ¿Qué archivo está en conflicto?
- ¿Qué intentaban modificar ambas partes?

Después diseñá una estrategia de resolución.

---

# Desafío 48 — Diagnóstico remoto

Una persona afirma:

> "Hice `git push`, pero GitHub me dice que no puedo subir los cambios."

### Objetivo

Enumerá posibles causas.

No hace falta resolverlas todas.

La intención es desarrollar una estrategia de diagnóstico antes de ejecutar comandos al azar.

---

# Desafío 49 — Revisar el proceso

Después de completar varios desafíos, analizá tu propio flujo de trabajo.

Respondé:

```text
¿Qué parte del proceso fue más sencilla?

¿Qué parte fue más difícil?

¿Qué errores cometí?

¿Qué aprendí de esos errores?

¿Qué regla agregaría a CONTRIBUTING.md?

¿Qué cambiaría en mi forma de trabajar?
```

---

# Desafío 50 — Desafío final

Construí un flujo colaborativo completo sobre un repositorio real.

Debe incluir:

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
cambio solicitado
   ↓
nuevo commit
   ↓
push
   ↓
nueva revisión
   ↓
merge
```

Además:

- otra persona debe participar como revisora;
- debe existir al menos un comentario de revisión;
- debe documentarse el flujo;
- debe analizarse la historia final.

Ejecutá al finalizar:

```bash
git status
git branch
git log --oneline --graph --all
```

---

# Reflexión final

Respondé sin copiar definiciones:

### 1.

¿Qué problema concreto resuelve el trabajo con ramas en un equipo?

### 2.

¿Por qué una Issue puede ser útil antes de comenzar a trabajar?

### 3.

¿Por qué una Pull Request no es simplemente "hacer merge"?

### 4.

¿Qué aporta una revisión?

### 5.

¿Por qué una Pull Request puede ser considerada una conversación técnica?

### 6.

¿Qué diferencia existe entre publicar un cambio y integrarlo?

### 7.

¿Qué aprendiste de los conflictos?

### 8.

¿Qué características debería tener una buena comunicación técnica?

### 9.

¿Qué reglas considerás indispensables para un equipo pequeño?

### 10.

¿Qué cambiarías de tu forma de trabajar después de este módulo?

---

# Criterio de resolución

Un desafío está correctamente resuelto cuando se puede explicar:

```text
qué problema existe
       ↓
qué decisión se tomó
       ↓
qué herramienta se utilizó
       ↓
qué ocurrió
       ↓
cómo se verificó
       ↓
por qué el resultado es adecuado
```

La meta no es convertir el trabajo colaborativo en una receta rígida.

La meta es desarrollar criterio para elegir un flujo adecuado para cada proyecto.

> **Una buena colaboración no consiste en que todos hagan cambios. Consiste en que los cambios de todos puedan convertirse en un proyecto coherente.**