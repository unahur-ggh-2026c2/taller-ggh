# Cheatsheet — Markdown

> Referencia rápida para escribir documentación en Markdown, especialmente en GitHub.

---

## Títulos

```md
# Título principal

## Sección

### Subsección
```

Usá los niveles de encabezado de manera jerárquica.

---

## Texto

**Negrita:**

```md
**texto importante**
```

*Cursiva:*

```md
*texto destacado*
```

~~Tachado:~~

```md
~~texto eliminado~~
```

---

## Listas

Lista sin ordenar:

```md
- Elemento
- Elemento
- Elemento
```

Lista ordenada:

```md
1. Primer paso
2. Segundo paso
3. Tercer paso
```

---

## Enlaces

```md
[Texto del enlace](https://ejemplo.com)
```

Ejemplo:

```md
[Documentación de Git](https://git-scm.com/docs)
```

---

## Imágenes

```md
![Texto alternativo](ruta/imagen.png)
```

El texto alternativo describe la imagen cuando esta no puede visualizarse.

---

## Código en línea

Para mencionar un comando o elemento dentro de un párrafo:

```md
Usá `git status` para consultar el estado.
```

Resultado:

Usá `git status` para consultar el estado.

---

## Bloques de código

Código sin indicar lenguaje:

````md
```
git status
git add .
git commit -m "Mensaje"
```
````

Indicando lenguaje:

````md
```bash
git status
git add .
git commit -m "Mensaje"
```
````

Para código Python:

````md
```python
print("Hola")
```
````

> En los bloques de código del material del curso se utilizan **tres backticks de apertura y tres de cierre**.

---

## Citas

```md
> Esta es una cita.
```

Para varias líneas:

```md
> Primera línea.
>
> Segunda línea.
```

---

## Separador

```md
---
```

Útil para separar secciones de un documento.

---

## Tablas

```md
| Comando | Función |
|---|---|
| `git status` | Ver estado |
| `git add` | Preparar cambios |
| `git commit` | Registrar cambios |
```

Resultado:

| Comando      | Función           |
| ------------ | ----------------- |
| `git status` | Ver estado        |
| `git add`    | Preparar cambios  |
| `git commit` | Registrar cambios |

---

## Listas de tareas

```md
- [ ] Pendiente
- [x] Completado
```

Resultado:

* [ ] Pendiente
* [x] Completado

---

## Escapar caracteres

Si necesitás mostrar un carácter que Markdown interpreta de manera especial, podés utilizar `\`.

Ejemplo:

```md
\*Este texto no será cursiva\*
```

---

## README

Un README puede organizarse, por ejemplo, así:

```md
# Nombre del proyecto

Descripción breve.

## Objetivo

...

## Requisitos

...

## Instalación

...

## Uso

...

## Estructura

...

## Próximos pasos

...
```

No es necesario utilizar todas las secciones.

La estructura debe adaptarse al proyecto.

---

## Enlaces internos

Podés enlazar archivos del mismo repositorio:

```md
[Guía de instalación](docs/instalacion.md)
```

También podés enlazar directorios:

```md
[Ejemplos](ejemplos/)
```

Verificá que las rutas existan.

---

## Buenas prácticas

```text
Usar títulos claros
Mantener una jerarquía coherente
Preferir listas cuando corresponda
Usar código para comandos
Agregar texto alternativo a imágenes
Verificar enlaces
Mantener actualizado el README
```

---

## Errores frecuentes

### Encabezados sin jerarquía

Evitar saltar arbitrariamente:

```md
# Título

#### Sección
```

Preferir una estructura coherente:

```md
# Título

## Sección

### Subsección
```

### Código sin indicar lenguaje

Cuando corresponda, indicar:

````md
```bash
git status
```
````

en lugar de:

````md
```
git status
```
````

---

## Markdown y GitHub

GitHub interpreta Markdown en:

```text
README
Issues
Pull Requests
Discussions
comentarios
otros archivos .md
```

Por eso Markdown forma parte de la documentación y de la colaboración.

---

## Comandos y Markdown

Para documentar comandos:

````md
```bash
git status
git add .
git commit -m "Agrega documentación"
```
````

Para explicar un comando dentro del texto:

```md
Ejecutá `git status` antes de crear el commit.
```

---

## Checklist

Antes de publicar documentación:

```text
[ ] Los títulos tienen una jerarquía clara.
[ ] Los enlaces funcionan.
[ ] Los ejemplos de código son correctos.
[ ] Los bloques de código indican el lenguaje cuando corresponde.
[ ] Las imágenes tienen texto alternativo.
[ ] Las rutas internas son correctas.
[ ] El contenido está actualizado.
```

---

## Referencia rápida

| Necesidad      | Sintaxis                |
| -------------- | ----------------------- |
| Título         | `# Título`              |
| Subtítulo      | `## Título`             |
| Negrita        | `**texto**`             |
| Cursiva        | `*texto*`               |
| Tachado        | `~~texto~~`             |
| Lista          | `- elemento`            |
| Lista numerada | `1. elemento`           |
| Enlace         | `[texto](url)`          |
| Imagen         | `![alt](ruta)`          |
| Código inline  | `` `código` ``          |
| Código         | ` ```lenguaje ... ``` ` |
| Cita           | `> texto`               |
| Separador      | `---`                   |
| Checkbox       | `- [ ] tarea`           |

> **Markdown no busca complicar la documentación: busca permitir escribirla de manera simple, legible y estructurada.**
