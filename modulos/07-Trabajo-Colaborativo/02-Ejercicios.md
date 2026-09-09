# Ejercicios
## Módulo 07 — Trabajo Colaborativo

Estos ejercicios buscan consolidar los conceptos fundamentales del trabajo colaborativo con Git y GitHub.

La intención es avanzar desde situaciones simples hacia escenarios donde sea necesario tomar decisiones sobre ramas, sincronización, revisión e integración.

No se busca solamente ejecutar comandos.

En cada ejercicio intentá seguir este proceso:

```text
comprender
    ↓
anticipar
    ↓
ejecutar
    ↓
verificar
    ↓
explicar
```

---

# Ejercicio 1 — Git y GitHub

Explicá con tus palabras la diferencia entre:

```text
Git
```

y:

```text
GitHub
```

Después completá:

```text
Git permite ______________________________

GitHub permite ___________________________
```

---

# Ejercicio 2 — Repositorio compartido

Imaginá:

```text
              GitHub
                 │
        ┌────────┼────────┐
        │        │        │
     Persona A Persona B Persona C
```

Respondé:

1. ¿Qué tiene en común cada persona?
2. ¿Qué tiene cada persona localmente?
3. ¿Por qué el repositorio remoto resulta útil?
4. ¿Qué podría ocurrir si todas las personas modificaran directamente `main`?

---

# Ejercicio 3 — Clonar

Tenés un repositorio disponible en GitHub.

¿Qué comando utilizarías para obtener una copia local?

Explicá qué representa:

```text
repositorio remoto
        ↓
       clone
        ↓
repositorio local
```

---

# Ejercicio 4 — Identidad

¿Por qué Git necesita conocer información como:

```bash
git config --global user.name
git config --global user.email
```

¿Qué relación tiene esta información con los commits?

---

# Ejercicio 5 — Crear una tarea

Imaginá un proyecto que necesita:

> Agregar instrucciones de instalación.

Redactá una Issue adecuada.

Debe contener:

```text
Título
Descripción
Objetivo
```

Evitá títulos demasiado genéricos como:

```text
Cambios
Problema
Instalación
```

---

# Ejercicio 6 — Issue o Pull Request

Indicá cuál utilizarías en cada situación.

### A

> "El README no explica cómo instalar el proyecto."

### B

> "Ya realicé los cambios para corregir el README y quiero que los revisen."

### C

> "Sería conveniente agregar ejemplos de uso."

### D

> "Tengo una rama con la solución y quiero incorporarla a `main`."

Justificá cada respuesta.

---

# Ejercicio 7 — Issue y rama

Partimos de:

```text
Issue
  ↓
¿Qué necesitamos hacer?
```

Proponé una rama apropiada para:

> Agregar instrucciones de instalación.

Después explicá la relación:

```text
Issue
  ↓
rama
```

---

# Ejercicio 8 — Commit y Pull Request

Explicá la diferencia entre:

```text
commit
```

y:

```text
Pull Request
```

Completá:

```text
Un commit ________________________________

Una Pull Request _________________________
```

---

# Ejercicio 9 — Flujo básico

Ordená correctamente estas etapas:

```text
merge
push
commit
crear rama
Pull Request
revisión
```

Escribí la secuencia completa.

---

# Ejercicio 10 — Crear una rama para una tarea

Partís de:

```text
main
```

Tenés que desarrollar:

> Nueva sección de documentación.

¿Qué comando utilizarías para crear una rama y cambiarte a ella?

¿Qué nombre le pondrías?

Justificá el nombre.

---

# Ejercicio 11 — Predecir la historia

Partimos de:

```text
A ── B ── C
          ↑
        main
```

Creamos:

```text
docs-instalacion
```

y realizamos dos commits:

```text
D
E
```

Dibujá la historia resultante.

---

# Ejercicio 12 — Publicar la rama

Ya realizaste:

```text
A ── B ── C
          \
           D ── E
```

La rama se llama:

```text
docs-instalacion
```

¿Qué comando utilizarías para publicarla en GitHub?

Explicá qué significa:

```text
-u
```

y qué representa:

```text
origin
```

---

# Ejercicio 13 — ¿Dónde está el cambio?

Un estudiante realizó:

```bash
git switch -c feature
```

Después hizo tres commits.

Luego ejecutó:

```bash
git switch main
```

y afirma:

> "Perdí mis cambios."

¿Es correcto?

Explicá qué ocurrió.

---

# Ejercicio 14 — Pull Request

Tenés:

```text
feature
   ↓
commits
   ↓
push
```

¿Qué operación debería realizarse en GitHub para proponer la incorporación de esos cambios a `main`?

Explicá qué información debería permitir revisar esa operación.

---

# Ejercicio 15 — Descripción de una Pull Request

Una persona crea una Pull Request con:

```text
Título:
Cambios

Descripción:
Hice unas cosas.
```

Analizá el problema.

Proponé una descripción mejor.

Podés utilizar:

```md
## Qué hice

...

## Por qué

...

## Cómo lo probé

...
```

---

# Ejercicio 16 — Revisar una Pull Request

Una Pull Request modifica:

```text
README.md
configuracion.txt
ejemplo.py
```

Antes de aprobarla, ¿qué aspectos revisarías?

Proponé al menos cinco preguntas.

---

# Ejercicio 17 — Comentario útil

Transformá estos comentarios en observaciones técnicas útiles.

### A

> Está mal.

### B

> Cambialo.

### C

> No me gusta.

### D

> Esto no sirve.

Explicá qué información debería aportar una buena observación.

---

# Ejercicio 18 — Corrección solicitada

Una Pull Request recibe esta observación:

> "La nueva sección explica cómo instalar el proyecto, pero no indica qué versión de Python se necesita."

¿Qué debería hacer la persona que creó la Pull Request?

Describí el proceso completo desde la corrección hasta la actualización de la Pull Request.

---

# Ejercicio 19 — Pull Request que cambia

Respondé:

> ¿Una Pull Request queda congelada una vez creada?

Explicá qué ocurre si la persona realiza:

```bash
git commit
git push
```

sobre la rama asociada a la Pull Request.

---

# Ejercicio 20 — Aprobar o solicitar cambios

Tenés una Pull Request.

El cambio:

- resuelve la tarea;
- está documentado;
- no contiene cambios innecesarios;
- fue probado correctamente.

¿Qué acción realizarías?

Ahora imaginá que:

- falta una parte importante;
- existe un error;
- la documentación es insuficiente.

¿Qué acción realizarías?

Justificá ambas decisiones.

---

# Ejercicio 21 — Merge

Partimos de:

```text
main
  \
   feature
```

La Pull Request fue revisada y aprobada.

¿Qué operación permite incorporar los cambios?

Explicá qué significa integrar `feature` en `main`.

---

# Ejercicio 22 — Rama actual

Un estudiante ejecuta:

```bash
git switch feature
git merge main
```

y dice:

> "Integré feature en main."

Analizá la situación.

¿Es correcta la afirmación?

¿Qué rama estaba activa?

¿Qué operación realizó realmente?

---

# Ejercicio 23 — Push

Explicá qué ocurre conceptualmente al ejecutar:

```bash
git push
```

Completá:

```text
Repositorio local
        ↓
      push
        ↓
________________
```

---

# Ejercicio 24 — Pull

Explicá qué ocurre conceptualmente al ejecutar:

```bash
git pull
```

Completá:

```text
________________
        ↓
      pull
        ↓
Repositorio local
```

---

# Ejercicio 25 — Fetch

Explicá qué diferencia conceptual existe entre:

```bash
git fetch
```

y:

```bash
git pull
```

No es necesario describir internamente todas las operaciones que Git realiza.

Concentrate en qué efecto tiene cada una sobre tu trabajo local.

---

# Ejercicio 26 — Otra persona hizo un cambio

Tu compañero realizó:

```text
commit
 ↓
push
```

Ahora el repositorio remoto tiene cambios que vos todavía no tenés.

Respondé:

1. ¿Tu repositorio local está necesariamente actualizado?
2. ¿Qué comando podrías utilizar para obtener e integrar los cambios?
3. ¿Qué otro comando permite consultar primero la información remota sin integrarla automáticamente?

---

# Ejercicio 27 — Historia colaborativa

Observá:

```text
              D ── E
             /       \
A ── B ── C ────────── M
```

Suponiendo que:

```text
D y E → trabajo de una persona
M → integración
```

respondé:

1. ¿Dónde se separó la línea de trabajo?
2. ¿Qué commits fueron realizados en ella?
3. ¿Qué representa `M`?
4. ¿Qué operación pudo producir `M`?

---

# Ejercicio 28 — Dos personas

Dos estudiantes trabajan sobre:

```text
main
```

Uno crea:

```text
feature-login
```

y otro:

```text
feature-documentacion
```

Ambos trabajan independientemente.

Dibujá la historia.

Después explicá por qué las ramas permiten reducir la interferencia entre los trabajos.

---

# Ejercicio 29 — Trabajo paralelo

Partimos de:

```text
A ── B ── C
```

Persona A realiza:

```text
D ── E
```

sobre una rama.

Persona B realiza:

```text
F
```

sobre otra.

Dibujá la historia completa.

Después indicá qué información debería observar un revisor antes de integrar cada rama.

---

# Ejercicio 30 — Conflicto

Dos personas parten del mismo commit.

Ambas modifican exactamente la misma línea:

```text
Título del proyecto
```

Persona A escribe:

```text
Proyecto Educativo
```

Persona B escribe:

```text
Proyecto de Aprendizaje
```

Respondé:

1. ¿Por qué puede aparecer un conflicto?
2. ¿Puede Git decidir automáticamente cuál es mejor?
3. ¿Quién debería decidir el resultado?
4. ¿Qué información debería analizarse?

---

# Ejercicio 31 — Resolver un conflicto

Después de un merge aparece:

```text
<<<<<<< HEAD
Proyecto Educativo
=======
Proyecto de Aprendizaje
>>>>>>> feature
```

¿Qué representa cada parte?

¿Qué deberías hacer antes de ejecutar:

```bash
git add
```

---

# Ejercicio 32 — Conflicto y Pull Request

Una Pull Request muestra que existen conflictos con `main`.

¿Qué significa esto?

¿Qué debería hacer la persona que creó la Pull Request?

Describí conceptualmente el proceso para resolver la situación.

---

# Ejercicio 33 — Revisar una Pull Request con conflicto

Sos revisor de una Pull Request que muestra:

```text
This branch has conflicts that must be resolved.
```

¿Deberías aprobarla inmediatamente?

Explicá qué información necesitás antes de aprobarla.

---

# Ejercicio 34 — CONTRIBUTING.md

Un repositorio recibe colaboradores nuevos.

¿Qué información incluirías en:

```text
CONTRIBUTING.md
```

Proponé al menos seis secciones.

---

# Ejercicio 35 — Normas de commits

Un equipo acuerda que los commits deben ser claros.

Compará:

```text
Cambios
```

con:

```text
Agrega instrucciones de instalación
```

¿Cuál es más útil?

¿Por qué?

Proponé tres ejemplos de buenos mensajes de commit.

---

# Ejercicio 36 — Normas de ramas

Proponé una convención de nombres para ramas.

Por ejemplo:

```text
feature-...
fix-...
docs-...
```

Después proponé nombres para:

- nueva búsqueda;
- corrección del login;
- actualización del README;
- experimento con configuración.

---

# Ejercicio 37 — CODE_OF_CONDUCT

Explicá qué propósito puede tener:

```text
CODE_OF_CONDUCT.md
```

¿Por qué puede resultar útil en un proyecto donde participan varias personas?

---

# Ejercicio 38 — GitHub como espacio de colaboración

Un compañero dice:

> "GitHub sirve para guardar el código."

¿Es suficiente esta definición?

Ampliá la respuesta incorporando:

- Issues;
- Pull Requests;
- revisiones;
- discusiones;
- repositorios compartidos.

---

# Ejercicio 39 — Diseñar un flujo

Para una nueva funcionalidad, diseñá el siguiente flujo:

```text
necesidad
   ↓
?
   ↓
?
   ↓
?
   ↓
?
   ↓
integración
```

Completá los pasos utilizando:

```text
Issue
Branch
Commit
Push
Pull Request
Review
Merge
```

---

# Ejercicio 40 — ¿Qué herramienta utilizar?

Relacioná cada necesidad con la herramienta más apropiada.

| Necesidad | Herramienta |
|---|---|
| Registrar un cambio | ? |
| Plantear una tarea | ? |
| Trabajar aisladamente | ? |
| Publicar cambios | ? |
| Proponer una integración | ? |
| Revisar cambios | ? |
| Integrar cambios | ? |
| Obtener cambios remotos | ? |

Utilizá:

```text
Issue
Branch
Commit
Push
Pull Request
Review
Merge
Pull
```

---

# Ejercicio 41 — Un repositorio sin reglas

Imaginá un equipo donde:

- cualquiera modifica `main`;
- no existen Pull Requests;
- los commits se llaman `cambio`, `fix`, `cosas`;
- nadie revisa los cambios;
- no existe documentación para nuevos colaboradores.

Enumerá los problemas que podrían aparecer.

Después proponé cinco reglas concretas para mejorar la situación.

---

# Ejercicio 42 — Proteger `main`

¿Por qué un equipo podría decidir proteger:

```text
main
```

y exigir Pull Requests?

Explicá qué problema intenta evitar.

---

# Ejercicio 43 — Flujo de incorporación

Diseñá un procedimiento para que una persona nueva pueda incorporarse a un proyecto.

Debería incluir como mínimo:

```text
1.
2.
3.
4.
5.
```

Podés considerar:

- clonar;
- configurar;
- leer documentación;
- crear rama;
- trabajar;
- publicar;
- Pull Request.

---

# Ejercicio 44 — Leer una Pull Request

Imaginá que una Pull Request contiene:

```text
Título:
Actualiza documentación

Archivos modificados:
README.md
CONTRIBUTING.md

Commits:
Agrega sección de instalación
Agrega guía de contribución
```

Respondé:

1. ¿Qué tarea parece resolver?
2. ¿Qué revisarías?
3. ¿Qué información adicional pedirías si fuera necesaria?
4. ¿Qué indicaría que el cambio está listo para integrar?

---

# Ejercicio 45 — Diseñar una Issue

Creá una Issue para:

> Incorporar una sección de preguntas frecuentes al README.

Incluí:

```md
# Título

...

## Descripción

...

## Objetivo

...

## Resultado esperado

...
```

Después proponé el nombre de la rama que utilizarías.

---

# Ejercicio 46 — Issue → Pull Request

Partiendo de la Issue anterior, describí todo el flujo hasta la integración:

```text
Issue
 ↓
?
 ↓
?
 ↓
?
 ↓
?
 ↓
Merge
```

Completalo y explicá cada paso.

---

# Ejercicio 47 — Simular una revisión

Creá una pequeña Pull Request sobre un repositorio propio.

Después revisala como si fueras otra persona.

Escribí:

```text
1 observación positiva
1 pregunta
1 sugerencia de mejora
```

El objetivo es practicar diferentes tipos de comunicación técnica.

---

# Ejercicio 48 — Mejorar una Pull Request

Tomá una Pull Request propia con una descripción deficiente.

Por ejemplo:

```text
Cambios en documentación.
```

Reescribila para que incluya:

```text
qué
por qué
cómo fue probado
```

Compará ambas versiones.

---

# Ejercicio 49 — Actualizar una rama

Una Pull Request está abierta.

Mientras tanto, `main` recibió nuevos cambios.

Respondé:

1. ¿Qué problema puede generar esto?
2. ¿Por qué podría ser necesario actualizar la rama de trabajo?
3. ¿Qué podría ocurrir al intentar integrarla?

No es necesario resolver técnicamente todas las variantes.

El objetivo es comprender la situación.

---

# Ejercicio 50 — Flujo completo

Realizá en un repositorio propio:

```text
1. Crear una Issue.
2. Crear una rama.
3. Realizar dos commits.
4. Publicar la rama.
5. Crear una Pull Request.
6. Revisar los cambios.
7. Realizar una corrección.
8. Publicar la corrección.
9. Volver a revisar.
10. Integrar.
11. Actualizar main local.
12. Analizar la historia.
```

Al finalizar ejecutá:

```bash
git status
git branch
git log --oneline --graph --all
```

---

# Comprobación final

Sin consultar la documentación, respondé:

### 1.

¿Qué diferencia existe entre Git y GitHub?

### 2.

¿Qué problema resuelve una rama en un equipo?

### 3.

¿Qué función cumple una Issue?

### 4.

¿Qué función cumple una Pull Request?

### 5.

¿Qué diferencia existe entre un commit y una Pull Request?

### 6.

¿Qué significa revisar una Pull Request?

### 7.

¿Qué diferencia existe entre `push`, `pull` y `fetch`?

### 8.

¿Por qué pueden aparecer conflictos?

### 9.

¿Qué significa resolver un conflicto?

### 10.

¿Qué información debería contener una buena Pull Request?

### 11.

¿Qué propósito tiene `CONTRIBUTING.md`?

### 12.

¿Por qué un proyecto puede proteger `main`?

---

# Criterio de resolución

No alcanza con obtener el resultado correcto.

En los ejercicios de este módulo interesa especialmente poder explicar:

```text
qué problema existe
       ↓
qué herramienta corresponde
       ↓
qué operación se realiza
       ↓
qué resultado se obtiene
       ↓
por qué ese resultado es correcto
```

El objetivo es comenzar a pensar Git y GitHub como herramientas de coordinación del trabajo, y no solamente como un conjunto de comandos.

> **Colaborar con Git no significa solamente compartir código. Significa poder coordinar cambios, discutirlos, revisarlos e integrarlos manteniendo una historia comprensible del proyecto.**