# Módulo 03 — Historial

> **Si Git registra la evolución de un proyecto, necesitamos aprender a leer esa historia.**

---

## ¿Qué vamos a aprender?

En los módulos anteriores aprendimos a:

- crear un repositorio;
- observar su estado;
- preparar cambios;
- registrar commits.

Ahora vamos a trabajar sobre una consecuencia natural de ese proceso:

> **¿Cómo podemos consultar y comprender lo que ocurrió en el proyecto?**

El historial de Git permite reconstruir la evolución registrada de un repositorio.

No se trata solamente de ejecutar:

```bash
git log
```

y mirar una lista de commits.

Vamos a aprender a interpretar esa información y utilizarla para responder preguntas sobre el proyecto.

---

## El historial como una historia

Cada commit representa un punto registrado en la evolución del proyecto.

Podemos imaginar:

```text
Commit 1
   ↓
Commit 2
   ↓
Commit 3
   ↓
Commit 4
```

Cada nuevo commit se incorpora al historial.

Por lo tanto, el historial permite observar cómo fue evolucionando el proyecto a través del tiempo.

---

## ¿Qué información conserva un commit?

Un commit contiene información que permite identificar, entre otras cosas:

- quién realizó el registro;
- cuándo fue realizado;
- qué mensaje lo describe;
- qué estado del proyecto representa;
- cómo se relaciona con otros commits.

Esta información permite reconstruir parte de la historia del proyecto.

---

## Consultar el historial

El comando básico es:

```bash
git log
```

También podemos utilizar:

```bash
git log --oneline
```

La segunda forma presenta una versión resumida, especialmente útil para obtener una visión rápida de la evolución.

---

## Leer, no solamente mirar

Ante un historial como:

```text
Crea documentación inicial
Agrega objetivos
Actualiza descripción
Corrige error de documentación
Incorpora instrucciones de uso
```

podemos comenzar a responder preguntas:

- ¿Qué ocurrió primero?
- ¿Qué se agregó después?
- ¿Cuándo se corrigió un problema?
- ¿Qué cambios fueron registrados?
- ¿Quién realizó determinado cambio?

El historial se convierte así en una herramienta de trabajo.

---

## Volver al pasado

Una de las características más importantes de Git es que conserva los estados registrados mediante commits.

Esto permite investigar cómo estaba el proyecto en determinados momentos.

Más adelante aprenderemos diferentes herramientas para:

- consultar un commit;
- comparar versiones;
- identificar cambios;
- recuperar información;
- investigar problemas.

En este módulo comenzaremos por comprender el historial antes de avanzar hacia esas operaciones.

---

## El identificador del commit

Cada commit posee un identificador único.

En Git este identificador se representa mediante un hash.

Por ejemplo:

```text
a84f9c2...
```

No es necesario memorizar estos identificadores.

Su importancia está en que permiten referirse a un commit específico.

Conceptualmente:

```text
Historial
   │
   ├── commit A
   ├── commit B
   ├── commit C
   └── commit D
          ↑
     identificador
```

---

## El historial no es solamente una lista

Los commits están relacionados entre sí.

Podemos representarlo inicialmente como:

```text
A ← B ← C ← D
```

Cada commit forma parte de una secuencia de evolución.

Esta relación será fundamental cuando trabajemos posteriormente con ramas y colaboración.

---

## ¿Qué vamos a practicar?

Durante este módulo vamos a:

- consultar el historial;
- interpretar commits;
- utilizar `git log`;
- utilizar `git log --oneline`;
- reconocer identificadores;
- observar autores y fechas;
- analizar mensajes;
- identificar la evolución de un proyecto;
- comparar diferentes estados;
- comenzar a investigar cambios registrados.

---

## Los mensajes vuelven a importar

En el módulo anterior vimos que un buen mensaje ayuda a construir un historial comprensible.

Ahora vamos a comprobar por qué.

Compará:

```text
cambios
update
arreglo
final
```

con:

```text
Crea estructura inicial
Agrega objetivos del proyecto
Corrige descripción del README
Actualiza instrucciones de instalación
```

El segundo historial permite reconstruir mucho mejor la evolución.

Por eso:

> **Un buen historial comienza con buenos commits.**

---

## El historial como herramienta de diagnóstico

Supongamos que alguien dice:

> "Antes funcionaba y ahora no."

Si tenemos un historial correctamente construido, podemos comenzar a investigar:

```text
Estado actual
      ↓
Historial
      ↓
Identificar cambios
      ↓
Comparar estados
      ↓
Buscar dónde apareció el problema
```

Esta forma de trabajar será especialmente importante cuando el proyecto crezca.

---

## ¿Qué deberías poder hacer al terminar?

Al finalizar el módulo deberías poder:

- consultar el historial;
- reconocer los elementos principales de un commit;
- interpretar una secuencia de commits;
- utilizar una vista resumida del historial;
- identificar un commit específico;
- explicar por qué los mensajes son importantes;
- utilizar el historial para investigar la evolución de un proyecto.

Y, sobre todo:

> **deberías poder mirar un historial y obtener información útil de él.**

---

## Actividades

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

> **El valor de un historial no está solamente en conservar cambios, sino en permitir comprender cómo y por qué evolucionó el proyecto.**

A partir de este módulo, Git deja de ser solamente una herramienta para registrar cambios y comienza a convertirse también en una herramienta para **investigar el pasado del proyecto**.