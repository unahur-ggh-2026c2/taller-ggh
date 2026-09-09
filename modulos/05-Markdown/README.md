# Módulo 05 — Markdown

> **Markdown permite transformar texto simple en documentación estructurada, legible y publicable.**

---

## ¿Qué vamos a aprender?

Hasta este punto trabajamos con Git y GitHub para gestionar y publicar proyectos.

Ahora vamos a incorporar una herramienta que aparece constantemente dentro de ese ecosistema:

**Markdown.**

Markdown es un lenguaje de marcado ligero que permite estructurar texto utilizando una sintaxis sencilla y legible incluso antes de ser procesada.

Lo vamos a utilizar principalmente para crear documentación dentro de nuestros repositorios.

El recorrido será:

```text
Texto
  ↓
Markdown
  ↓
Documento estructurado
  ↓
Git
  ↓
GitHub
```

---

## ¿Por qué Markdown?

Cuando publicamos un proyecto en GitHub, no alcanza con que el código funcione.

También necesitamos poder explicar:

- qué es el proyecto;
- para qué sirve;
- cómo instalarlo;
- cómo utilizarlo;
- cómo está organizado;
- cómo contribuir;
- qué decisiones se tomaron.

Markdown permite construir esa documentación de manera simple.

---

## Markdown y GitHub

GitHub interpreta archivos Markdown y los presenta como documentos formateados.

Por eso es habitual encontrar archivos como:

```text
README.md
CONTRIBUTING.md
CHANGELOG.md
LICENSE.md
```

La extensión:

```text
.md
```

identifica normalmente un archivo Markdown.

---

## Markdown no es un procesador de textos

Markdown utiliza texto plano.

Por ejemplo:

```md
# Título

Este es un párrafo.

- Elemento uno
- Elemento dos
- Elemento tres
```

El mismo archivo puede leerse directamente como texto y, al mismo tiempo, ser interpretado por herramientas que reconocen Markdown.

Esto permite mantener una documentación:

- simple;
- portable;
- editable;
- versionable;
- legible.

---

## Elementos fundamentales

Durante el módulo vamos a trabajar progresivamente con:

- títulos;
- subtítulos;
- párrafos;
- énfasis;
- listas;
- enlaces;
- imágenes;
- código;
- bloques de código;
- tablas;
- citas;
- separación de secciones.

No se busca memorizar una sintaxis extensa.

El objetivo es aprender a utilizar Markdown para comunicar información de manera clara.

---

## Títulos

Los títulos se escriben utilizando `#`.

Por ejemplo:

```md
# Título principal

## Sección

### Subsección
```

La cantidad de `#` representa el nivel del encabezado.

La estructura debe utilizarse de manera jerárquica.

---

## Énfasis

Markdown permite destacar partes del texto.

Por ejemplo:

```md
**texto importante**

*texto enfatizado*
```

Esto permite agregar énfasis sin recurrir a herramientas visuales complejas.

---

## Listas

Una lista puede escribirse utilizando `-`:

```md
- Git
- GitHub
- Markdown
```

También pueden utilizarse listas numeradas:

```md
1. Instalar Git
2. Crear el repositorio
3. Realizar un commit
4. Publicar el proyecto
```

Las listas resultan especialmente útiles para instrucciones y procedimientos.

---

## Enlaces

Los enlaces utilizan una sintaxis sencilla:

```md
[GitHub](https://github.com/)
```

El texto visible aparece entre corchetes y la dirección entre paréntesis.

---

## Código

Para mencionar un comando o fragmento corto de código dentro de una oración se utilizan comillas invertidas:

```md
Ejecutá `git status` para consultar el estado.
```

Para fragmentos más extensos pueden utilizarse bloques de código:


````md
```bash
git status
git add .
git commit -m "Actualiza documentación"    
```
````
