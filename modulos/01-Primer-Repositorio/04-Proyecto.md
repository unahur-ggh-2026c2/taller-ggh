# Proyecto
## Módulo 01 — Mi primer repositorio

---

## 1. Propósito

En este proyecto vas a construir desde cero un repositorio Git y utilizarlo para comenzar a registrar la evolución de un pequeño proyecto documental.

La actividad integra los conceptos trabajados durante el módulo:

- repositorio;
- inicialización;
- archivos;
- estado;
- seguimiento;
- área de preparación;
- commit;
- historial inicial.

El proyecto será deliberadamente sencillo.

La dificultad no está en el contenido de los archivos, sino en **aprender a administrar correctamente su evolución con Git**.

---

## 2. El proyecto

Vas a crear un proyecto llamado:

```text
mi-primer-repositorio
```

El proyecto representará la documentación inicial de una aplicación ficticia.

La estructura final deberá ser:

```text
mi-primer-repositorio/
├── README.md
├── objetivos.md
├── integrantes.md
└── notas.md
```

---

## 3. Crear el repositorio

Creá la carpeta:

```text
mi-primer-repositorio
```

Abrila con Visual Studio Code.

Inicializá Git dentro de ella.

Después comprobá que Git reconoce el proyecto mediante:

```bash
git status
```

Antes de continuar, verificá que comprendés qué ocurrió al ejecutar `git init`.

---

## 4. Crear la documentación inicial

### `README.md`

Creá el archivo con:

```md
# Mi primer repositorio

Este proyecto fue creado como práctica para aprender Git.

## Descripción

El proyecto representa la documentación inicial de una aplicación ficticia.
```

### `objetivos.md`

Creá:

```md
# Objetivos

- Aprender los conceptos fundamentales de Git.
- Practicar el registro de cambios.
- Comprender el funcionamiento de un repositorio.
```

### `integrantes.md`

Creá:

```md
# Integrantes

- Nombre:
- Apellido:
```

Completá tus datos.

### `notas.md`

Creá:

```md
# Notas

Este archivo contiene observaciones realizadas durante el aprendizaje.
```

---

## 5. Observar antes de registrar

Consultá:

```bash
git status
```

Antes de ejecutar `git add`, observá cuidadosamente qué información proporciona Git.

Respondé:

- ¿qué archivos detecta?
- ¿qué significa que estén sin seguimiento?
- ¿existe todavía algún commit?
- ¿qué información falta para que exista un historial?

---

## 6. Primer registro

Prepará los archivos:

```bash
git add README.md
git add objetivos.md
git add integrantes.md
git add notas.md
```

Consultá nuevamente:

```bash
git status
```

Verificá que los cuatro archivos estén preparados.

Ahora realizá el primer commit:

```bash
git commit -m "Crea documentación inicial del proyecto"
```

Finalmente:

```bash
git status
```

El repositorio debería quedar limpio.

---

## 7. Primera evolución

Ahora el proyecto comienza a evolucionar.

Modificá `README.md` agregando:

```md
## Características

- Organización de documentación.
- Registro de objetivos.
- Identificación de integrantes.
```

Modificá también `objetivos.md` agregando:

```md
- Comprender el flujo básico de trabajo con Git.
```

Guardá ambos archivos.

Consultá:

```bash
git status
```

Observá qué cambios detectó Git.

---

## 8. Segundo commit

Prepará los cambios y realizá un segundo commit.

Utilizá un mensaje que describa claramente qué incorporaste.

Por ejemplo:

```bash
git commit -m "Amplia documentación y objetivos"
```

Consultá nuevamente:

```bash
git status
```

El repositorio debería volver a quedar limpio.

---

## 9. Una modificación selectiva

Ahora realizá cambios diferentes en los archivos:

### `README.md`

Agregá una sección:

```md
## Estado

El proyecto se encuentra en desarrollo.
```

### `integrantes.md`

Agregá:

```md
## Rol

Responsable del proyecto.
```

### `notas.md`

Agregá una observación personal relacionada con lo aprendido.

Guardá todos los archivos.

---

## 10. Preparar solamente algunos cambios

Ahora prepará solamente:

```text
README.md
integrantes.md
```

No prepares `notas.md`.

Consultá:

```bash
git status
```

Observá la diferencia entre:

- cambios preparados;
- cambios que todavía no están preparados.

---

## 11. Tercer commit

Registrá solamente los cambios preparados.

Utilizá un mensaje descriptivo.

Por ejemplo:

```bash
git commit -m "Actualiza estado e integrantes"
```

Después ejecutá:

```bash
git status
```

Debería quedar pendiente únicamente el cambio realizado en:

```text
notas.md
```

Esto es importante.

El commit anterior no debería contener ese cambio.

---

## 12. Registrar el cambio restante

Ahora prepará `notas.md` y realizá un nuevo commit.

El mensaje deberá describir el cambio realizado.

Por ejemplo:

```bash
git commit -m "Agrega notas de aprendizaje"
```

Consultá nuevamente:

```bash
git status
```

El repositorio debería quedar limpio.

---

## 13. Construir una evolución comprensible

Llegado este punto deberías tener varios commits.

La evolución debería poder interpretarse aproximadamente así:

```text
Crea documentación inicial del proyecto
        ↓
Amplia documentación y objetivos
        ↓
Actualiza estado e integrantes
        ↓
Agrega notas de aprendizaje
```

Los mensajes concretos pueden ser diferentes.

Lo importante es que permitan comprender qué ocurrió.

---

## 14. Revisar el historial

Ahora vamos a observar por primera vez el historial del repositorio.

Ejecutá:

```bash
git log
```

Observá:

- los commits;
- los mensajes;
- el autor;
- la fecha;
- el identificador de cada commit.

Después ejecutá:

```bash
git log --oneline
```

Compará ambas salidas.

---

## 15. Interpretar el historial

Respondé:

1. ¿Cuántos commits realizaste?
2. ¿Cuál es el más reciente?
3. ¿Cuál es el más antiguo?
4. ¿Qué información conserva cada commit?
5. ¿Los mensajes permiten comprender la evolución del proyecto?
6. ¿Qué ocurriría si todos los mensajes fueran simplemente `cambios`?

Registrá las respuestas en:

```text
reflexion.md
```

---

## 16. Modificación final

Realizá una última modificación significativa sobre `README.md`.

Agregá:

```md
## Aprendizaje

Este repositorio fue construido como práctica para comprender
el funcionamiento básico de Git y el registro de cambios.
```

Registrá el cambio en un nuevo commit.

Utilizá un mensaje claro y descriptivo.

---

## 17. Verificación final

Ejecutá:

```bash
git status
```

El repositorio debe quedar limpio.

Después ejecutá:

```bash
git log --oneline
```

Verificá que el nuevo commit aparezca en el historial.

---

## 18. Estado final del proyecto

La estructura debería ser:

```text
mi-primer-repositorio/
├── .git/
├── README.md
├── objetivos.md
├── integrantes.md
├── notas.md
└── reflexion.md
```

El contenido puede haber evolucionado respecto de la versión inicial.

Lo importante es que Git conserve esa evolución mediante commits.

---

## 19. Reflexión

Completá `reflexion.md`:

```md
# Reflexión

## ¿Qué aprendí?

...

## ¿Qué diferencia existe entre modificar un archivo y registrar un cambio?

...

## ¿Qué función cumple `git add`?

...

## ¿Qué función cumple `git commit`?

...

## ¿Qué información puedo obtener del historial?

...

## ¿Qué me resultó más difícil?

...

## ¿Qué necesito seguir practicando?

...
```

Respondé con tus propias palabras.

No copies definiciones de la documentación.

---

## 20. Criterios de finalización

El proyecto está terminado cuando:

- existe un repositorio Git correctamente inicializado;
- los archivos del proyecto están registrados;
- existen varios commits;
- los commits tienen mensajes descriptivos;
- se realizaron cambios en diferentes momentos;
- se registraron cambios de manera selectiva;
- se consultó el estado del repositorio;
- se consultó el historial;
- el repositorio termina en estado limpio;
- la reflexión final está completa.

---

## 21. La pregunta importante

Al terminar, deberías poder responder sin consultar documentación:

> **¿Qué diferencia existe entre trabajar sobre un archivo y registrar su evolución mediante Git?**

Y también:

> **¿Por qué no alcanza con ejecutar comandos sin comprender el estado del repositorio?**

Si podés responder ambas preguntas y completar el proyecto de manera autónoma, estás preparado para avanzar.

---

## 22. Puente hacia el siguiente módulo

Hasta ahora aprendimos a:

```text
crear un repositorio
       ↓
observar su estado
       ↓
preparar cambios
       ↓
registrar commits
       ↓
consultar el historial
```

Pero todavía falta una pregunta fundamental:

> **¿Qué ocurre exactamente con nuestros archivos entre un commit y otro?**

En el próximo módulo vamos a profundizar en el proceso de **guardar cambios** y comprender mejor el recorrido que realiza una modificación antes de formar parte del historial.