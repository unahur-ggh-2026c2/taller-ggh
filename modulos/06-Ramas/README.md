# Módulo 06 — Ramas

> **Las ramas permiten trabajar sobre distintas líneas de evolución de un proyecto sin perder su historia.**

---

## ¿Qué vamos a aprender?

Hasta este punto trabajamos con repositorios, commits, historial, GitHub y documentación.

Nuestro trabajo se desarrolló principalmente sobre una única línea de evolución:

```text
A
↓
B
↓
C
↓
D
```

Ahora vamos a incorporar una de las características fundamentales de Git:

**las ramas.**

Una rama permite crear una nueva línea de trabajo a partir de un punto determinado de la historia.

El recorrido conceptual será:

```text
                 C
                /
A ───── B ─────
                \
                 D
```

A partir de un mismo punto pueden existir diferentes líneas de evolución.

---

## ¿Por qué necesitamos ramas?

Imaginemos que tenemos un proyecto funcionando:

```text
A ── B ── C
```

Queremos desarrollar una nueva característica.

Podríamos continuar directamente:

```text
A ── B ── C ── D
```

Pero mientras desarrollamos esa característica puede ocurrir que:

- necesitemos corregir un error;
- queramos experimentar;
- tengamos que trabajar en otra funcionalidad;
- otra persona necesite trabajar sobre una parte diferente;
- todavía no queramos incorporar nuestros cambios a la línea principal.

Las ramas permiten separar esas líneas de trabajo.

---

## Una rama no es una copia independiente

Una rama no debe imaginarse simplemente como:

> "otra carpeta con otra versión del proyecto".

Una rama es una referencia dentro de la historia de Git que permite trabajar sobre una determinada línea de commits.

Podemos representarlo de manera simplificada:

```text
A ── B ── C
          ↑
        main
```

Creamos una nueva rama:

```text
A ── B ── C
          ↑
        main
          \
           D
            ↑
         nueva-rama
```

Ahora existen dos líneas de evolución.

---

## Crear una rama

Podemos crear una rama mediante:

```bash
git branch nueva-rama
```

Después podemos cambiar a ella mediante:

```bash
git switch nueva-rama
```

También podemos crearla y cambiar directamente a ella:

```bash
git switch -c nueva-rama
```

Durante el módulo trabajaremos principalmente con `git switch` porque hace explícita la idea de cambiar de línea de trabajo.

---

## Consultar las ramas

Para consultar las ramas locales:

```bash
git branch
```

Git indicará cuál es la rama actual.

Por ejemplo:

```text
* main
  nueva-rama
```

El símbolo:

```text
*
```

indica la rama en la que estamos trabajando.

---

## Cambiar de rama

Para cambiar de una rama a otra:

```bash
git switch main
```

o:

```bash
git switch nueva-rama
```

El cambio de rama modifica el estado de los archivos del directorio de trabajo para representar la historia correspondiente a esa rama.

---

## Crear una línea de trabajo

Supongamos:

```text
A ── B ── C
          ↑
        main
```

Creamos:

```bash
git switch -c nueva-funcionalidad
```

Ahora:

```text
A ── B ── C
          ↑
        main
          ↑
     nueva-funcionalidad
```

Realizamos un cambio y hacemos un commit:

```text
A ── B ── C ── D
          ↑     ↑
        main  nueva-funcionalidad
```

La rama `main` continúa apuntando a `C`.

La nueva rama apunta a `D`.

---

## Las ramas avanzan

Una característica importante es que una rama se mueve cuando realizamos nuevos commits.

Por ejemplo:

```text
A ── B ── C
          ↑
        main
```

Después:

```text
git switch -c prueba
```

Tenemos:

```text
A ── B ── C
          ↑
       main
       prueba
```

Realizamos un commit:

```text
A ── B ── C ── D
          ↑     ↑
        main  prueba
```

La rama `prueba` avanzó.

La rama `main` permaneció donde estaba.

---

## Rama actual

Git siempre necesita saber sobre qué línea de trabajo estamos operando.

Podemos consultarlo mediante:

```bash
git branch
```

o:

```bash
git status
```

Es importante desarrollar el hábito de comprobar la rama actual antes de realizar operaciones importantes.

---

## `HEAD`

Git utiliza una referencia llamada:

```text
HEAD
```

para representar dónde estamos trabajando actualmente.

De manera simplificada:

```text
HEAD
 ↓
main
 ↓
C
```

Si cambiamos a otra rama:

```text
HEAD
 ↓
feature
 ↓
D
```

No es necesario memorizar todavía todos los detalles internos de `HEAD`.

Lo importante en esta etapa es comprender que Git necesita conocer la posición actual dentro de la historia.

---

## Ramas y commits

Las ramas no reemplazan a los commits.

Una rama utiliza los commits existentes para construir una línea de evolución.

Por ejemplo:

```text
A ── B ── C
          \
           D ── E
```

Los commits siguen formando parte de la historia.

La rama simplemente identifica una línea particular de esa historia.

---

## Fusionar ramas

Cuando una línea de trabajo está terminada, podemos necesitar incorporarla a otra rama.

Esta operación se denomina:

**merge**.

Por ejemplo:

```text
A ── B ── C
          \
           D ── E
```

Podemos integrar la rama en `main`:

```text
A ── B ── C ── D ── E
```

o, dependiendo de la historia, Git puede necesitar crear un commit de merge:

```text
A ── B ── C ─────── M
          \         /
           D ── E ─
```

La integración de ramas será trabajada progresivamente.

---

## `git merge`

Para fusionar una rama en la rama actual utilizamos:

```bash
git merge nombre-de-la-rama
```

Es importante comprender una idea fundamental:

> **La rama que estamos incorporando se fusiona sobre la rama actual.**

Por eso, antes de ejecutar un merge debemos verificar en qué rama estamos.

---

## El orden importa

Supongamos:

```text
main
feature
```

Si queremos incorporar `feature` a `main`, primero debemos ubicarnos en `main`:

```bash
git switch main
```

y luego:

```bash
git merge feature
```

No es equivalente a estar en `feature` y ejecutar:

```bash
git merge main
```

La operación se realiza sobre la rama actual.

---

## Eliminar una rama

Cuando una rama ya no resulta necesaria podemos eliminarla:

```bash
git branch -d nombre-de-la-rama
```

Eliminar una rama no significa necesariamente eliminar los commits que fueron creados en ella.

Esto es importante.

Una rama es una referencia.

Los commits forman parte de la historia.

---

## Ramas y GitHub

Hasta ahora trabajamos principalmente con:

```text
Repositorio local
       ↓
Repositorio remoto
       ↓
GitHub
```

Las ramas también pueden existir en el repositorio remoto.

Podemos tener:

```text
Repositorio local
├── main
└── feature
```

y:

```text
GitHub
├── main
└── feature
```

Esto permite que diferentes líneas de trabajo puedan compartirse y coordinarse mediante un repositorio remoto.

---

## Publicar una rama

Una rama local puede publicarse en GitHub mediante:

```bash
git push -u origin nombre-de-la-rama
```

Después de publicarla, GitHub podrá mostrar esa línea de trabajo.

---

## Ramas locales y remotas

Es importante distinguir:

```text
rama local
```

de:

```text
rama remota
```

Una rama local pertenece al repositorio local.

Una rama publicada también puede estar representada en el repositorio remoto.

No debemos asumir que crear una rama local hace que aparezca automáticamente en GitHub.

---

## El flujo básico con ramas

El recorrido que vamos a practicar es:

```text
Repositorio
     ↓
Crear rama
     ↓
Cambiar de rama
     ↓
Modificar
     ↓
Commit
     ↓
Seguir trabajando
     ↓
Fusionar
     ↓
Eliminar rama
```

Y posteriormente:

```text
Rama local
     ↓
Push
     ↓
Rama remota
     ↓
GitHub
```

---

## Ramas para experimentar

Una rama puede utilizarse para experimentar sin modificar inmediatamente la línea principal.

Por ejemplo:

```text
main
  ↓
versión estable

experimento
  ↓
nuevos cambios
```

Esto permite probar una idea y decidir posteriormente si debe incorporarse.

---

## Ramas para desarrollar funcionalidades

Un uso habitual es crear una rama para una nueva funcionalidad:

```text
main
  │
  └── feature-login
```

La funcionalidad puede desarrollarse mediante varios commits:

```text
main
  │
  └── feature-login
          ↓
          A
          ↓
          B
          ↓
          C
```

Cuando el trabajo está listo, puede integrarse.

---

## Ramas para corregir errores

También podemos utilizar ramas para trabajar sobre una corrección:

```text
main
  │
  └── fix-documentacion
```

Esto permite mantener separado el trabajo de corrección hasta que esté listo para incorporarse.

---

## Ramas y colaboración

Las ramas adquieren todavía mayor importancia cuando varias personas trabajan sobre el mismo proyecto.

Podemos imaginar:

```text
                 feature-A
                /
main ──────────
                \
                 feature-B
```

Cada persona puede desarrollar una línea de trabajo diferente.

Posteriormente, las ramas pueden integrarse.

Este modelo será desarrollado en profundidad en el módulo de trabajo colaborativo.

---

## No todo necesita una rama

Las ramas son una herramienta.

No debemos convertirlas en una obligación mecánica.

Para un cambio pequeño y directo puede ser suficiente trabajar sobre la rama principal, según el contexto del proyecto.

La decisión depende de:

- tamaño del cambio;
- complejidad;
- riesgo;
- cantidad de personas;
- flujo de trabajo;
- reglas del proyecto.

---

## Buenas prácticas

Durante este módulo comenzaremos a desarrollar algunos hábitos.

### Verificar la rama actual

Antes de realizar cambios importantes:

```bash
git status
```

o:

```bash
git branch
```

### Usar nombres descriptivos

Preferir:

```text
feature-login
fix-readme
experimento-api
```

en lugar de:

```text
rama1
prueba
cosas
```

### Mantener commits claros

Los commits deben representar cambios comprensibles.

### Integrar ramas terminadas

Una rama que ya no tiene un propósito debería revisarse y eventualmente eliminarse.

---

## ¿Qué vamos a practicar?

Durante este módulo vamos a:

- comprender qué es una rama;
- crear ramas;
- consultar ramas;
- cambiar de rama;
- realizar commits sobre diferentes ramas;
- observar cómo evolucionan;
- comprender `HEAD`;
- fusionar ramas;
- eliminar ramas;
- publicar ramas en GitHub;
- distinguir ramas locales y remotas;
- trabajar con situaciones de divergencia;
- introducir los conflictos de merge.

---

## ¿Qué deberías poder hacer al terminar?

Al finalizar el módulo deberías poder:

- explicar qué es una rama;
- crear una rama;
- cambiar de rama;
- identificar la rama actual;
- desarrollar cambios sobre una rama independiente;
- comprender cómo una rama avanza mediante commits;
- fusionar una rama;
- eliminar una rama que ya no se necesita;
- publicar una rama en GitHub;
- reconocer la diferencia entre ramas locales y remotas;
- interpretar visualmente una historia con ramas.

Y, fundamentalmente:

> **deberías poder decidir cuándo tiene sentido separar una línea de trabajo y comprender qué ocurre con la historia del proyecto cuando lo hacés.**

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

> **Una rama es una línea de evolución del proyecto.**

Aprender ramas no significa aprender una lista de comandos.

Significa poder observar una historia, comprender que pueden existir diferentes líneas de trabajo y utilizar Git para desarrollarlas y, cuando corresponda, integrarlas.

El objetivo final es pasar de pensar:

```text
"Git tiene ramas"
```

a comprender:

```text
"Necesito una línea de trabajo independiente,
por eso creo una rama."
```