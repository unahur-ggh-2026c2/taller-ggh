# Guía Plus — Pistas

> Pistas progresivas para los ejercicios de la Guía Plus.
>
> Intentá resolver cada desafío antes de consultar las pistas.

---

## Ejercicio 01 — El repositorio abandonado

### Pista 1

Antes de ejecutar comandos, inspeccioná qué archivos existen y preguntate cuáles forman parte del proyecto.

### Pista 2

Necesitás convertir una carpeta existente en un repositorio Git.

¿Qué comando inicializa un repositorio?

### Pista 3

Antes del primer commit, revisá el estado y decidí qué archivos deben quedar bajo seguimiento.

### Pista 4

Hay archivos que no deberían incorporarse al repositorio.

Pensá en qué tipo de archivos conviene excluir mediante `.gitignore`.

---

## Ejercicio 02 — El historial sospechoso

### Pista 1

No intentes solucionar el problema modificando el historial existente.

Primero analizá qué información permite obtener ese historial.

### Pista 2

Preguntate qué debería poder responder un commit:

> ¿Qué cambio se realizó?

### Pista 3

Los mensajes son demasiado genéricos.

Pensá en qué información debería contener un buen mensaje de commit.

### Pista 4

No solamente importa el mensaje.

También importa que cada commit represente una unidad de trabajo comprensible.

---

## Ejercicio 03 — Catálogo de películas

### Pista 1

Hay dos tareas independientes.

¿Conviene que ambas compartan la misma línea de trabajo?

### Pista 2

Cada tarea puede tener su propia rama.

Pensá qué nombres permitirían identificar rápidamente el propósito de cada una.

### Pista 3

Antes de comenzar una tarea, asegurate de partir de una versión actualizada de `main`.

### Pista 4

Una vez terminada una tarea:

```text
rama
 ↓
commit
 ↓
push
 ↓
Pull Request
```

Después de integrar una tarea, actualizá `main` antes de continuar con la siguiente.

---

## Ejercicio 04 — Dos personas, una decisión

### Pista 1

Para provocar el conflicto, las dos ramas deben partir del mismo estado.

### Pista 2

No alcanza con modificar archivos distintos.

Para producir el conflicto buscado, ambas ramas deben modificar la misma línea de manera incompatible.

### Pista 3

Cuando Git informe el conflicto:

```bash
git status
```

te indicará qué archivo necesita atención.

### Pista 4

Abrí el archivo y buscá las marcas:

```text
<<<<<<<
=======
>>>>>>>
```

No las dejes en el archivo final.

### Pista 5

Git no puede determinar cuál versión representa la intención correcta.

La resolución requiere una decisión humana.

---

## Ejercicio 05 — ¿Cuándo apareció?

### Pista 1

No empieces mirando todos los commits del repositorio.

El problema está asociado a un archivo concreto.

### Pista 2

Consultá la historia de ese archivo.

### Pista 3

Cuando encuentres un commit sospechoso, necesitás conocer exactamente qué cambió.

¿Qué comando permite inspeccionar un commit?

### Pista 4

No alcanza con decir:

> "Este commit parece sospechoso."

Buscá evidencia en los cambios registrados.

### Pista 5

La investigación debería poder explicar:

```text
problema
   ↓
historial
   ↓
commit
   ↓
cambio
   ↓
conclusión
```

---

## Ejercicio 06 — Cambio solicitado

### Pista 1

La Issue ya define el trabajo.

No agregues funcionalidades que no forman parte de ella.

### Pista 2

Partí de `main` actualizado y creá una rama específica para la tarea.

### Pista 3

La Pull Request debe permitir que otra persona comprenda:

```text
qué cambió
por qué
cómo fue probado
```

### Pista 4

La revisión tiene que producir feedback real.

No alcanza con escribir simplemente:

> "Está bien."

Buscá una observación concreta que permita mejorar o verificar el cambio.

### Pista 5

Una observación que requiere modificación debe resolverse mediante un nuevo commit sobre la misma rama.

---

## Ejercicio 07 — Proyecto de otra persona

### Pista 1

No empieces escribiendo documentación.

Primero tratá de comprender el proyecto.

### Pista 2

La pregunta central es:

> ¿Qué necesitaría saber una persona que recibe este proyecto por primera vez?

### Pista 3

Como mínimo, el README debería permitir responder:

```text
¿Qué es?
¿Para qué sirve?
¿Qué necesita?
¿Cómo se instala?
¿Cómo se ejecuta?
¿Cómo se utiliza?
```

### Pista 4

Probá las instrucciones que escribiste.

Si una persona necesita preguntarte algo para completar el procedimiento, probablemente falte documentación.

---

## Ejercicio 08 — Proyecto heredado

### Pista 1

No empieces modificando archivos.

Primero diagnosticá el estado del repositorio.

```bash
git status
git log --oneline --graph --all
```

### Pista 2

Separá el problema en etapas:

```text
diagnóstico
   ↓
preparación
   ↓
nueva funcionalidad
   ↓
revisión
   ↓
integración
```

### Pista 3

No mezcles la preparación del repositorio con la nueva funcionalidad si son cambios independientes.

### Pista 4

Para la nueva funcionalidad, utilizá una rama específica.

### Pista 5

La Pull Request debe permitir revisar solamente el cambio correspondiente a la nueva funcionalidad.

### Pista 6

Después de la revisión, corregí la observación en la misma rama y actualizá la Pull Request.

### Pista 7

Al finalizar, revisá nuevamente:

```bash
git status
git log --oneline --graph --all
```

Preguntate:

> ¿El historial permite entender qué ocurrió?

---

# Pista general

Cuando no sepas por dónde empezar, no busques primero un comando.

Primero identificá:

```text
¿Qué situación tengo?
        ↓
¿Qué quiero conseguir?
        ↓
¿Qué concepto de Git/GitHub resuelve esa situación?
        ↓
¿Qué comando necesito?
        ↓
¿Cómo verifico el resultado?
```

---

> **La mejor pista suele ser volver a definir el problema antes de intentar resolverlo.**
