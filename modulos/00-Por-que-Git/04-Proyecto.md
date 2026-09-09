# Proyecto
## Módulo 00 — ¿Por qué Git?

---

## 1. Propósito

El proyecto de este módulo consiste en construir, de manera deliberada, una situación que permita experimentar las dificultades de administrar versiones de un proyecto sin utilizar un sistema de control de versiones.

La actividad servirá como punto de partida para comenzar a pensar qué características debería ofrecer una herramienta como Git.

No se busca todavía construir un repositorio Git funcional.

El objetivo es **modelar el problema antes de aprender la herramienta que lo resuelve**.

---

## 2. Situación

Vas a trabajar sobre un pequeño proyecto de documentación llamado:

```text
proyecto-documentacion/
```

El proyecto representará la documentación inicial de una aplicación ficticia.

Deberá contener como mínimo:

```text
proyecto-documentacion/
├── README.md
├── objetivos.md
└── integrantes.md
```

---

## 3. Versión inicial

Creá `README.md` con:

```md
# Proyecto de documentación

Este proyecto contiene la documentación de una aplicación ficticia.
```

Creá `objetivos.md` con:

```md
# Objetivos

- Organizar la documentación del proyecto.
- Registrar la evolución de los contenidos.
- Trabajar de manera colaborativa.
```

Creá `integrantes.md` con:

```md
# Integrantes

La información de los integrantes será incorporada durante el desarrollo.
```

Esta será la **versión inicial** del proyecto.

---

## 4. Primera evolución

Realizá una primera modificación sobre cada archivo.

Por ejemplo:

### `README.md`

Agregá:

```md
## Descripción

La aplicación permitirá organizar información de un proyecto académico.
```

### `objetivos.md`

Agregá:

```md
- Facilitar el trabajo entre integrantes.
- Mantener la documentación organizada.
```

### `integrantes.md`

Agregá los nombres de las personas que participan.

---

## 5. Crear una segunda versión

Ahora necesitás conservar el estado anterior y continuar trabajando.

Sin utilizar Git, buscá una forma de conservar ambas versiones.

Podés utilizar una estrategia como:

```text
proyecto-documentacion/
proyecto-documentacion-v2/
```

Continuá trabajando sobre la segunda versión.

Realizá nuevas modificaciones.

---

## 6. Crear una tercera versión

Después de realizar nuevos cambios, conservá nuevamente una copia.

Por ejemplo:

```text
proyecto-documentacion/
proyecto-documentacion-v2/
proyecto-documentacion-v3/
```

Ahora intentá identificar:

* cuál es la versión más reciente;
* qué cambió entre las versiones;
* qué información se perdió;
* qué información se duplicó;
* qué dificultades aparecen al mantener las copias.

---

## 7. Simular trabajo colaborativo

Ahora vamos a introducir una segunda persona.

Una persona trabajará sobre:

```text
README.md
```

y otra sobre:

```text
objetivos.md
```

Ambas personas realizarán modificaciones sobre sus respectivas copias.

Después deberán intentar integrar manualmente los cambios en una única versión del proyecto.

Registren las dificultades encontradas.

---

## 8. Simular un cambio sobre el mismo archivo

Ahora ambas personas deberán trabajar sobre:

```text
README.md
```

La primera persona agregará:

```md
## Características

- Organización de proyectos.
- Gestión de documentación.
```

La segunda persona agregará:

```md
## Características

- Organización de proyectos académicos.
- Trabajo colaborativo.
```

Ambos cambios deben realizarse sin que una persona vea inicialmente el trabajo de la otra.

Después deberán intentar obtener una única versión del archivo.

---

## 9. Resolver la situación

Comparen los dos cambios.

Determinen qué debería quedar finalmente en `README.md`.

No existe necesariamente una única respuesta correcta.

Lo importante es que puedan justificar la decisión.

Registren:

* qué cambios conservaron;
* qué cambios descartaron;
* por qué tomaron esas decisiones;
* qué información necesitaron para resolver la situación.

---

## 10. Diseñar una solución

Ahora imaginá que tenés que construir una herramienta que resuelva todos los problemas experimentados.

Creá un archivo:

```text
solucion.md
```

y completá:

```md
# ¿Qué debería hacer nuestra herramienta?

## Registrar cambios

...

## Conservar versiones

...

## Consultar el historial

...

## Comparar cambios

...

## Recuperar versiones anteriores

...

## Trabajar en paralelo

...

## Integrar cambios

...

## Resolver conflictos

...
```

No utilices nombres de comandos de Git.

Pensá exclusivamente en **capacidades que debería tener la herramienta**.

---

## 11. Presentación del proyecto

Prepará una breve presentación para compartir con el resto del grupo.

La presentación deberá responder:

1. ¿Qué problema encontramos?
2. ¿Qué dificultades tuvimos trabajando con copias?
3. ¿Qué ocurrió cuando dos personas modificaron el mismo archivo?
4. ¿Qué información nos hubiera gustado conservar?
5. ¿Qué debería resolver una herramienta de control de versiones?

---

## 12. Reflexión final

Antes de finalizar, respondé en `reflexion.md`:

```md
# Reflexión

## El problema

¿Qué problema principal experimentamos?

## Lo que nos faltó

¿Qué información nos hubiera gustado tener?

## Una herramienta ideal

¿Qué debería permitirnos hacer una herramienta de control de versiones?

## Git

Después de lo trabajado en este módulo, ¿por qué tiene sentido utilizar Git?
```

---

## 13. Criterios de finalización

El proyecto se considera completo cuando:

* existe una versión inicial del proyecto;
* se generaron diferentes versiones;
* se experimentó con cambios realizados por diferentes personas;
* se produjo al menos una situación de modificación simultánea sobre un mismo archivo;
* se documentaron las dificultades encontradas;
* se propuso una solución conceptual;
* se realizó una reflexión sobre el problema que Git intenta resolver.

No se evalúa todavía el dominio de comandos.

La producción principal de este módulo es la **comprensión del problema**.

---

## 14. Puente hacia el siguiente módulo

Al finalizar este proyecto deberías haber llegado a una conclusión:

> Necesitamos una forma mejor de administrar la evolución de nuestros proyectos.

El siguiente paso será comenzar a utilizar Git para resolver exactamente los problemas que acabamos de experimentar.

En el **Módulo 01 — Mi primer repositorio**, vamos a dejar atrás las copias manuales y construir nuestro primer repositorio Git.
