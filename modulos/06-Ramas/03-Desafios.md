# Desafíos
## Módulo 06 — Ramas

Los desafíos de este módulo proponen situaciones menos guiadas.

La consigna ya no indica necesariamente cada comando que debés ejecutar.

El objetivo es que puedas:

```text
analizar el problema
      ↓
diseñar una estrategia
      ↓
elegir las operaciones
      ↓
ejecutarlas
      ↓
verificar el resultado
      ↓
explicar qué ocurrió
```

---

## Desafío 1 — Una nueva funcionalidad

Tenés un proyecto que funciona correctamente en:

```text
main
```

Te solicitan agregar una nueva funcionalidad, pero todavía no está claro si el resultado será aceptado.

### Objetivo

Desarrollá la funcionalidad sin modificar directamente `main`.

### Condiciones

- creá una rama apropiada;
- realizá al menos dos commits;
- mantené `main` sin los cambios mientras desarrollás;
- verificá la historia;
- finalmente integrá la funcionalidad.

### Entregable

Mostrá:

```bash
git log --oneline --graph --all
```

y explicá:

1. dónde se creó la rama;
2. qué commits pertenecen a ella;
3. cuándo se integró;
4. cómo quedó la historia.

---

# Desafío 2 — Corrección aislada

Detectaste un error en la documentación del proyecto.

La corrección es pequeña, pero querés mantenerla separada del resto del trabajo.

### Objetivo

Creá una rama específica para la corrección.

Realizá el cambio y registralo.

Después integralo en `main`.

### Condición adicional

El nombre de la rama debe permitir comprender qué problema resuelve.

### Reflexión

¿Por qué puede resultar útil separar incluso una modificación pequeña?

---

# Desafío 3 — Dos funcionalidades simultáneas

Dos personas podrían trabajar simultáneamente sobre:

```text
feature-busqueda
feature-exportacion
```

Simulá ambas líneas de trabajo vos mismo.

### Objetivo

Construí:

```text
                 búsqueda
                /
main ──────────
                \
                 exportación
```

Cada rama deberá tener al menos dos commits.

Después integrá ambas ramas.

### Preguntas

1. ¿Cuál integraste primero?
2. ¿Qué ocurrió con la segunda?
3. ¿Se produjo algún conflicto?
4. ¿Cómo quedó la historia?

---

# Desafío 4 — Trabajo paralelo con documentación

El proyecto tiene una funcionalidad en desarrollo.

Mientras tanto, querés mejorar el README.

No querés mezclar ambos trabajos.

### Objetivo

Construí:

```text
main
 ├── feature-funcionalidad
 └── docs-readme
```

Realizá cambios independientes en ambas ramas.

Después:

1. integrá `docs-readme`;
2. continuá trabajando sobre `feature-funcionalidad`;
3. integrá finalmente `feature-funcionalidad`.

### Pregunta

¿Por qué las ramas permiten separar responsabilidades aunque trabajes solo?

---

# Desafío 5 — Rama experimental

Querés probar una modificación importante del proyecto.

No sabés si la solución funcionará.

### Objetivo

Creá:

```text
experimento
```

Realizá varios commits.

Después decidí que el experimento no debe incorporarse.

### Condición

`main` no debe recibir los cambios del experimento.

### Finalmente

Eliminá la rama.

### Reflexión

Respondé:

> ¿Qué ventaja te proporcionó la rama aunque finalmente hayas descartado el trabajo?

---

# Desafío 6 — Reconstruir una historia

Te entregan esta historia:

```text
*   M
|\
| * E
| * D
|/
* C
* B
* A
```

No conocés los comandos que produjeron el resultado.

### Objetivo

Reconstruí una secuencia plausible de operaciones que podría haber generado esta historia.

No existe una única respuesta.

Tu propuesta debe incluir:

- creación de una rama;
- al menos dos commits sobre ella;
- trabajo sobre `main`;
- integración.

---

# Desafío 7 — Predecir antes de ejecutar

Partís de:

```text
A ── B ── C
```

Ejecutás conceptualmente:

```text
crear feature
hacer commit D
volver a main
hacer commit E
```

### Objetivo

Dibujá la historia antes de ejecutar nada.

Después realizá las operaciones realmente en Git.

Compará:

```text
predicción
    vs.
resultado
```

### Reflexión

Si fueron diferentes, explicá por qué.

---

# Desafío 8 — Encontrar el error

Un compañero te entrega esta secuencia:

```bash
git switch feature
git add .
git commit -m "Nueva funcionalidad"
git merge main
```

Dice:

> "Ya integré mi funcionalidad en main."

### Objetivo

Analizá la secuencia.

Respondé:

1. ¿Está realmente integrada la funcionalidad en `main`?
2. ¿Sobre qué rama se ejecutó el merge?
3. ¿Qué debería haber hecho para integrar `feature` en `main`?

No ejecutes nada hasta haber respondido.

---

# Desafío 9 — Merge con conflicto

Creá dos ramas desde el mismo punto.

Por ejemplo:

```text
main
 ├── feature-a
 └── feature-b
```

En ambas ramas modificá exactamente la misma línea de un archivo, pero con contenidos diferentes.

Ejemplo:

### Rama A

```text
Nombre del proyecto: Proyecto A
```

### Rama B

```text
Nombre del proyecto: Proyecto B
```

Realizá commits en ambas.

Intentá integrar las dos ramas.

### Objetivo

Provocar deliberadamente un conflicto y resolverlo correctamente.

### Entregable

Documentá:

1. qué modificó cada rama;
2. por qué Git no pudo resolver automáticamente el conflicto;
3. qué decisión tomaste;
4. cómo quedó finalmente el archivo;
5. qué commit registró la resolución.

---

# Desafío 10 — Resolver sin perder información

Generá un conflicto entre dos ramas.

Al resolverlo, no elijas automáticamente una de las dos versiones.

Intentá construir una tercera versión que conserve la información válida de ambas.

### Reflexión

Explicá:

> ¿Por qué resolver un conflicto no significa necesariamente elegir "A" o "B"?

---

# Desafío 11 — Rama publicada

Creá una rama:

```text
feature-remota
```

Desarrollá una pequeña modificación.

Publicala en GitHub.

Después verificá desde GitHub que la rama exista.

### Objetivo

Demostrar el recorrido:

```text
rama local
    ↓
commit
    ↓
push
    ↓
rama en GitHub
```

### Entregable

Indicá los comandos utilizados y explicá qué hizo cada uno.

---

# Desafío 12 — La rama que nadie publicó

Un compañero afirma:

> "Creé la rama `feature-login`, hice tres commits y no aparece en GitHub."

### Objetivo

Explicarle qué ocurrió.

Tu respuesta debe diferenciar:

```text
crear una rama
```

de:

```text
publicar una rama
```

Incluí el comando necesario para publicarla.

---

# Desafío 13 — Local y remoto

Tenés:

```text
main
feature
```

en tu repositorio local.

En GitHub existe:

```text
main
feature
```

pero otra persona realizó nuevos commits sobre `feature`.

### Objetivo

Analizar conceptualmente la situación.

Respondé:

1. ¿Tu rama local necesariamente está actualizada?
2. ¿Qué información representa el repositorio remoto?
3. ¿Qué problemas podrían aparecer si trabajás sin actualizar tu información?
4. ¿Qué conceptos nuevos necesitarías estudiar para resolver completamente esta situación?

Este desafío no requiere todavía resolver toda la sincronización remota.

---

# Desafío 14 — La rama equivocada

Estás trabajando sobre:

```text
feature-login
```

y realizaste tres commits.

Después descubrís que uno de ellos debía haber sido realizado sobre:

```text
fix-documentacion
```

### Objetivo

Analizar el problema antes de modificar la historia.

No se busca necesariamente resolverlo con comandos avanzados.

Respondé:

1. ¿Qué información necesitás conocer?
2. ¿Dónde quedaron registrados los commits?
3. ¿Por qué es importante no ejecutar comandos al azar?
4. ¿Qué alternativas conceptuales existen?

---

# Desafío 15 — Historia para un proyecto real

Elegí un proyecto propio.

Diseñá un esquema de ramas que permita trabajar en:

```text
funcionalidad
corrección
documentación
experimento
```

No hace falta implementar todavía todas las ramas.

### Objetivo

Definir una estrategia razonable de nombres y propósitos.

Por ejemplo:

```text
main
 ├── feature-...
 ├── fix-...
 ├── docs-...
 └── experimento-...
```

### Pregunta

¿Por qué elegiste esos nombres?

---

# Desafío 16 — ¿Necesito una rama?

Analizá las siguientes situaciones.

### Situación A

Cambiar una palabra mal escrita en un README.

### Situación B

Agregar una funcionalidad nueva.

### Situación C

Experimentar con una modificación que podría romper el proyecto.

### Situación D

Realizar una corrección urgente mientras existe otra funcionalidad en desarrollo.

### Situación E

Cambiar cinco archivos relacionados con una nueva característica.

### Objetivo

Decidir para cada caso:

```text
main
```

o:

```text
nueva rama
```

No alcanza con responder.

Justificá cada decisión.

---

# Desafío 17 — Historia incompleta

Observá:

```text
A ── B ── C
          \
           D ── E
```

No se muestran los nombres de las ramas.

### Objetivo

Proponer una asignación posible:

```text
main → ?
feature → ?
```

Después explicá qué información adicional necesitarías para saberlo con certeza.

---

# Desafío 18 — Leer un gráfico de Git

Ejecutá:

```bash
git log --oneline --graph --all
```

sobre uno de tus repositorios.

### Objetivo

Explicar el gráfico utilizando lenguaje cotidiano.

No describas solamente:

> "Hay una rama."

Explicá:

- dónde se separó;
- qué cambios ocurrieron;
- qué líneas avanzaron;
- dónde se integraron;
- qué ramas siguen existiendo.

---

# Desafío 19 — Eliminar o conservar

Tenés estas ramas:

```text
main
feature-login
feature-exportacion
fix-readme
experimento
```

Sabés que:

- `feature-login` fue integrada;
- `feature-exportacion` sigue en desarrollo;
- `fix-readme` fue integrada;
- `experimento` fue descartada;
- `main` continúa siendo la línea principal.

### Objetivo

Decidir qué ramas deberían conservarse y cuáles podrían eliminarse.

Justificá.

---

# Desafío 20 — Ramas como líneas de evolución

Construí una historia que represente:

```text
1. Proyecto inicial.
2. Nueva funcionalidad.
3. Corrección independiente.
4. Desarrollo simultáneo.
5. Integración de una línea.
6. Integración de la otra.
```

Representala gráficamente.

Después implementala en Git.

Finalmente compará:

```text
historia diseñada
```

con:

```text
historia real
```

---

# Desafío 21 — El proyecto como historia

Elegí un proyecto pequeño y construí una historia con:

```text
main
feature
fix
docs
```

Cada rama debe representar una intención diferente.

No agregues ramas solamente para cumplir la consigna.

### Objetivo

Demostrar que las ramas representan decisiones sobre la evolución del proyecto.

---

# Desafío 22 — Documentar el flujo

Elegí uno de los desafíos anteriores.

Creá:

```text
docs/flujo-de-ramas.md
```

Documentá:

```md
# Flujo de ramas

## Objetivo

...

## Ramas utilizadas

...

## Desarrollo

...

## Integración

...

## Resultado

...

## Aprendizajes

...
```

Después:

```bash
git add .
git commit -m "Documenta flujo de ramas"
```

Publicá el resultado en GitHub.

---

# Desafío 23 — Diseñar antes de ejecutar

Para un proyecto ficticio llamado:

```text
sistema-biblioteca
```

diseñá una estrategia de ramas para desarrollar:

- búsqueda de libros;
- registro de usuarios;
- corrección de préstamos;
- actualización de documentación.

### Objetivo

No ejecutes comandos.

Primero diseñá:

```text
main
 ├── ...
 ├── ...
 ├── ...
 └── ...
```

Después explicá el propósito de cada rama.

---

# Desafío 24 — Detectar una mala estrategia

Un equipo utiliza estas ramas:

```text
rama1
rama2
rama-final
rama-final2
prueba
prueba-nueva
prueba-ahora-si
```

### Objetivo

Analizá los problemas de esta estrategia.

Proponé una alternativa.

No existe una única convención correcta, pero los nombres deberían comunicar intención.

---

# Desafío 25 — Integrador

Construí un proyecto desde cero o utilizá uno existente.

Realizá este recorrido:

```text
                    feature
                   /       \
                  /         \
main ────────────            ─── merge
                  \         /
                   \       /
                    fix
```

El proyecto deberá tener:

- una rama principal;
- una rama de funcionalidad;
- una rama de corrección;
- al menos dos commits de trabajo;
- una integración;
- al menos una rama publicada en GitHub;
- una revisión de la historia mediante `git log --graph`.

### Entregable

Presentá:

```text
1. Nombre y propósito de cada rama.
2. Comandos principales utilizados.
3. Historia antes del merge.
4. Historia después del merge.
5. Captura o salida de git log --graph.
6. Explicación del proceso.
7. Reflexión final.
```

---

# Desafío 26 — Explicarlo sin comandos

Explicale a una persona que nunca utilizó Git qué es una rama.

No podés utilizar comandos.

No podés decir simplemente:

> "Es una rama de Git."

Utilizá una analogía o representación que permita comprender:

- punto de partida;
- separación;
- trabajo independiente;
- integración.

Después compará tu explicación con el modelo:

```text
A ── B ── C
          \
           D ── E
```

---

# Desafío 27 — Explicarlo con comandos

Ahora explicá el mismo concepto utilizando solamente operaciones básicas de Git.

La explicación debe incluir:

```bash
git switch
git commit
git merge
```

pero cada comando debe estar acompañado por una explicación de qué problema resuelve.

---

# Desafío 28 — Modelo mental

Completá:

```text
Una rama es ____________________________

Un commit es ___________________________

HEAD representa ________________________

Un merge permite ________________________

Una rama local _________________________

Una rama remota ________________________

Un conflicto aparece cuando ____________
```

Después compará tus respuestas con los conceptos trabajados durante el módulo.

---

# Desafío 29 — Explicar una decisión

Elegí una situación real o ficticia donde hayas decidido utilizar una rama.

Escribí:

```md
## Decisión

### Problema

...

### Alternativas

...

### Decisión

...

### Motivo

...

### Resultado

...
```

El objetivo es comenzar a justificar decisiones de flujo de trabajo y no solamente ejecutar comandos.

---

# Desafío 30 — Desafío final

Sin consultar la práctica ni los ejercicios, realizá el siguiente recorrido:

```text
1. Partir de main.
2. Crear una rama.
3. Realizar dos commits.
4. Crear una segunda rama desde main.
5. Realizar un commit.
6. Volver a main.
7. Realizar otro commit.
8. Observar la divergencia.
9. Integrar una rama.
10. Integrar la otra.
11. Resolver cualquier conflicto que aparezca.
12. Publicar una rama en GitHub.
13. Analizar la historia.
14. Eliminar las ramas que ya no sean necesarias.
```

Al finalizar ejecutá:

```bash
git status
git branch
git log --oneline --graph --all
```

---

# Reflexión final

Respondé sin copiar definiciones:

### 1.

¿Por qué las ramas son útiles?

### 2.

¿Qué problema concreto te resultó más fácil resolver utilizando una rama?

### 3.

¿Qué parte del trabajo con ramas te resultó más difícil?

### 4.

¿Qué diferencia existe entre trabajar en una rama y trabajar directamente sobre `main`?

### 5.

¿Por qué un merge debe realizarse comprendiendo qué rama está actualmente activa?

### 6.

¿Qué aprendiste al provocar deliberadamente un conflicto?

### 7.

¿Qué información aporta el gráfico de `git log --graph`?

### 8.

¿En qué situaciones de un proyecto real utilizarías ramas?

---

# Criterio de resolución

Un desafío está correctamente resuelto cuando no solamente se obtiene el resultado esperado, sino cuando se puede explicar:

```text
qué se quería hacer
       ↓
qué decisión se tomó
       ↓
qué operaciones se realizaron
       ↓
qué ocurrió con la historia
       ↓
por qué el resultado es correcto
```

La dificultad de estos desafíos está deliberadamente por encima de la práctica guiada.

La intención es comenzar a pasar de:

> **"Sé ejecutar los comandos."**

a:

> **"Sé decidir qué necesito hacer y puedo utilizar Git para hacerlo."**

---

> **Una buena utilización de ramas no consiste en tener muchas ramas. Consiste en utilizar una rama cuando representa una línea de trabajo que conviene separar.**