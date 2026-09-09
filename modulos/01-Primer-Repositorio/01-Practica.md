# Práctica
## Módulo 01 — Mi primer repositorio

---

## 1. Objetivo

En esta práctica vamos a crear nuestro primer repositorio Git.

Hasta ahora trabajamos con el problema que aparece cuando necesitamos controlar la evolución de un proyecto.

Ahora vamos a utilizar Git para comenzar a resolverlo.

La práctica se centra en tres ideas:

- crear un repositorio;
- observar qué información administra Git;
- consultar el estado del proyecto.

Todavía no vamos a trabajar con GitHub.

---

## 2. Preparar el proyecto

Creá una carpeta llamada:

```text
laboratorio-git
```

Abrila con Visual Studio Code.

Dentro de la carpeta creá los siguientes archivos:

```text
laboratorio-git/
├── README.md
├── objetivos.md
└── integrantes.md
```

---

## 3. Crear los archivos

### `README.md`

Escribí:

```md
# Laboratorio Git

Este proyecto será utilizado para experimentar con Git.
```

### `objetivos.md`

Escribí:

```md
# Objetivos

- Aprender a trabajar con Git.
- Comprender qué es un repositorio.
- Registrar la evolución de un proyecto.
```

### `integrantes.md`

Escribí:

```md
# Integrantes

- Nombre:
- Apellido:
```

Completá tus datos.

---

## 4. Abrir la terminal

Desde Visual Studio Code abrí una terminal.

Verificá que la terminal esté ubicada dentro de la carpeta:

```text
laboratorio-git
```

Podés comprobar tu ubicación utilizando los comandos disponibles en tu sistema operativo.

Lo importante es que Git se inicialice dentro de la carpeta del proyecto y no en una carpeta equivocada.

---

## 5. Verificar que Git esté instalado

Ejecutá:

```bash
git --version
```

Deberías obtener una respuesta similar a:

```text
git version 2.x.x
```

La versión concreta puede ser diferente.

No es necesario que todos tengan exactamente la misma versión.

---

## 6. Configurar tu identidad

Antes de comenzar a registrar cambios, Git necesita saber quién realiza esos cambios.

Configurá tu nombre:

```bash
git config --global user.name "Tu Nombre"
```

Configurá tu correo electrónico:

```bash
git config --global user.email "tu-correo@example.com"
```

Utilizá los datos que quieras asociar a tus futuros commits.

No copies literalmente los valores del ejemplo.

---

## 7. Consultar la configuración

Podés comprobar la configuración utilizando:

```bash
git config --global --list
```

Verificá que aparezcan tu nombre y tu correo electrónico.

---

## 8. Inicializar el repositorio

Ahora viene nuestro primer paso importante.

Desde la carpeta `laboratorio-git`, ejecutá:

```bash
git init
```

Git debería informar que se creó un repositorio vacío.

---

## 9. Observar qué cambió

Volvé a observar la estructura de la carpeta.

Antes teníamos:

```text
laboratorio-git/
├── README.md
├── objetivos.md
└── integrantes.md
```

Después de ejecutar `git init`, deberías encontrar también:

```text
laboratorio-git/
├── .git/
├── README.md
├── objetivos.md
└── integrantes.md
```

La carpeta `.git` es administrada por Git.

No la modifiques ni elimines.

---

## 10. Pregunta para pensar

Antes de continuar, respondé:

> ¿Qué diferencia existe ahora entre esta carpeta y una carpeta común que contiene exactamente los mismos archivos?

Escribí tu respuesta en un archivo llamado:

```text
observacion.md
```

Por ejemplo:

```md
# Observación

Antes de ejecutar `git init`, la carpeta era...

Después de ejecutar `git init`, la carpeta...

La diferencia principal es...
```

No busques una definición en Internet.

Intentá explicarlo con tus propias palabras.

---

## 11. Consultar el estado

Ahora ejecutá:

```bash
git status
```

Leé cuidadosamente la respuesta.

No ejecutes otro comando inmediatamente.

Intentá identificar:

- en qué rama estás;
- si existen commits;
- qué archivos detecta Git;
- cuáles están sin seguimiento.

---

## 12. Interpretar la respuesta

Git debería indicar que existen archivos que todavía no están siendo rastreados.

Estos archivos son:

```text
README.md
objetivos.md
integrantes.md
observacion.md
```

Esto es importante.

Los archivos existen en nuestra carpeta, pero eso **no significa que formen parte del historial de Git**.

Por ahora tenemos:

```text
Carpeta de trabajo
        │
        ├── README.md
        ├── objetivos.md
        ├── integrantes.md
        └── observacion.md
                │
                ▼
              Git
                │
                └── archivos sin seguimiento
```

---

## 13. Crear un nuevo archivo

Ahora creá:

```text
notas.md
```

Con el siguiente contenido:

```md
# Notas

Estoy aprendiendo a utilizar Git.
```

Guardá el archivo.

Volvé a ejecutar:

```bash
git status
```

Observá qué cambió en la respuesta.

---

## 14. Modificar un archivo existente

Abrí:

```text
README.md
```

y agregá:

```md
## Descripción

Este repositorio forma parte del curso de Git y GitHub.
```

Guardá el archivo.

Volvé a ejecutar:

```bash
git status
```

Observá si Git informa alguna diferencia respecto de la situación anterior.

---

## 15. Una observación importante

En este punto podemos distinguir dos situaciones:

### Archivo nuevo

Un archivo que existe en la carpeta pero que Git todavía no conoce.

### Archivo modificado

Un archivo que ya existe dentro del proyecto y cuyo contenido fue modificado.

Más adelante aprenderemos cómo Git registra formalmente estas modificaciones.

Por ahora solamente necesitamos aprender a **observar el estado**.

---

## 16. Explorar la carpeta `.git`

Desde Visual Studio Code podés observar que existe:

```text
.git/
```

No modifiques su contenido.

El objetivo de esta actividad es solamente reconocer que Git necesita almacenar información propia para poder administrar el repositorio.

Si la carpeta `.git` desaparece, Git deja de reconocer esa carpeta como repositorio.

---

## 17. Una prueba

Para comprobarlo conceptualmente, podés realizar el siguiente experimento:

1. Cerrá Visual Studio Code.
2. Abrí nuevamente la carpeta.
3. Consultá el estado con:

```bash
git status
```

Deberías seguir teniendo el mismo repositorio.

La información no depende de que Visual Studio Code esté abierto.

Git funciona independientemente del editor.

---

## 18. ¿Dónde está Git?

Ahora respondé esta pregunta:

> ¿Dónde está Git?

Hay varias cosas diferentes que pueden confundirse:

- Git instalado en la computadora;
- el repositorio;
- la carpeta `.git`;
- los archivos del proyecto;
- Visual Studio Code.

Escribí una explicación breve en `observacion.md`.

---

## 19. Crear otro repositorio

Ahora vamos a comprobar que un repositorio Git es independiente de los demás.

Creá una nueva carpeta:

```text
otro-proyecto
```

Dentro de ella creá:

```text
README.md
```

Con:

```md
# Otro proyecto

Este proyecto no pertenece al laboratorio anterior.
```

Desde esa carpeta ejecutá:

```bash
git status
```

Observá qué sucede.

Después ejecutá:

```bash
git init
```

y nuevamente:

```bash
git status
```

Compará los resultados.

---

## 20. Dos repositorios independientes

Ahora deberías tener dos proyectos:

```text
laboratorio-git/
└── .git/

otro-proyecto/
└── .git/
```

Cada carpeta contiene su propio repositorio.

Los dos repositorios son independientes.

Esto permite comenzar a comprender que Git no administra "toda la computadora".

Administra proyectos específicos a través de sus repositorios.

---

## 21. Volver al laboratorio

Volvé a trabajar sobre:

```text
laboratorio-git/
```

Consultá nuevamente:

```bash
git status
```

Observá que el estado de este repositorio no fue afectado por las operaciones realizadas sobre `otro-proyecto`.

---

## 22. Qué hicimos

Durante esta práctica:

- verificamos la instalación de Git;
- configuramos nuestra identidad;
- creamos un proyecto;
- inicializamos un repositorio;
- observamos la carpeta `.git`;
- consultamos el estado del repositorio;
- identificamos archivos sin seguimiento;
- modificamos archivos;
- observamos nuevamente el estado;
- creamos un segundo repositorio;
- comprobamos que los repositorios son independientes.

Todavía no registramos ningún cambio en el historial.

Eso será el próximo paso.

---

## 23. Preguntas de cierre

Respondé en `observacion.md`:

### 1.

¿Qué hace `git init`?

### 2.

¿Qué es la carpeta `.git`?

### 3.

¿Todos los archivos que están dentro de la carpeta del proyecto forman automáticamente parte del historial?

### 4.

¿Para qué sirve `git status`?

### 5.

¿Qué diferencia existe entre tener un archivo dentro de la carpeta y tenerlo registrado por Git?

### 6.

¿Podés utilizar Git sin tener una cuenta de GitHub?

### 7.

¿Qué diferencia existe entre Git y Visual Studio Code?

---

## 24. Estado final

Al terminar la práctica, tu proyecto debería tener aproximadamente esta estructura:

```text
laboratorio-git/
├── .git/
├── README.md
├── objetivos.md
├── integrantes.md
├── observacion.md
└── notas.md
```

Git reconoce el proyecto como un repositorio, pero todavía no existe ningún registro en su historial.

Ese será nuestro próximo problema:

> **Tenemos cambios. ¿Cómo hacemos para registrarlos?**

La respuesta comienza en el **Módulo 02 — Guardar cambios**.