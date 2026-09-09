# Guía Plus de Ejercicios

> Ejercicios complementarios y optativos para practicar Git y GitHub
> mediante situaciones diferentes a las trabajadas durante el curso.

Esta guía no introduce contenidos nuevos.

Su objetivo es practicar, combinar conceptos y tomar decisiones.

---

## Cómo usar esta guía

Los ejercicios son independientes.

No es necesario resolverlos todos.

Se recomienda:

```text
resolver
   ↓
revisar
   ↓
explicar qué hiciste
   ↓
consultar la solución solo si es necesario
```

No se busca memorizar comandos.

Se busca poder decidir:

* qué hacer;
* por qué hacerlo;
* qué registrar;
* cómo verificar el resultado.

---

# Nivel 1 — Resolver

## Ejercicio 01 — El repositorio abandonado

### Situación

Recibís un pequeño proyecto llamado `biblioteca`.

El proyecto contiene:

```text
biblioteca/
├── programa.py
├── README.md
└── notas.txt
```

Nunca se utilizó Git.

### Objetivo

Convertirlo en un repositorio Git correctamente organizado.

### Tareas

1. Inicializar Git.
2. Crear un `.gitignore` apropiado.
3. Registrar el estado inicial.
4. Crear un commit inicial.
5. Consultar el historial.

### Condición

El commit inicial debe contener solamente los archivos que realmente forman parte del proyecto.

### Pregunta

¿Por qué decidiste incluir o excluir cada archivo?

---

# Nivel 2 — Analizar

## Ejercicio 02 — El historial sospechoso

Te entregan este historial:

```text
a91c2e1 final
82d71aa cambios
54a90bc fix
3c81f12 prueba
17fa912 ahora sí
```

El proyecto funciona, pero nadie entiende cómo evolucionó.

### Objetivo

Analizar el problema y proponer una estrategia para mejorar la trazabilidad de futuros cambios.

### Tareas

1. Identificar problemas del historial.
2. Proponer mejores mensajes de commit.
3. Explicar qué debería representar cada commit.
4. Proponer un flujo de trabajo para las próximas tareas.

### Importante

No hace falta reescribir el historial existente.

El objetivo es tomar decisiones sobre cómo trabajar a partir de ahora.

---

# Nivel 3 — Aplicar

## Ejercicio 03 — Catálogo de películas

### Situación

Vas a trabajar en un proyecto que administra un catálogo de películas.

Dos tareas aparecen simultáneamente:

```text
Tarea A
Agregar búsqueda por título.

Tarea B
Actualizar la documentación del proyecto.
```

### Objetivo

Organizar ambas tareas utilizando ramas.

### Tareas

1. Crear una rama para cada tarea.
2. Realizar al menos un commit coherente por tarea.
3. Publicar las ramas.
4. Integrar los cambios mediante Pull Requests.
5. Actualizar `main`.

### Pregunta

¿Por qué no conviene realizar ambas tareas directamente sobre `main`?

---

# Nivel 4 — Resolver problemas

## Ejercicio 04 — Dos personas, una decisión

### Situación

Dos personas trabajan sobre el mismo archivo:

```text
configuracion.txt
```

Una modifica:

```text
modo=desarrollo
```

La otra modifica la misma línea:

```text
modo=produccion
```

Ambos cambios son correctos dentro de su contexto.

### Objetivo

Resolver el conflicto de integración.

### Tareas

1. Crear las dos ramas.
2. Realizar los cambios.
3. Integrarlas en `main`.
4. Provocar el conflicto.
5. Resolverlo tomando una decisión explícita.
6. Registrar la resolución.
7. Verificar el historial.

### Pregunta

¿Por qué Git no puede decidir automáticamente cuál versión es correcta?

---

# Nivel 5 — Investigar

## Ejercicio 05 — ¿Cuándo apareció?

### Situación

Una aplicación de recetas funcionaba correctamente.

Después de varios cambios, una funcionalidad dejó de funcionar.

El archivo afectado es:

```text
src/recetas.py
```

### Objetivo

Utilizar el historial para investigar el problema.

### Tareas

1. Consultar la historia del archivo.
2. Identificar commits relevantes.
3. Analizar uno o más commits con `git show`.
4. Determinar qué cambio pudo introducir el problema.
5. Documentar la investigación.

### Entrega

Crear:

```text
INVESTIGACION.md
```

con:

```md
# Investigación

## Problema

...

## Commit sospechoso

...

## Evidencia

...

## Conclusión

...
```

---

# Nivel 6 — Trabajar como equipo

## Ejercicio 06 — Cambio solicitado

### Situación

Un equipo mantiene una aplicación de turnos.

Se crea la siguiente Issue:

```text
Título:
Agregar cancelación de turnos

Objetivo:
Permitir cancelar un turno existente.

Criterios:
- El turno debe poder identificarse.
- Debe poder cancelarse.
- La documentación debe actualizarse.
```

### Objetivo

Realizar el ciclo completo.

### Tareas

```text
Issue
  ↓
rama
  ↓
desarrollo
  ↓
commit
  ↓
push
  ↓
Pull Request
  ↓
revisión
  ↓
corrección
  ↓
merge
```

### Condición

La Pull Request debe recibir al menos una observación antes de integrarse.

La observación puede ser simulada por otra persona.

---

# Nivel 7 — Documentar

## Ejercicio 07 — Proyecto de otra persona

### Situación

Recibís un proyecto que funciona, pero su README contiene solamente:

```text
# Agenda

Proyecto para manejar contactos.
```

No conocés el proyecto previamente.

### Objetivo

Mejorar la documentación sin modificar el funcionamiento.

### Tareas

Crear un README que permita responder:

```text
¿Qué es?
¿Para qué sirve?
¿Qué necesita?
¿Cómo se instala?
¿Cómo se ejecuta?
¿Cómo se utiliza?
¿Cuál es su estado?
```

### Condición

Otra persona debería poder seguir las instrucciones sin recibir una explicación oral.

---

# Nivel 8 — Desafío integrador

## Ejercicio 08 — Proyecto heredado

### Situación

Recibís un repositorio llamado:

```text
agenda-cultural
```

Tiene:

```text
README.md
src/
datos/
```

Pero presenta varios problemas:

* no tiene `.gitignore`;
* la documentación está incompleta;
* hay cambios pendientes;
* el historial tiene mensajes poco descriptivos;
* se solicita agregar una nueva funcionalidad;
* otra persona debe revisar el cambio.

### Objetivo

Mejorar el proyecto sin perder el trabajo existente.

### Tareas

#### Etapa 1 — Diagnóstico

Analizar:

```bash
git status
git log --oneline --graph --all
```

Documentar los problemas encontrados.

---

#### Etapa 2 — Preparación

Crear o actualizar:

```text
.gitignore
README.md
```

Registrar los cambios mediante commits coherentes.

---

#### Etapa 3 — Nueva funcionalidad

Crear una rama para:

```text
Agregar búsqueda por fecha.
```

Desarrollar la funcionalidad.

---

#### Etapa 4 — Publicación

Publicar la rama y crear una Pull Request.

---

#### Etapa 5 — Revisión

Realizar una revisión.

Registrar al menos:

* un aspecto correcto;
* una observación;
* una sugerencia de mejora.

---

#### Etapa 6 — Corrección

Resolver la observación mediante un nuevo commit.

---

#### Etapa 7 — Integración

Integrar la Pull Request.

Actualizar `main`.

---

#### Etapa 8 — Cierre

Revisar:

```bash
git status
git log --oneline --graph --all
```

Actualizar la documentación final.

---

# Autoevaluación

Al terminar un ejercicio, preguntate:

```text
[ ] ¿Entendí el problema antes de ejecutar comandos?
[ ] ¿Elegí una estrategia de trabajo?
[ ] ¿Los commits son comprensibles?
[ ] ¿Puedo explicar por qué creé cada rama?
[ ] ¿Revisé mis cambios?
[ ] ¿Puedo reconstruir lo que hice mirando el historial?
[ ] ¿La documentación permite reproducir el trabajo?
```

---

# Desafío extra

Elegí uno de los ejercicios y resolvelo sin consultar los cheatsheets.

Después:

1. compará tu procedimiento;
2. revisá el historial;
3. identificá qué decisiones tomaste;
4. explicá qué harías diferente la próxima vez.

> El objetivo de estos ejercicios no es llegar al resultado de cualquier manera.
> Es desarrollar criterio para trabajar con Git y GitHub.

