# Guía Plus — Soluciones

> Propuestas de resolución para los ejercicios de la Guía Plus.
>
> Estas soluciones no representan la única forma válida de resolver los ejercicios.
> Lo importante es que el procedimiento sea correcto, coherente y verificable.

---

## Ejercicio 01 — El repositorio abandonado

### Resolución

Inicializar el repositorio:

```bash
git init
```

Crear un `.gitignore` adecuado para el proyecto.

Revisar:

```bash
git status
```

Agregar solamente los archivos correspondientes:

```bash
git add .
```

Verificar lo preparado:

```bash
git diff --staged
```

Crear el commit:

```bash
git commit -m "Inicializa repositorio de biblioteca"
```

Comprobar:

```bash
git status
git log --oneline
```

### Resultado esperado

El proyecto queda bajo seguimiento de Git y tiene un primer commit coherente.

---

## Ejercicio 02 — El historial sospechoso

### Resolución

No es necesario modificar el historial existente.

El problema principal está en la calidad de los mensajes y posiblemente en la falta de unidades de trabajo claras.

Una estrategia futura podría ser:

```text
cambio coherente
   ↓
revisión
   ↓
commit descriptivo
```

Por ejemplo:

```text
Agrega búsqueda de libros
Corrige validación de ISBN
Actualiza instrucciones de instalación
```

En lugar de:

```text
cambios
fix
prueba
final
```

### Resultado esperado

Una política de trabajo que produzca commits comprensibles y relacionados con cambios concretos.

---

## Ejercicio 03 — Catálogo de películas

### Resolución

Actualizar `main`:

```bash
git switch main
git pull
```

Crear la primera rama:

```bash
git switch -c feature-busqueda-titulo
```

Realizar el cambio:

```bash
git add .
git commit -m "Agrega búsqueda por título"
git push -u origin feature-busqueda-titulo
```

Crear la Pull Request e integrarla.

Luego actualizar `main`:

```bash
git switch main
git pull
```

Crear la segunda rama:

```bash
git switch -c docs-actualizacion
```

Realizar la documentación:

```bash
git add .
git commit -m "Actualiza documentación del catálogo"
git push -u origin docs-actualizacion
```

Crear la segunda Pull Request e integrarla.

### Resultado esperado

Dos tareas independientes, cada una con:

```text
rama
 ↓
commit
 ↓
Pull Request
 ↓
merge
```

---

## Ejercicio 04 — Dos personas, una decisión

### Resolución

Crear el repositorio y el commit inicial.

Crear `feature-a`:

```bash
git switch -c feature-a
```

Modificar la línea:

```text
modo=desarrollo
```

Registrar:

```bash
git add configuracion.txt
git commit -m "Configura modo de desarrollo"
```

Volver al estado original y crear `feature-b`:

```bash
git switch main
git switch -c feature-b
```

Modificar la misma línea:

```text
modo=produccion
```

Registrar:

```bash
git add configuracion.txt
git commit -m "Configura modo de produccion"
```

Integrar `feature-a`:

```bash
git switch main
git merge feature-a
```

Intentar integrar `feature-b`:

```bash
git merge feature-b
```

Se producirá el conflicto.

Revisar:

```bash
git status
```

Resolver manualmente `configuracion.txt`.

Por ejemplo, si el proyecto requiere un modo explícito:

```text
modo=desarrollo-produccion
```

o elegir una de las alternativas según el contexto del proyecto.

Después:

```bash
git add configuracion.txt
git commit -m "Resuelve conflicto de configuración"
```

Finalmente:

```bash
git log --oneline --graph --all
```

### Resultado esperado

El conflicto queda resuelto mediante una decisión explícita y registrada.

No existe una única respuesta correcta para el contenido final: depende del contexto planteado.

---

## Ejercicio 05 — ¿Cuándo apareció?

### Resolución

Consultar la historia del archivo:

```bash
git log --oneline -- src/recetas.py
```

Identificar commits relevantes.

Inspeccionar uno:

```bash
git show ID_DEL_COMMIT
```

Comparar el cambio con el comportamiento que dejó de funcionar.

Documentar:

```md
# Investigación

## Problema

La funcionalidad dejó de funcionar al procesar ...

## Commit sospechoso

`abc1234`

## Evidencia

El commit modifica ...

## Conclusión

El cambio introducido en ese commit explica el comportamiento observado porque ...
```

### Resultado esperado

Una investigación basada en evidencia del historial, no solamente en una suposición.

---

## Ejercicio 06 — Cambio solicitado

### Resolución

Partir de `main` actualizado:

```bash
git switch main
git pull
```

Crear rama:

```bash
git switch -c feature-cancelar-turnos
```

Implementar la funcionalidad.

Registrar:

```bash
git add .
git commit -m "Agrega cancelación de turnos"
```

Publicar:

```bash
git push -u origin feature-cancelar-turnos
```

Crear la Pull Request vinculándola con la Issue.

Realizar una revisión.

Ejemplo de observación:

> La documentación no explica qué ocurre cuando se intenta cancelar un turno inexistente.

Resolver:

```bash
git add .
git commit -m "Documenta cancelación de turnos inexistentes"
git push
```

Actualizar la Pull Request.

Una vez aprobada:

```text
Pull Request
 ↓
merge
```

Actualizar localmente:

```bash
git switch main
git pull
```

### Resultado esperado

La Issue queda vinculada con el trabajo realizado y la Pull Request contiene también la corrección surgida de la revisión.

---

## Ejercicio 07 — Proyecto de otra persona

### Resolución

Primero comprender el proyecto.

Revisar:

```text
estructura
código
dependencias
forma de ejecución
```

Después construir el README alrededor de las necesidades reales del proyecto.

Una estructura posible:

```md
# Agenda

Descripción.

## Objetivo

...

## Tecnologías

...

## Requisitos

...

## Instalación

...

## Uso

...

## Ejemplo

...

## Estado

...
```

Después seguir las instrucciones desde el principio.

Por ejemplo:

```text
README
 ↓
instalación
 ↓
ejecución
 ↓
uso
```

Corregir cualquier paso que no sea reproducible.

### Resultado esperado

Una persona que no conoce el proyecto puede instalarlo y utilizarlo siguiendo el README.

---

## Ejercicio 08 — Proyecto heredado

### Resolución

### Etapa 1 — Diagnóstico

```bash
git status
git log --oneline --graph --all
```

Identificar:

```text
estado del repositorio
historial
archivos pendientes
problemas de documentación
```

---

### Etapa 2 — Preparación

Crear o actualizar `.gitignore`.

Actualizar `README.md`.

Separar los cambios en commits coherentes.

Por ejemplo:

```bash
git add .gitignore
git commit -m "Agrega reglas de archivos ignorados"
```

Luego:

```bash
git add README.md
git commit -m "Actualiza documentación del proyecto"
```

---

### Etapa 3 — Nueva funcionalidad

Actualizar `main`:

```bash
git switch main
git pull
```

Crear rama:

```bash
git switch -c feature-busqueda-fecha
```

Implementar:

```text
búsqueda por fecha
```

Registrar:

```bash
git add .
git commit -m "Agrega búsqueda de eventos por fecha"
```

Publicar:

```bash
git push -u origin feature-busqueda-fecha
```

---

### Etapa 4 — Pull Request

Crear la Pull Request describiendo:

```text
qué se agregó
por qué
cómo se probó
```

---

### Etapa 5 — Revisión

Realizar una observación concreta.

Ejemplo:

> La búsqueda no documenta qué formato debe utilizar la fecha.

---

### Etapa 6 — Corrección

Actualizar la documentación o implementación correspondiente.

```bash
git add .
git commit -m "Documenta formato de búsqueda por fecha"
git push
```

---

### Etapa 7 — Integración

Una vez aprobada:

```text
Pull Request
 ↓
merge
```

Actualizar:

```bash
git switch main
git pull
```

---

### Etapa 8 — Cierre

Comprobar:

```bash
git status
git log --oneline --graph --all
```

Verificar que:

```text
README
.gitignore
funcionalidad
historial
```

se encuentren en el estado esperado.

### Resultado esperado

El proyecto queda mejor organizado y con una nueva funcionalidad desarrollada mediante un flujo colaborativo completo.

---

# Criterio de corrección

Una solución puede diferir de estas propuestas y seguir siendo correcta.

Evaluar principalmente:

```text
comprensión del problema
        +
elección adecuada de herramientas
        +
historial coherente
        +
verificación
        +
capacidad de explicar las decisiones
```

No evaluar solamente si se ejecutaron exactamente los mismos comandos.

---

> **En Git puede haber varios caminos correctos. Lo importante es entender qué estado se quiere alcanzar y poder justificar cómo se llegó hasta él.**

