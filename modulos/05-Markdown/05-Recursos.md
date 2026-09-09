# Recursos
## Módulo 05 — Markdown

Los recursos de este módulo están orientados a consultar la sintaxis de Markdown, comprender su uso en GitHub y profundizar en la construcción de documentación técnica.

---

## 1. Especificación de Markdown

### CommonMark

https://spec.commonmark.org/

CommonMark propone una especificación formal de Markdown orientada a establecer un comportamiento común entre diferentes implementaciones.

Puede utilizarse como referencia cuando sea necesario comprender con precisión cómo se interpreta determinada sintaxis.

No es necesario estudiarla de manera completa para desarrollar las actividades del módulo.

---

## 2. GitHub Flavored Markdown

GitHub utiliza una variante de Markdown denominada **GitHub Flavored Markdown (GFM)**.

Documentación oficial:

https://github.github.com/gfm/

Esta referencia resulta especialmente útil para comprender las características de Markdown disponibles en GitHub.

Entre ellas se encuentran:

- tablas;
- listas de tareas;
- enlaces;
- bloques de código;
- resaltado de sintaxis;
- otras extensiones de Markdown.

---

## 3. Markdown en GitHub

GitHub ofrece documentación específica sobre Markdown:

https://docs.github.com/es/get-started/writing-on-github

Este recurso reúne información sobre la escritura y el formato de contenido dentro de GitHub.

Puede utilizarse como referencia para:

- archivos Markdown;
- README;
- documentación;
- comentarios;
- otros contenidos de GitHub.

---

## 4. Sintaxis básica de escritura

Documentación oficial de GitHub:

https://docs.github.com/es/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github

Es una referencia especialmente útil para consultar:

- encabezados;
- texto;
- énfasis;
- listas;
- enlaces;
- imágenes;
- citas;
- código;
- tablas.

Se recomienda utilizarla como material de consulta durante la práctica.

---

## 5. Markdown para documentación

GitHub también dispone de documentación específica sobre la utilización de Markdown para estructurar contenido.

https://docs.github.com/es/get-started/writing-on-github/working-with-advanced-formatting

Este material permite profundizar en características adicionales que pueden resultar útiles cuando los documentos comienzan a crecer.

---

## 6. README

GitHub utiliza habitualmente `README.md` como punto de entrada de un repositorio.

Documentación oficial:

https://docs.github.com/es/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes

Este recurso permite profundizar en:

- función del README;
- ubicación;
- presentación;
- utilización dentro de repositorios.

La idea central trabajada en el módulo es:

> **El README debe orientar al lector y permitirle comprender rápidamente el proyecto.**

---

## 7. Pro Git en español

### Chacon, S. y Straub, B. — Pro Git

https://git-scm.com/book/es/v2

Aunque el libro está centrado en Git, resulta especialmente útil para comprender el contexto en el que utilizamos Markdown durante el curso.

Los archivos Markdown pueden formar parte de un repositorio Git y evolucionar junto con el proyecto.

Por eso resulta importante comprender la relación:

```text
Markdown
   ↓
Archivo
   ↓
Git
   ↓
Commit
   ↓
Historial
   ↓
GitHub
```

---

## 8. Visual Studio Code

### Visual Studio Code

https://code.visualstudio.com/

Visual Studio Code será utilizado como editor para crear y modificar archivos Markdown.

Su integración con Markdown permite trabajar con:

- edición;
- vista previa;
- navegación;
- archivos;
- carpetas;
- repositorios Git.

---

## 9. Vista previa de Markdown en Visual Studio Code

Documentación oficial:

https://code.visualstudio.com/docs/languages/markdown

La documentación explica las herramientas disponibles para trabajar con Markdown dentro de Visual Studio Code.

La vista previa resulta especialmente útil para comprobar:

```text
Escritura
   ↓
Visualización
   ↓
Revisión
   ↓
Corrección
```

---

## 10. Markdown Preview Enhanced

Como recurso complementario puede utilizarse:

### Markdown Preview Enhanced

https://shd101wyy.github.io/markdown-preview-enhanced/

Esta extensión amplía las posibilidades de visualización de Markdown dentro de Visual Studio Code.

No es necesaria para aprender la sintaxis básica.

Su utilización queda como complemento para quienes quieran explorar herramientas adicionales.

---

## 11. Cheatsheet de Markdown

### Markdown Guide — Basic Syntax

https://www.markdownguide.org/basic-syntax/

Esta referencia permite consultar rápidamente la sintaxis de:

- títulos;
- párrafos;
- énfasis;
- listas;
- enlaces;
- imágenes;
- código;
- tablas;
- citas.

Es especialmente útil como referencia rápida mientras se realizan ejercicios.

---

## 12. Markdown Guide — Extended Syntax

https://www.markdownguide.org/extended-syntax/

Permite consultar características adicionales de Markdown.

Puede utilizarse para profundizar después de dominar la sintaxis básica.

No es necesario incorporar todos estos elementos a los proyectos del curso.

---

## 13. Tablas

Para consultar específicamente la sintaxis de tablas puede utilizarse:

https://www.markdownguide.org/extended-syntax/#tables

Recordá que una tabla debe utilizarse cuando facilite la comparación o presentación de información.

No toda información estructurada necesita una tabla.

---

## 14. Bloques de código

Referencia:

https://www.markdownguide.org/basic-syntax/#code-blocks

Los bloques de código resultan especialmente importantes dentro de documentación técnica.

Por ejemplo:

````md
```bash
git status
git add .
git commit -m "Actualiza documentación"
```
````

Cuando sea posible, indicá el lenguaje para facilitar el resaltado de sintaxis.

---

## 15. Enlaces

Referencia:

[https://www.markdownguide.org/basic-syntax/#links](https://www.markdownguide.org/basic-syntax/#links)

La sintaxis básica es:

```md
[Texto visible](https://ejemplo.com)
```

El texto del enlace debe ser suficientemente descriptivo para que el lector comprenda su destino.

---

## 16. Imágenes

Referencia:

[https://www.markdownguide.org/basic-syntax/#images](https://www.markdownguide.org/basic-syntax/#images)

La sintaxis básica es:

```md
![Descripción de la imagen](ruta/de/la/imagen.png)
```

La descripción alternativa debe aportar información sobre la imagen.

---

## 17. Listas

Referencia:

[https://www.markdownguide.org/basic-syntax/#lists](https://www.markdownguide.org/basic-syntax/#lists)

Las listas permiten representar información:

* agrupada;
* ordenada;
* secuencial;
* jerárquica.

Deben utilizarse según la naturaleza de la información.

---

## 18. Citas

Referencia:

[https://www.markdownguide.org/basic-syntax/#blockquotes](https://www.markdownguide.org/basic-syntax/#blockquotes)

La sintaxis básica es:

```md
> Texto citado.
```

Las citas pueden utilizarse para destacar información o referencias.

---

## 19. Listas de tareas

GitHub permite utilizar listas de tareas:

```md
- [ ] Tarea pendiente
- [x] Tarea completada
```

Este recurso puede resultar útil para:

* seguimiento de actividades;
* checklists;
* issues;
* planificación.

No es necesario incorporarlo a todos los documentos.

---

## 20. Markdown dentro de GitHub

Una vez que un archivo Markdown forma parte de un repositorio, GitHub puede interpretarlo y mostrarlo como contenido formateado.

El recorrido es:

```text
README.md
    ↓
Repositorio Git
    ↓
git push
    ↓
GitHub
    ↓
Visualización Markdown
```

Esto explica por qué Markdown resulta especialmente útil dentro de proyectos alojados en GitHub.

---

## 21. Recursos para consultar durante la práctica

No es necesario memorizar toda la sintaxis.

Durante la práctica se recomienda tener a disposición:

```text
Documentación oficial de GitHub
        ↓
Referencia de Markdown
        ↓
Prueba en Visual Studio Code
        ↓
Vista previa
        ↓
Corrección
```

La consulta de documentación forma parte del proceso normal de trabajo.

---

## 22. Estrategia para resolver dudas

Cuando no recuerdes una sintaxis, evitá buscar inmediatamente un tutorial completo.

Intentá seguir este procedimiento:

```text
Identificar qué quiero hacer
        ↓
Buscar el elemento Markdown
        ↓
Consultar la sintaxis
        ↓
Probarla
        ↓
Visualizarla
        ↓
Adaptarla al documento
```

Por ejemplo:

> "Necesito una tabla."

La búsqueda debería estar orientada a:

```text
Markdown tables
```

y no necesariamente a:

```text
Curso completo de Markdown
```

La capacidad de encontrar rápidamente una referencia adecuada es parte de la competencia que buscamos desarrollar.

---

## 23. Recursos complementarios

Una vez dominados los elementos fundamentales, podés investigar:

* GitHub Flavored Markdown;
* listas de tareas;
* HTML dentro de Markdown;
* referencias de enlaces;
* emojis;
* tablas avanzadas;
* diagramas;
* extensiones de Markdown;
* herramientas de documentación.

Estos contenidos son complementarios y no forman parte del núcleo necesario para completar el módulo.

---

## 24. Qué recursos priorizar

Si necesitás resolver una duda durante una actividad, priorizá:

### Para GitHub

[GitHub Docs en español](https://docs.github.com/es?utm_source=chatgpt.com)

### Para Markdown en GitHub

[Writing and formatting on GitHub](https://docs.github.com/es/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github?utm_source=chatgpt.com)

### Para una referencia rápida

[Markdown Guide — Basic Syntax](https://www.markdownguide.org/basic-syntax/?utm_source=chatgpt.com)

### Para la especificación

[CommonMark](https://spec.commonmark.org/?utm_source=chatgpt.com)

### Para Git

[Pro Git en español](https://git-scm.com/book/es/v2?utm_source=chatgpt.com)

---

## 25. Recursos mínimos del módulo

Si solamente querés conservar las referencias esenciales:

1. **GitHub Docs**
   [https://docs.github.com/es](https://docs.github.com/es)

2. **Markdown en GitHub**
   [https://docs.github.com/es/get-started/writing-on-github](https://docs.github.com/es/get-started/writing-on-github)

3. **Pro Git en español**
   [https://git-scm.com/book/es/v2](https://git-scm.com/book/es/v2)

4. **CommonMark**
   [https://spec.commonmark.org/](https://spec.commonmark.org/)

5. **Markdown Guide**
   [https://www.markdownguide.org/basic-syntax/](https://www.markdownguide.org/basic-syntax/)

6. **Visual Studio Code — Markdown**
   [https://code.visualstudio.com/docs/languages/markdown](https://code.visualstudio.com/docs/languages/markdown)

---

## 26. Criterio de uso

Los recursos de este módulo no están pensados para ser estudiados de manera lineal.

Se recomienda:

```text
Practicar
   ↓
Encontrar una duda
   ↓
Consultar
   ↓
Probar
   ↓
Visualizar
   ↓
Corregir
```

La documentación de referencia debe convertirse en una herramienta de trabajo habitual.

---

> **No necesitás memorizar Markdown. Necesitás saber qué querés comunicar, cómo estructurarlo y dónde consultar la sintaxis cuando no la recuerdes.**
