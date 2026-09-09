# Recursos
## Módulo 09 — Proyecto Final

Este documento reúne recursos para continuar profundizando los contenidos utilizados durante el Proyecto Final.

La idea no es memorizar documentación.

La documentación debe convertirse en una herramienta habitual de trabajo:

```text
necesidad
   ↓
buscar
   ↓
leer
   ↓
probar
   ↓
verificar
```

---

# 1. Git

## Documentación oficial

https://git-scm.com/docs

Es la referencia principal para consultar comandos y comportamiento de Git.

Puede utilizarse para profundizar en:

```text
repositorios
commits
ramas
historial
merge
remotos
```

---

# 2. Pro Git

https://git-scm.com/book/es/v2

El libro Pro Git permite profundizar en los conceptos y mecanismos internos de Git.

Es especialmente útil para comprender:

```text
ramificaciones
merge
repositorios remotos
historial
flujos de trabajo
```

No es necesario leerlo completo.

Puede utilizarse como material de consulta cuando aparezca una necesidad concreta.

---

# 3. Git Reference

https://git-scm.com/docs

La referencia de Git permite consultar comandos específicos.

Por ejemplo:

```text
git init
git status
git add
git commit
git log
git diff
git branch
git switch
git merge
git remote
git push
git pull
```

La recomendación es consultar la referencia cuando exista una duda sobre el comportamiento de un comando.

---

# 4. GitHub Docs

https://docs.github.com/es

Es la documentación oficial de GitHub.

Permite consultar:

```text
repositorios
Issues
Pull Requests
ramas
revisiones
colaboración
perfiles
seguridad
```

---

# 5. GitHub Skills

https://skills.github.com/

GitHub Skills ofrece ejercicios prácticos para continuar aprendiendo GitHub.

Puede utilizarse después del curso para practicar:

```text
Issues
Pull Requests
ramas
colaboración
automatización
```

Es especialmente útil para continuar aprendiendo mediante práctica.

---

# 6. GitHub — Pull Requests

https://docs.github.com/es/pull-requests

La documentación permite profundizar en:

```text
crear Pull Requests
revisar cambios
comentar
solicitar modificaciones
integrar cambios
```

Es un recurso especialmente relevante para continuar practicando el flujo colaborativo.

---

# 7. GitHub — Revisiones

https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests

Permite profundizar en el proceso de revisión de cambios.

Recordá la idea central trabajada durante el curso:

```text
Pull Request
      ↓
revisión
      ↓
feedback
      ↓
mejora
```

---

# 8. GitHub — Issues

https://docs.github.com/es/issues

Las Issues permiten organizar y realizar seguimiento del trabajo.

Pueden utilizarse para registrar:

```text
problemas
tareas
mejoras
ideas
```

No es necesario convertir cada actividad del proyecto en una Issue.

Deben representar trabajo real.

---

# 9. GitHub — Conflictos

https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts

La documentación oficial explica cómo abordar conflictos durante la integración de cambios.

La resolución técnica debe complementarse con una decisión:

```text
¿Qué resultado necesita el proyecto?
```

---

# 10. Git — `git merge`

https://git-scm.com/docs/git-merge

La documentación oficial permite profundizar en la integración de ramas.

Es útil para comprender:

```text
merge
conflictos
integración
historial
```

---

# 11. Git — `git switch`

https://git-scm.com/docs/git-switch

Permite consultar el comportamiento de:

```bash
git switch
```

y utilizarlo para cambiar de rama y crear ramas.

---

# 12. Git — `git branch`

https://git-scm.com/docs/git-branch

Permite consultar las operaciones relacionadas con ramas.

Por ejemplo:

```bash
git branch
```

y otras operaciones de administración de ramas.

---

# 13. Git — `git log`

https://git-scm.com/docs/git-log

Es especialmente útil para analizar la historia del Proyecto Final.

Por ejemplo:

```bash
git log --oneline --graph --all
```

Puede ayudar a reconstruir:

```text
qué ocurrió
cuándo
en qué rama
cómo se integraron los cambios
```

---

# 14. Git — `git diff`

https://git-scm.com/docs/git-diff

Permite analizar diferencias entre estados del proyecto.

Por ejemplo:

```bash
git diff
```

es útil antes de registrar un cambio.

La idea es:

```text
modificar
   ↓
revisar
   ↓
registrar
```

---

# 15. Git — `git status`

https://git-scm.com/docs/git-status

`git status` es una de las herramientas más útiles para comprender el estado actual del repositorio.

Por ejemplo:

```bash
git status
```

Permite identificar cambios pendientes y otros estados relevantes del repositorio.

---

# 16. Git — remotos

https://git-scm.com/book/es/v2/Git-en-el-servidor-Git-en-la-red

La documentación y Pro Git permiten profundizar en el trabajo con repositorios remotos.

Conceptos relevantes:

```text
origin
fetch
pull
push
```

---

# 17. Git — `git push`

https://git-scm.com/docs/git-push

Permite consultar cómo se envían referencias y cambios hacia un repositorio remoto.

Es especialmente relevante cuando se trabaja con GitHub.

---

# 18. Git — `git pull`

https://git-scm.com/docs/git-pull

Permite consultar cómo obtener e integrar cambios desde un repositorio remoto.

Debe distinguirse de:

```text
git fetch
```

y:

```text
git push
```

---

# 19. Git — `.gitignore`

https://git-scm.com/docs/gitignore

La documentación oficial explica cómo funciona `.gitignore`.

Puede utilizarse para evitar incorporar al repositorio:

```text
archivos temporales
archivos generados
configuración local
entornos
```

Las reglas deben adaptarse al proyecto.

---

# 20. Plantillas de `.gitignore`

https://github.com/github/gitignore

GitHub mantiene plantillas de `.gitignore` para diferentes lenguajes y herramientas.

Son útiles como referencia.

No conviene copiar una plantilla completa sin analizarla.

La pregunta correcta es:

> ¿Qué archivos genera realmente mi proyecto y cuáles no deberían versionarse?

---

# 21. Seguridad en GitHub

https://docs.github.com/es/code-security

GitHub ofrece diferentes herramientas relacionadas con la seguridad.

Entre ellas:

```text
secret scanning
dependencias
alertas
protección del repositorio
```

No todas son necesarias para todos los proyectos.

---

# 22. Secret Scanning

https://docs.github.com/es/code-security/secret-scanning

Permite conocer las funcionalidades de GitHub relacionadas con la detección de determinados secretos expuestos.

No reemplaza las buenas prácticas.

La prevención continúa siendo fundamental.

---

# 23. Secretos y Git

Si un secreto ya fue registrado en Git, agregar posteriormente el archivo a `.gitignore` no elimina automáticamente el secreto de la historia.

Por eso el principio fundamental es:

```text
prevenir
   ↓
revisar
   ↓
publicar
```

y no:

```text
publicar
   ↓
esperar que una herramienta lo detecte
```

---

# 24. GitHub — Seguridad del repositorio

https://docs.github.com/es/code-security

Antes de publicar un repositorio conviene revisar:

```text
contenido actual
historial
configuración
dependencias
secretos
```

La seguridad debe formar parte del proceso y no ser una tarea exclusivamente final.

---

# 25. GitHub — Documentación

https://docs.github.com/es/get-started/writing-on-github

Este recurso permite profundizar en las herramientas de escritura disponibles en GitHub.

Incluye contenidos relacionados con:

```text
Markdown
referencias
enlaces
listas
código
tablas
```

---

# 26. GitHub Flavored Markdown

https://github.github.com/gfm/

GitHub utiliza una variante de Markdown con funcionalidades adicionales.

Puede consultarse cuando se necesite conocer con precisión cómo se interpreta determinado contenido.

---

# 27. README

https://docs.github.com/es/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes

El README funciona como puerta de entrada al repositorio.

Puede incluir:

```text
descripción
instalación
uso
ejemplos
estructura
información adicional
```

---

# 28. GitHub — Perfil

https://docs.github.com/es/account-and-profile/setting-up-and-managing-your-github-profile

Permite consultar las posibilidades actuales de configuración del perfil.

Para el Proyecto Final resulta útil como referencia para decidir qué proyectos mostrar y cómo presentarlos.

---

# 29. GitHub — Personalizar el perfil

https://docs.github.com/es/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile

Permite profundizar en:

```text
README de perfil
repositorios destacados
información pública
```

El criterio debe ser siempre:

```text
evidencia
+
coherencia
```

y no cantidad.

---

# 30. GitHub Pages

https://pages.github.com/

GitHub Pages permite publicar determinados contenidos directamente desde GitHub.

Puede utilizarse para construir:

```text
portafolios
documentación
sitios de proyectos
páginas personales
```

No es necesario para completar el Proyecto Final.

Es un recurso de profundización.

---

# 31. GitHub Pages — Documentación

https://docs.github.com/es/pages

La documentación oficial permite consultar las posibilidades y configuración de GitHub Pages.

Puede resultar útil como continuación del curso para quienes quieran transformar un proyecto en una presentación web.

---

# 32. CONTRIBUTING.md

https://docs.github.com/es/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors

`CONTRIBUTING.md` puede utilizarse para documentar cómo contribuir a un proyecto.

Por ejemplo:

```text
cómo crear Issues
cómo trabajar con ramas
cómo abrir Pull Requests
convenciones
```

No es obligatorio para todos los proyectos.

---

# 33. CODE_OF_CONDUCT.md

https://docs.github.com/es/communities/setting-up-your-project-for-healthy-contributions/adding-a-code-of-conduct-to-your-project

Un código de conducta puede resultar útil en proyectos con una comunidad o múltiples colaboradores.

No constituye un requisito general del Proyecto Final.

---

# 34. GitHub Discussions

https://docs.github.com/es/discussions

GitHub Discussions permite mantener conversaciones dentro de determinados proyectos.

Puede utilizarse para:

```text
preguntas
ideas
debates
anuncios
```

Una distinción sencilla:

```text
Issue
 ↓
trabajo concreto

Discussion
 ↓
conversación
```

---

# 35. GitHub Community

https://docs.github.com/es/communities

Puede consultarse para profundizar en prácticas relacionadas con proyectos colaborativos y comunidades.

---

# 36. Recursos para continuar aprendiendo

Una vez terminado el curso, se recomienda continuar mediante proyectos.

Una estrategia posible:

```text
Proyecto personal
       ↓
usar Git
       ↓
usar GitHub
       ↓
documentar
       ↓
revisar
       ↓
mejorar
```

Después repetir el ciclo con un nuevo proyecto.

---

# 37. No memorizar

No es necesario memorizar todos los comandos.

Es más importante saber:

```text
qué necesito hacer
        ↓
qué herramienta puede ayudarme
        ↓
dónde consultar
        ↓
cómo probar
        ↓
cómo verificar
```

La documentación forma parte del trabajo cotidiano de desarrollo.

---

# 38. Qué recurso consultar

| Necesidad | Recurso |
|---|---|
| Comandos Git | Git Docs |
| Conceptos Git | Pro Git |
| Ramas | Git Docs / Pro Git |
| Historial | `git log` |
| Diferencias | `git diff` |
| Estado | `git status` |
| GitHub | GitHub Docs |
| Issues | GitHub Docs |
| Pull Requests | GitHub Docs |
| Revisiones | GitHub Docs |
| Conflictos | GitHub Docs |
| Markdown | GitHub Docs / GFM |
| README | GitHub Docs |
| `.gitignore` | Git Docs |
| Seguridad | GitHub Code Security |
| Perfil | GitHub Profile Docs |
| Práctica | GitHub Skills |
| Portafolio web | GitHub Pages |

---

# 39. Recursos fundamentales

Si necesitás conservar solamente algunos recursos, priorizá:

### Git

https://git-scm.com/docs

### Pro Git

https://git-scm.com/book/es/v2

### GitHub Docs

https://docs.github.com/es

### GitHub Skills

https://skills.github.com/

### GitHub Security

https://docs.github.com/es/code-security

---

# 40. Cómo investigar un problema

Cuando aparezca una dificultad técnica, evitá buscar solamente:

```text
"cómo arreglar mi error"
```

Intentá identificar primero:

```text
qué comando ejecuté
qué esperaba que ocurriera
qué ocurrió realmente
qué mensaje apareció
```

Después buscá información utilizando esos datos.

Por ejemplo:

```text
git merge conflict
```

es más útil que:

```text
git no funciona
```

---

# 41. Leer los mensajes de Git

Cuando Git muestre un mensaje de error o advertencia, no lo ignores automáticamente.

Primero:

```text
leer
 ↓
interpretar
 ↓
buscar
 ↓
probar
```

Los mensajes de Git forman parte de la información disponible para resolver el problema.

---

# 42. Usar la ayuda local

Git también incluye ayuda local.

Por ejemplo:

```bash
git help
```

o:

```bash
git help log
```

Según el entorno, también puede utilizarse:

```bash
git log --help
```

La documentación local puede ser útil cuando no se dispone de conexión o se quiere consultar rápidamente la sintaxis.

---

# 43. Recursos como herramientas

Los recursos de este documento no deben considerarse una lista de lecturas obligatorias.

Utilizalos según la necesidad:

```text
problema
   ↓
recurso
   ↓
prueba
   ↓
solución
```

La capacidad de aprender de manera autónoma es uno de los resultados más importantes del curso.

---

# 44. Continuidad después del curso

El Proyecto Final no debería ser el último repositorio que trabajes con Git.

La mejor forma de consolidar lo aprendido es continuar utilizando estas herramientas.

Por ejemplo:

```text
nuevo proyecto
 ↓
repositorio
 ↓
Issues
 ↓
ramas
 ↓
commits
 ↓
Pull Requests
 ↓
revisión
 ↓
merge
 ↓
README
```

Cada nuevo proyecto permite practicar nuevamente el ciclo.

---

# 45. Cierre

Git y GitHub tienen muchas funcionalidades que quedan fuera de este curso.

Eso está bien.

El objetivo de este recorrido fue construir una base sólida para poder seguir aprendiendo.

La competencia más importante es:

```text
no sé
 ↓
sé qué necesito averiguar
 ↓
sé dónde buscar
 ↓
sé cómo probarlo
 ↓
sé cómo verificarlo
```

> **Aprender Git no significa memorizar todos sus comandos. Significa adquirir una forma de trabajar y la capacidad de seguir aprendiendo cuando aparece un problema nuevo.**