# Práctica
## Módulo 05 — Markdown

---

## 1. Objetivo

En esta práctica vamos a aprender a utilizar Markdown para crear documentación estructurada y legible.

La práctica parte de una idea sencilla:

> **No escribimos Markdown para decorar un texto. Lo utilizamos para organizar información y comunicarla mejor.**

Vamos a trabajar progresivamente desde texto simple hasta la construcción de un README completo para un proyecto.

---

## 2. Preparar el entorno

Para esta práctica utilizaremos:

- Visual Studio Code;
- Git;
- un repositorio Git;
- Markdown Preview Enhanced;
- un navegador web.

Creá una carpeta para la práctica:

```text
practica-markdown
```

Ingresá en ella y creá:

```text
README.md
```

Abrí el archivo con Visual Studio Code.

---

## 3. Primer documento

Escribí:

```md
# Mi primer documento Markdown

Estoy aprendiendo a utilizar Markdown.

Este documento forma parte de una práctica del curso.
```

Guardá el archivo.

Observá que el contenido sigue siendo texto plano.

Ahora abrí la vista previa de Markdown.

Compará:

```text
código Markdown
```

con:

```text
documento visualizado
```

### Pregunta

¿Qué diferencia observás?

---

## 4. Título principal

El símbolo:

```text
#
```

permite crear un encabezado.

Probá:

```md
# Título principal
```

Después agregá:

```md
## Sección

### Subsección
```

El documento debería quedar:

```md
# Mi primer documento Markdown

## Sección

### Subsección
```

Visualizá nuevamente.

---

## 5. Experimentar con la jerarquía

Construí:

```md
# Proyecto

## Descripción

## Objetivos

### Objetivo general

### Objetivos específicos

## Características
```

Observá la jerarquía.

Después respondé:

> ¿Por qué `###` resulta apropiado para "Objetivo general" pero no necesariamente para "Características"?

---

## 6. Párrafos

Agregá varios párrafos:

```md
# Proyecto

Este proyecto tiene como objetivo practicar Markdown.

Markdown permite estructurar documentos utilizando una sintaxis sencilla.

Los archivos Markdown son archivos de texto y pueden formar parte de un repositorio Git.
```

Observá cómo se separan los párrafos.

Probá también qué ocurre si escribís dos frases en líneas consecutivas sin dejar una línea vacía.

---

## 7. Énfasis

Agregá:

```md
Este texto contiene **información importante**.

Este texto contiene *información enfatizada*.
```

Visualizá el resultado.

Después escribí una oración que utilice ambos tipos de énfasis.

---

## 8. Listas no ordenadas

Creá:

```md
## Herramientas

- Git
- GitHub
- Visual Studio Code
- Markdown
```

Visualizá el resultado.

Después agregá tres herramientas más.

---

## 9. Listas ordenadas

Creá:

```md
## Pasos

1. Crear el repositorio.
2. Crear el archivo.
3. Escribir el contenido.
4. Visualizar el documento.
5. Guardar los cambios.
```

Observá la diferencia entre una lista ordenada y una no ordenada.

---

## 10. Listas dentro de listas

Probá:

```md
## Contenidos

- Git
  - Repositorios
  - Commits
  - Historial
- GitHub
  - Repositorios remotos
  - Push
  - Pull
- Markdown
  - Títulos
  - Listas
  - Enlaces
```

Observá cómo Markdown representa diferentes niveles.

---

## 11. Enlaces

Agregá:

```md
## Recursos

[Git](https://git-scm.com/)

[GitHub](https://github.com/)

[Documentación de GitHub](https://docs.github.com/es)
```

Visualizá el documento.

Después agregá un enlace a un recurso que estés utilizando durante el curso.

---

## 12. Enlaces dentro de una oración

Escribí:

```md
El proyecto utiliza [Git](https://git-scm.com/) para controlar versiones.
```

Observá cómo el enlace puede formar parte de una oración sin interrumpir su lectura.

---

## 13. Código en línea

Agregá:

```md
Para consultar el estado del repositorio utilizamos `git status`.

Para registrar un cambio utilizamos `git commit`.
```

Observá la diferencia visual entre el código y el texto.

---

## 14. Bloques de código

Agregá:

````md
```bash
git status
git add .
git commit -m "Actualiza documentación"
```