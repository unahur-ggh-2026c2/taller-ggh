# Ejercicios
## Módulo 05 — Markdown

Estos ejercicios buscan consolidar el uso de Markdown mediante situaciones concretas de documentación.

La consigna general es:

> **Elegí la estructura que mejor comunique la información. No utilices Markdown solamente porque podés hacerlo.**

---

## Ejercicio 1 — Reconocer Markdown

Indicá cuáles de los siguientes elementos forman parte de la estructura habitual de un documento Markdown:

```text
# Título
## Subtítulo
- Lista
[Enlace](URL)
`código`
**énfasis**
```

Explicá qué función cumple cada uno.

---

## Ejercicio 2 — Títulos

Transformá el siguiente texto en una estructura Markdown adecuada:

```text
Proyecto

Descripción

Objetivos

Objetivo general

Objetivos específicos

Instalación

Uso
```

La estructura esperada debe diferenciar:

- título principal;
- secciones;
- subsecciones.

---

## Ejercicio 3 — Corregir una jerarquía

El siguiente documento presenta una jerarquía incorrecta:

```md
# Proyecto

### Descripción

## Objetivos

##### Objetivo general

# Instalación

### Pasos
```

Corregilo.

Después explicá por qué elegiste cada nivel de encabezado.

---

## Ejercicio 4 — Párrafos

Convertí el siguiente texto en un documento Markdown legible:

```text
Git permite controlar versiones de los archivos de un proyecto. Esto permite registrar cambios y consultar su historial. GitHub permite trabajar con repositorios remotos y compartir proyectos.
```

Separá la información en párrafos donde consideres apropiado.

---

## Ejercicio 5 — Énfasis

Transformá las siguientes frases utilizando énfasis:

1. Git es importante para controlar versiones.
2. El repositorio debe estar limpio antes de continuar.
3. No debemos confundir `commit` con `push`.

Utilizá `**` o `*` según corresponda.

---

## Ejercicio 6 — Lista no ordenada

Transformá en una lista Markdown:

```text
Git
GitHub
Markdown
Visual Studio Code
```

Utilizá una lista no ordenada.

---

## Ejercicio 7 — Lista ordenada

Transformá en una secuencia de pasos:

```text
Crear el archivo.
Escribir el contenido.
Guardar el archivo.
Visualizar el resultado.
Corregir errores.
Publicar los cambios.
```

Utilizá una lista ordenada.

---

## Ejercicio 8 — Elegir el tipo de lista

Indicá si utilizarías una lista ordenada o no ordenada en cada situación.

### A

Características de un proyecto.

### B

Pasos para instalar una aplicación.

### C

Herramientas utilizadas.

### D

Procedimiento para publicar un repositorio.

Justificá cada decisión.

---

## Ejercicio 9 — Lista anidada

Representá mediante Markdown:

```text
Git
    Repositorios
    Commits
    Historial

GitHub
    Repositorios remotos
    Push
    Pull

Markdown
    Títulos
    Listas
    Enlaces
```

Utilizá listas anidadas.

---

## Ejercicio 10 — Enlaces

Creá enlaces Markdown para:

```text
Git
https://git-scm.com/

GitHub
https://github.com/

GitHub Docs
https://docs.github.com/es
```

El texto visible debe ser el nombre de cada recurso.

---

## Ejercicio 11 — Código en línea

Transformá las siguientes frases:

```text
Para consultar el estado utilizamos git status.
Para preparar cambios utilizamos git add.
Para registrar cambios utilizamos git commit.
```

Utilizá código en línea para los comandos.

---

## Ejercicio 12 — Bloque de código

Transformá esta secuencia en un bloque de código Bash:

```text
git status
git add .
git commit -m "Actualiza documentación"
git push
```

Indicá correctamente el lenguaje.

---

## Ejercicio 13 — Código de otro lenguaje

Escribí un bloque Markdown que muestre:

```python
nombre = "Mauricio"
print(nombre)
```

Indicá el lenguaje correspondiente.

---

## Ejercicio 14 — Diferenciar código y explicación

Construí una sección Markdown que explique cómo consultar el estado de un repositorio.

Debe incluir:

1. una explicación;
2. el comando como código en línea;
3. un bloque de código;
4. una segunda explicación.

---

## Ejercicio 15 — Tabla

Construí una tabla con esta información:

| Comando | Función |
|---|---|
| `git status` | Consulta el estado |
| `git add` | Prepara cambios |
| `git commit` | Registra cambios |
| `git push` | Publica cambios |
| `git pull` | Incorpora cambios |

Escribila utilizando sintaxis Markdown.

---

## Ejercicio 16 — Diseñar una tabla

Construí una tabla con tres columnas para describir herramientas:

```text
Herramienta
Función
Contexto de uso
```

Incluí al menos cuatro herramientas.

---

## Ejercicio 17 — ¿Tabla o lista?

Decidí qué estructura utilizarías para cada caso.

### A

Una lista de características de un proyecto.

### B

Una comparación entre cinco comandos indicando función y propósito.

### C

Una secuencia de pasos.

### D

Una lista de herramientas.

Justificá cada decisión.

---

## Ejercicio 18 — Citas

Convertí en una cita Markdown:

```text
La documentación también forma parte del proyecto.
```

Después escribí una segunda cita relacionada con Git.

---

## Ejercicio 19 — Imagen

Suponiendo que existe:

```text
imagenes/git.png
```

escribí Markdown para incorporarla.

La descripción alternativa debe explicar qué contiene la imagen.

---

## Ejercicio 20 — Documento completo

Construí un documento llamado:

```text
proyecto.md
```

Debe contener:

```md
# Nombre del proyecto

Descripción breve.

## Objetivos

- Objetivo 1
- Objetivo 2
- Objetivo 3

## Características

- Característica 1
- Característica 2

## Instalación

Pasos.

## Uso

Explicación.

## Recursos

Enlaces.
```

Agregá al menos:

- un bloque de código;
- una tabla;
- una cita.

---

## Ejercicio 21 — README

Creá un README para un proyecto ficticio.

Debe responder:

1. ¿Qué es?
2. ¿Para qué sirve?
3. ¿Qué características tiene?
4. ¿Cómo se instala?
5. ¿Cómo se utiliza?
6. ¿Dónde se puede obtener más información?

Utilizá Markdown para organizar las respuestas.

---

## Ejercicio 22 — Mejorar un README

Utilizá este documento:

```md
# Mi proyecto

Este proyecto sirve para aprender Git. Tiene comandos y ejemplos. Para instalarlo hay que clonar el repositorio y entrar a la carpeta. Después se puede consultar la documentación.

Git sirve para controlar versiones.

GitHub permite compartir el proyecto.

git clone https://github.com/usuario/proyecto.git

Hay varios recursos.

Git
GitHub
Markdown
```

Mejoralo utilizando:

- títulos;
- párrafos;
- listas;
- enlaces;
- código;
- bloques de código.

---

## Ejercicio 23 — Organización

Un compañero escribió todo en un único bloque:

```md
# Proyecto

Este proyecto es una aplicación educativa. Tiene tres características. La primera permite registrar usuarios. La segunda permite consultar información. La tercera permite generar informes. Para instalarla hay que clonar el repositorio y ejecutar el comando correspondiente. Los requisitos son Git y Python. Para más información consultar la documentación.
```

Reorganizá el documento utilizando secciones.

---

## Ejercicio 24 — Separación entre contenido y estructura

Tomá este contenido:

```text
El proyecto utiliza Git para controlar versiones.
GitHub se utiliza para alojar el repositorio remoto.
Markdown se utiliza para documentar el proyecto.
```

Construí una estructura Markdown que permita presentar:

```text
Tecnologías
    Git
    GitHub
    Markdown
```

sin cambiar el contenido conceptual.

---

## Ejercicio 25 — Documentar un procedimiento

Documentá el siguiente procedimiento:

```text
Crear una carpeta.
Ingresar en la carpeta.
Inicializar Git.
Crear un archivo.
Realizar el primer commit.
```

El documento debe contener:

- una explicación breve;
- una lista ordenada;
- los comandos correspondientes.

---

## Ejercicio 26 — Detectar problemas

Analizá:

```md
# Proyecto

### Instalación

## Objetivos

##### Objetivo 1

# Características

### Uso

## Recursos
```

Identificá todos los problemas de estructura que encuentres.

Después corregilo.

---

## Ejercicio 27 — Elegir la herramienta adecuada

Para cada situación elegí el elemento Markdown más apropiado:

| Situación | Elemento |
|---|---|
| Título principal | |
| Lista de características | |
| Pasos de instalación | |
| URL de documentación | |
| Comando dentro de una oración | |
| Conjunto de comandos | |
| Datos comparables | |
| Frase destacada | |
| Imagen | |

---

## Ejercicio 28 — Documentar Git

Creá un documento llamado:

```text
git-basico.md
```

Debe contener:

```md
# Git básico

## ¿Qué es Git?

...

## Comandos principales

...

## Crear un repositorio

...

## Registrar cambios

...

## Consultar el historial

...
```

Incluí comandos reales en bloques de código.

---

## Ejercicio 29 — Documentar GitHub

Creá:

```text
github.md
```

Incluí:

```md
# GitHub

## ¿Qué es?

...

## Repositorios remotos

...

## Publicar cambios

...

## Obtener cambios

...

## Recursos

...
```

Utilizá enlaces hacia documentación oficial.

---

## Ejercicio 30 — Documentar Markdown

Creá:

```text
markdown.md
```

El documento debe explicar:

- qué es Markdown;
- para qué sirve;
- qué extensión utilizan normalmente sus archivos;
- cómo crear títulos;
- cómo crear listas;
- cómo crear enlaces;
- cómo mostrar código.

Incluí ejemplos de sintaxis.

---

## Ejercicio 31 — Crear una guía

Construí:

```text
guia.md
```

Debe tener esta estructura:

```md
# Guía de trabajo

## Introducción

## Requisitos

## Instalación

## Configuración

## Uso

## Problemas frecuentes

## Recursos
```

Completá cada sección con contenido.

---

## Ejercicio 32 — Documentación orientada a otra persona

Elegí un procedimiento que conozcas.

Puede ser:

- instalar un programa;
- ejecutar un proyecto;
- configurar una herramienta;
- realizar una operación con Git.

Documentalo pensando en una persona que nunca lo realizó.

La documentación debe permitirle completar el procedimiento sin preguntarte qué hacer en cada paso.

---

## Ejercicio 33 — Revisar claridad

Elegí uno de los documentos anteriores.

Revisalo utilizando estas preguntas:

```text
¿Tiene un título claro?
¿La información está organizada?
¿La jerarquía es correcta?
¿Las instrucciones son comprensibles?
¿Los comandos se distinguen del texto?
¿Los enlaces son claros?
¿Hay información innecesaria?
¿Falta información?
```

Realizá las mejoras necesarias.

---

## Ejercicio 34 — Markdown y Git

Tomá uno de tus documentos Markdown.

Consultá:

```bash
git status
```

Registrá el archivo:

```bash
git add .
git commit -m "Agrega documentación Markdown"
```

Después consultá:

```bash
git log --oneline
```

Respondé:

> ¿Qué relación existe entre el archivo Markdown y el commit?

---

## Ejercicio 35 — Markdown y GitHub

Publicá el documento mediante:

```bash
git push
```

Ingresá al repositorio desde GitHub.

Observá cómo se presenta el documento.

Respondé:

1. ¿Qué elementos Markdown se interpretaron?
2. ¿Qué diferencias observaste respecto de la vista previa local?
3. ¿El documento resulta comprensible?

---

## Ejercicio 36 — Documentación distribuida

Creá:

```text
README.md
INSTALACION.md
USO.md
RECURSOS.md
```

El README debe funcionar como punto de entrada.

Incluí enlaces desde `README.md` hacia los demás documentos.

Construí una estructura como:

```text
README
  ├── Instalación
  ├── Uso
  └── Recursos
```

---

## Ejercicio 37 — README como punto de entrada

Revisá el README anterior.

Sin abrir ningún otro archivo, respondé:

> ¿Una persona nueva podría comprender de qué trata el proyecto?

> ¿Sabría dónde encontrar las instrucciones de instalación?

> ¿Sabría dónde encontrar las instrucciones de uso?

Si la respuesta es negativa, mejorá el README.

---

## Ejercicio 38 — Corregir un documento real

Elegí un README público de GitHub.

Analizá:

- estructura;
- títulos;
- listas;
- enlaces;
- código;
- tablas;
- claridad.

No copies el contenido.

Identificá al menos cinco decisiones de organización que consideres acertadas o mejorables.

---

## Ejercicio 39 — Sintaxis vs. comunicación

Construí dos versiones de un mismo documento.

### Versión A

Utilizá todos los elementos Markdown que puedas.

### Versión B

Utilizá solamente los elementos que realmente aporten claridad.

Comparalas.

Respondé:

> ¿Cuál comunica mejor la información?

> ¿Por qué?

---

## Ejercicio 40 — Ejercicio integrador

Construí un documento técnico completo.

Debe incluir:

- título;
- introducción;
- secciones;
- subsecciones;
- párrafos;
- énfasis;
- lista no ordenada;
- lista ordenada;
- enlace;
- código en línea;
- bloque de código;
- tabla;
- cita;
- imagen.

Después revisá el documento y eliminá cualquier elemento que no aporte valor.

---

## Comprobación final

Sin consultar documentación, intentá responder:

### 1.

¿Cómo se crea un título principal?

### 2.

¿Cómo se crea una subsección?

### 3.

¿Cómo se crea una lista no ordenada?

### 4.

¿Cómo se crea una lista ordenada?

### 5.

¿Cómo se crea un enlace?

### 6.

¿Cómo se muestra código dentro de una oración?

### 7.

¿Cómo se crea un bloque de código?

### 8.

¿Cómo se crea una tabla?

### 9.

¿Cómo se crea una cita?

### 10.

¿Cómo se incorpora una imagen?

### 11.

¿Qué función cumple normalmente un `README.md`?

### 12.

¿Por qué Markdown resulta especialmente útil en un repositorio Git?

---

## Criterio de resolución

No se evalúa solamente que la sintaxis sea correcta.

También se debe considerar:

- organización;
- claridad;
- jerarquía;
- legibilidad;
- elección adecuada de cada elemento;
- utilidad de la documentación.

> **Una documentación técnicamente correcta pero difícil de leer sigue siendo una mala documentación.**