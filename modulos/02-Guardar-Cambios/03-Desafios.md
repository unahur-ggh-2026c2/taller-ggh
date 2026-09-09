# Desafíos
## Módulo 02 — Guardar cambios

Estos desafíos buscan que puedas tomar decisiones sobre el estado de un repositorio sin depender de una receta de comandos.

La consigna general es:

> **Primero observá. Después interpretá. Recién entonces actuá.**

---

## Desafío 1 — Tres estados

Partí de un repositorio limpio.

Realizá estas acciones:

1. Modificá `README.md`.
2. Consultá el estado.
3. Prepará el cambio.
4. Consultá nuevamente el estado.
5. Realizá un commit.
6. Consultá nuevamente el estado.

Para cada etapa explicá qué está ocurriendo.

Tu explicación debería distinguir claramente:

```text
Área de trabajo
       ↓
Área de preparación
       ↓
Historial
```

---

## Desafío 2 — El commit que falta

Un compañero modificó:

```text
README.md
```

y ejecutó:

```bash
git add README.md
```

Después dice:

> "No entiendo por qué el cambio no aparece cuando miro el historial."

### Tu desafío

Explicale qué ocurrió.

No alcanza con decir:

> "Te falta hacer commit."

Explicá **por qué** el cambio todavía no forma parte del historial.

---

## Desafío 3 — El archivo que quedó afuera

Tenés:

```text
README.md
objetivos.md
notas.md
```

Los tres fueron modificados.

El objetivo es crear un commit que contenga solamente:

```text
README.md
objetivos.md
```

El cambio de `notas.md` debe quedar pendiente.

### Condición

No utilices una operación que prepare automáticamente todos los archivos.

Después del commit, demostrale a un compañero que `notas.md` quedó fuera del registro.

---

## Desafío 4 — Dos intenciones diferentes

Modificaste:

```text
README.md
```

para corregir una descripción.

También modificaste:

```text
objetivos.md
```

para incorporar un nuevo objetivo.

Ambos cambios son válidos, pero representan intenciones diferentes.

### Tu desafío

Decidí si conviene:

- realizar un único commit;
- realizar dos commits.

No existe una respuesta automática.

Lo importante es justificar la decisión desde la perspectiva de la claridad del historial.

---

## Desafío 5 — El mensaje imposible

Un repositorio tiene este historial:

```text
cambios
cambios
cambios
cambios
cambios
```

El proyecto lleva varios meses de desarrollo.

### Tu desafío

Explicá qué dificultades tendría alguien que quisiera comprender la evolución del proyecto.

Después diseñá cinco mensajes que podrían haber representado mejor esos cambios.

No es necesario reconstruir exactamente qué ocurrió.

El objetivo es pensar qué información debería transmitir un commit.

---

## Desafío 6 — El repositorio no queda limpio

Un estudiante afirma:

> "Hice el commit, pero Git todavía muestra cambios."

Consultás:

```bash
git status
```

y aparecen archivos modificados.

### Tu desafío

Construí al menos **tres explicaciones posibles** antes de tocar nada.

Después analizá cuál corresponde según la información que proporciona `git status`.

La idea es desarrollar una estrategia de diagnóstico y no asumir automáticamente que Git cometió un error.

---

## Desafío 7 — Modificación después de preparar

Partí de un repositorio limpio.

1. Modificá `README.md`.
2. Ejecutá `git add README.md`.
3. Volvé a modificar `README.md`.
4. Ejecutá:

```bash
git status
```

### Tu desafío

Explicá por qué Git puede mostrar simultáneamente información relacionada con un cambio preparado y con una modificación posterior.

No busques resolverlo inmediatamente.

Primero construí un modelo de lo que ocurrió.

---

## Desafío 8 — Separar los cambios

Modificá tres archivos:

```text
README.md
objetivos.md
notas.md
```

La modificación de cada archivo representa una tarea diferente.

Tu desafío es construir **tres commits independientes**.

Cada commit debe contener solamente el cambio correspondiente.

Al finalizar:

```bash
git log --oneline
```

debería permitir distinguir las tres tareas.

---

## Desafío 9 — Un solo commit, muchas cosas

Imaginá que alguien realizó durante una tarde:

- una corrección de documentación;
- una modificación de objetivos;
- una actualización de integrantes;
- una nueva sección del README;
- nuevas notas personales.

Al final ejecutó:

```bash
git add .
git commit -m "Actualiza proyecto"
```

### Tu desafío

Analizá la situación.

Respondé:

1. ¿El commit es válido?
2. ¿Git permite hacerlo?
3. ¿El problema, si existe, está en Git o en la forma de organizar el historial?
4. ¿Cómo podría haberse construido un historial más claro?

---

## Desafío 10 — La historia como herramienta

Tenés estos dos historiales:

### Proyecto A

```text
cambios
cambios
arreglo
update
final
```

### Proyecto B

```text
Crea estructura inicial
Agrega documentación
Corrige descripción
Actualiza objetivos
Incorpora instrucciones de uso
```

### Tu desafío

Sin ejecutar ningún comando, explicá qué proyecto sería más fácil de mantener y por qué.

Después respondé:

> ¿Un historial claro tiene valor solamente para quien escribió los commits?

---

## Desafío 11 — Resolver con `git status`

Un estudiante te entrega un repositorio y solamente te dice:

> "No sé qué pasó."

No podés preguntarle qué comandos ejecutó.

### Tu desafío

Diseñá una estrategia para comenzar el diagnóstico.

La primera herramienta disponible será:

```bash
git status
```

Después de observar el resultado, explicá qué información necesitás para decidir el siguiente paso.

La consigna no busca una única secuencia de comandos.

Busca desarrollar una metodología:

```text
observar
   ↓
interpretar
   ↓
formular hipótesis
   ↓
actuar
   ↓
verificar
```

---

## Desafío 12 — ¿Qué debería contener el próximo commit?

Partís de este estado conceptual:

```text
README.md       modificado
objetivos.md    modificado
notas.md        modificado
```

Los cambios de `README.md` y `objetivos.md` corresponden a la misma tarea.

El cambio de `notas.md` corresponde a otra.

### Tu desafío

Decidí qué debería formar parte del próximo commit.

Explicá:

- qué prepararías;
- qué dejarías fuera;
- qué mensaje utilizarías;
- por qué.

Después implementá tu decisión.

---

## Desafío 13 — Construir un historial

Creá un proyecto documental pequeño.

Realizá al menos cinco modificaciones significativas.

Condiciones:

- cada commit debe representar una intención concreta;
- los mensajes deben ser descriptivos;
- no todos los cambios tienen que entrar necesariamente en el mismo commit;
- al finalizar, el repositorio debe quedar limpio.

Después observá:

```bash
git log --oneline
```

### Pregunta

> ¿Tu historial cuenta una historia razonablemente comprensible?

---

## Desafío 14 — El mensaje que no alcanza

Realizaste una modificación compleja que afecta varios archivos relacionados.

Pensás utilizar:

```text
Actualiza proyecto
```

### Tu desafío

Mejorá el mensaje.

El nuevo mensaje debería permitir responder, sin mirar los archivos:

> ¿Qué intención tuvo este cambio?

Proponé tres alternativas y elegí la que consideres más clara.

---

## Desafío 15 — El commit como unidad de trabajo

Elegí una tarea pequeña de un proyecto ficticio.

Por ejemplo:

> "Agregar la información de instalación."

Realizá todas las modificaciones necesarias para completar esa tarea.

Después:

1. observá el estado;
2. seleccioná los cambios relacionados;
3. realizá un commit;
4. escribí un mensaje descriptivo;
5. comprobá el estado;
6. consultá el historial.

### Pregunta

> ¿Qué relación existe entre una tarea y un commit?

No afirmes que necesariamente deben ser exactamente lo mismo.

Explicá qué criterio utilizarías.

---

## Desafío 16 — Detectar una mala práctica

Analizá esta secuencia:

```bash
git add .
git commit -m "cambios"
```

La persona que la ejecuta dice:

> "Esta es la forma correcta de trabajar con Git."

### Tu desafío

Explicá qué parte de la afirmación es problemática.

No hace falta afirmar que esos comandos sean incorrectos.

Analizá qué conocimiento falta para poder utilizarlos conscientemente.

---

## Desafío 17 — Sin mirar la documentación

Creá un repositorio nuevo.

Sin consultar apuntes ni prácticas anteriores, realizá:

1. un commit inicial;
2. una modificación;
3. un segundo commit;
4. otra modificación;
5. un tercer commit;
6. una modificación que deliberadamente quede sin registrar.

Después consultá:

```bash
git status
```

y:

```bash
git log --oneline
```

Explicá la diferencia entre:

```text
lo que está actualmente en la carpeta
```

y:

```text
lo que está registrado en el historial
```

---

## Desafío 18 — Enseñárselo a otro

Imaginá que un compañero nunca utilizó Git.

Tenés cinco minutos para explicarle:

```text
git status
git add
git commit
```

No podés comenzar por los comandos.

Primero explicá el problema que resuelve cada etapa.

Después mostrale un ejemplo práctico.

El objetivo es comprobar si realmente comprendés el modelo y no solamente la sintaxis.

---

## Desafío 19 — El historial que cuenta una historia

Construí un repositorio cuya evolución pueda resumirse mediante estos commits:

```text
Crea documentación inicial
Agrega objetivos
Incorpora información del proyecto
Corrige descripción
Agrega notas de trabajo
```

No es obligatorio utilizar exactamente esos mensajes.

El desafío consiste en producir una historia equivalente mediante modificaciones reales.

Después observá el historial y evaluá:

- claridad;
- orden;
- relación entre cambios;
- utilidad de los mensajes.

---

## Desafío 20 — Desafío de autonomía

Creá un repositorio nuevo desde cero.

El proyecto debe contener documentación sobre un tema que elijas.

No se proporciona una secuencia de comandos.

Debés decidir por tu cuenta:

- cuándo consultar el estado;
- qué cambios preparar;
- cuándo realizar commits;
- cómo escribir los mensajes;
- cuándo volver a verificar el estado.

Realizá al menos cinco commits.

Al finalizar, el repositorio debe estar limpio.

Después respondé:

### 1.

¿Qué decisiones tomaste sobre la organización de los commits?

### 2.

¿Por qué elegiste esos mensajes?

### 3.

¿Hubo cambios que decidiste no incluir en un commit determinado?

### 4.

¿Qué información obtuviste mediante `git status`?

### 5.

¿Qué información obtuviste mediante `git log`?

### 6.

¿Qué parte del proceso todavía realizás siguiendo una receta?

### 7.

¿Qué parte ya podés realizar de manera autónoma?

---

## Desafío final — Explicar el modelo

Sin utilizar comandos, explicá el siguiente recorrido:

```text
Archivo modificado
       ↓
Área de trabajo
       ↓
Área de preparación
       ↓
Commit
       ↓
Historial
```

La explicación debe dejar claro:

- dónde ocurre cada cosa;
- qué decisión toma el usuario;
- qué información conserva Git;
- qué significa que un cambio esté preparado;
- qué significa que un cambio esté registrado;
- por qué un archivo puede estar modificado sin formar parte del último commit.

Después demostrá el recorrido utilizando un repositorio real.

> **Si podés explicar el modelo, diagnosticar el estado y decidir qué registrar sin depender de una receta, el objetivo central del módulo está cumplido.**