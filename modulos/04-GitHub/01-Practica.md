# Práctica
## Módulo 04 — GitHub

---

## 1. Objetivo

En esta práctica vamos a conectar un repositorio Git local con un repositorio remoto en GitHub.

Hasta ahora trabajamos con:

```text
Repositorio local
      ↓
Cambios
      ↓
Commits
      ↓
Historial
```

Ahora incorporamos:

```text
Repositorio local
      ↓
Repositorio remoto
      ↓
GitHub
```

El objetivo es comprender qué ocurre en cada etapa y diferenciar claramente:

- modificar;
- hacer commit;
- hacer push;
- hacer pull.

---

## 2. Antes de comenzar

Necesitás:

- Git instalado;
- una cuenta en GitHub;
- acceso a GitHub desde un navegador;
- un repositorio local creado durante los módulos anteriores.

Utilizaremos un proyecto de práctica.

---

## 3. Crear un repositorio local

Si ya tenés un repositorio disponible para esta práctica, podés utilizarlo.

En caso contrario, creá una carpeta:

```text
laboratorio-github
```

Ingresá en ella:

```bash
cd laboratorio-github
```

Inicializá Git:

```bash
git init
```

---

## 4. Crear la documentación inicial

Creá:

```text
README.md
```

con:

```md
# Laboratorio GitHub

Repositorio de práctica para trabajar con Git y GitHub.

## Propósito

Aprender a relacionar un repositorio local con un repositorio remoto.
```

Consultá:

```bash
git status
```

---

## 5. Crear el primer commit

Prepará el archivo:

```bash
git add README.md
```

Realizá el commit:

```bash
git commit -m "Crea documentación inicial"
```

Verificá:

```bash
git status
```

El repositorio local debería quedar limpio.

Consultá también:

```bash
git log --oneline
```

Tenés ahora:

```text
Repositorio local
       │
       └── commit
```

Todavía no existe ninguna relación con GitHub.

---

## 6. Crear el repositorio remoto

Ingresá a GitHub y creá un nuevo repositorio.

Utilizá un nombre como:

```text
laboratorio-github
```

Para esta primera práctica, creá el repositorio remoto sin agregar archivos iniciales.

El objetivo es que el repositorio local ya existente sea el que proporcione la historia inicial.

---

## 7. Observar la diferencia

Ahora tenés dos repositorios:

```text
Computadora                  GitHub

┌─────────────────┐          ┌─────────────────┐
│ Repositorio     │          │ Repositorio     │
│ local           │          │ remoto          │
│                 │          │                 │
│ README.md       │          │                 │
│                 │          │                 │
│ Commit          │          │                 │
└─────────────────┘          └─────────────────┘
```

Todavía no están vinculados.

La siguiente tarea será establecer esa relación.

---

## 8. Vincular el repositorio local

Git permite agregar un repositorio remoto mediante:

```bash
git remote add origin URL_DEL_REPOSITORIO
```

Utilizá la URL correspondiente a **tu propio repositorio de GitHub**.

No copies una URL de ejemplo.

Después consultá:

```bash
git remote -v
```

Deberías observar algo similar a:

```text
origin  URL_DEL_REPOSITORIO (fetch)
origin  URL_DEL_REPOSITORIO (push)
```

---

## 9. Comprender `origin`

Acabás de crear una referencia llamada:

```text
origin
```

Es importante comprender qué significa.

`origin`:

- no es GitHub;
- no es un comando;
- no es una palabra reservada;
- es el nombre que estamos utilizando para identificar el repositorio remoto.

Conceptualmente:

```text
Repositorio local
       │
       └── origin ─────→ Repositorio en GitHub
```

---

## 10. Verificar el vínculo

Ejecutá:

```bash
git remote -v
```

Respondé:

1. ¿Qué nombre tiene el remoto?
2. ¿Qué URL tiene asociada?
3. ¿Qué diferencia existe entre las referencias `fetch` y `push`?

No es necesario profundizar todavía en las diferencias operativas entre ambas.

Lo importante es reconocer que el repositorio local conoce dónde está ubicado el remoto.

---

## 11. Publicar el historial

Ahora vamos a enviar al repositorio remoto el commit que ya existe localmente.

Utilizá:

```bash
git push -u origin main
```

Si tu rama inicial tiene otro nombre, utilizá el nombre correspondiente.

La primera publicación establece la relación necesaria para facilitar los próximos `push`.

---

## 12. Observar GitHub

Volvé al repositorio en GitHub y actualizá la página.

Ahora debería aparecer:

```text
README.md
```

También debería estar disponible el historial correspondiente al commit realizado localmente.

La idea importante es:

> **El commit existía antes de hacer `push`.**

El `push` permitió publicarlo en el repositorio remoto.

---

## 13. Commit no es push

Detengámonos acá.

El recorrido fue:

```text
Modificar README.md
       ↓
git add
       ↓
git commit
       ↓
Commit local
       ↓
git push
       ↓
Commit publicado en GitHub
```

Por lo tanto:

```text
git commit ≠ git push
```

El primero registra.

El segundo publica.

---

## 14. Realizar una modificación local

Ahora modificá `README.md`.

Agregá:

```md
## Estado

Repositorio utilizado para practicar la comunicación
entre Git y GitHub.
```

Guardá el archivo.

Consultá:

```bash
git status
```

Todavía no hiciste commit.

Por lo tanto:

```text
Archivo modificado
       ↓
Repositorio local
       ↓
NO está registrado en el historial
       ↓
NO está publicado en GitHub
```

---

## 15. Registrar el cambio

Prepará:

```bash
git add README.md
```

Realizá:

```bash
git commit -m "Agrega estado del laboratorio"
```

Consultá:

```bash
git log --oneline
```

Ahora el nuevo cambio forma parte del historial local.

Pero todavía no fue publicado.

---

## 16. Una pregunta importante

Antes de ejecutar ningún comando más, respondé:

> ¿El nuevo cambio ya está en GitHub?

La respuesta debería ser:

> **No necesariamente.**

Existe un nuevo commit local, pero todavía no hicimos:

```bash
git push
```

---

## 17. Publicar el segundo commit

Ejecutá:

```bash
git push
```

Observá la salida.

Después volvé a GitHub.

El nuevo commit debería aparecer en el historial remoto.

---

## 18. Construir el modelo

Hasta ahora:

```text
LOCAL                         GITHUB

README.md
   │
   ├── Commit 1 ──────────────► Commit 1
   │
   └── Commit 2 ──────────────► Commit 2
```

Los dos repositorios comparten esos commits.

---

## 19. Realizar otro cambio

Modificá nuevamente `README.md`.

Agregá:

```md
## Aprendizajes

- Diferencia entre Git y GitHub.
- Repositorio local y remoto.
- Publicación de commits.
```

Consultá:

```bash
git status
```

---

## 20. Registrar sin publicar

Realizá:

```bash
git add README.md
```

y:

```bash
git commit -m "Agrega aprendizajes del laboratorio"
```

Ahora consultá:

```bash
git status
```

y:

```bash
git log --oneline
```

El repositorio local contiene un commit que todavía no está en GitHub.

---

## 21. Observar la diferencia

Podemos representarlo así:

```text
LOCAL                         GITHUB

Commit 1 ───────────────────► Commit 1
Commit 2 ───────────────────► Commit 2
Commit 3
```

El tercer commit existe localmente.

Todavía no existe en el remoto.

---

## 22. Publicar nuevamente

Ejecutá:

```bash
git push
```

Volvé a GitHub.

Ahora deberías encontrar:

```text
Commit 1
Commit 2
Commit 3
```

El repositorio remoto volvió a estar actualizado respecto del local.

---

## 23. Crear un cambio desde GitHub

Ahora vamos a experimentar el flujo contrario.

Desde GitHub, modificá `README.md` utilizando la interfaz web.

Agregá:

```md
## Repositorio remoto

Este contenido fue incorporado desde GitHub.
```

Realizá el commit desde GitHub.

Ahora existe un cambio en el remoto que todavía no está en tu repositorio local.

---

## 24. La situación actual

Conceptualmente:

```text
LOCAL                         GITHUB

Commit 1 ───────────────────► Commit 1
Commit 2 ───────────────────► Commit 2
Commit 3 ───────────────────► Commit 3
                              │
                              └── Commit 4
```

El cuarto commit existe en GitHub.

Todavía no está incorporado a tu repositorio local.

---

## 25. Obtener el cambio

Para incorporar el cambio remoto utilizaremos:

```bash
git pull
```

Ejecutalo.

Después observá:

```bash
git log --oneline
```

El nuevo commit debería formar parte de tu historia local.

---

## 26. Observar el archivo

Abrí:

```text
README.md
```

Comprobá que también esté disponible el contenido incorporado desde GitHub.

Ahora ambos repositorios contienen la evolución correspondiente.

---

## 27. El flujo completo

La práctica permitió recorrer ambos sentidos:

### Local → GitHub

```text
Modificar
   ↓
git add
   ↓
git commit
   ↓
git push
   ↓
GitHub
```

### GitHub → Local

```text
Cambio remoto
   ↓
git pull
   ↓
Repositorio local
```

---

## 28. Diagnóstico

Ahora respondé:

### Situación A

> "Modifiqué un archivo, pero GitHub no muestra el cambio."

¿Qué deberías comprobar?

---

### Situación B

> "Hice commit, pero GitHub todavía no muestra el cambio."

¿Qué falta?

---

### Situación C

> "Otra persona modificó el repositorio en GitHub y yo no veo el cambio localmente."

¿Qué operación podría ser necesaria?

---

### Situación D

> "Git me muestra que el repositorio local y el remoto están diferentes."

¿Qué deberías hacer antes de ejecutar comandos al azar?

---

## 29. Repetir el ciclo

Realizá nuevamente:

1. una modificación local;
2. `git status`;
3. `git add`;
4. `git commit`;
5. `git log --oneline`;
6. `git push`;
7. comprobación en GitHub.

Después realizá una modificación desde GitHub y:

1. observá el repositorio remoto;
2. ejecutá `git pull`;
3. verificá el archivo;
4. consultá el historial.

---

## 30. Observar la relación

Ejecutá:

```bash
git remote -v
```

y:

```bash
git log --oneline
```

Respondé:

1. ¿Cuál es el repositorio remoto?
2. ¿Qué nombre tiene?
3. ¿Cuántos commits tenés localmente?
4. ¿Cuántos commits observás en GitHub?
5. ¿Están sincronizados?
6. ¿Cómo podés determinarlo?

---

## 31. Reflexión

Respondé con tus propias palabras:

### ¿Qué es Git?

...

### ¿Qué es GitHub?

...

### ¿Qué diferencia existe entre un repositorio local y uno remoto?

...

### ¿Qué hace `git commit`?

...

### ¿Qué hace `git push`?

...

### ¿Qué hace `git pull`?

...

### ¿Qué significa `origin`?

...

---

## 32. Comprobación final

Sin consultar la práctica, realizá el siguiente recorrido en tu repositorio:

```text
Modificar
   ↓
Consultar estado
   ↓
Preparar
   ↓
Commit
   ↓
Consultar historial
   ↓
Push
   ↓
Verificar en GitHub
```

Después realizá:

```text
Modificar desde GitHub
   ↓
Pull
   ↓
Verificar localmente
   ↓
Consultar historial
```

Si podés realizar ambos recorridos y explicar qué ocurre en cada etapa, el objetivo principal de la práctica está cumplido.

---

## 33. Idea de cierre

Hasta ahora Git nos permitía conservar la historia de un proyecto.

Ahora aprendimos a compartir esa historia.

El concepto central de esta práctica es:

> **Un cambio no está publicado solamente porque exista en nuestro repositorio local. Para compartirlo con el repositorio remoto debemos enviarlo.**

Y en sentido contrario:

> **Un cambio que existe en el repositorio remoto no aparece automáticamente en nuestro repositorio local. Debemos obtenerlo.**