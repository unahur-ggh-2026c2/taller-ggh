# Módulo 07 — Trabajo Colaborativo

> **Git permite registrar cambios. El trabajo colaborativo consiste en organizar cómo distintas personas producen, revisan e integran esos cambios.**

---

## ¿Qué vamos a aprender?

Hasta ahora aprendimos a trabajar con Git de manera individual.

Creamos repositorios, registramos cambios, consultamos el historial, trabajamos con GitHub y aprendimos a utilizar ramas:

```text
Repositorio
    ↓
Cambios
    ↓
Commits
    ↓
Ramas
    ↓
Historial
```

Ahora vamos a incorporar una nueva dimensión:

```text
Persona A
     \
      \
       → Repositorio ←
      /
     /
Persona B
```

El proyecto deja de ser solamente nuestro.

Otras personas pueden:

- consultar el código;
- crear ramas;
- realizar cambios;
- publicar trabajo;
- revisar modificaciones;
- proponer integraciones;
- detectar problemas;
- aportar mejoras.

El desafío ya no es solamente saber utilizar Git.

El desafío es **coordinar cambios realizados por diferentes personas sobre un mismo proyecto**.

---

# ¿Por qué necesitamos un flujo de trabajo?

Imaginemos un repositorio utilizado por varias personas.

Cada una puede trabajar sobre una funcionalidad diferente:

```text
                    feature-A
                   /
main ─────────────
                   \
                    feature-B
```

Si todas modificaran directamente `main`, rápidamente aparecerían problemas:

- cambios mezclados;
- dificultades para revisar;
- commits poco claros;
- modificaciones que todavía no están terminadas;
- conflictos;
- dificultad para saber quién hizo qué;
- incorporación accidental de cambios.

Necesitamos entonces un flujo que permita:

```text
trabajar
   ↓
registrar
   ↓
publicar
   ↓
revisar
   ↓
integrar
```

---

# Git y GitHub

Git y GitHub cumplen funciones relacionadas, pero diferentes.

## Git

Git es el sistema de control de versiones.

Permite:

- registrar cambios;
- crear commits;
- trabajar con ramas;
- consultar historial;
- comparar cambios;
- integrar líneas de trabajo.

## GitHub

GitHub proporciona una plataforma donde podemos alojar repositorios Git y facilitar el trabajo entre personas.

Permite, entre otras cosas:

- compartir repositorios;
- publicar ramas;
- realizar Pull Requests;
- revisar cambios;
- comentar;
- gestionar Issues;
- coordinar trabajo.

Una representación simplificada es:

```text
Git
 ↓
control de versiones

GitHub
 ↓
colaboración alrededor del repositorio
```

---

# Repositorio compartido

Un equipo puede trabajar sobre un mismo repositorio:

```text
                 GitHub
                    │
          ┌─────────┼─────────┐
          │         │         │
       Persona A Persona B Persona C
          │         │         │
          ↓         ↓         ↓
        Git       Git       Git
```

Cada persona tiene normalmente una copia local del repositorio.

El repositorio remoto actúa como punto de coordinación.

---

# Clonar un repositorio

Para comenzar a trabajar sobre un repositorio existente podemos clonarlo:

```bash
git clone URL_DEL_REPOSITORIO
```

Esto permite obtener una copia local del proyecto.

El recorrido conceptual es:

```text
GitHub
   ↓
git clone
   ↓
Repositorio local
   ↓
Trabajo
```

---

# Identidad dentro del proyecto

Cuando varias personas realizan cambios, los commits deben permitir identificar quién los realizó.

Git utiliza información de autor asociada a cada commit.

Podemos consultar la configuración mediante:

```bash
git config --list
```

La identidad debe estar correctamente configurada antes de comenzar a trabajar.

---

# Ramas para trabajar en equipo

En un flujo colaborativo, las ramas permiten separar el trabajo de cada línea de desarrollo.

Por ejemplo:

```text
main
 │
 ├── feature-login
 ├── feature-busqueda
 └── fix-documentacion
```

Cada rama representa una intención concreta.

Esto permite evitar que todo el trabajo se mezcle inmediatamente en la rama principal.

---

# El flujo básico

Un flujo colaborativo sencillo puede representarse:

```text
main
  ↓
crear rama
  ↓
trabajar
  ↓
commit
  ↓
push
  ↓
Pull Request
  ↓
revisión
  ↓
merge
```

Este flujo será el eje central del módulo.

---

# Pull Request

Una **Pull Request** es una propuesta para incorporar cambios de una rama en otra.

Por ejemplo:

```text
feature-login
      ↓
Pull Request
      ↓
main
```

La Pull Request permite que otras personas puedan revisar el trabajo antes de integrarlo.

Puede incluir:

- descripción;
- cambios realizados;
- comentarios;
- revisión;
- discusión;
- correcciones;
- aprobación;
- integración.

---

# Una Pull Request no es un commit

Es importante diferenciar:

```text
commit
```

de:

```text
Pull Request
```

Un commit registra un cambio en la historia.

Una Pull Request es un mecanismo de colaboración para proponer y revisar cambios.

Podemos representarlo:

```text
cambios
   ↓
commits
   ↓
rama
   ↓
Pull Request
   ↓
revisión
   ↓
integración
```

---

# Revisar antes de integrar

Uno de los objetivos principales del trabajo colaborativo es evitar que los cambios lleguen directamente a la línea principal sin revisión.

Una persona puede proponer:

```text
feature
```

y otra puede revisar:

```text
¿Qué cambió?
¿Está correcto?
¿Cumple el objetivo?
¿Hay problemas?
¿Hace falta modificar algo?
```

La revisión puede producir nuevos cambios antes de la integración.

---

# Comentarios y discusión

Una Pull Request permite discutir los cambios.

La conversación puede centrarse en:

- decisiones técnicas;
- errores;
- mejoras;
- estilo;
- documentación;
- pruebas;
- posibles problemas.

La discusión queda asociada al cambio.

Esto permite que el conocimiento del proceso no dependa exclusivamente de conversaciones externas.

---

# Issue

GitHub también permite registrar problemas, tareas o propuestas mediante **Issues**.

Una Issue puede representar:

```text
problema
tarea
mejora
idea
bug
```

Por ejemplo:

```text
Issue #15
Corregir instalación en Windows
```

Después puede crearse una rama para resolverla:

```text
fix-instalacion-windows
```

y finalmente proponer una Pull Request.

---

# Issue y Pull Request

Son conceptos diferentes.

Una forma sencilla de distinguirlos:

```text
Issue
  ↓
¿Qué problema o tarea tenemos?

Pull Request
  ↓
¿Qué cambios proponemos para resolverlo?
```

Pueden relacionarse entre sí.

Por ejemplo:

```text
Issue #15
    ↓
fix-instalacion
    ↓
Pull Request
    ↓
merge
    ↓
Issue resuelta
```

---

# Push

Cuando trabajamos localmente, nuestros commits existen en nuestro repositorio local.

Para publicarlos:

```bash
git push
```

El recorrido es:

```text
commit local
     ↓
git push
     ↓
repositorio remoto
```

Esto permite que otras personas puedan acceder a nuestro trabajo.

---

# Pull

Si otras personas realizaron cambios en el repositorio remoto, necesitamos actualizar nuestra copia local.

Una operación habitual es:

```bash
git pull
```

Conceptualmente:

```text
repositorio remoto
       ↓
git pull
       ↓
repositorio local actualizado
```

Durante este módulo vamos a prestar especial atención a qué ocurre cuando distintas personas trabajan sobre el mismo proyecto.

---

# Fetch

También podemos obtener información del repositorio remoto sin integrar inmediatamente esos cambios en nuestra rama actual:

```bash
git fetch
```

Conceptualmente:

```text
GitHub
  ↓
git fetch
  ↓
información remota actualizada
```

La diferencia entre `fetch` y `pull` será trabajada mediante ejemplos.

---

# Sincronización

En un equipo, el repositorio remoto cambia constantemente.

Podemos tener:

```text
Persona A
   ↓
push
   ↓
GitHub
   ↑
   │
Persona B
   ↑
pull
```

Por eso trabajar colaborativamente implica aprender a sincronizar los repositorios.

---

# Conflictos colaborativos

Los conflictos pueden aparecer cuando diferentes personas modifican partes incompatibles del proyecto.

Por ejemplo:

```text
Persona A
    ↓
modifica archivo X

Persona B
    ↓
modifica la misma parte de archivo X
```

Al intentar integrar los cambios, Git puede no saber qué resultado corresponde.

Entonces:

```text
cambios diferentes
       ↓
conflicto
       ↓
análisis
       ↓
decisión
       ↓
resolución
```

---

# Resolver conflictos es una actividad colaborativa

Un conflicto no debe entenderse solamente como un problema de Git.

También representa una decisión sobre el proyecto.

Ante:

```text
versión A
```

y:

```text
versión B
```

alguien debe determinar:

```text
¿qué resultado necesita el proyecto?
```

La herramienta ayuda a combinar cambios.

La decisión pertenece al equipo.

---

# Convenciones de trabajo

Cuando varias personas trabajan sobre un repositorio, resulta útil acordar reglas.

Por ejemplo:

- cómo nombrar ramas;
- cómo escribir commits;
- qué debe contener una Pull Request;
- quién revisa cambios;
- cuándo se puede integrar;
- qué archivos no deben modificarse;
- cómo resolver conflictos.

Estas reglas pueden documentarse en el repositorio.

---

# CONTRIBUTING.md

GitHub permite utilizar un archivo:

```text
CONTRIBUTING.md
```

para documentar las pautas de contribución de un proyecto.

Puede incluir:

- cómo comenzar;
- cómo crear ramas;
- cómo realizar commits;
- cómo abrir Issues;
- cómo crear Pull Requests;
- criterios de revisión;
- normas del proyecto.

Este archivo será utilizado como parte de las actividades del módulo.

---

# CODE_OF_CONDUCT.md

Los proyectos colaborativos también pueden establecer pautas de convivencia mediante:

```text
CODE_OF_CONDUCT.md
```

Este archivo puede establecer principios para la participación dentro del proyecto.

No es el objetivo principal de este módulo, pero forma parte de las herramientas que pueden acompañar un proyecto abierto.

---

# README y colaboración

El `README.md` continúa siendo importante.

En un proyecto colaborativo debe permitir comprender:

- qué es el proyecto;
- cómo comenzar;
- cómo utilizarlo;
- dónde encontrar información;
- cómo contribuir, cuando corresponda.

Podemos tener:

```text
README.md
CONTRIBUTING.md
CODE_OF_CONDUCT.md
```

Cada archivo tiene un propósito diferente.

---

# Revisiones

Una revisión no consiste solamente en buscar errores.

También puede servir para:

- compartir conocimiento;
- detectar riesgos;
- mejorar diseño;
- mejorar documentación;
- mantener coherencia;
- aprender de otras personas.

Una buena revisión debe centrarse en el trabajo y no en la persona.

---

# El flujo completo

Durante el módulo vamos a trabajar con un flujo como este:

```text
             Issue
               ↓
          crear rama
               ↓
             trabajo
               ↓
            commits
               ↓
              push
               ↓
         Pull Request
               ↓
            revisión
               ↓
          correcciones
               ↓
            aprobación
               ↓
             merge
               ↓
          actualizar main
```

No todas las situaciones reales requieren exactamente este recorrido, pero constituye un modelo útil para comprender el proceso.

---

# Protección de `main`

En proyectos colaborativos puede ser conveniente evitar que cualquier persona pueda modificar directamente `main`.

GitHub permite establecer reglas de protección.

Conceptualmente:

```text
main
 ↓
protegida
 ↓
cambios mediante Pull Request
```

Esto ayuda a reducir la posibilidad de incorporar cambios sin revisión.

---

# Trabajo colaborativo y responsabilidad

Trabajar en equipo implica comprender que nuestros cambios pueden afectar a otras personas.

Antes de publicar un cambio conviene preguntarse:

```text
¿Funciona?
¿Está documentado?
¿El commit es claro?
¿La rama tiene un propósito?
¿La Pull Request explica el cambio?
¿Hay archivos innecesariamente modificados?
```

La calidad técnica y la calidad de comunicación forman parte del mismo proceso.

---

# ¿Qué vamos a practicar?

Durante este módulo vamos a:

- clonar repositorios;
- configurar la identidad de Git;
- trabajar con repositorios compartidos;
- crear ramas para tareas;
- publicar ramas;
- utilizar `push`;
- utilizar `fetch`;
- utilizar `pull`;
- crear Issues;
- relacionar Issues con cambios;
- crear Pull Requests;
- revisar cambios;
- realizar comentarios;
- responder observaciones;
- corregir una Pull Request;
- integrar cambios;
- resolver conflictos;
- documentar pautas de contribución.

---

# ¿Qué deberías poder hacer al terminar?

Al finalizar el módulo deberías poder:

- explicar la diferencia entre Git y GitHub;
- trabajar sobre un repositorio compartido;
- crear una rama para una tarea;
- publicar una rama;
- sincronizar cambios;
- comprender la función de una Issue;
- crear una Pull Request;
- explicar qué se revisa en una Pull Request;
- realizar y recibir comentarios;
- corregir cambios solicitados;
- comprender un conflicto colaborativo;
- participar de una integración;
- documentar reglas básicas de contribución.

Y fundamentalmente:

> **deberías poder participar en un proyecto colaborativo sin depender de que otra persona te explique cada paso.**

---

# Actividades

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

# Idea central

Hasta ahora aprendimos a gestionar nuestra propia historia.

Ahora debemos aprender a gestionar una historia construida por varias personas.

El cambio conceptual es:

```text
Trabajo individual

       ↓

Repositorio
       ↓
Commits
       ↓
Ramas
       ↓
GitHub
```

hacia:

```text
Trabajo colaborativo

Persona A ─┐
Persona B ─┼→ Ramas → Pull Requests → Revisión → Integración
Persona C ─┘
```

El objetivo no es simplemente aprender a usar Pull Requests.

Es comprender un flujo de trabajo donde:

```text
cada cambio
    ↓
queda registrado
    ↓
puede ser revisado
    ↓
puede ser discutido
    ↓
puede ser mejorado
    ↓
puede ser integrado
```

> **Colaborar no significa que varias personas editen el mismo archivo al mismo tiempo. Significa coordinar cambios sobre un mismo proyecto de manera que la historia siga siendo comprensible, revisable y confiable.**