# Ejercicios
## Módulo 02 — Guardar cambios

Estos ejercicios buscan consolidar el modelo de trabajo fundamental de Git:

```text
modificar
   ↓
observar
   ↓
preparar
   ↓
registrar
   ↓
consultar
```

La prioridad está puesta en comprender qué ocurre en cada etapa y poder interpretar el estado del repositorio.

---

## Ejercicio 1 — Guardar no es registrar

Partí de un repositorio limpio.

1. Modificá `README.md`.
2. Guardá el archivo.
3. No ejecutes ningún comando de Git.
4. Preguntate si existe un nuevo commit.
5. Ejecutá:

```bash
git status
```

Respondé:

1. ¿Qué detectó Git?
2. ¿Existe un nuevo commit?
3. ¿Qué diferencia existe entre guardar el archivo y registrar el cambio?

---

## Ejercicio 2 — Preparar un cambio

Modificá nuevamente `README.md`.

Después ejecutá:

```bash
git add README.md
```

y:

```bash
git status
```

Respondé:

1. ¿Qué cambió respecto del ejercicio anterior?
2. ¿El cambio ya está en el historial?
3. ¿Qué significa que el archivo esté preparado?
4. ¿Qué operación falta para registrarlo?

---

## Ejercicio 3 — Crear un commit

Tomando el cambio preparado en el ejercicio anterior:

1. Creá un commit.
2. Utilizá un mensaje descriptivo.
3. Consultá el estado.
4. Consultá el historial.

Usá:

```bash
git commit -m "Mensaje descriptivo"
```

y después:

```bash
git status
```

y:

```bash
git log --oneline
```

Respondé:

> ¿Qué información nueva aparece en el historial después del commit?

---

## Ejercicio 4 — El recorrido completo

Realizá el siguiente proceso sobre un archivo:

```text
Modificar
   ↓
git status
   ↓
git add
   ↓
git status
   ↓
git commit
   ↓
git status
```

En cada momento registrá qué informa Git.

Completá:

| Momento | Estado observado |
|---|---|
| Después de modificar | |
| Después de `git add` | |
| Después de `git commit` | |

Explicá qué cambió entre cada estado.

---

## Ejercicio 5 — Dos archivos, un solo commit

Creá:

```text
archivo-a.md
archivo-b.md
```

Prepará ambos:

```bash
git add archivo-a.md
git add archivo-b.md
```

Realizá un único commit.

Después consultá:

```bash
git status
```

y:

```bash
git log --oneline
```

Respondé:

> ¿Puede un commit contener cambios de más de un archivo?

Justificá con lo que observaste.

---

## Ejercicio 6 — Dos archivos, dos commits

Modificá:

```text
archivo-a.md
archivo-b.md
```

Esta vez:

1. prepará solamente `archivo-a.md`;
2. realizá un commit;
3. consultá el estado;
4. prepará `archivo-b.md`;
5. realizá un segundo commit;
6. consultá nuevamente el historial.

Respondé:

1. ¿Cuántos commits se generaron?
2. ¿Qué contiene cada uno?
3. ¿Qué ventaja tiene separar estos cambios?

---

## Ejercicio 7 — Un archivo quedó afuera

Modificá tres archivos:

```text
README.md
objetivos.md
notas.md
```

Prepará solamente:

```text
README.md
objetivos.md
```

Realizá un commit.

Después ejecutá:

```bash
git status
```

Respondé:

1. ¿Qué archivo quedó pendiente?
2. ¿Por qué?
3. ¿El commit registró todos los cambios realizados?
4. ¿Cómo registrarías el cambio restante?

---

## Ejercicio 8 — Interpretar el estado

Para cada situación, indicá qué debería informar Git.

### Situación A

El archivo fue modificado pero todavía no se ejecutó `git add`.

### Situación B

El archivo fue preparado pero todavía no se ejecutó `git commit`.

### Situación C

El cambio fue registrado mediante un commit.

### Situación D

El archivo fue modificado nuevamente después del commit.

Completá:

| Situación | ¿Qué ocurre? |
|---|---|
| A | |
| B | |
| C | |
| D | |

---

## Ejercicio 9 — El mensaje del commit

Analizá estos mensajes:

```text
cambios
```

```text
update
```

```text
arreglo
```

```text
Agrega objetivos del proyecto
```

```text
Corrige descripción del README
```

```text
Actualiza información de integrantes
```

Ordenalos de menor a mayor utilidad para comprender el historial.

Después explicá el criterio utilizado.

---

## Ejercicio 10 — Mejorar mensajes

Transformá los siguientes mensajes en mensajes más descriptivos:

```text
cambios
```

```text
cosas nuevas
```

```text
modificaciones
```

```text
final
```

```text
arreglos varios
```

No existe una única respuesta correcta.

El mensaje debe permitir comprender qué cambio fue registrado.

---

## Ejercicio 11 — ¿Qué se está registrando?

Supongamos que modificaste:

```text
README.md
objetivos.md
```

y luego ejecutaste:

```bash
git add README.md
git commit -m "Actualiza README"
```

Respondé:

1. ¿Qué cambio se registró?
2. ¿Qué cambio no se registró?
3. ¿Qué debería mostrar `git status`?
4. ¿Qué harías para registrar el segundo cambio?

Comprobalo en un repositorio de práctica.

---

## Ejercicio 12 — Un commit, una intención

Realizá tres modificaciones independientes:

1. corregí una descripción;
2. agregá un objetivo;
3. agregá una nota.

Registrá cada una en un commit diferente.

Después ejecutá:

```bash
git log --oneline
```

Respondé:

> ¿Qué relación existe entre cada modificación y cada commit?

---

## Ejercicio 13 — El repositorio limpio

Realizá un commit y ejecutá:

```bash
git status
```

Git debería informar que no hay cambios pendientes.

Respondé:

1. ¿Qué significa que el repositorio esté limpio?
2. ¿Significa que el proyecto está terminado?
3. ¿Significa que no existen archivos?
4. ¿Qué relación existe entre el estado limpio y el último commit?

---

## Ejercicio 14 — Modificar después del commit

Partí de un repositorio limpio.

1. Modificá `README.md`.
2. Prepará el cambio.
3. Antes de hacer el commit, modificá nuevamente `README.md`.
4. Ejecutá:

```bash
git status
```

Observá la información.

Respondé:

> ¿Por qué el estado del archivo puede no coincidir exactamente con lo que estaba preparado?

No intentes solucionar la situación todavía.

El objetivo es comprender qué ocurrió.

---

## Ejercicio 15 — Selección de cambios

Modificá tres archivos:

```text
README.md
objetivos.md
notas.md
```

Prepará solamente dos.

Consultá:

```bash
git status
```

Antes del commit, explicá:

- qué cambios están preparados;
- cuáles no;
- cuáles formarán parte del próximo commit;
- cuáles quedarán fuera.

Después realizá el commit y verificá el resultado.

---

## Ejercicio 16 — Reconstruir una historia

Supongamos que un proyecto tiene estos commits:

```text
Crea README inicial
Agrega objetivos
Actualiza descripción
Corrige error de documentación
Agrega notas del proyecto
```

Respondé:

1. ¿Qué información podés inferir?
2. ¿Qué información no podés conocer solamente a partir de esos mensajes?
3. ¿Por qué un buen mensaje ayuda a comprender la evolución?

---

## Ejercicio 17 — ¿Qué comando corresponde?

Para cada situación, indicá qué herramienta utilizarías.

### A

Querés saber qué cambios existen actualmente.

### B

Querés preparar un archivo para el próximo commit.

### C

Querés registrar los cambios preparados.

### D

Querés consultar los commits anteriores.

### E

Querés comprobar si el repositorio quedó limpio.

Podés utilizar:

```text
git status
git add
git commit
git log
```

Justificá cada respuesta.

---

## Ejercicio 18 — Explicar `git add`

Explicá con tus palabras qué significa:

```bash
git add README.md
```

Tu explicación debe dejar claro:

- qué archivo se está seleccionando;
- para qué se selecciona;
- qué todavía no ocurrió;
- qué operación falta para que el cambio forme parte del historial.

---

## Ejercicio 19 — Explicar `git commit`

Explicá con tus palabras qué significa:

```bash
git commit -m "Actualiza documentación"
```

Tu explicación debe incluir:

- qué se registra;
- de dónde provienen los cambios;
- qué información adicional acompaña al registro;
- dónde podremos consultar posteriormente ese registro.

---

## Ejercicio 20 — Detectar el error

Un estudiante realiza:

```bash
git add README.md
```

y luego dice:

> "Listo, ya está guardado en Git."

¿La afirmación es correcta?

Explicá qué parte está bien y qué parte falta.

---

## Ejercicio 21 — Detectar otro error

Otro estudiante realiza:

```bash
git commit -m "Actualiza proyecto"
```

Git responde que no hay cambios para registrar.

El estudiante dice:

> "Git está roto."

Respondé:

1. ¿Qué puede estar ocurriendo?
2. ¿Qué información consultarías?
3. ¿Qué comando utilizarías para observar el estado?
4. ¿Qué debería verificar antes de volver a intentar?

---

## Ejercicio 22 — La secuencia incompleta

Completá:

```text
Modificar un archivo
        ↓
        ?
        ↓
Área de preparación
        ↓
        ?
        ↓
Historial
```

Después indicá qué comandos permiten realizar las operaciones que faltan.

---

## Ejercicio 23 — Sin copiar comandos

Creá un repositorio nuevo.

Sin consultar las prácticas anteriores:

1. agregá un archivo;
2. registrá un primer commit;
3. modificá el archivo;
4. registrá un segundo commit;
5. modificá nuevamente el archivo;
6. dejá el cambio sin registrar;
7. consultá el estado.

Finalmente explicá qué diferencia existe entre:

```text
último estado registrado
```

y:

```text
estado actual del archivo
```

---

## Ejercicio 24 — Historial legible

Creá al menos cinco commits sobre un repositorio de práctica.

Cada commit debe representar un cambio diferente.

Al finalizar:

```bash
git log --oneline
```

Analizá tu propio historial.

Respondé:

> Si mañana otra persona tuviera que continuar este proyecto, ¿los mensajes le permitirían comprender qué ocurrió?

Si la respuesta es no, mejorá los mensajes en los próximos commits.

---

## Ejercicio 25 — Integración

Construí un pequeño proyecto documental con:

```text
README.md
objetivos.md
notas.md
```

Realizá una evolución de al menos cinco pasos.

Cada paso debe:

1. modificar el proyecto;
2. consultar el estado;
3. decidir qué cambios registrar;
4. preparar los cambios;
5. realizar un commit descriptivo;
6. comprobar el estado final.

Al terminar:

```bash
git status
```

debe indicar que el repositorio está limpio.

Después:

```bash
git log --oneline
```

debe mostrar una historia comprensible.

---

## Comprobación final

Sin consultar documentación, explicá:

> **¿Qué diferencia existe entre modificar, preparar y registrar un cambio?**

Después explicá:

> **¿Por qué Git separa la preparación del registro del cambio?**

Finalmente, realizá una demostración práctica en un repositorio nuevo.

Si podés explicar el concepto y demostrarlo con Git, el objetivo principal de estos ejercicios está cumplido.