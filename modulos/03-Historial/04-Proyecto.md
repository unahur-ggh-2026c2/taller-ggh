# Proyecto
## Módulo 03 — Historial

---

## 1. Propósito

En este proyecto vas a construir y analizar la historia de un pequeño proyecto documental.

La actividad integra los conceptos trabajados durante el módulo:

- commits;
- historial;
- identificadores;
- autores;
- fechas;
- mensajes;
- lectura de la evolución;
- diferencia entre estado actual e historial;
- utilización del historial como herramienta de investigación.

El objetivo principal no es generar una gran cantidad de commits.

El objetivo es construir una historia que pueda ser **leída, interpretada y utilizada para comprender el proyecto**.

---

## 2. El proyecto

Creá un repositorio llamado:

```text
historia-de-un-proyecto
```

El tema puede ser elegido libremente.

Puede representar:

- una aplicación;
- un proyecto académico;
- una biblioteca;
- un juego;
- una herramienta;
- una organización;
- una idea de emprendimiento.

El repositorio deberá contener inicialmente:

```text
historia-de-un-proyecto/
├── README.md
├── objetivos.md
└── notas.md
```

---

## 3. Primera versión

### `README.md`

Creá:

```md
# Nombre del proyecto

Descripción inicial del proyecto.

## Propósito

Explicación del propósito general.
```

### `objetivos.md`

Creá:

```md
# Objetivos

- Objetivo inicial 1
- Objetivo inicial 2
- Objetivo inicial 3
```

### `notas.md`

Creá:

```md
# Notas

Notas iniciales del proyecto.
```

Adaptá el contenido al proyecto que elegiste.

---

## 4. Primer commit

Inicializá el repositorio.

Consultá:

```bash
git status
```

Prepará los archivos y realizá el primer commit.

Utilizá un mensaje que describa claramente la creación inicial.

Por ejemplo:

```bash
git commit -m "Crea estructura inicial del proyecto"
```

Después:

```bash
git status
```

El repositorio debe quedar limpio.

---

## 5. Construir la historia

Ahora vas a desarrollar progresivamente el proyecto.

Realizá al menos **ocho commits adicionales**.

Cada commit debe representar una modificación concreta.

No los hagas todos de una sola vez.

Entre una modificación y otra:

1. modificá;
2. guardá;
3. observá el estado;
4. decidí qué registrar;
5. prepará los cambios;
6. realizá el commit;
7. verificá el estado.

---

## 6. Primera evolución

Ampliá `README.md`.

Agregá:

```md
## Características

- Característica 1
- Característica 2
- Característica 3
```

Registrá el cambio con un mensaje descriptivo.

---

## 7. Segunda evolución

Modificá `objetivos.md`.

Agregá al menos un nuevo objetivo.

Registrá el cambio en un nuevo commit.

El mensaje debe permitir comprender qué incorporaste.

---

## 8. Tercera evolución

Ampliá `notas.md`.

Agregá una sección:

```md
## Decisiones

- Decisión 1
- Decisión 2
```

Registrá el cambio en un nuevo commit.

---

## 9. Cuarta evolución — una corrección

Realizá deliberadamente una corrección sobre algún contenido existente.

Puede ser:

- una descripción;
- un objetivo;
- una instrucción;
- una nota.

Registrá la corrección en un commit independiente.

El mensaje debe dejar claro que se trata de una corrección.

Por ejemplo:

```text
Corrige descripción del proyecto
```

---

## 10. Quinta evolución — documentación

Incorporá una nueva sección documental en `README.md`.

Por ejemplo:

```md
## Uso

Descripción de cómo se utilizaría el proyecto.
```

Registrá el cambio en un nuevo commit.

---

## 11. Sexta evolución — nueva característica

Agregá una característica adicional al proyecto.

Puede ser ficticia.

Modificá los archivos necesarios y registrá el cambio.

El mensaje debe expresar claramente la intención.

---

## 12. Séptima evolución — actualización

Realizá una modificación posterior que amplíe alguno de los contenidos existentes.

Registrala mediante un nuevo commit.

Intentá que el mensaje permita diferenciar este cambio de los anteriores.

---

## 13. Octava evolución — estado actual

Agregá al `README.md` una sección:

```md
## Estado actual

El proyecto se encuentra en desarrollo.
```

Registrá el cambio.

---

## 14. Verificar la historia

Ahora ejecutá:

```bash
git log
```

Observá cuidadosamente todos los commits.

Identificá:

- commit inicial;
- commit más reciente;
- commits intermedios;
- autores;
- fechas;
- mensajes;
- identificadores.

---

## 15. Vista resumida

Ejecutá:

```bash
git log --oneline
```

Observá la historia completa.

Deberías poder reconocer aproximadamente:

```text
estructura inicial
       ↓
características
       ↓
objetivos
       ↓
decisiones
       ↓
corrección
       ↓
documentación
       ↓
nueva característica
       ↓
actualización
       ↓
estado actual
```

Los mensajes concretos dependerán de tu proyecto.

---

## 16. Reconstruir la evolución

Creá un archivo:

```text
historia.md
```

Escribí una explicación de la evolución del proyecto.

La estructura mínima será:

```md
# Historia del proyecto

## Inicio

...

## Primeras modificaciones

...

## Evolución

...

## Correcciones

...

## Estado actual

...
```

La explicación debe construirse a partir del historial.

No agregues acontecimientos que no puedan sostenerse mediante la información disponible.

---

## 17. Analizar los commits

En `historia.md`, agregá:

```md
## Commits relevantes

### Commit inicial

Identificador:

Mensaje:

Autor:

Fecha:

Descripción:

### Corrección

Identificador:

Mensaje:

Autor:

Fecha:

Descripción:

### Commit más reciente

Identificador:

Mensaje:

Autor:

Fecha:

Descripción:
```

Completá la información consultando:

```bash
git log
```

---

## 18. Analizar los mensajes

Agregá:

```md
## Calidad de los mensajes

### Mensajes claros

...

### Mensajes que podrían mejorar

...

### Mejoras propuestas

...
```

Analizá tus propios mensajes.

Preguntate:

> ¿Una persona que no participó del proyecto podría comprender la evolución leyendo solamente los mensajes?

---

## 19. Investigar una afirmación

Ahora formulá una afirmación sobre la historia del proyecto.

Por ejemplo:

> "La característica X fue incorporada después de los objetivos."

Registrala en:

```md
## Investigación

### Afirmación

...

### Evidencia disponible

...

### Conclusión

...
```

Utilizá el historial para determinar si podés sostener la afirmación.

Si la información disponible no alcanza, indicá qué necesitarías consultar.

---

## 20. Diferenciar presente y pasado

Ahora realizá una modificación en `README.md`.

No hagas commit todavía.

Ejecutá:

```bash
git status
```

y:

```bash
git log --oneline
```

Registrá en `historia.md`:

```md
## Estado actual e historial

### ¿Qué muestra `git status`?

...

### ¿Qué muestra `git log`?

...

### ¿Qué diferencia existe entre ambos?

...
```

---

## 21. Registrar el cambio pendiente

Ahora prepará y registrá la modificación anterior.

Utilizá un mensaje descriptivo.

Después:

```bash
git status
```

El repositorio debe quedar limpio.

Volvé a consultar:

```bash
git log --oneline
```

Observá cómo el cambio pasó de ser parte del estado actual a formar parte del historial registrado.

---

## 22. Evaluar el historial completo

En `historia.md`, agregá:

```md
## Evaluación del historial

### Claridad

...

### Coherencia

...

### Calidad de los mensajes

...

### Utilidad para investigar

...

### Mejoras posibles

...
```

Evaluá tu propio historial como si fueras una persona externa que acaba de incorporarse al proyecto.

---

## 23. Crear una línea de tiempo

Construí una línea de tiempo textual:

```text
Inicio
  │
  ├── Commit 1
  │
  ├── Commit 2
  │
  ├── Commit 3
  │
  ├── Commit 4
  │
  ├── Commit 5
  │
  └── Estado actual
```

Reemplazá cada elemento con una descripción concreta de lo que ocurrió.

Podés incluir los identificadores abreviados.

Por ejemplo:

```text
a84f9c2 — Crea estructura inicial
b71d4e8 — Agrega características
c92ab31 — Incorpora objetivos
...
```

---

## 24. El historial como memoria

Agregá a `historia.md`:

```md
## Reflexión

¿Qué información sobre el proyecto puedo reconstruir a partir del historial?

...

¿Qué información no puedo conocer solamente mediante el historial?

...

¿Por qué los mensajes de commit son importantes?

...

¿Cómo podría utilizar el historial para investigar un problema?

...
```

Respondé con tus propias palabras.

---

## 25. Verificación final

Ejecutá:

```bash
git status
```

El repositorio debe estar limpio.

Después:

```bash
git log --oneline
```

Verificá que exista una historia suficientemente extensa y comprensible.

Finalmente:

```bash
git log
```

Seleccioná:

- el primer commit;
- un commit intermedio;
- el commit de una corrección;
- el último commit.

Verificá sus datos.

---

## 26. Producto final

La estructura mínima será:

```text
historia-de-un-proyecto/
├── .git/
├── README.md
├── objetivos.md
├── notas.md
└── historia.md
```

El repositorio deberá contener:

- al menos nueve commits;
- una evolución coherente;
- al menos una corrección;
- mensajes descriptivos;
- una línea de tiempo;
- un análisis del historial;
- una investigación basada en evidencia;
- una reflexión final.

---

## 27. Criterios de finalización

El proyecto está terminado cuando:

- existe una historia de commits suficientemente extensa;
- los commits representan cambios concretos;
- los mensajes permiten comprender las intenciones;
- se puede identificar el commit inicial;
- se puede identificar el commit más reciente;
- se pueden identificar commits intermedios;
- se puede reconstruir la evolución general;
- se distingue entre estado actual e historial;
- se utilizó el historial para investigar una afirmación;
- se documentaron las conclusiones;
- el repositorio termina limpio.

---

## 28. Pregunta final

Sin consultar documentación, respondé:

> **¿Qué diferencia existe entre tener un historial y tener un historial útil?**

Después:

> **¿Qué información puede proporcionarnos el historial cuando necesitamos investigar cómo evolucionó un proyecto?**

Y finalmente:

> **¿Qué responsabilidad tiene quien crea un commit respecto de las personas que leerán ese historial en el futuro?**

Si podés responder estas preguntas y demostrarlo mediante el proyecto, completaste el objetivo principal del módulo.