# Proyecto
## Módulo 05 — Markdown

---

## 1. Propósito

En este proyecto vas a aplicar Markdown para construir la documentación de un proyecto real.

El objetivo no es demostrar que conocés una determinada cantidad de elementos de Markdown.

El objetivo es producir documentación que otra persona pueda leer, comprender y utilizar sin necesidad de recibir una explicación oral.

El recorrido será:

```text
Proyecto
   ↓
Información
   ↓
Organización
   ↓
Documentación
   ↓
Markdown
   ↓
Git
   ↓
GitHub
```

---

## 2. Consigna general

Elegí uno de los proyectos desarrollados durante el curso.

También podés utilizar un proyecto propio, siempre que tenga suficiente contenido para ser documentado.

Construí una documentación completa utilizando Markdown.

El resultado deberá estar publicado dentro del repositorio GitHub del proyecto.

---

## 3. Producto final

El repositorio deberá incorporar, como mínimo:

```text
README.md
docs/
├── instalacion.md
├── uso.md
└── recursos.md
```

La estructura puede ampliarse si el proyecto lo necesita.

Por ejemplo:

```text
docs/
├── instalacion.md
├── uso.md
├── configuracion.md
├── arquitectura.md
├── problemas-frecuentes.md
└── recursos.md
```

No agregues documentos solamente para aumentar la cantidad.

Cada documento debe tener una función concreta.

---

## 4. README

El archivo `README.md` será el punto de entrada al proyecto.

Debe permitir comprender rápidamente:

- qué es el proyecto;
- cuál es su propósito;
- qué características tiene;
- qué requisitos existen;
- cómo comenzar;
- dónde encontrar documentación adicional.

Utilizá como estructura mínima:

```md
# Nombre del proyecto

Descripción breve del proyecto.

## Propósito

Explicación del propósito.

## Características

- Característica 1
- Característica 2
- Característica 3

## Requisitos

- Requisito 1
- Requisito 2

## Instalación

Resumen del procedimiento.

## Uso

Resumen de utilización.

## Documentación

- [Instalación](docs/instalacion.md)
- [Uso](docs/uso.md)
- [Recursos](docs/recursos.md)
```

Adaptá la estructura al proyecto.

---

## 5. Documento de instalación

Creá:

```text
docs/instalacion.md
```

Debe explicar cómo preparar el proyecto.

Podés utilizar:

```md
# Instalación

## Requisitos

...

## Obtener el proyecto

...

## Configuración

...

## Verificación

...
```

Si existen comandos, incorporalos mediante bloques de código.

Por ejemplo:

````md
```bash
git clone URL_DEL_REPOSITORIO
cd proyecto
```
````

La persona lectora debería poder seguir el procedimiento sin necesidad de preguntarte qué hacer.

---

## 6. Documento de uso

Creá:

```text
docs/uso.md
```

Explicá cómo utilizar el proyecto.

Podés utilizar:

```md
# Uso

## Inicio

...

## Procedimiento

1. ...
2. ...
3. ...

## Ejemplo

...

## Resultado esperado

...
```

Utilizá ejemplos concretos cuando ayuden a comprender el funcionamiento.

---

## 7. Documento de recursos

Creá:

```text
docs/recursos.md
```

Incluí los recursos relacionados con el proyecto.

Por ejemplo:

```md
# Recursos

## Documentación

- [Recurso 1](URL)
- [Recurso 2](URL)

## Referencias

...

## Material complementario

...
```

No agregues enlaces solamente para llenar la sección.

Cada recurso debe tener relación con el proyecto.

---

## 8. Utilizar Markdown de manera significativa

La documentación deberá utilizar, cuando corresponda:

* títulos;
* subtítulos;
* párrafos;
* énfasis;
* listas;
* listas numeradas;
* enlaces;
* código en línea;
* bloques de código;
* tablas;
* citas;
* imágenes.

No es obligatorio utilizar todos los elementos.

La decisión debe depender de la información que necesitás comunicar.

---

## 9. Código

Cuando debas mencionar un comando dentro de una oración, utilizá código en línea.

Ejemplo:

```md
Para consultar el estado utilizá `git status`.
```

Cuando debas presentar un conjunto de comandos, utilizá un bloque:

````md
```bash
git status
git add .
git commit -m "Actualiza documentación"
```
````

El código debe estar acompañado por una explicación cuando sea necesario.

---

## 10. Tablas

Utilizá tablas cuando permitan comparar información.

Por ejemplo:

```md
| Comando | Propósito |
|---|---|
| `git status` | Consultar el estado |
| `git add` | Preparar cambios |
| `git commit` | Registrar cambios |
```

No utilices una tabla si una lista o un párrafo resulta más claro.

---

## 11. Imágenes

Si una imagen aporta información relevante, incorporala al documento.

Por ejemplo:

```md
![Descripción de la imagen](../recursos/imagen.png)
```

La descripción debe permitir comprender qué representa la imagen.

No agregues imágenes únicamente como decoración.

---

## 12. Navegación

El README debe permitir acceder fácilmente a la documentación.

Como mínimo:

```md
## Documentación

- [Instalación](docs/instalacion.md)
- [Uso](docs/uso.md)
- [Recursos](docs/recursos.md)
```

Cada documento puede incluir un enlace para regresar al README:

```md
[← Volver al README](../README.md)
```

La documentación debe poder recorrerse de manera sencilla.

---

## 13. Primera versión

Construí una primera versión funcional de la documentación.

No intentes conseguir el documento perfecto desde el principio.

El primer objetivo es disponer de:

```text
README.md
docs/instalacion.md
docs/uso.md
docs/recursos.md
```

con contenido suficiente para ser revisado.

---

## 14. Revisar la estructura

Ahora revisá los documentos.

Para cada uno preguntate:

> ¿Tiene un propósito claro?

> ¿La información está organizada?

> ¿La jerarquía de títulos es correcta?

> ¿Hay información repetida?

> ¿Falta información?

> ¿Hay secciones que podrían eliminarse?

Realizá los cambios necesarios.

---

## 15. Revisar desde el punto de vista del lector

Ahora olvidá que vos escribiste el documento.

Imaginá que sos una persona que acaba de encontrar el repositorio.

Intentá responder:

```text
¿Qué es este proyecto?
¿Para qué sirve?
¿Qué necesito?
¿Cómo lo instalo?
¿Cómo lo utilizo?
¿Dónde encuentro información adicional?
```

Si alguna respuesta no resulta evidente, mejorá la documentación.

---

## 16. Revisión de enlaces

Comprobá todos los enlaces.

Verificá:

* enlaces internos;
* enlaces externos;
* enlaces hacia documentación;
* enlaces hacia imágenes.

Un enlace roto también es un problema de documentación.

---

## 17. Revisión de código

Comprobá que:

* los comandos estén correctamente escritos;
* los bloques indiquen el lenguaje cuando corresponda;
* los ejemplos sean coherentes;
* no haya comandos innecesarios;
* las explicaciones correspondan al código mostrado.

La documentación no debe enseñar un procedimiento incorrecto.

---

## 18. Visualización local

Visualizá todos los documentos mediante la vista previa de Markdown.

Recorré:

```text
README.md
     ↓
instalacion.md
     ↓
uso.md
     ↓
recursos.md
```

Observá:

* títulos;
* listas;
* enlaces;
* tablas;
* bloques de código;
* imágenes;
* separación de contenido.

Corregí cualquier problema de visualización.

---

## 19. Primera versión en Git

Consultá:

```bash
git status
```

Agregá los documentos:

```bash
git add README.md docs/
```

Registrá la primera versión:

```bash
git commit -m "Agrega documentación del proyecto"
```

Consultá:

```bash
git log --oneline
```

Observá que la documentación ahora forma parte de la historia del proyecto.

---

## 20. Publicar

Publicá los cambios:

```bash
git push
```

Ingresá al repositorio en GitHub.

Comprobá:

```text
README
   ↓
Documentación
   ↓
Enlaces
   ↓
Archivos Markdown
```

Verificá que todo funcione desde el entorno remoto.

---

## 21. Segunda iteración

Ahora realizá una revisión más profunda.

Buscá:

* información redundante;
* explicaciones demasiado largas;
* instrucciones incompletas;
* títulos poco claros;
* enlaces innecesarios;
* ejemplos insuficientes;
* problemas de navegación.

Mejorá la documentación.

---

## 22. Registrar la evolución

Después de realizar las mejoras:

```bash
git status
```

Revisá los cambios.

Después:

```bash
git diff
```

Observá qué modificaste.

Registrá la segunda versión:

```bash
git add .
git commit -m "Mejora documentación del proyecto"
```

Publicá:

```bash
git push
```

---

## 23. Comparar versiones

Consultá:

```bash
git log --oneline
```

Identificá los commits relacionados con la documentación.

Respondé:

```md
## Evolución

### Primera versión

¿Qué documentación incorporé?

...

### Segunda versión

¿Qué mejoré?

...

### ¿Por qué?

...
```

El objetivo es comprender que la documentación también evoluciona.

---

## 24. Evaluación por otra persona

Si es posible, entregá el repositorio a otra persona.

No expliques oralmente cómo funciona.

Pedile que intente:

1. comprender qué es el proyecto;
2. encontrar los requisitos;
3. instalarlo;
4. utilizarlo;
5. encontrar información adicional.

Observá dónde tiene dificultades.

Registrá:

```md
## Prueba con otra persona

### Dificultad 1

...

### Dificultad 2

...

### Dificultad 3

...

### Mejoras realizadas

...
```

Esta etapa es especialmente importante.

La documentación debe evaluarse por su capacidad de ayudar a otra persona, no solamente por lo clara que resulta para quien la escribió.

---

## 25. Revisión final

Utilizá esta lista de comprobación:

```text
[ ] El proyecto está claramente identificado.
[ ] El propósito está explicado.
[ ] Las características principales están documentadas.
[ ] Los requisitos están indicados.
[ ] La instalación está explicada.
[ ] El uso está explicado.
[ ] Existe documentación adicional cuando es necesaria.
[ ] Los enlaces funcionan.
[ ] Los títulos tienen una jerarquía correcta.
[ ] Las listas se utilizan adecuadamente.
[ ] Los comandos están diferenciados del texto.
[ ] Los bloques de código indican el lenguaje cuando corresponde.
[ ] Las tablas aportan claridad.
[ ] Las imágenes tienen descripción.
[ ] Los documentos pueden recorrerse fácilmente.
[ ] La documentación fue visualizada localmente.
[ ] La documentación fue publicada en GitHub.
[ ] El repositorio está limpio.
```

---

## 26. Estructura final sugerida

Una posible estructura final:

```text
proyecto/
├── README.md
├── docs/
│   ├── instalacion.md
│   ├── uso.md
│   └── recursos.md
└── ...
```

El resto de los archivos dependerá del proyecto elegido.

---

## 27. Reflexión final

Creá un archivo:

```text
docs/reflexion.md
```

y respondé:

```md
# Reflexión

## ¿Qué aprendí sobre Markdown?

...

## ¿Qué aprendí sobre documentación?

...

## ¿Qué elemento de Markdown utilizo con mayor facilidad?

...

## ¿Qué elemento necesito seguir practicando?

...

## ¿Qué diferencia existe entre escribir y documentar?

...

## ¿Qué relación existe entre Markdown y Git?

...

## ¿Qué relación existe entre Markdown y GitHub?

...

## ¿Qué mejoré respecto de la primera versión?

...

## ¿Qué haría diferente en un próximo proyecto?

...
```

---

## 28. Producto final

El proyecto final del módulo deberá dejar evidencia de que Markdown puede utilizarse como parte real del flujo de trabajo.

El recorrido completo será:

```text
Información
    ↓
Organización
    ↓
Markdown
    ↓
Visualización
    ↓
Revisión
    ↓
Git
    ↓
Commit
    ↓
GitHub
    ↓
Documentación publicada
```

La documentación deberá ser:

```text
clara
organizada
legible
útil
navegable
versionable
```

---

## 29. Criterios de evaluación

El proyecto será considerado logrado cuando:

### Estructura

La documentación presenta una organización clara y coherente.

### Sintaxis

Los elementos Markdown utilizados están correctamente implementados.

### Comunicación

La información puede ser comprendida por una persona que no participó del desarrollo.

### Navegación

Los documentos y enlaces permiten recorrer la información fácilmente.

### Integración

La documentación forma parte del repositorio Git y está publicada en GitHub.

### Revisión

Se evidencia al menos una instancia de mejora posterior a la primera versión.

---

## 30. Pregunta final

Al finalizar, deberías poder responder:

> **Si mañana te entregaran un proyecto y te pidieran documentarlo para que otra persona pueda utilizarlo sin tu ayuda, ¿sabrías cómo organizar la información y convertirla en una documentación clara utilizando Markdown?**

Si la respuesta es sí, el objetivo principal de este módulo está cumplido.

---

> **Un proyecto que funciona pero nadie puede entender ni utilizar fácilmente está incompleto. La documentación también es parte del proyecto.**

