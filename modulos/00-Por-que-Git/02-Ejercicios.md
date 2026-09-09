# Ejercicios
## Módulo 00 — ¿Por qué Git?

Los siguientes ejercicios buscan consolidar las ideas trabajadas durante la práctica.

En esta etapa no se evalúa la capacidad de memorizar comandos.

El objetivo es poder **reconocer problemas que Git permite resolver** y explicar por qué una situación determinada requiere control de versiones.

---

## Ejercicio 1 — El problema de las copias

Un estudiante trabaja sobre un proyecto y, para conservar las distintas versiones, crea las siguientes carpetas:

```text
trabajo/
trabajo-v2/
trabajo-v2-corregido/
trabajo-v3/
trabajo-v3-final/
trabajo-v3-final-definitivo/
```

Respondé:

1. ¿Qué problema está intentando resolver?
2. ¿Qué información puede perderse utilizando únicamente este método?
3. ¿Cómo determinarías qué cambios existen entre `trabajo-v2` y `trabajo-v3`?
4. ¿Cómo sabrías quién realizó un cambio?
5. ¿Cómo recuperarías una versión anterior?
6. ¿Qué dificultades aparecerían si varias personas trabajaran de esta manera?

Finalmente:

> Explicá con tus palabras por qué este método puede resultar insuficiente cuando un proyecto comienza a crecer.

---

## Ejercicio 2 — Reconocer la necesidad

Para cada situación indicá si existe o no un problema que podría beneficiarse del uso de un sistema de control de versiones.

### Situación A

Una persona escribe un documento de una sola página y lo entrega una única vez.

### Situación B

Un grupo trabaja durante varias semanas sobre un conjunto de archivos y necesita conservar los cambios realizados.

### Situación C

Dos personas modifican simultáneamente el mismo archivo.

### Situación D

Una persona necesita recuperar el estado que tenía un proyecto hace tres días.

### Situación E

Un estudiante guarda solamente la versión final de un trabajo y nunca vuelve a modificarlo.

Para cada respuesta, justificá brevemente tu decisión.

---

## Ejercicio 3 — ¿Qué debería resolver una herramienta?

Supongamos que estás diseñando una herramienta para administrar la evolución de un proyecto.

Sin pensar todavía en Git, escribí una lista de funcionalidades que considerarías necesarias.

Como mínimo, pensá en:

* versiones;
* cambios;
* historial;
* recuperación;
* comparación;
* colaboración.

Después compará tu lista con la de tus compañeros.

### Pregunta

¿Cuáles funcionalidades fueron mencionadas por todos?

¿Cuáles aparecieron solamente en algunas respuestas?

¿Por qué?

---

## Ejercicio 4 — Una historia de cambios

Tenemos un archivo:

```text
README.md
```

Durante una semana se realizaron los siguientes cambios:

```text
Lunes
    Se creó el archivo.

Martes
    Se agregó la descripción del proyecto.

Miércoles
    Se agregaron los integrantes.

Jueves
    Se modificó la descripción.

Viernes
    Se eliminó accidentalmente la lista de integrantes.
```

Respondé:

1. ¿Qué información sería útil conservar?
2. ¿Cómo podríamos saber qué ocurrió el jueves?
3. ¿Cómo podríamos recuperar la lista eliminada el viernes?
4. ¿Qué ventajas tendría conservar un historial de los cambios?

No es necesario indicar comandos.

Explicá qué debería permitir hacer una herramienta adecuada.

---

## Ejercicio 5 — Dos personas, un archivo

Ana y Juan trabajan sobre:

```text
README.md
```

Ana agrega:

```md
## Descripción

Proyecto de aprendizaje de Git.
```

Juan agrega:

```md
## Integrantes

- Ana
- Juan
```

Ambos terminan sus modificaciones.

### Preguntas

1. ¿Existe un problema?
2. ¿Los dos cambios pueden coexistir?
3. ¿Qué información necesitamos para combinarlos correctamente?
4. ¿Qué debería hacer una herramienta de control de versiones en esta situación?

Ahora imaginá que ambos modifican la misma sección:

### Ana

```md
## Descripción

Proyecto de aprendizaje de Git.
```

### Juan

```md
## Descripción

Proyecto de aprendizaje de Git y GitHub.
```

Respondé:

5. ¿Qué cambió respecto de la situación anterior?
6. ¿Puede una herramienta decidir automáticamente qué versión representa la intención correcta?
7. ¿Qué debería ocurrir cuando dos cambios son incompatibles?

---

## Ejercicio 6 — Git no es GitHub

Completá las siguientes afirmaciones con tus propias palabras:

### Git

Es:

> ...

Sirve para:

> ...

### GitHub

Es:

> ...

Sirve para:

> ...

### Relación

Git y GitHub:

> ...

No consultes una definición textual de Internet para responder.

Primero intentá construir la explicación a partir de lo trabajado en clase.

Después comparala con la documentación oficial.

---

## Ejercicio 7 — Verdadero o falso

Indicá si cada afirmación es verdadera o falsa y justificá tu respuesta.

### A

> Git y GitHub son exactamente lo mismo.

### B

> Git permite registrar la evolución de un proyecto.

### C

> Git solamente sirve para proyectos escritos en lenguajes de programación.

### D

> Un repositorio Git es simplemente una carpeta común.

### E

> Git puede utilizarse para trabajar sobre archivos Markdown.

### F

> Git permite conservar información sobre diferentes estados de un proyecto.

### G

> GitHub reemplaza a Git.

### H

> Los conflictos pueden aparecer cuando diferentes personas realizan cambios incompatibles.

No alcanza con indicar `Verdadero` o `Falso`.

La justificación forma parte del ejercicio.

---

## Ejercicio 8 — El proyecto sin historial

Imaginá que recibís un proyecto con esta estructura:

```text
proyecto/
├── README.md
├── objetivos.md
├── integrantes.md
└── conclusiones.md
```

El proyecto funciona correctamente, pero no existe ningún historial.

La persona que te lo entrega te dice:

> "Es la última versión. No sé qué cambios se hicieron antes."

Respondé:

1. ¿Qué información te gustaría conocer?
2. ¿Qué dificultades podrías encontrar para continuar el trabajo?
3. ¿Qué información habría sido útil conservar desde el comienzo?
4. ¿Qué problema concreto resolvería Git en este escenario?

---

## Ejercicio 9 — Diseñar una solución

Volvé al problema inicial de las carpetas:

```text
proyecto/
proyecto-v2/
proyecto-v3/
proyecto-final/
proyecto-final-correcto/
```

Ahora diseñá una solución conceptual utilizando Git.

No escribas comandos.

Describí:

1. qué tendría que existir;
2. qué información debería conservarse;
3. cómo debería registrarse cada cambio;
4. cómo debería consultarse la evolución del proyecto;
5. cómo debería recuperarse un estado anterior.

El objetivo es que diseñes la solución **antes de aprender a implementarla**.

---

## Ejercicio 10 — Explicarlo sin usar la palabra "Git"

Este ejercicio es intencionalmente difícil.

Explicale a una persona que nunca utilizó Git por qué debería utilizar un sistema de control de versiones.

No podés utilizar las palabras:

* Git;
* GitHub;
* commit;
* repositorio.

Tenés que explicar el problema utilizando solamente situaciones concretas.

Por ejemplo:

> "Imaginá que estás trabajando durante tres semanas sobre un proyecto..."

La explicación debe tener entre 100 y 200 palabras.

---

## Ejercicio 11 — Del problema a la herramienta

Completá el siguiente esquema:

```text
PROBLEMA
   ↓
¿Qué necesitamos conservar?
   ↓
¿Qué necesitamos consultar?
   ↓
¿Qué necesitamos recuperar?
   ↓
¿Qué necesitamos compartir?
   ↓
¿Qué ocurre si varias personas trabajan al mismo tiempo?
   ↓
¿Qué tipo de herramienta necesitamos?
```

Escribí una respuesta breve en cada etapa.

---

## Ejercicio 12 — Reflexión final

Respondé individualmente:

> **¿Cuál era el principal problema que intentabas resolver antes de conocer Git?**

Después de la práctica y los ejercicios, respondé nuevamente:

> **¿Cuál es ahora tu definición del problema que Git intenta resolver?**

Compará ambas respuestas.

### Pregunta final

¿Qué cambió entre tu primera explicación y la segunda?

---

## Criterio de resolución

En estos ejercicios no se busca que todas las respuestas utilicen exactamente las mismas palabras.

Se valorará especialmente que puedas:

* identificar el problema;
* relacionarlo con la necesidad de controlar versiones;
* reconocer la importancia del historial;
* distinguir Git de GitHub;
* comprender la necesidad de registrar cambios;
* reconocer las dificultades del trabajo simultáneo;
* explicar por qué una solución basada únicamente en copias de archivos resulta limitada.

> **Si podés explicar el problema con claridad, estás en condiciones de empezar a entender la herramienta que intenta resolverlo.**
