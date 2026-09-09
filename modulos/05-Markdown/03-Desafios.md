# Desafíos
## Módulo 05 — Markdown

Estos desafíos buscan llevar Markdown desde la sintaxis básica hacia situaciones reales de documentación.

La consigna general es:

> **No se trata de demostrar cuánto Markdown conocés, sino de producir documentación que otra persona pueda entender y utilizar.**

---

## Desafío 1 — Rescatar un README

Recibís este README:

```md
# proyecto

este proyecto sirve para aprender git

git es una herramienta para controlar versiones

para instalar hay que clonar el repositorio

git clone https://github.com/usuario/proyecto.git

despues hay que entrar a la carpeta

cd proyecto

hay varios comandos

git status
git add
git commit
git push

tambien hay recursos
git
github
markdown
```

### Tu desafío

Reorganizalo para que resulte adecuado como README de un proyecto.

Debe incluir como mínimo:

- descripción;
- propósito;
- instalación;
- uso;
- comandos;
- recursos.

No agregues información que no puedas justificar.

---

## Desafío 2 — Documentación para una persona desconocida

Elegí una tarea que sepas realizar.

Por ejemplo:

- crear un repositorio Git;
- publicar un repositorio en GitHub;
- instalar una herramienta;
- ejecutar un proyecto;
- crear un README.

Documentala como si la persona que la va a realizar no pudiera preguntarte nada.

La documentación debe incluir:

```text
Qué necesita
    ↓
Qué debe hacer
    ↓
Qué comandos debe ejecutar
    ↓
Qué debería observar
    ↓
Qué hacer si necesita más información
```

---

## Desafío 3 — La jerarquía correcta

Construí una documentación para un proyecto que tenga:

```text
Proyecto
├── Descripción
├── Objetivos
│   ├── Objetivo general
│   └── Objetivos específicos
├── Instalación
│   ├── Requisitos
│   └── Pasos
├── Uso
└── Recursos
```

Representá esa estructura utilizando exclusivamente títulos Markdown.

Después completá cada sección.

---

## Desafío 4 — Markdown sin formato visual

Escribí primero una documentación utilizando solamente:

- títulos;
- párrafos;
- listas.

No utilices:

- tablas;
- imágenes;
- citas;
- separadores;
- énfasis.

Después revisá el documento y agregá únicamente los elementos adicionales que realmente mejoren su comprensión.

Compará ambas versiones.

---

## Desafío 5 — Tabla o lista

Tenés que documentar los siguientes comandos:

```text
git status — consultar el estado
git add — preparar cambios
git commit — registrar cambios
git push — publicar cambios
git pull — incorporar cambios
```

Creá una primera versión utilizando una lista.

Después creá una segunda utilizando una tabla.

Analizá:

> ¿Cuál permite comparar mejor la información?

> ¿Cuál resulta más cómoda de leer?

> ¿Cuál utilizarías en un README?

No existe necesariamente una única respuesta correcta.

Justificá la decisión.

---

## Desafío 6 — El README demasiado grande

Un README contiene:

```text
Descripción
Instalación
Configuración
Uso
Arquitectura
Decisiones técnicas
Historia del proyecto
Contribución
Preguntas frecuentes
Problemas conocidos
Referencias
Licencia
Changelog
```

### Tu desafío

Decidí:

1. qué información debería permanecer en `README.md`;
2. qué información podría trasladarse a otros documentos;
3. cómo organizarías esos documentos.

Proponé una estructura:

```text
README.md
docs/
    ...
    ...
```

El objetivo es evitar que el README se convierta en un documento inmanejable.

---

## Desafío 7 — Construir navegación

Creá:

```text
README.md
INSTALACION.md
USO.md
RECURSOS.md
```

El README debe permitir llegar a los otros documentos.

Construí una sección:

```md
## Documentación

- [Instalación](INSTALACION.md)
- [Uso](USO.md)
- [Recursos](RECURSOS.md)
```

Después agregá enlaces de retorno hacia el README.

Verificá que la navegación funcione.

---

## Desafío 8 — Documentar un comando

Elegí un comando Git.

Por ejemplo:

```text
git status
```

Documentalo como una pequeña referencia técnica.

Debe contener:

```md
# git status

## Propósito

...

## Sintaxis

...

## Ejemplo

...

## Resultado esperado

...

## Recursos

...
```

Incluí el comando en un bloque de código.

---

## Desafío 9 — Crear una referencia rápida

Construí un documento:

```text
CHEATSHEET.md
```

que contenga una referencia rápida de Git.

Organizalo por categorías:

```text
Estado
Preparación
Commit
Historial
Remoto
```

Utilizá una tabla cuando resulte apropiado.

La referencia debe permitir encontrar rápidamente un comando.

---

## Desafío 10 — Documentar un problema

Imaginá este problema:

> "Hice un commit pero el cambio no aparece en GitHub."

Construí una pequeña guía de diagnóstico.

Debe permitir investigar progresivamente:

```text
¿El archivo cambió?
       ↓
¿Se hizo git add?
       ↓
¿Se hizo commit?
       ↓
¿El commit existe localmente?
       ↓
¿Se hizo push?
       ↓
¿El remoto es correcto?
```

No te limites a listar comandos.

Explicá qué intenta comprobar cada paso.

---

## Desafío 11 — Documentar un error

Construí una sección:

```md
## Problemas frecuentes
```

Incluí al menos tres problemas relacionados con Git o GitHub.

Para cada uno:

```md
### Problema

Descripción.

### Posible causa

...

### Cómo comprobarlo

...

### Posible solución

...
```

La documentación debe ser comprensible para alguien que todavía está aprendiendo.

---

## Desafío 12 — La documentación como recorrido

Construí un README que guíe al lector mediante este recorrido:

```text
¿Qué es?
   ↓
¿Por qué existe?
   ↓
¿Qué necesito?
   ↓
¿Cómo lo instalo?
   ↓
¿Cómo lo utilizo?
   ↓
¿Dónde encuentro más información?
```

Cada pregunta debe corresponder a una sección o enlace.

---

## Desafío 13 — Revisar un README real

Elegí un repositorio público de GitHub.

Analizá su README.

Registrá:

```md
# Análisis de README

## ¿Qué explica primero?

...

## ¿Cómo está organizado?

...

## ¿Qué información resulta útil?

...

## ¿Qué información falta?

...

## ¿Qué decisión de estructura me parece acertada?

...

## ¿Qué cambiaría?

...
```

No copies el contenido del README.

Analizá sus decisiones de documentación.

---

## Desafío 14 — README para un proyecto académico

Elegí uno de tus proyectos de una materia.

Creá un README que permita a otra persona comprender:

- qué problema resuelve;
- qué aprendiste;
- qué herramientas utilizaste;
- cómo ejecutar el proyecto;
- dónde consultar el código.

El documento debe estar pensado para alguien que no estuvo presente durante el desarrollo.

---

## Desafío 15 — README para un proyecto profesional

Imaginá que el mismo proyecto académico será presentado como parte de un portfolio profesional.

Reescribí el README.

Ahora debe poner el foco en:

- propósito;
- características;
- tecnologías;
- funcionamiento;
- documentación;
- estado del proyecto.

Compará las dos versiones.

Respondé:

> ¿Cambió solamente el contenido o también cambió la forma de organizarlo?

---

## Desafío 16 — Documentación con código

Creá una guía que explique un procedimiento mediante:

1. explicación;
2. comando en línea;
3. bloque de código;
4. explicación del resultado.

Por ejemplo:

```md
Para consultar el estado utilizamos `git status`.

```bash
git status
```

El comando muestra...
```

El desafío consiste en lograr que el código forme parte de una explicación y no aparezca aislado.

---

## Desafío 17 — El documento ilegible

Construí deliberadamente una documentación utilizando:

- párrafos muy largos;
- listas donde no corresponden;
- demasiados títulos;
- tablas innecesarias;
- bloques de código sin explicación.

Después revisala.

Eliminá los elementos que dificulten la lectura.

Explicá qué cambiaste.

---

## Desafío 18 — La documentación mínima

Ahora hacé lo contrario.

Construí una documentación excesivamente mínima:

```md
# Proyecto

Es un proyecto.

## Instalación

Instalarlo.

## Uso

Usarlo.
```

Después mejorala progresivamente.

La pregunta que debe guiarte es:

> ¿Qué información necesita realmente otra persona para poder utilizar el proyecto?

---

## Desafío 19 — README como contrato de uso

Construí un README que permita que otra persona utilice el proyecto sin tener que preguntarte:

- qué es;
- qué necesita;
- cómo instalarlo;
- cómo ejecutarlo;
- qué puede hacer;
- dónde consultar información adicional.

Una vez terminado, entregáselo a otra persona.

No le expliques nada.

Observá dónde encuentra dificultades.

Después corregí la documentación.

---

## Desafío 20 — Documentación colaborativa

Trabajá con otra persona.

Cada uno deberá revisar el README del otro.

La revisión debe responder:

```text
¿Entiendo el proyecto?
¿Sé cómo empezar?
¿Encuentro rápidamente la instalación?
¿Encuentro rápidamente el uso?
¿Los comandos son claros?
¿Los enlaces funcionan?
¿Hay información innecesaria?
¿Falta información importante?
```

Registrá las observaciones.

Después incorporá las mejoras que consideres pertinentes.

---

## Desafío 21 — Crear una documentación distribuida

Construí:

```text
README.md
docs/
├── instalacion.md
├── uso.md
├── arquitectura.md
└── recursos.md
```

El README debe actuar como punto de entrada.

Incluí enlaces hacia cada documento.

Cada documento debe incluir un enlace de regreso al README.

---

## Desafío 22 — Documentación y control de versiones

Realizá una modificación importante en `README.md`.

Registrala:

```bash
git add README.md
git commit -m "Mejora documentación del proyecto"
```

Después realizá otra modificación.

Registrala con otro commit.

Consultá:

```bash
git log --oneline
```

Analizá cómo la documentación quedó incorporada al historial.

Respondé:

> ¿Por qué puede resultar útil versionar la documentación?

---

## Desafío 23 — El README evoluciona

Partí de un README inicial.

Creá al menos cuatro versiones mediante commits.

Por ejemplo:

```text
Commit 1 — Crea README
Commit 2 — Agrega instalación
Commit 3 — Agrega uso
Commit 4 — Agrega recursos
```

Después consultá el historial.

Reconstruí la evolución del documento.

---

## Desafío 24 — Publicar documentación

Tomá un documento Markdown completo.

Publicalo en GitHub.

Verificá:

```text
archivo local
      ↓
commit
      ↓
push
      ↓
GitHub
      ↓
visualización
```

Comprobá cada etapa.

---

## Desafío 25 — El enlace roto

Creá deliberadamente un enlace incorrecto:

```md
[Instalación](INSTALACION.md)
```

sin crear el archivo.

Publicá el README en GitHub.

Observá el comportamiento.

Después creá el archivo correcto y verificá nuevamente.

El objetivo es comprender que los enlaces también forman parte de la calidad de una documentación.

---

## Desafío 26 — Documentación visual

Elegí un proceso que pueda beneficiarse de una imagen.

Por ejemplo:

- estructura de un proyecto;
- flujo Git;
- arquitectura;
- organización de carpetas.

Creá o seleccioná una imagen apropiada.

Incorporala mediante Markdown.

Agregá una descripción alternativa significativa.

Después explicá:

> ¿Qué aporta la imagen que el texto no comunica con la misma facilidad?

---

## Desafío 27 — Markdown como lenguaje de estructura

Tomá un documento cualquiera y marcá conceptualmente:

```text
Título
Sección
Subsección
Párrafo
Lista
Código
Enlace
Tabla
Imagen
```

Después transformá cada elemento a Markdown.

El objetivo es reconocer la estructura antes de escribir la sintaxis.

---

## Desafío 28 — Sin consultar documentación

Intentá construir desde cero un documento que contenga:

```text
Título
Subtítulos
Párrafos
Lista
Lista numerada
Enlace
Código
Bloque de código
Tabla
Cita
Imagen
```

No consultes documentación durante los primeros diez minutos.

Después compará tu resultado con la referencia de Markdown.

Registrá qué elementos recordabas y cuáles necesitaste consultar.

---

## Desafío 29 — Consultar documentación correctamente

Elegí un elemento Markdown cuya sintaxis no recuerdes.

No busques un tutorial completo.

Intentá encontrar únicamente la información necesaria para resolver el problema.

Registrá:

```md
## Elemento consultado

...

## Fuente

...

## Sintaxis encontrada

...

## Cómo la utilicé

...
```

El objetivo es desarrollar la capacidad de consultar documentación de manera autónoma.

---

## Desafío 30 — README profesional

Construí una versión final del README de uno de tus proyectos.

Como mínimo deberá contener:

```md
# Nombre

Descripción breve.

## Propósito

...

## Características

...

## Requisitos

...

## Instalación

...

## Uso

...

## Documentación

...

## Recursos

...
```

Incluí enlaces, comandos y ejemplos cuando sean necesarios.

---

## Desafío 31 — Revisión técnica

Antes de publicar tu README, verificá:

```text
[ ] El título identifica claramente el proyecto.
[ ] La descripción permite entenderlo rápidamente.
[ ] La jerarquía de títulos es correcta.
[ ] Los párrafos son claros.
[ ] Las listas se utilizan cuando corresponde.
[ ] Los comandos están diferenciados.
[ ] Los bloques de código indican el lenguaje cuando corresponde.
[ ] Los enlaces funcionan.
[ ] Las imágenes tienen descripción.
[ ] Las tablas aportan información.
[ ] La documentación adicional está enlazada.
```

Corregí todos los problemas encontrados.

---

## Desafío 32 — Revisión editorial

Ahora ignorá la sintaxis Markdown.

Leé el documento como una persona que necesita utilizar el proyecto.

Preguntate:

> ¿Qué necesito saber primero?

> ¿Qué información buscaría después?

> ¿Dónde me detendría?

> ¿Qué parte podría resultar confusa?

> ¿Qué información sobra?

Realizá una segunda revisión exclusivamente desde el punto de vista de la persona lectora.

---

## Desafío 33 — Documentación mínima viable

Construí el README más pequeño que podría considerarse suficiente para presentar un proyecto.

Debe permitir responder:

```text
¿Qué es?
¿Cómo lo obtengo?
¿Cómo lo utilizo?
¿Dónde encuentro más información?
```

Después comparalo con tu README completo.

Analizá qué información adicional justifica conservar.

---

## Desafío 34 — Documentación como producto

Elegí uno de tus proyectos.

Tratálos como si el README fuera parte del producto y no una tarea de la materia.

Preguntate:

- ¿lo leería alguien externo?
- ¿está actualizado?
- ¿los ejemplos funcionan?
- ¿los enlaces funcionan?
- ¿la instalación está clara?
- ¿el proyecto se entiende sin explicación oral?

Realizá las mejoras necesarias.

---

## Desafío final — El proyecto documentado

Tomá uno de tus proyectos y construí una documentación completa utilizando Markdown.

El repositorio debe contener como mínimo:

```text
README.md
docs/
    instalacion.md
    uso.md
    recursos.md
```

El README debe funcionar como punto de entrada.

Debe contener:

- descripción;
- propósito;
- características;
- requisitos;
- instalación;
- uso;
- enlaces hacia documentación adicional.

La documentación deberá incluir cuando resulte apropiado:

- listas;
- enlaces;
- código;
- bloques de código;
- tablas;
- imágenes;
- citas.

Después:

1. revisá la estructura;
2. visualizá los documentos;
3. corregí problemas;
4. registrá los cambios con Git;
5. publicalos en GitHub;
6. verificá la documentación publicada.

Finalmente respondé:

```md
# Reflexión final

## ¿Qué aprendí sobre Markdown?

...

## ¿Qué elemento utilizo con mayor facilidad?

...

## ¿Qué elemento me resulta más difícil?

...

## ¿Cómo cambió mi forma de escribir documentación?

...

## ¿Qué diferencia existe entre escribir información y documentar?

...

## ¿Qué relación encuentro entre Markdown, Git y GitHub?

...
```

---

## Criterio de superación

El desafío se considera logrado cuando podés recibir información sin estructura y transformarla en una documentación:

```text
clara
  +
organizada
  +
legible
  +
navegable
  +
versionable
  =
documentación útil
```

> **Markdown es la herramienta. La capacidad que estamos construyendo es comunicar información técnica de manera clara y reproducible.**