# Recursos
## Módulo 07 — Trabajo Colaborativo

Este documento reúne recursos para profundizar los conceptos trabajados durante el módulo.

La documentación no debe estudiarse necesariamente de manera lineal.

La propuesta es utilizarla como material de consulta cuando aparezca una necesidad concreta durante la práctica o el proyecto.

---

# 1. Documentación oficial de Git

La documentación oficial de Git es la referencia principal para consultar comandos, opciones y comportamiento.

https://git-scm.com/docs

Durante este módulo resulta especialmente útil consultar:

```text
git clone
git branch
git switch
git add
git commit
git push
git fetch
git pull
git merge
git log
```

La documentación debe utilizarse como herramienta de trabajo, no solamente como material de estudio.

---

# 2. Pro Git

**Pro Git** es un recurso completo para profundizar en Git.

https://git-scm.com/book/es/v2

Puede consultarse especialmente para ampliar conceptos relacionados con:

- repositorios remotos;
- ramas;
- trabajo distribuido;
- GitHub;
- flujos de trabajo;
- colaboración.

No es necesario leer el libro completo para completar este módulo.

---

# 3. GitHub Docs

La documentación oficial de GitHub:

https://docs.github.com/es

es la referencia principal para las funcionalidades de colaboración que utilizamos en este módulo.

Entre ellas:

- repositorios;
- Issues;
- Pull Requests;
- revisiones;
- ramas;
- conflictos;
- colaboración.

---

# 4. GitHub — Repositorios

La documentación de GitHub sobre repositorios permite profundizar en la administración y utilización de repositorios.

https://docs.github.com/es/repositories

Es útil como referencia para comprender el repositorio como espacio compartido de trabajo.

---

# 5. GitHub — Issues

Las Issues permiten registrar tareas, problemas, propuestas y mejoras.

https://docs.github.com/es/issues

Durante el módulo las utilizamos para representar necesidades del proyecto:

```text
problema
tarea
mejora
propuesta
```

La idea fundamental es:

```text
Issue
  ↓
¿Qué necesitamos hacer?
```

---

# 6. GitHub — Pull Requests

La documentación oficial sobre Pull Requests:

https://docs.github.com/es/pull-requests

permite profundizar en la creación, revisión y administración de Pull Requests.

El concepto central trabajado en el módulo es:

```text
rama
  ↓
Pull Request
  ↓
revisión
  ↓
integración
```

---

# 7. Acerca de las Pull Requests

GitHub explica el propósito de las Pull Requests como mecanismo para proponer y revisar cambios.

https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests

Es un recurso especialmente útil para reforzar la diferencia entre:

```text
commit
```

y:

```text
Pull Request
```

Un commit registra un cambio.

Una Pull Request permite proponer y discutir un conjunto de cambios.

---

# 8. Revisar Pull Requests

La documentación de GitHub sobre revisión:

https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests

permite profundizar en:

- comentarios;
- revisiones;
- aprobación;
- solicitudes de cambios.

La revisión debe entenderse como parte del proceso de desarrollo.

```text
cambio
  ↓
revisión
  ↓
feedback
  ↓
mejora
```

---

# 9. Comentarios sobre cambios

Los comentarios permiten discutir modificaciones concretas.

La documentación de GitHub sobre revisión de cambios:

https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests

puede utilizarse como referencia cuando sea necesario comprender las diferentes posibilidades de una revisión.

Una buena observación debería ayudar a responder:

```text
¿Qué se observó?
¿Por qué importa?
¿Qué podría mejorarse?
```

---

# 10. GitHub — Conflictos de combinación

GitHub documenta los conflictos de merge en:

https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/about-merge-conflicts

Un conflicto aparece cuando Git no puede determinar automáticamente cómo combinar cambios.

El concepto central es:

```text
cambios diferentes
       ↓
conflicto
       ↓
decisión humana
       ↓
resolución
```

---

# 11. Resolver conflictos

Documentación oficial:

https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-using-the-command-line

Este recurso permite consultar el procedimiento para resolver conflictos desde la línea de comandos.

La recomendación pedagógica continúa siendo:

> Primero comprender el conflicto; después resolverlo.

No conviene convertir la resolución en una receta mecánica.

---

# 12. Git Merge

Documentación oficial:

https://git-scm.com/docs/git-merge

`git merge` permite integrar cambios provenientes de otra rama.

Durante este módulo aparece especialmente al integrar trabajo colaborativo.

Ejemplo:

```bash
git switch main
git merge feature
```

La pregunta importante no es solamente:

> ¿Qué comando uso?

Sino:

> ¿Qué ramas estoy integrando y cuál debería ser el resultado?

---

# 13. Git Push

Documentación oficial:

https://git-scm.com/docs/git-push

`git push` publica commits locales en el repositorio remoto.

Conceptualmente:

```text
repositorio local
       ↓
     push
       ↓
repositorio remoto
```

Es importante distinguir:

```text
commit
```

de:

```text
push
```

Un commit registra el cambio localmente.

El push publica ese cambio en el remoto.

---

# 14. Git Fetch

Documentación oficial:

https://git-scm.com/docs/git-fetch

`git fetch` permite obtener información del repositorio remoto sin integrar automáticamente esos cambios en la rama actual.

Conceptualmente:

```text
repositorio remoto
       ↓
      fetch
       ↓
información actualizada
```

Es especialmente útil para inspeccionar cambios remotos antes de decidir qué hacer con ellos.

---

# 15. Git Pull

Documentación oficial:

https://git-scm.com/docs/git-pull

`git pull` permite actualizar el repositorio local a partir de cambios disponibles en el repositorio remoto.

Conceptualmente:

```text
repositorio remoto
       ↓
      pull
       ↓
repositorio local actualizado
```

Durante el módulo se busca comprender la diferencia conceptual entre:

```bash
git fetch
```

y:

```bash
git pull
```

---

# 16. Git Clone

Documentación oficial:

https://git-scm.com/docs/git-clone

`git clone` permite obtener una copia local de un repositorio existente.

Ejemplo:

```bash
git clone URL_DEL_REPOSITORIO
```

Conceptualmente:

```text
GitHub
  ↓
clone
  ↓
repositorio local
```

Es una operación habitual al incorporarse a un proyecto existente.

---

# 17. Git Branch

Documentación oficial:

https://git-scm.com/docs/git-branch

Permite consultar, crear y administrar ramas.

Ejemplos:

```bash
git branch
```

```bash
git branch nombre-rama
```

```bash
git branch -d nombre-rama
```

---

# 18. Git Switch

Documentación oficial:

https://git-scm.com/docs/git-switch

Permite cambiar de rama y crear nuevas ramas.

Ejemplos:

```bash
git switch main
```

```bash
git switch feature
```

```bash
git switch -c feature
```

En este módulo se utiliza especialmente para separar tareas de trabajo.

---

# 19. Git Log

Documentación oficial:

https://git-scm.com/docs/git-log

Para analizar la historia colaborativa resulta especialmente útil:

```bash
git log --oneline --graph --all
```

Permite observar visualmente las diferentes líneas de desarrollo.

Por ejemplo:

```text
*   M
|\
| * E
| * D
|/
* C
* B
* A
```

Intentá utilizar esta herramienta para reconstruir cómo evolucionó el proyecto.

---

# 20. GitHub — Ramas

La documentación de GitHub sobre ramas puede consultarse en:

https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/working-with-branches

Las ramas permiten trabajar sobre diferentes líneas de desarrollo.

En un proyecto colaborativo pueden representar:

```text
feature
fix
docs
```

entre otras posibilidades.

---

# 21. GitHub — Protección de ramas

GitHub permite configurar reglas para proteger determinadas ramas.

Documentación:

https://docs.github.com/es/repositories/configuring-branches-and-merges-in-your-repository/managing-rulesets/about-rulesets

Esto puede utilizarse para establecer condiciones antes de incorporar cambios a ramas importantes.

Por ejemplo:

```text
main
 ↓
protegida
 ↓
Pull Request
 ↓
revisión
 ↓
merge
```

La protección de ramas no es necesaria en todos los proyectos.

Debe entenderse como una herramienta para controlar el flujo de integración.

---

# 22. CONTRIBUTING.md

GitHub reconoce `CONTRIBUTING.md` como una forma habitual de documentar cómo contribuir a un proyecto.

Información general:

https://docs.github.com/es/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors

Puede utilizarse para documentar:

- cómo comenzar;
- cómo crear ramas;
- convenciones;
- Issues;
- commits;
- Pull Requests;
- revisiones.

En este módulo se utiliza como herramienta práctica para establecer las reglas del equipo.

---

# 23. CODE_OF_CONDUCT.md

Los proyectos colaborativos también pueden incluir un código de conducta.

GitHub proporciona información sobre este tema:

https://docs.github.com/es/communities/setting-up-your-project-for-healthy-contributions/adding-a-code-of-conduct-to-your-project

El objetivo es establecer expectativas sobre la participación y comunicación dentro de una comunidad.

No constituye un requisito técnico de Git.

Es una herramienta complementaria para proyectos colaborativos.

---

# 24. GitHub — Colaboradores

La documentación sobre colaboración en repositorios permite profundizar en la administración de personas que trabajan sobre un proyecto.

https://docs.github.com/es/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/managing-repository-settings

La forma concreta de administrar permisos depende del tipo de repositorio y de la configuración de GitHub.

Para este curso interesa principalmente comprender el concepto:

```text
repositorio
     ↓
personas
     ↓
permisos
     ↓
trabajo colaborativo
```

---

# 25. GitHub Desktop

GitHub Desktop ofrece una interfaz gráfica para trabajar con repositorios Git.

https://desktop.github.com/

Puede resultar útil como herramienta complementaria para visualizar:

- ramas;
- commits;
- cambios;
- sincronización.

Sin embargo, durante el curso se recomienda mantener la terminal como herramienta principal para comprender explícitamente las operaciones de Git.

---

# 26. Visual Studio Code

Visual Studio Code incluye herramientas para trabajar con Git.

https://code.visualstudio.com/docs/sourcecontrol/overview

Puede utilizarse para:

- revisar cambios;
- administrar ramas;
- visualizar diferencias;
- resolver conflictos.

La herramienta gráfica puede facilitar algunas tareas, pero no reemplaza la comprensión de lo que Git está haciendo.

---

# 27. Resolución de conflictos en Visual Studio Code

Visual Studio Code proporciona herramientas visuales para resolver conflictos.

https://code.visualstudio.com/docs/sourcecontrol/overview

Cuando aparece un conflicto pueden observarse diferentes versiones del contenido.

La herramienta ayuda a editar el archivo.

Pero la decisión sigue siendo:

```text
¿Qué resultado necesita el proyecto?
```

---

# 28. GitHub Skills

GitHub ofrece recursos educativos prácticos mediante GitHub Skills.

https://skills.github.com/

Pueden resultar útiles para continuar practicando conceptos como:

- GitHub;
- Issues;
- Pull Requests;
- colaboración;
- workflows.

Son especialmente apropiados como material de profundización autónoma.

---

# 29. Documentación para nuevos colaboradores

Al incorporarse a un proyecto, una persona debería poder encontrar rápidamente:

```text
README.md
CONTRIBUTING.md
```

y, cuando corresponda:

```text
CODE_OF_CONDUCT.md
```

Estos documentos ayudan a separar diferentes tipos de información:

```text
README
 ↓
¿Qué es este proyecto?

CONTRIBUTING
 ↓
¿Cómo participo?

CODE_OF_CONDUCT
 ↓
¿Cómo nos relacionamos?
```

---

# 30. Recursos de consulta rápida

Si necesitás consultar solamente los recursos fundamentales del módulo:

### Git

:contentReference[oaicite:0]{index=0}

### Pro Git

:contentReference[oaicite:1]{index=1}

### GitHub Docs

:contentReference[oaicite:2]{index=2}

### GitHub Pull Requests

:contentReference[oaicite:3]{index=3}

### GitHub Issues

:contentReference[oaicite:4]{index=4}

### GitHub Skills

:contentReference[oaicite:5]{index=5}

---

# 31. Referencia rápida de comandos

| Necesidad | Comando |
|---|---|
| Clonar repositorio | `git clone URL` |
| Consultar ramas | `git branch` |
| Crear rama | `git branch nombre` |
| Crear y cambiar | `git switch -c nombre` |
| Cambiar de rama | `git switch nombre` |
| Registrar cambios | `git add` + `git commit` |
| Publicar cambios | `git push` |
| Obtener información remota | `git fetch` |
| Actualizar localmente | `git pull` |
| Integrar rama | `git merge` |
| Ver historia | `git log --oneline` |
| Ver historia gráfica | `git log --oneline --graph --all` |

---

# 32. Conceptos para consultar

Cuando aparezca una duda, intentá identificar primero el concepto.

| Necesito... | Consultar |
|---|---|
| Obtener un proyecto | `git clone` |
| Crear una línea de trabajo | `git branch` / `git switch` |
| Registrar un cambio | `git commit` |
| Publicar cambios | `git push` |
| Ver qué hay en remoto | `git fetch` |
| Actualizar mi copia | `git pull` |
| Integrar cambios | `git merge` |
| Proponer cambios | Pull Request |
| Registrar una tarea | Issue |
| Revisar cambios | Pull Request Review |
| Resolver un conflicto | Merge conflicts |
| Documentar colaboración | `CONTRIBUTING.md` |

---

# 33. Cómo utilizar estos recursos

No intentes memorizar todo.

Utilizá la documentación siguiendo este patrón:

```text
Tengo un problema
       ↓
Identifico la operación
       ↓
Busco la documentación
       ↓
Leo el ejemplo
       ↓
Pruebo
       ↓
Verifico
```

Por ejemplo:

> "Necesito publicar una rama."

Buscás:

```text
git push
```

> "Necesito saber qué cambió en remoto."

Buscás:

```text
git fetch
```

> "Tengo conflictos."

Buscás:

```text
git merge conflict
```

La capacidad de consultar documentación forma parte de la competencia profesional.

---

# 34. Material complementario

Una vez comprendido el flujo básico de colaboración, se puede profundizar en:

- protección avanzada de ramas;
- reglas de repositorio;
- estrategias de branching;
- revisiones obligatorias;
- permisos;
- equipos;
- automatización;
- GitHub Actions;
- integración continua;
- plantillas de Issues;
- plantillas de Pull Requests;
- automatización de workflows.

Estos contenidos exceden el núcleo del módulo.

Su estudio queda como material complementario para quienes quieran profundizar.

---

# 35. Lectura recomendada

Para consolidar el módulo, se recomienda poder responder estas preguntas consultando la documentación cuando sea necesario:

```text
¿Qué diferencia existe entre Git y GitHub?

¿Qué diferencia existe entre commit y Pull Request?

¿Qué diferencia existe entre push, pull y fetch?

¿Qué es una Issue?

¿Qué es una Pull Request?

¿Qué significa revisar una Pull Request?

¿Por qué aparecen conflictos?

¿Cómo se resuelve un conflicto?

¿Qué información debería contener CONTRIBUTING.md?

¿Por qué podría protegerse main?
```

Si podés responder estas preguntas y además realizar el flujo práctico, los recursos de referencia están cumpliendo su función.

---

# 36. Idea final

La documentación oficial no está solamente para cuando algo sale mal.

Forma parte del trabajo cotidiano de una persona que utiliza herramientas técnicas.

El objetivo profesional es pasar de:

```text
"me acuerdo de este comando"
```

a:

```text
"sé qué necesito hacer,
sé dónde buscarlo
y sé cómo verificar el resultado."
```

> **No necesitás memorizar GitHub. Necesitás aprender a trabajar con GitHub.**