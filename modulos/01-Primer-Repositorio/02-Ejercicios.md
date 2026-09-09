# Ejercicios
## Módulo 01 — Mi primer repositorio

Estos ejercicios tienen como objetivo consolidar la comprensión del repositorio Git, su estado y la relación entre la carpeta de trabajo y la información administrada por Git.

No se busca todavía resolver situaciones complejas.

La prioridad es que puedas **observar lo que ocurre y explicar por qué ocurre**.

---

## Ejercicio 1 — ¿Es un repositorio?

Tenés las siguientes carpetas:

```text
proyecto-a/
├── README.md
├── objetivos.md
└── integrantes.md
```

y:

```text
proyecto-b/
├── .git/
├── README.md
├── objetivos.md
└── integrantes.md
```

Respondé:

1. ¿Cuál de las dos es un repositorio Git?
2. ¿Qué diferencia existe entre ambas?
3. ¿Qué función cumple `.git`?
4. ¿Podrías utilizar Git sobre `proyecto-a` sin convertirla previamente en un repositorio?

Justificá tus respuestas.

---

## Ejercicio 2 — Crear un repositorio

Creá una carpeta llamada:

```text
ejercicio-repositorio
```

Dentro de ella creá:

```text
README.md
```

Con el siguiente contenido:

```md
# Ejercicio de repositorio

Este proyecto fue creado para practicar Git.
```

Inicializá el repositorio.

Después ejecutá:

```bash
git status
```

Respondé:

1. ¿Qué información te muestra Git?
2. ¿Qué archivos aparecen?
3. ¿Existe algún commit?
4. ¿El archivo `README.md` forma parte todavía del historial?

---

## Ejercicio 3 — Observar antes y después

Realizá la siguiente secuencia:

1. Creá una carpeta nueva.
2. Creá un archivo `README.md`.
3. Ejecutá `git status`.
4. Inicializá Git.
5. Ejecutá nuevamente `git status`.

Registrá las diferencias entre ambos estados.

Podés utilizar una tabla:

| Momento | ¿Es repositorio? | ¿Qué informa Git? |
|---|---|---|
| Antes de `git init` | | |
| Después de `git init` | | |

---

## Ejercicio 4 — Archivos sin seguimiento

Dentro de un repositorio existente creá:

```text
uno.md
dos.md
tres.md
```

Consultá:

```bash
git status
```

Respondé:

1. ¿Qué archivos aparecen?
2. ¿Por qué aparecen?
3. ¿Git los modificó?
4. ¿Git los registró en el historial?
5. ¿Qué significa que estén sin seguimiento?

No utilices todavía `git add`.

---

## Ejercicio 5 — Agregar un archivo

Ahora sí vamos a introducir una nueva operación.

Elegí uno de los archivos creados anteriormente y ejecutá:

```bash
git add uno.md
```

Después ejecutá:

```bash
git status
```

Compará el resultado con el estado anterior.

Respondé:

1. ¿Qué cambió?
2. ¿Qué archivo aparece ahora?
3. ¿El archivo ya forma parte del historial?
4. ¿Qué significa que esté preparado para ser registrado?

Todavía no hagas un commit.

---

## Ejercicio 6 — Preparar varios archivos

Creá dos archivos nuevos:

```text
notas.md
ideas.md
```

Después preparalos para ser registrados.

Podés hacerlo individualmente:

```bash
git add notas.md
git add ideas.md
```

Consultá nuevamente:

```bash
git status
```

Identificá:

- archivos sin seguimiento;
- archivos preparados;
- archivos que todavía no fueron registrados.

---

## Ejercicio 7 — El área de preparación

Hasta ahora vimos que existe una situación intermedia entre modificar un archivo y registrar formalmente el cambio.

Representá mediante un esquema el siguiente recorrido:

```text
Archivo
   ↓
Cambio
   ↓
?
   ↓
Historial
```

Completá el esquema indicando qué elemento falta.

Después explicá con tus palabras qué función cumple esa etapa intermedia.

---

## Ejercicio 8 — Primer commit

Utilizando uno de los archivos preparados en los ejercicios anteriores, realizá tu primer commit.

Usá un mensaje descriptivo.

Por ejemplo:

```bash
git commit -m "Agrega notas iniciales"
```

Después ejecutá:

```bash
git status
```

Respondé:

1. ¿Qué cambió?
2. ¿Qué informa ahora Git?
3. ¿Qué significa que el árbol de trabajo esté limpio?
4. ¿Existe ahora un registro en el historial?

---

## Ejercicio 9 — El mensaje del commit

Compará los siguientes mensajes:

```text
cambios
```

```text
cosas nuevas
```

```text
modificaciones varias
```

con:

```text
Agrega descripción inicial del proyecto
```

y:

```text
Incorpora objetivos del proyecto
```

Respondé:

1. ¿Cuáles son más útiles?
2. ¿Por qué?
3. ¿Qué debería permitir comprender un mensaje de commit?
4. ¿Qué problemas puede generar un historial lleno de mensajes poco descriptivos?

---

## Ejercicio 10 — Modificar después del commit

Partiendo de un repositorio que ya tenga al menos un commit:

1. Modificá `README.md`.
2. Guardá el archivo.
3. Ejecutá:

```bash
git status
```

4. Observá el estado.
5. Prepará el cambio.
6. Volvé a consultar el estado.
7. Realizá un nuevo commit.
8. Consultá nuevamente el estado.

Registrá las diferentes situaciones.

Completá:

```text
Antes de modificar:
________________________

Después de modificar:
________________________

Después de git add:
________________________

Después de git commit:
________________________
```

---

## Ejercicio 11 — ¿Qué está pasando?

Durante el ejercicio anterior atravesaste varias situaciones.

Relacioná cada una con su descripción.

### Situaciones

A. Archivo modificado.

B. Archivo preparado.

C. Cambio registrado.

### Descripciones

1. El cambio forma parte de un commit.

2. El contenido del archivo es diferente respecto del último estado registrado.

3. El cambio fue seleccionado para formar parte del próximo commit.

Completá:

```text
A → __

B → __

C → __
```

---

## Ejercicio 12 — El estado limpio

Realizá un commit y después ejecutá:

```bash
git status
```

Git debería indicar que no existen cambios pendientes.

Explicá:

> ¿Qué significa realmente que el repositorio esté "limpio"?

No significa que el proyecto no tenga archivos.

No significa que el proyecto esté terminado.

Explicá qué significa en relación con Git.

---

## Ejercicio 13 — Agregar no es registrar

Respondé con tus palabras:

> ¿Cuál es la diferencia entre `git add` y `git commit`?

Podés utilizar el siguiente esquema como ayuda:

```text
Modificar
    ↓
git add
    ↓
?
    ↓
git commit
    ↓
?
```

Completá los dos espacios.

---

## Ejercicio 14 — El archivo que quedó afuera

Supongamos que modificaste tres archivos:

```text
README.md
objetivos.md
integrantes.md
```

Pero ejecutaste:

```bash
git add README.md
git add objetivos.md
```

y luego:

```bash
git commit -m "Actualiza documentación"
```

Respondé:

1. ¿Qué cambio quedó registrado?
2. ¿Qué cambio quedó afuera?
3. ¿Qué debería mostrar `git status`?
4. ¿El commit puede contener solamente una parte de los cambios realizados?

Experimentalo en tu repositorio.

---

## Ejercicio 15 — Preparar selectivamente

Realizá modificaciones diferentes en:

```text
README.md
objetivos.md
integrantes.md
```

Prepará solamente:

```text
README.md
```

Realizá un commit.

Después consultá:

```bash
git status
```

Identificá qué cambios quedaron pendientes.

Luego prepará los restantes y realizá otro commit.

### Pregunta

¿Por qué puede ser útil decidir exactamente qué cambios forman parte de cada commit?

---

## Ejercicio 16 — Leer el estado

Ejecutá:

```bash
git status
```

en diferentes momentos del trabajo.

Para cada estado, completá una tabla:

| Situación | ¿Qué muestra Git? | ¿Qué significa? |
|---|---|---|
| Repositorio recién creado | | |
| Archivo nuevo | | |
| Archivo preparado | | |
| Archivo modificado | | |
| Después de un commit | | |

El objetivo es que `git status` deje de ser una salida que simplemente leemos y pase a ser una herramienta que sabemos interpretar.

---

## Ejercicio 17 — Ordenar el proceso

Las siguientes acciones están desordenadas:

```text
git commit
modificar archivo
git init
git add
crear archivo
git status
```

Ordenalas para construir un recorrido lógico desde una carpeta común hasta el registro de un primer cambio.

Después explicá por qué elegiste ese orden.

---

## Ejercicio 18 — Situación problemática

Un compañero realiza lo siguiente:

```bash
git init
git add .
git commit -m "proyecto"
```

y afirma:

> "Listo. Ya aprendí a usar Git."

¿Qué le responderías?

No es necesario enumerar todos los comandos que todavía desconoce.

Explicá qué conceptos debería comprender además de saber ejecutar una secuencia de comandos.

---

## Ejercicio 19 — Explicar el recorrido

Explicá con tus palabras el siguiente proceso:

```text
Proyecto
   ↓
git init
   ↓
Repositorio
   ↓
Modificar archivo
   ↓
git add
   ↓
Área de preparación
   ↓
git commit
   ↓
Historial
```

Tu explicación debería poder ser comprendida por alguien que nunca utilizó Git.

---

## Ejercicio 20 — Comprobación final

Sin mirar apuntes, creá un repositorio nuevo llamado:

```text
prueba-final-modulo-01
```

Realizá las siguientes acciones:

1. Inicializá Git.
2. Creá un `README.md`.
3. Consultá el estado.
4. Prepará el archivo.
5. Consultá nuevamente el estado.
6. Realizá un commit.
7. Consultá nuevamente el estado.
8. Modificá el `README.md`.
9. Consultá el estado.
10. Prepará nuevamente el cambio.
11. Realizá un segundo commit.
12. Consultá el estado final.

Al terminar, explicá sin consultar documentación:

> **¿Qué diferencia existe entre modificar un archivo, preparar un cambio y registrar un commit?**

Si podés responder y realizar el recorrido sin seguir una receta, el objetivo principal del módulo está cumplido.