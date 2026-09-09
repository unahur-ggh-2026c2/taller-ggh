# Práctica
## Módulo 00 — ¿Por qué Git?

---

## 1. Antes de usar Git

En esta primera práctica todavía no vamos a aprender comandos de Git.

Primero vamos a experimentar el problema que Git intenta resolver.

La actividad consiste en simular el trabajo sobre un proyecto utilizando únicamente archivos y carpetas.

La idea es comprobar qué ocurre cuando un proyecto comienza a crecer y varias personas necesitan conservar diferentes versiones de los mismos archivos.

---

## 2. Situación inicial

Imaginá que estás trabajando en un proyecto llamado:

```text
mi-proyecto/
```

Dentro del proyecto existe un archivo:

```text
README.md
```

Su contenido inicial es:

```md
# Mi proyecto

Este es mi primer proyecto.
```

Hasta acá no hay ningún problema.

Tenemos un proyecto, un archivo y una versión inicial.

---

## 3. Primera modificación

Realizá una modificación en `README.md`.

Por ejemplo:

```md
# Mi proyecto

Este es mi primer proyecto.

## Descripción

Este proyecto forma parte de una actividad de aprendizaje.
```

Guardá el archivo.

Ahora tenemos una pregunta:

> ¿Cómo conservamos la versión anterior?

Una alternativa sería copiar toda la carpeta.

Por ejemplo:

```text
mi-proyecto/
mi-proyecto-v2/
```

La segunda carpeta contiene la nueva versión.

---

## 4. Continuamos trabajando

Realizá otra modificación.

Agregá:

```md
## Objetivos

- Aprender a trabajar con versiones.
- Registrar los cambios.
- Mantener un historial del proyecto.
```

Ahora volvemos a copiar la carpeta:

```text
mi-proyecto/
mi-proyecto-v2/
mi-proyecto-v3/
```

Continuá trabajando hasta tener al menos tres versiones diferentes.

---

## 5. El problema comienza a aparecer

Ahora detené el trabajo y observá las carpetas.

Tenemos:

```text
mi-proyecto/
mi-proyecto-v2/
mi-proyecto-v3/
```

Respondé las siguientes preguntas:

1. ¿Cuál es la versión más reciente?
2. ¿Qué cambió entre `v1` y `v2`?
3. ¿Qué cambió entre `v2` y `v3`?
4. ¿Quién realizó cada modificación?
5. ¿Por qué se realizó cada cambio?
6. ¿Podemos identificar rápidamente qué versión necesitamos?
7. ¿Qué sucede si eliminamos accidentalmente una de las carpetas?
8. ¿Qué ocurre si dos personas trabajan simultáneamente sobre `README.md`?
9. ¿Cómo podríamos combinar los cambios realizados por ambas personas?

No busques todavía una solución con Git.

Primero intentá identificar el problema.

---

## 6. Una situación más realista

Ahora vamos a complicar un poco el escenario.

Supongamos que dos personas están trabajando sobre el mismo proyecto:

```text
Proyecto
├── README.md
├── objetivos.md
└── integrantes.md
```

Las dos personas reciben una copia del proyecto.

### Persona A

Modifica `README.md` y agrega:

```md
## Descripción

Proyecto desarrollado como actividad práctica.
```

### Persona B

Modifica el mismo archivo y agrega:

```md
## Integrantes

- Ana
- Juan
```

Ambas personas terminan su trabajo.

Ahora tenemos dos versiones diferentes de `README.md`.

---

## 7. Intentemos integrar los cambios manualmente

Compará ambas versiones.

El resultado esperado sería un único archivo que contenga:

```md
# Proyecto

Este es nuestro proyecto.

## Descripción

Proyecto desarrollado como actividad práctica.

## Integrantes

- Ana
- Juan
```

Parece sencillo.

Pero ahora imaginá que ambas personas modificaron exactamente la misma sección:

### Persona A

```md
## Descripción

Proyecto desarrollado para aprender Git.
```

### Persona B

```md
## Descripción

Proyecto desarrollado para aprender Git y GitHub.
```

¿Qué versión debería quedar?

¿Quién decide?

¿Y cómo sabemos qué escribió cada persona?

---

## 8. Experimentación

Realizá nuevamente el ejercicio anterior.

Esta vez:

1. Creá dos copias del proyecto.
2. Modificá el mismo archivo desde ambas copias.
3. Realizá cambios diferentes.
4. Intentá combinar manualmente los cambios.
5. Registrá las dificultades que encontraste.

No busques una solución perfecta.

El objetivo es experimentar.

---

## 9. Puesta en común

Después de realizar la actividad, discutí con tus compañeros:

### Sobre las versiones

* ¿Cuántas copias terminamos teniendo?
* ¿Es fácil saber cuál es la correcta?
* ¿Es fácil recuperar una versión anterior?

### Sobre los cambios

* ¿Podemos saber exactamente qué cambió?
* ¿Podemos saber quién hizo cada cambio?
* ¿Podemos explicar por qué se hizo?

### Sobre la colaboración

* ¿Qué ocurre cuando dos personas modifican el mismo archivo?
* ¿Qué significa "integrar" dos trabajos?
* ¿Qué información necesitamos para hacerlo correctamente?

---

## 10. El problema que necesitamos resolver

A partir de la experiencia anterior, intentá escribir con tus propias palabras qué debería permitirnos una herramienta destinada a controlar las versiones de un proyecto.

Como mínimo, debería permitir:

* registrar cambios;
* conservar versiones;
* consultar el historial;
* comparar estados;
* recuperar información;
* trabajar sobre diferentes líneas de trabajo;
* compartir cambios;
* colaborar con otras personas.

Todavía no necesitamos saber cómo hacerlo.

Primero necesitamos saber **qué problema queremos resolver**.

---

## 11. Primera aproximación a Git

Ahora sí podemos introducir Git.

Git es un sistema de control de versiones distribuido que permite registrar y gestionar la evolución de un proyecto.

A diferencia de nuestro procedimiento manual, Git mantiene información estructurada sobre los cambios realizados.

La carpeta del proyecto puede convertirse en un repositorio Git.

A partir de ese momento, Git comenzará a gestionar la evolución del proyecto.

---

## 12. Una comparación

Volvamos a nuestro ejemplo.

### Sin Git

```text
mi-proyecto/
mi-proyecto-v2/
mi-proyecto-v3/
mi-proyecto-v3-final/
mi-proyecto-v3-final-definitivo/
```

### Con Git

```text
mi-proyecto/
│
├── README.md
├── objetivos.md
└── integrantes.md

        +
        
       Git
        │
        ▼
     Historial
```

La diferencia fundamental no es simplemente que Git "guarde versiones".

Git permite construir y consultar un historial estructurado de la evolución del proyecto.

---

## 13. Primer contacto con un repositorio

En esta etapa no vamos a estudiar todavía todo el funcionamiento interno de Git.

Solamente queremos observar qué sucede cuando un proyecto comienza a estar bajo control de versiones.

Abrí Visual Studio Code y prepará una carpeta llamada:

```text
laboratorio-git/
```

Dentro de ella creá:

```text
README.md
```

Con el siguiente contenido:

```md
# Laboratorio Git

Este repositorio será utilizado para experimentar con Git.
```

Por ahora, no hagas nada más.

Observá el proyecto.

---

## 14. Pregunta de cierre

Antes de continuar con el siguiente módulo, respondé:

> **Si mañana modificás diez veces este archivo, ¿cómo te gustaría poder saber qué cambió, cuándo cambió y cómo estaba anteriormente?**

Guardá tu respuesta.

No existe una única respuesta correcta.

La pregunta es el punto de partida para comprender por qué necesitamos Git.
