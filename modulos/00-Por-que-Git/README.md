# Módulo 00 — ¿Por qué Git?

> **Antes de aprender Git, necesitamos entender por qué existe.**

---

## ¿Qué problema intenta resolver Git?

Cuando un proyecto evoluciona, sus archivos cambian.

Una modificación puede mejorar el proyecto, pero también puede introducir un error. Dos personas pueden modificar el mismo archivo. Podemos necesitar recuperar una versión anterior o saber exactamente qué cambió.

Una estrategia habitual consiste en crear copias:

```text
proyecto/
proyecto-v2/
proyecto-v2-corregido/
proyecto-final/
proyecto-final-definitivo/
```

Funciona... hasta que deja de funcionar.

¿Cuál es la versión correcta?

¿Qué cambió entre una y otra?

¿Quién hizo cada modificación?

¿Podemos recuperar exactamente el estado que tenía el proyecto hace una semana?

¿Y qué pasa si dos personas trabajaron sobre el mismo archivo?

Estas son algunas de las situaciones que intenta resolver un **sistema de control de versiones**.

---

## ¿Qué vamos a aprender?

En este módulo vamos a construir las ideas que necesitamos para comprender Git:

* qué es el control de versiones;
* qué problemas aparecen cuando administramos versiones manualmente;
* qué es Git;
* qué es un repositorio;
* qué significa registrar un cambio;
* qué es un historial;
* por qué resulta útil conservar la evolución de un proyecto;
* qué problemas aparecen cuando varias personas trabajan simultáneamente;
* qué diferencia existe entre Git y GitHub.

Todavía no vamos a aprender una gran cantidad de comandos.

Primero vamos a entender **el problema**.

---

## Aprender haciendo

Vamos a trabajar con un proyecto sencillo construido mediante archivos Markdown.

Durante las actividades vamos a experimentar situaciones como:

```text
crear
  ↓
modificar
  ↓
guardar una nueva versión
  ↓
modificar nuevamente
  ↓
comparar
  ↓
recuperar
  ↓
trabajar con otra persona
  ↓
intentar integrar cambios
```

La idea es que los problemas aparezcan antes de aprender las herramientas que permiten resolverlos.

---

## ¿Por qué usamos Markdown?

No necesitamos comenzar trabajando con código para aprender Git.

Los archivos Markdown nos permiten concentrarnos en el problema del control de versiones sin agregar la complejidad de compilar o ejecutar un programa.

Un archivo de texto puede:

* modificarse;
* compararse;
* versionarse;
* compartirse;
* integrarse;
* entrar en conflicto.

Lo que aprendamos acá podrá aplicarse posteriormente a proyectos de programación.

---

## Git y GitHub no son lo mismo

Una distinción fundamental desde el comienzo:

**Git** es un sistema de control de versiones distribuido.

**GitHub** es una plataforma que permite alojar repositorios Git y proporciona herramientas para compartir y colaborar sobre ellos.

Podemos pensar inicialmente en:

```text
Git
│
└── Repositorio local
       │
       │ sincronización
       ▼
    GitHub
       │
       └── Repositorio remoto
```

La relación entre ambos se desarrollará con mayor profundidad más adelante.

---

## ¿Qué tenés que llevarte de este módulo?

No necesitás salir de este módulo sabiendo comandos de Git.

Necesitás poder explicar, con tus propias palabras:

> **¿Qué problema resuelve Git que resulta difícil resolver utilizando solamente copias de nuestros archivos?**

Si podés responder esa pregunta con un ejemplo concreto, estamos listos para empezar a utilizar Git.

---

## Actividades

### Práctica

Comenzá por:

**[01 — Práctica](01-Practica.md)**

### Ejercicios

Después de realizar la práctica:

**[02 — Ejercicios](02-Ejercicios.md)**

### Desafíos

Cuando quieras poner a prueba tu comprensión:

**[03 — Desafíos](03-Desafios.md)**

### Proyecto

Para integrar lo trabajado:

**[04 — Proyecto](04-Proyecto.md)**

### Recursos

Material de consulta y profundización:

**[05 — Recursos](05-Recursos.md)**

---

## Idea central

> **Los proyectos cambian. Git nos permite registrar y comprender esos cambios.**

Ese es el punto de partida.

A partir del próximo módulo vamos a dejar de imaginar cómo debería funcionar una herramienta de control de versiones y vamos a empezar a utilizar Git para comprobarlo.
