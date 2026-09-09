# Proyecto
## Módulo 04 — GitHub

---

## 1. Propósito

En este proyecto vas a tomar un repositorio Git local y convertirlo en un proyecto publicado en GitHub.

La actividad integra los conceptos trabajados durante el módulo:

- Git y GitHub;
- repositorio local;
- repositorio remoto;
- remotos;
- `origin`;
- commits;
- `git push`;
- `git pull`;
- publicación de cambios;
- obtención de cambios;
- diferencia entre registrar y publicar.

El objetivo no es solamente "subir un proyecto a GitHub".

El objetivo es comprender el recorrido completo:

```text
Proyecto local
      ↓
Repositorio Git
      ↓
Repositorio remoto
      ↓
GitHub
```

y también el recorrido inverso:

```text
GitHub
   ↓
Repositorio remoto
   ↓
Repositorio local
```

---

## 2. El proyecto

Creá un repositorio llamado:

```text
proyecto-github
```

El tema es libre.

Podés utilizar:

- un proyecto académico;
- una aplicación ficticia;
- una herramienta;
- un juego;
- una biblioteca;
- un proyecto documental;
- una idea personal.

No es necesario desarrollar software funcional.

El foco del proyecto está puesto en el uso de Git y GitHub.

---

## 3. Estructura inicial

El repositorio deberá comenzar con:

```text
proyecto-github/
├── README.md
├── objetivos.md
└── notas.md
```

Adaptá el contenido al proyecto elegido.

---

## 4. Crear el repositorio local

Creá la carpeta del proyecto e ingresá en ella:

```bash
cd proyecto-github
```

Inicializá Git:

```bash
git init
```

Verificá:

```bash
git status
```

---

## 5. Crear la documentación inicial

### `README.md`

Incluí:

```md
# Nombre del proyecto

Descripción breve del proyecto.

## Propósito

Explicación del propósito general.

## Estado

Proyecto en desarrollo.
```

### `objetivos.md`

Incluí al menos tres objetivos.

```md
# Objetivos

- Objetivo 1
- Objetivo 2
- Objetivo 3
```

### `notas.md`

Incluí algunas notas iniciales:

```md
# Notas

Notas iniciales del proyecto.
```

---

## 6. Primer commit

Consultá:

```bash
git status
```

Prepará los archivos:

```bash
git add .
```

Realizá el primer commit:

```bash
git commit -m "Crea estructura inicial del proyecto"
```

Después:

```bash
git status
```

y:

```bash
git log --oneline
```

El repositorio local debe quedar limpio.

---

## 7. Crear el repositorio en GitHub

Ingresá a GitHub y creá un repositorio nuevo.

Utilizá el mismo nombre:

```text
proyecto-github
```

Para esta etapa, no agregues archivos iniciales desde GitHub.

El repositorio remoto debe quedar disponible para recibir la historia del repositorio local.

---

## 8. Vincular local y remoto

Desde el repositorio local agregá el remoto:

```bash
git remote add origin URL_DEL_REPOSITORIO
```

Utilizá la URL correspondiente a tu repositorio.

Después verificá:

```bash
git remote -v
```

Deberías identificar:

```text
origin
```

y la URL del repositorio remoto.

---

## 9. Analizar el vínculo

Antes de continuar, explicá:

```md
## Repositorio remoto

Nombre del remoto:

...

URL:

...

¿Qué representa `origin`?

...

¿Dónde está almacenado el repositorio local?

...

¿Dónde está almacenado el repositorio remoto?

...
```

---

## 10. Primer `push`

Publicá la historia inicial:

```bash
git push -u origin main
```

Si tu rama inicial tiene otro nombre, utilizá el nombre correspondiente.

Después ingresá al repositorio en GitHub.

Verificá:

- archivos;
- README;
- commit;
- historial.

---

## 11. Documentar el primer intercambio

Agregá a `notas.md`:

```md
## Primera publicación

El repositorio local fue vinculado con GitHub.

Remoto:

...

Primer commit publicado:

...

¿Qué diferencia existe entre crear el commit y publicarlo?

...
```

Realizá un nuevo commit:

```bash
git add notas.md
git commit -m "Documenta primera publicación"
```

Publicalo:

```bash
git push
```

---

## 12. Incorporar una evolución local

Modificá `README.md`.

Agregá:

```md
## Características

- Característica 1
- Característica 2
- Característica 3
```

Consultá:

```bash
git status
```

Registrá el cambio:

```bash
git add README.md
git commit -m "Agrega características del proyecto"
```

Consultá:

```bash
git log --oneline
```

Todavía no publiques el cambio.

---

## 13. Analizar antes de publicar

Antes de ejecutar `git push`, respondé:

> ¿El nuevo commit existe localmente?

> ¿Existe en GitHub?

> ¿Qué operación falta para publicarlo?

Después ejecutá:

```bash
git push
```

Comprobá el resultado en GitHub.

---

## 14. Segunda evolución

Modificá `objetivos.md`.

Agregá o ampliá objetivos.

Por ejemplo:

```md
- Facilitar el aprendizaje de Git.
- Comprender el uso de repositorios remotos.
- Practicar la publicación de cambios.
```

Registrá:

```bash
git add objetivos.md
git commit -m "Amplía objetivos del proyecto"
```

Publicá:

```bash
git push
```

---

## 15. Crear un cambio remoto

Ahora vamos a modificar el proyecto directamente desde GitHub.

Editá `README.md` desde la interfaz web.

Agregá:

```md
## Repositorio remoto

Este contenido fue agregado directamente desde GitHub.
```

Realizá el commit desde GitHub.

Ahora existe una modificación que todavía no fue incorporada al repositorio local.

---

## 16. Analizar la situación

Antes de ejecutar `git pull`, respondé:

```md
## Cambio remoto

¿Qué cambió en GitHub?

...

¿Está ese cambio en mi repositorio local?

...

¿Cómo podría comprobarlo?

...

¿Qué operación debería analizar?

...
```

---

## 17. Obtener el cambio

Desde el repositorio local ejecutá:

```bash
git pull
```

Después:

```bash
git log --oneline
```

y abrí:

```text
README.md
```

Verificá que el contenido remoto esté disponible localmente.

---

## 18. Documentar el `pull`

Agregá a `notas.md`:

```md
## Cambio remoto

Se realizó una modificación directamente en GitHub.

¿Qué operación permitió incorporarla localmente?

...

¿Qué cambió en el historial local?

...

¿Qué diferencia existe entre `git push` y `git pull`?

...
```

Registrá el cambio:

```bash
git add notas.md
git commit -m "Documenta incorporación de cambio remoto"
```

Publicalo:

```bash
git push
```

---

## 19. Construir una evolución completa

Realizá ahora al menos tres nuevas modificaciones locales.

Cada modificación deberá:

1. representar una intención concreta;
2. registrarse mediante un commit;
3. utilizar un mensaje descriptivo;
4. publicarse mediante `git push`.

Ejemplo:

```text
Modificación
    ↓
git status
    ↓
git add
    ↓
git commit
    ↓
git log --oneline
    ↓
git push
    ↓
verificación en GitHub
```

---

## 20. Crear una segunda modificación remota

Realizá una nueva modificación desde GitHub.

Esta vez modificá `notas.md`.

Agregá:

```md
## Aprendizaje

El repositorio remoto permite compartir la historia del proyecto
y mantener un punto de intercambio con otros colaboradores.
```

Realizá el commit desde GitHub.

Después, desde tu computadora:

```bash
git pull
```

Verificá el resultado.

---

## 21. Analizar el historial

Ejecutá:

```bash
git log --oneline
```

Identificá:

- commit inicial;
- primer commit publicado;
- modificaciones locales;
- modificaciones realizadas desde GitHub;
- último commit.

Después ejecutá:

```bash
git log
```

Seleccioná tres commits y registrá:

```text
Identificador:
Mensaje:
Autor:
Fecha:
Origen del cambio:
```

En `Origen del cambio` indicá:

```text
Local
```

o:

```text
GitHub
```

según corresponda.

---

## 22. Construir una línea de tiempo

Agregá a `notas.md`:

```md
## Evolución del proyecto

```text
Inicio
  ↓
Estructura inicial
  ↓
Primera publicación
  ↓
Características
  ↓
Objetivos
  ↓
Cambio remoto
  ↓
Nueva evolución
  ↓
Estado actual
```
```

Adaptá la línea de tiempo a los cambios reales que realizaste.

---

## 23. Analizar local y remoto

Respondé:

```md
## Estado de los repositorios

### Repositorio local

...

### Repositorio remoto

...

### ¿Están sincronizados?

...

### ¿Cómo lo comprobé?

...
```

La respuesta debe basarse en observaciones concretas.

---

## 24. Diagnóstico

Construí deliberadamente esta situación:

```text
LOCAL

Tiene al menos un commit que todavía no fue publicado.
```

Identificá la situación.

Después resolvela mediante la operación correspondiente.

Luego construí:

```text
GITHUB

Tiene al menos un commit que todavía no está localmente.
```

Identificá la situación.

Resolvela mediante la operación correspondiente.

Documentá ambos casos.

---

## 25. Crear `historia.md`

Agregá un archivo:

```text
historia.md
```

Con la siguiente estructura:

```md
# Historia del proyecto

## Inicio

...

## Primera publicación

...

## Evolución local

...

## Cambios remotos

...

## Estado actual

...
```

La explicación debe reconstruirse a partir del historial.

---

## 26. Analizar la publicación

En `historia.md`, agregá:

```md
## Publicación

¿Qué significa publicar un commit?

...

¿Por qué `git commit` y `git push` son operaciones diferentes?

...

¿Qué información queda disponible en GitHub?

...
```

Respondé con tus propias palabras.

---

## 27. Analizar la obtención

Agregá:

```md
## Incorporación de cambios

¿Qué significa obtener un cambio desde el repositorio remoto?

...

¿Qué función cumple `git pull`?

...

¿Qué diferencia existe entre un cambio local y uno remoto?

...
```

---

## 28. Evaluar el repositorio publicado

Ingresá a tu repositorio desde GitHub.

Observá el proyecto como si fueras una persona externa.

Evaluá:

| Aspecto | Evaluación |
|---|---|
| README | |
| Organización | |
| Historial | |
| Mensajes | |
| Descripción | |
| Comprensión general | |

Después escribí tres mejoras posibles.

---

## 29. Verificación técnica

Ejecutá:

```bash
git status
```

El repositorio debe quedar limpio.

Después:

```bash
git remote -v
```

Verificá que `origin` apunte al repositorio correcto.

Después:

```bash
git log --oneline
```

Verificá que la historia sea coherente.

Finalmente ingresá a GitHub y comprobá que el repositorio refleje el estado esperado.

---

## 30. Producto final

La estructura mínima será:

```text
proyecto-github/
├── .git/
├── README.md
├── objetivos.md
├── notas.md
└── historia.md
```

El repositorio remoto deberá estar publicado en GitHub.

Deberá contener:

- documentación;
- varios commits;
- historial comprensible;
- al menos una evolución local;
- al menos una modificación realizada desde GitHub;
- utilización de `git push`;
- utilización de `git pull`;
- un remoto configurado;
- documentación del proceso.

---

## 31. Criterios de finalización

El proyecto está terminado cuando podés demostrar que:

- comprendés la diferencia entre Git y GitHub;
- comprendés la diferencia entre local y remoto;
- podés crear un repositorio remoto;
- podés vincularlo con un repositorio local;
- podés identificar `origin`;
- podés publicar commits;
- podés obtener cambios;
- podés distinguir commit de push;
- podés distinguir push de pull;
- podés verificar el estado de ambos repositorios;
- podés explicar qué ocurrió durante el intercambio.

---

## 32. Reflexión final

Respondé en `historia.md`:

### ¿Qué aprendí?

...

### ¿Qué diferencia existe entre registrar y publicar?

...

### ¿Qué diferencia existe entre publicar y obtener?

...

### ¿Cómo sé dónde está un cambio?

...

### ¿Qué representa GitHub dentro del flujo de trabajo?

...

### ¿Qué parte del proceso todavía me resulta difícil?

...

---

## 33. Pregunta final

Sin consultar documentación, explicá este recorrido:

```text
Modificar
   ↓
git add
   ↓
git commit
   ↓
Historial local
   ↓
git push
   ↓
Repositorio remoto
   ↓
GitHub
```

Y este:

```text
GitHub
   ↓
Repositorio remoto
   ↓
git pull
   ↓
Repositorio local
```

Finalmente respondé:

> **Si mañana recibieras un repositorio Git conectado con GitHub y te pidieran realizar un cambio y asegurarte de que quede publicado, ¿qué harías y cómo verificarías que efectivamente quedó publicado?**

Si podés resolver esa situación sin seguir una receta paso a paso, el objetivo principal del módulo está cumplido.