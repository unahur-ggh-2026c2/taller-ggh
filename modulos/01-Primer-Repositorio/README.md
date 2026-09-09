# Módulo 01 — Mi primer repositorio

> **Ya entendimos el problema. Ahora vamos a empezar a resolverlo con Git.**

---

## ¿Qué vamos a hacer?

En el módulo anterior trabajamos sobre el problema que aparece cuando un proyecto cambia y necesitamos conservar, consultar y organizar su evolución.

Ahora vamos a crear nuestro primer **repositorio Git** y comenzar a trabajar con él.

Vamos a pasar de esto:

```text
proyecto/
proyecto-v2/
proyecto-final/
proyecto-final-definitivo/
```

a una única carpeta cuyo historial será administrado por Git:

```text
proyecto/
├── README.md
├── objetivos.md
└── integrantes.md
```

Git se encargará de registrar la evolución del proyecto.

---

## ¿Qué vamos a aprender?

En este módulo vamos a trabajar con:

* instalación y configuración inicial de Git;
* identificación del usuario;
* configuración básica;
* creación de un repositorio;
* estructura de un repositorio Git;
* inicialización de un proyecto existente;
* repositorio local;
* estado del repositorio;
* archivos controlados y no controlados;
* relación entre la carpeta de trabajo y Git;
* `.git`;
* primera exploración del estado de un repositorio.

El objetivo principal es comprender **qué ocurre cuando una carpeta pasa a estar bajo control de Git**.

---

## Una carpeta no es todavía un repositorio

Podemos tener:

```text
mi-proyecto/
├── README.md
├── objetivos.md
└── integrantes.md
```

y todavía no estar utilizando Git.

Git necesita inicializar el proyecto para comenzar a administrar su evolución.

Conceptualmente:

```text
Carpeta común
     │
     │ inicializar Git
     ▼
Repositorio Git
     │
     ├── archivos del proyecto
     └── información administrada por Git
```

Este paso será nuestro primer contacto real con Git.

---

## El repositorio es local

En este módulo vamos a trabajar principalmente con un repositorio **local**.

Eso significa que Git estará administrando el proyecto en nuestra propia computadora.

Todavía no necesitamos GitHub.

Primero vamos a comprender cómo funciona Git localmente.

Más adelante incorporaremos el repositorio remoto y la sincronización con GitHub.

---

## ¿Qué vamos a observar?

Durante las prácticas vamos a prestar especial atención al estado del repositorio.

No alcanza con ejecutar un comando y comprobar que "funcionó".

Queremos entender:

* qué archivos está viendo Git;
* cuáles todavía no están bajo control de versiones;
* qué información administra Git;
* qué cambió después de cada operación;
* qué nos informa Git sobre el estado del proyecto.

La observación del estado del repositorio será una práctica permanente durante todo el curso.

---

## La carpeta `.git`

Cuando inicializamos un repositorio Git, aparece una carpeta especial:

```text
.git/
```

Esta carpeta contiene la información interna que Git necesita para administrar el repositorio.

No debemos modificarla manualmente.

Por ahora alcanza con comprender que:

> **La carpeta `.git` es la que convierte una carpeta común en un repositorio Git.**

Durante el curso vamos a trabajar con Git mediante sus comandos y herramientas, no modificando directamente el contenido interno de `.git`.

---

## Herramientas

Vamos a trabajar principalmente con:

* Git;
* Visual Studio Code;
* terminal;
* archivos Markdown.

Visual Studio Code será nuestro entorno de trabajo.

La terminal nos permitirá comenzar a interactuar directamente con Git y observar cómo responde ante nuestras acciones.

---

## Una idea importante

En este módulo todavía no vamos a preocuparnos por GitHub.

Primero necesitamos dominar este recorrido:

```text
Carpeta
   ↓
Repositorio
   ↓
Cambios
   ↓
Estado
   ↓
Registro
```

Los próximos módulos irán agregando nuevas piezas.

---

## Actividades

### Práctica

Actividad guiada para crear y explorar nuestro primer repositorio:

**[01 — Práctica](01-Practica.md)**

### Ejercicios

Actividades para consolidar los conceptos:

**[02 — Ejercicios](02-Ejercicios.md)**

### Desafíos

Situaciones para resolver con mayor autonomía:

**[03 — Desafíos](03-Desafios.md)**

### Proyecto

Actividad de integración:

**[04 — Proyecto](04-Proyecto.md)**

### Recursos

Material de consulta:

**[05 — Recursos](05-Recursos.md)**

---

## Antes de continuar

Al finalizar este módulo deberías poder explicar:

* qué es un repositorio Git;
* cómo convertir una carpeta en un repositorio;
* qué función cumple `.git`;
* qué diferencia existe entre una carpeta común y un repositorio;
* qué significa que un repositorio sea local;
* cómo consultar el estado de un repositorio.

Y, sobre todo:

> **deberías poder mirar una carpeta y saber si Git está administrando su evolución o no.**

---

## Idea central

> **Un repositorio Git es el punto de partida para comenzar a registrar la evolución de un proyecto.**

En el próximo módulo vamos a trabajar sobre lo que ocurre cuando **modificamos ese proyecto** y queremos guardar esos cambios correctamente.
