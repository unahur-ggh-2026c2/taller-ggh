# Desafíos
## Módulo 00 — ¿Por qué Git?

Los desafíos de este módulo no buscan evaluar el manejo de comandos.

El objetivo es comenzar a desarrollar la capacidad de **analizar situaciones de trabajo y reconocer cuándo resulta necesario utilizar un sistema de control de versiones**.

En todos los casos, primero analizá el problema y recién después pensá en una posible solución.

---

## Desafío 1 — El proyecto que creció demasiado

Comenzaste un proyecto personal hace tres meses.

Al principio solamente tenías:

```text
proyecto/
└── README.md
```

Con el tiempo incorporaste más archivos y comenzaste a guardar copias:

```text
proyecto/
proyecto-enero/
proyecto-febrero/
proyecto-febrero-corregido/
proyecto-marzo/
proyecto-marzo-final/
proyecto-marzo-final-2/
```

Ahora necesitás recuperar una versión específica del proyecto.

Sabés aproximadamente cuándo fue creada, pero no recordás qué archivos habían cambiado.

### Tu desafío

Sin utilizar Git todavía, intentá responder:

1. ¿Qué información te falta?
2. ¿Qué dificultades presenta la estrategia de copias?
3. ¿Qué información debería registrar automáticamente una herramienta de control de versiones?
4. ¿Qué características tendría que tener esa herramienta para resolver el problema?

### Entregable

Creá un archivo:

```text
desafio-01.md
```

y documentá tu propuesta.

---

## Desafío 2 — Diseñá tu propio sistema de versiones

Imaginá que Git no existe.

Necesitás diseñar un sistema para controlar las versiones de un proyecto compuesto por archivos Markdown.

Tu sistema debería permitir:

* conservar diferentes estados del proyecto;
* saber qué cambió;
* identificar cuándo ocurrió un cambio;
* identificar quién lo realizó;
* recuperar un estado anterior;
* trabajar sobre diferentes líneas de trabajo;
* combinar cambios realizados por diferentes personas.

### Tu desafío

Diseñá conceptualmente el sistema.

No podés utilizar comandos de Git.

Podés utilizar:

* diagramas;
* tablas;
* nombres inventados;
* ejemplos;
* estructuras de carpetas.

### Pregunta adicional

¿Qué problemas tendría tu solución cuando el proyecto aumentara de tamaño?

---

## Desafío 3 — Dos personas, dos decisiones

Dos personas trabajan sobre el mismo archivo.

El archivo comienza así:

```md
# Proyecto

## Descripción

Este proyecto tiene como objetivo aprender control de versiones.
```

### Persona A

Modifica la descripción:

```md
## Descripción

Este proyecto tiene como objetivo aprender Git.
```

### Persona B

También modifica la descripción:

```md
## Descripción

Este proyecto tiene como objetivo aprender Git y GitHub.
```

Ambas modificaciones son válidas desde el punto de vista de cada persona.

### Tu desafío

Decidí cómo debería resolverse la situación.

No alcanza con elegir una versión.

Explicá:

1. qué información debería mostrar la herramienta;
2. qué debería decidir automáticamente;
3. qué debería decidir una persona;
4. qué información debería conservarse después de resolver la situación.

---

## Desafío 4 — El historial cuenta una historia

Imaginá que recibís un proyecto que contiene solamente los archivos actuales.

No existe historial.

La persona que te lo entrega te dice:

> "Esto funciona. No sé exactamente cómo llegamos hasta acá."

Durante una revisión encontrás:

```text
README.md
objetivos.md
integrantes.md
conclusiones.md
```

### Tu desafío

Escribí cinco preguntas que te gustaría poder responder sobre la evolución del proyecto.

Por ejemplo:

> ¿Cuándo se incorporó `conclusiones.md`?

No utilices preguntas relacionadas únicamente con el contenido actual de los archivos.

Buscá preguntas sobre **la historia del proyecto**.

### Segunda parte

Explicá por qué cada pregunta sería útil para alguien que continúa trabajando sobre el proyecto.

---

## Desafío 5 — ¿Backup o control de versiones?

Un compañero afirma:

> "No necesito Git. Tengo una copia de seguridad todos los días."

Analizá su afirmación.

### Tu desafío

Escribí una respuesta argumentada explicando:

* qué problema resuelve una copia de seguridad;
* qué problemas adicionales aparecen durante la evolución de un proyecto;
* qué información proporciona un historial;
* qué sucede cuando trabajan varias personas.

No se trata de demostrar que tu compañero está equivocado.

Se trata de determinar **qué problema resuelve cada herramienta**.

---

## Desafío 6 — Git sin programación

Hasta este momento trabajamos únicamente con Markdown.

Ahora alguien te dice:

> "Entonces Git sirve solamente para documentos."

### Tu desafío

Respondé utilizando ejemplos de otros tipos de archivos.

Pensá en al menos cinco tipos diferentes de archivos que podrían formar parte de un proyecto.

Para cada uno explicá:

* por qué podría ser necesario conservar su evolución;
* qué problema aparecería si varias personas lo modificaran;
* qué utilidad tendría disponer de un historial.

---

## Desafío 7 — El proyecto abandonado

Te incorporás a un proyecto que otra persona comenzó hace seis meses.

Encontrás:

```text
proyecto/
├── README.md
├── notas.md
├── objetivos.md
├── objetivos-v2.md
├── objetivos-final.md
├── objetivos-final-real.md
└── backup/
```

No sabés cuál de los archivos es el correcto.

### Tu desafío

Antes de modificar absolutamente nada, elaborá una estrategia para investigar el proyecto.

Tu estrategia debe responder:

1. ¿Qué observarías primero?
2. ¿Qué información buscarías?
3. ¿Qué preguntas harías al autor?
4. ¿Qué riesgos existen al comenzar a modificar archivos?
5. ¿Qué debería ofrecer un sistema de control de versiones para facilitar esta situación?

---

## Desafío 8 — Pensar como integrante de un equipo

Imaginá que ingresás a un proyecto universitario en el que ya trabajan cuatro personas.

Te entregan una carpeta comprimida:

```text
proyecto.zip
```

La única instrucción es:

> "Abrilo y empezá a trabajar."

### Tu desafío

Elaborá una lista de información que necesitarías conocer antes de modificar cualquier archivo.

Organizala en tres categorías:

### Proyecto

¿Qué necesitás saber sobre el proyecto?

### Cambios

¿Qué necesitás saber sobre la evolución del proyecto?

### Colaboración

¿Qué necesitás saber sobre las demás personas que trabajan en él?

Finalmente:

> ¿Cuáles de estas necesidades podría resolver Git?

---

## Desafío 9 — Explicale Git a otra persona

Una persona que nunca utilizó Git te pregunta:

> "¿Para qué necesito Git si puedo guardar una copia de mis archivos?"

Tenés cinco minutos para explicárselo.

### Restricciones

No podés:

* mostrar comandos;
* hablar de GitHub;
* utilizar una explicación basada en definiciones;
* decir simplemente "porque es profesional".

Tenés que utilizar una situación concreta.

### Entregable

Escribí una explicación de entre 150 y 250 palabras.

El objetivo es que la persona comprenda **el problema**, aunque todavía no conozca la herramienta.

---

## Desafío 10 — Encontrar el problema detrás del comando

Un compañero te dice:

> "Necesito aprender estos comandos porque el profesor los va a tomar."

Le preguntás para qué sirven y responde:

> "No sé. Solo sé que hay que ejecutarlos en este orden."

### Tu desafío

Explicá por qué este enfoque puede resultar problemático.

Después proponé una estrategia diferente para aprender Git.

La propuesta debe incluir:

* problemas concretos;
* experimentación;
* interpretación de resultados;
* consulta de documentación;
* recuperación de errores.

---

## Desafío 11 — El requisito imposible

Un equipo establece la siguiente regla:

> "Nunca debemos tener conflictos."

Analizá la afirmación.

### Tu desafío

Respondé:

1. ¿Es posible garantizar que nunca existan conflictos?
2. ¿Qué situaciones pueden generarlos?
3. ¿Qué debería aprender un equipo para trabajar correctamente cuando aparecen?
4. ¿Por qué aprender a resolver conflictos puede ser más importante que intentar evitarlos completamente?

No busques todavía comandos ni procedimientos técnicos.

Pensá en términos de trabajo colaborativo.

---

## Desafío 12 — Definir el objetivo del curso

Llegaste al final del primer módulo.

Ahora completá esta frase:

> **El objetivo de aprender Git no es...**

y después:

> **El objetivo de aprender Git sí es...**

Escribí ambas respuestas.

Después comparalas con esta idea:

> **Una persona que trabaja en un proyecto debería poder utilizar Git y GitHub sin convertirse en un problema para el resto del equipo.**

### Pregunta final

¿Qué conocimientos y habilidades tendría que desarrollar una persona para alcanzar ese objetivo?

Construí una lista.

Esta lista será retomada y ampliada a lo largo de los siguientes módulos.

