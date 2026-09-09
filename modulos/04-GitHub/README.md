# Módulo 04 — GitHub

> **Git nos permite gestionar la historia del proyecto. GitHub nos permite compartirla y trabajar con otras personas.**

---

## ¿Qué vamos a aprender?

Hasta este punto trabajamos con Git de manera local.

Creamos repositorios, registramos cambios y consultamos su historial.

Ahora vamos a incorporar GitHub como plataforma para alojar repositorios Git y facilitar su publicación, acceso y colaboración.

El recorrido será:

```text
Repositorio local
       ↓
Git
       ↓
GitHub
       ↓
Repositorio remoto
       ↓
Intercambio de cambios
```

---

## Git y GitHub no son lo mismo

Es importante establecer esta diferencia desde el comienzo.

**Git** es un sistema de control de versiones.

**GitHub** es una plataforma que permite alojar repositorios Git y proporciona herramientas adicionales para trabajar sobre ellos.

Podemos pensar inicialmente:

```text
Git
│
├── Control de versiones
├── Commits
├── Historial
└── Trabajo local
```

y:

```text
GitHub
│
├── Repositorios remotos
├── Publicación
├── Colaboración
├── Documentación
└── Herramientas de trabajo
```

GitHub utiliza Git, pero Git no depende de GitHub.

---

## ¿Por qué incorporar GitHub?

Un repositorio local permite conservar la historia de un proyecto en nuestra computadora.

Pero un proyecto real puede necesitar:

- compartir el código;
- disponer de una copia remota;
- acceder al proyecto desde diferentes equipos;
- colaborar con otras personas;
- publicar documentación;
- revisar cambios;
- organizar el trabajo.

GitHub proporciona un entorno para realizar estas actividades.

---

## Repositorio local y remoto

A partir de este módulo vamos a trabajar con dos repositorios relacionados:

```text
Computadora
┌──────────────────────┐
│ Repositorio local    │
│                      │
│ Git                  │
└──────────┬───────────┘
           │
           │ intercambio
           ▼
┌──────────────────────┐
│ Repositorio remoto   │
│                      │
│ GitHub               │
└──────────────────────┘
```

El repositorio local continúa siendo un repositorio Git.

GitHub proporciona el repositorio remoto.

---

## Publicar un repositorio

Una de las primeras tareas será aprender a llevar un repositorio local a GitHub.

El proceso conceptual será:

```text
Proyecto local
      ↓
Repositorio Git
      ↓
Repositorio remoto
      ↓
GitHub
```

No se trata simplemente de "subir archivos".

Lo que se comparte es un repositorio Git y su historia.

---

## Remotos

Git permite asociar un repositorio local con uno o más repositorios remotos.

Un remoto es una referencia a otro repositorio Git.

Habitualmente utilizaremos un nombre convencional:

```text
origin
```

Por ejemplo:

```text
Repositorio local
       │
       └── origin ──→ GitHub
```

El nombre `origin` no representa a GitHub.

Es simplemente el nombre que normalmente se utiliza para identificar el remoto principal.

---

## Enviar cambios

Cuando realizamos nuevos commits localmente, esos cambios pertenecen inicialmente al repositorio local.

Para enviarlos al repositorio remoto utilizaremos:

```bash
git push
```

Conceptualmente:

```text
Local
  │
  │ git push
  ▼
GitHub
```

El objetivo es comprender primero esta relación antes de incorporar escenarios de colaboración más complejos.

---

## Obtener cambios

El flujo también puede producirse en sentido contrario.

Un repositorio remoto puede contener cambios que todavía no están presentes localmente.

Git proporciona herramientas para obtener esos cambios.

Entre ellas trabajaremos con:

```bash
git pull
```

Conceptualmente:

```text
GitHub
  │
  │ git pull
  ▼
Local
```

La comprensión de este flujo será fundamental para el módulo posterior de trabajo colaborativo.

---

## Una nueva dimensión del proyecto

Hasta ahora nuestro modelo era:

```text
Cambios
   ↓
Commits
   ↓
Historial
```

Ahora incorporamos:

```text
Cambios
   ↓
Commits
   ↓
Historial
   ↓
Repositorio remoto
```

Esto permite que la historia del proyecto pueda ser compartida.

---

## GitHub como espacio de trabajo

GitHub no se limita al almacenamiento de repositorios.

La plataforma incorpora herramientas que pueden utilizarse para:

- documentar proyectos;
- consultar código;
- revisar cambios;
- colaborar;
- gestionar tareas;
- publicar información;
- construir un perfil profesional.

Algunas de estas funcionalidades serán abordadas en este módulo y otras se desarrollarán posteriormente.

---

## README y documentación

Los repositorios de GitHub suelen utilizar un archivo:

```text
README.md
```

como punto de entrada al proyecto.

Este archivo permite explicar:

- qué es el proyecto;
- para qué sirve;
- cómo utilizarlo;
- cómo participar;
- dónde encontrar información adicional.

La documentación mediante Markdown será profundizada en un módulo específico.

En este módulo nos interesa principalmente comprender su función dentro del repositorio publicado.

---

## Perfil y repositorios públicos

GitHub también puede funcionar como espacio de presentación de proyectos.

Un repositorio correctamente organizado permite mostrar:

- proyectos realizados;
- documentación;
- evolución;
- conocimientos técnicos;
- capacidad de trabajo con Git;
- participación en proyectos colaborativos.

El desarrollo del perfil profesional será trabajado posteriormente.

---

## ¿Qué vamos a practicar?

Durante este módulo vamos a:

- crear o utilizar una cuenta de GitHub;
- comprender la relación entre Git y GitHub;
- crear repositorios remotos;
- vincular un repositorio local con un remoto;
- identificar el remoto `origin`;
- publicar commits;
- utilizar `git push`;
- obtener cambios;
- utilizar `git pull`;
- consultar repositorios desde GitHub;
- reconocer GitHub como espacio de colaboración.

---

## ¿Qué deberías poder hacer al terminar?

Al finalizar el módulo deberías poder:

- explicar la diferencia entre Git y GitHub;
- distinguir repositorio local y remoto;
- vincular un repositorio local con GitHub;
- identificar un remoto;
- publicar cambios;
- obtener cambios desde un repositorio remoto;
- interpretar la relación entre el repositorio local y el remoto;
- reconocer algunas de las posibilidades que GitHub ofrece para trabajar sobre proyectos.

Y, fundamentalmente:

> **deberías poder pasar de trabajar únicamente en tu computadora a mantener un proyecto Git conectado con un repositorio remoto en GitHub.**

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

> **Git gestiona la historia del proyecto; GitHub permite compartir esa historia y construir un espacio de trabajo alrededor de ella.**

A partir de este módulo, nuestro repositorio deja de vivir únicamente en nuestra computadora y comienza a formar parte de un entorno remoto que podemos compartir, consultar y utilizar para colaborar.