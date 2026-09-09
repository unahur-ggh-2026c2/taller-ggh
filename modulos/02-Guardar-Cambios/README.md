# Módulo 02 — Guardar cambios

> **Modificar un archivo no es lo mismo que registrar su cambio.**

---

## ¿Qué vamos a aprender?

En el módulo anterior creamos nuestro primer repositorio Git.

Ahora vamos a trabajar sobre una de las ideas fundamentales de Git:

> **¿Cómo registramos la evolución de un proyecto?**

Vamos a aprender a trabajar con el recorrido que realiza un cambio desde que modificamos un archivo hasta que queda registrado en el historial.

El flujo fundamental será:

```text
Modificar
    ↓
Observar
    ↓
Preparar
    ↓
Registrar
    ↓
Historial
```

Este recorrido va a aparecer una y otra vez durante todo el curso.

---

## Del archivo al historial

Supongamos que tenemos:

```text
README.md
```

y modificamos su contenido.

El archivo cambió, pero eso no significa que Git haya registrado ese cambio.

Podemos pensar inicialmente en tres espacios:

```text
┌──────────────────────┐
│ Carpeta de trabajo   │
│                      │
│ Archivos modificados │
└──────────┬───────────┘
           │
           │ preparar
           ▼
┌──────────────────────┐
│ Área de preparación  │
│                      │
│ Cambios seleccionados│
└──────────┬───────────┘
           │
           │ registrar
           ▼
┌──────────────────────┐
│ Historial            │
│                      │
│ Commits              │
└──────────────────────┘
```

Comprender este recorrido es mucho más importante que memorizar una lista de comandos.

---

## ¿Qué es un commit?

Un **commit** es un registro de cambios dentro del historial de un repositorio.

Podemos pensarlo como un punto concreto de la evolución del proyecto.

Cada commit contiene información que permite identificar, entre otras cosas:

- qué cambios fueron registrados;
- quién los registró;
- cuándo fueron registrados;
- qué mensaje describe el cambio;
- cómo se relaciona ese registro con el historial.

Los commits serán fundamentales para poder consultar posteriormente cómo evolucionó el proyecto.

---

## `git add` no guarda en el historial

Esta diferencia es fundamental.

Cuando ejecutamos:

```bash
git add README.md
```

estamos preparando un cambio.

Todavía no estamos creando un commit.

Después:

```bash
git commit -m "Actualiza README"
```

registramos los cambios que habían sido preparados.

Por eso:

```text
git add
   ↓
preparar

git commit
   ↓
registrar
```

---

## ¿Por qué existe una etapa intermedia?

Puede parecer innecesario tener que preparar un cambio antes de registrarlo.

Pero esta separación nos permite decidir exactamente **qué cambios queremos incluir en cada commit**.

Por ejemplo, podemos modificar:

```text
README.md
objetivos.md
integrantes.md
```

y decidir registrar solamente:

```text
README.md
objetivos.md
```

mientras dejamos `integrantes.md` para otro momento.

Esto permite construir un historial más claro y significativo.

---

## El mensaje del commit

Un commit debería tener un mensaje que permita comprender qué cambio fue registrado.

No es recomendable utilizar mensajes como:

```text
cambios
```

o:

```text
cosas
```

o:

```text
update
```

Es preferible algo como:

```text
Agrega descripción inicial del proyecto
```

o:

```text
Actualiza objetivos del proyecto
```

Un buen historial debería poder leerse como una historia de la evolución del proyecto.

---

## El estado del repositorio

Durante este módulo vamos a utilizar permanentemente:

```bash
git status
```

No como una formalidad, sino como herramienta de observación.

Después de cada modificación importante preguntate:

> **¿Qué sabe Git sobre lo que acaba de ocurrir?**

Y después de cada operación:

> **¿Qué cambió en el estado del repositorio?**

---

## El flujo que vamos a practicar

Durante las actividades vamos a repetir:

```text
1. Modificar un archivo
        ↓
2. Consultar el estado
        ↓
3. Preparar el cambio
        ↓
4. Consultar el estado
        ↓
5. Crear un commit
        ↓
6. Consultar el estado nuevamente
```

La repetición tiene un propósito.

Queremos que este recorrido se convierta en un hábito de trabajo.

---

## Los cambios son selectivos

Git no obliga a registrar todo lo que modificamos en un único commit.

Podemos seleccionar qué cambios queremos registrar.

Esto permite que un proyecto tenga un historial más comprensible.

Por ejemplo:

```text
Commit 1
Crea documentación inicial

Commit 2
Agrega objetivos

Commit 3
Actualiza integrantes

Commit 4
Corrige descripción del proyecto
```

Es preferible esto a:

```text
Commit 1
cambios
```

que contenga modificaciones completamente diferentes realizadas durante varios días.

---

## ¿Qué vamos a practicar?

Durante este módulo vamos a:

- modificar archivos;
- consultar el estado;
- interpretar cambios;
- preparar archivos;
- crear commits;
- escribir mensajes significativos;
- registrar cambios selectivamente;
- consultar el historial;
- reconocer un repositorio limpio;
- identificar cambios pendientes;
- comprender la diferencia entre trabajar y registrar.

---

## Algo importante: guardar no es registrar

Cuando presionás `Ctrl + S` en Visual Studio Code, guardás el archivo en el disco.

Eso **no crea un commit**.

Son operaciones diferentes:

```text
Ctrl + S
   ↓
Guardar archivo

git add
   ↓
Preparar cambio

git commit
   ↓
Registrar cambio en Git
```

Esta distinción va a ser una de las más importantes del módulo.

---

## ¿Qué deberías poder hacer al terminar?

Al finalizar el módulo deberías poder:

- modificar archivos dentro de un repositorio;
- consultar qué cambios detecta Git;
- preparar cambios;
- crear commits;
- escribir mensajes descriptivos;
- decidir qué cambios incluir en cada commit;
- interpretar el estado del repositorio;
- explicar la diferencia entre `git add` y `git commit`.

Pero, sobre todo:

> **deberías comprender qué está ocurriendo en cada etapa y no limitarte a repetir una receta.**

---

## Actividades

### Guía docente

**[00 — Guía del Docente](00-Guia-Docente.md)**

### Práctica

**[01 — Práctica](01-Practica.md)**

### Ejercicios

**[02 — Ejercicios](02-Ejercicios.md)**

### Desafíos

**[03 — Desafíos](03-Desafios.md)**

### Proyecto

**[04 — Proyecto](04-Proyecto.md)**

### Recursos

**[05 — Recursos](05-Recursos.md)**

---

## Idea central

> **Un archivo puede cambiar muchas veces. Un commit representa una decisión consciente de registrar un estado de esos cambios en la historia del proyecto.**

El próximo paso será aprender a consultar esa historia y comprender qué nos puede contar sobre la evolución del proyecto.