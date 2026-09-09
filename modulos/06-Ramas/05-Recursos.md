# Recursos
## Módulo 06 — Ramas

Los recursos de este módulo están orientados a profundizar el trabajo con ramas, integración de cambios, conflictos y trabajo con ramas remotas.

No es necesario estudiar toda la documentación de manera lineal.

La propuesta es utilizar estos recursos como material de consulta cuando aparezca una duda concreta durante la práctica.

---

## 1. Documentación oficial de Git

### Git Reference

https://git-scm.com/docs

La documentación oficial de Git permite consultar los comandos y sus opciones.

Es especialmente útil cuando necesitás conocer con precisión el comportamiento de una operación.

Durante este módulo podés consultar:

- `git branch`;
- `git switch`;
- `git merge`;
- `git log`;
- `git diff`;
- `git push`.

---

## 2. Pro Git

### Chacon, S. y Straub, B.

**Pro Git**

https://git-scm.com/book/es/v2

Es uno de los recursos de referencia más completos para aprender Git.

Para este módulo resultan especialmente relevantes los contenidos relacionados con:

- ramas;
- creación de ramas;
- cambio de ramas;
- integración;
- conflictos;
- ramas remotas.

No es necesario leer el libro completo para completar el módulo.

---

## 3. Git Branch

Documentación oficial:

https://git-scm.com/docs/git-branch

Permite consultar específicamente las operaciones relacionadas con ramas.

Entre otras posibilidades, documenta:

```bash
git branch
git branch nombre-rama
git branch -d nombre-rama
```

Utilizala como referencia cuando necesites comprobar cómo consultar, crear o eliminar ramas.

---

## 4. Git Switch

Documentación oficial:

https://git-scm.com/docs/git-switch

`git switch` permite cambiar de rama y crear una nueva rama.

Ejemplos trabajados durante el módulo:

```bash
git switch main
```

```bash
git switch feature
```

```bash
git switch -c feature
```

La documentación oficial permite consultar las diferentes opciones disponibles.

---

## 5. Git Merge

Documentación oficial:

https://git-scm.com/docs/git-merge

`git merge` permite integrar los cambios de una rama en otra.

El concepto fundamental trabajado en este módulo es:

```text
rama actual
     ↓
git merge otra-rama
     ↓
integración
```

La documentación oficial resulta útil para profundizar en las diferentes situaciones que pueden producirse durante una integración.

---

## 6. Conflictos de merge

GitHub ofrece una introducción a los conflictos de merge:

https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/about-merge-conflicts

Un conflicto aparece cuando Git no puede determinar automáticamente cómo combinar cambios realizados sobre una misma parte del proyecto.

El proceso general es:

```text
merge
  ↓
conflicto
  ↓
identificar archivos
  ↓
analizar cambios
  ↓
decidir resultado
  ↓
resolver
  ↓
git add
  ↓
completar integración
```

---

## 7. Resolución de conflictos desde la línea de comandos

GitHub documenta también el procedimiento general para resolver conflictos:

https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-using-the-command-line

Este recurso resulta especialmente útil después de provocar deliberadamente un conflicto durante los ejercicios.

No se recomienda memorizar el procedimiento.

La idea es comprender qué está ocurriendo y utilizar la documentación como referencia cuando sea necesario.

---

## 8. Git Log

Documentación oficial:

https://git-scm.com/docs/git-log

Durante este módulo utilizamos especialmente:

```bash
git log --oneline
```

y:

```bash
git log --oneline --graph --all
```

La segunda forma permite visualizar de manera más clara las diferentes líneas de evolución.

Ejemplo:

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

---

## 9. Git Diff

Documentación oficial:

https://git-scm.com/docs/git-diff

Permite comparar cambios.

Durante el módulo puede utilizarse para comparar ramas:

```bash
git diff main..feature
```

El objetivo no es memorizar todas las posibilidades de `git diff`, sino comenzar a utilizarlo como herramienta para analizar diferencias antes de integrar cambios.

---

## 10. Git Push

Documentación oficial:

https://git-scm.com/docs/git-push

Durante el módulo utilizamos:

```bash
git push -u origin nombre-rama
```

Esta operación permite publicar una rama local en el repositorio remoto.

Es importante distinguir:

```text
crear una rama
```

de:

```text
publicar una rama
```

Crear una rama local no hace que aparezca automáticamente en GitHub.

---

## 11. GitHub — Ramas

GitHub documenta el trabajo con ramas en:

https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/working-with-forks/about-permissions-and-visibility-of-forks

Para el trabajo específico con ramas también puede consultarse:

https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/working-with-branches

Estos recursos permiten profundizar en la utilización de ramas dentro de repositorios alojados en GitHub.

---

## 12. Ramas remotas

La documentación oficial de Git permite profundizar sobre las ramas remotas:

https://git-scm.com/book/es/v2/Git-en-el-servidor-Git-en-el-servidor

El concepto central que debemos conservar es:

```text
Repositorio local
       ↓
ramas locales

Repositorio remoto
       ↓
ramas remotas
```

La sincronización entre ambos mundos será cada vez más importante a medida que avancemos hacia el trabajo colaborativo.

---

## 13. GitHub — Comparación de ramas

GitHub permite comparar diferentes ramas de un repositorio.

La documentación correspondiente puede consultarse en:

https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/working-with-pull-requests/about-pull-requests

Esta posibilidad será especialmente relevante en el módulo siguiente, donde las ramas se utilizarán dentro de un flujo de trabajo colaborativo.

---

## 14. Pull Requests

Aunque el foco de este módulo está puesto en las ramas y no todavía en el trabajo colaborativo completo, es útil conocer el concepto de **Pull Request**.

Documentación oficial:

https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests

Una Pull Request permite proponer cambios realizados sobre una rama para que sean revisados e integrados en otra.

El flujo puede representarse:

```text
rama
  ↓
commits
  ↓
GitHub
  ↓
Pull Request
  ↓
revisión
  ↓
integración
```

Este concepto será retomado en profundidad en el módulo de trabajo colaborativo.

---

## 15. Visualizar ramas

Para comprender las ramas resulta especialmente útil observar la historia gráficamente.

Utilizá:

```bash
git log --oneline --graph --all
```

Practicá la lectura de historias como:

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

Intentá responder:

```text
¿Dónde se separaron las líneas?
¿Qué rama avanzó?
¿Qué commits pertenecen a cada línea?
¿Dónde se produjo la integración?
```

La capacidad de leer este gráfico es más importante que memorizar su formato.

---

## 16. Visualización gráfica adicional

Como herramienta complementaria, GitHub Desktop puede resultar útil para observar visualmente ramas y commits.

https://desktop.github.com/

No es necesario utilizarlo para realizar las prácticas.

El objetivo del curso continúa siendo comprender Git y poder trabajar con él desde la línea de comandos.

Una herramienta gráfica puede utilizarse como apoyo visual, pero no reemplaza la comprensión de los conceptos.

---

## 17. Visual Studio Code

Visual Studio Code también incorpora herramientas para trabajar con Git:

https://code.visualstudio.com/docs/sourcecontrol/overview

Puede utilizarse para:

- consultar cambios;
- cambiar de rama;
- observar modificaciones;
- resolver conflictos;
- revisar archivos.

Durante el curso se recomienda continuar utilizando principalmente la terminal para que las operaciones de Git sean explícitas.

---

## 18. Resolución de conflictos en Visual Studio Code

Visual Studio Code ofrece herramientas visuales para trabajar con conflictos:

https://code.visualstudio.com/docs/sourcecontrol/overview

Cuando aparece un conflicto, el editor puede mostrar las diferentes versiones y permitir seleccionar o combinar cambios.

Sin embargo, antes de utilizar estas herramientas es importante comprender el problema:

```text
dos líneas de trabajo
        ↓
cambios incompatibles
        ↓
Git no puede decidir
        ↓
decisión humana
```

La herramienta ayuda a resolverlo.

No reemplaza la decisión sobre qué contenido debe conservarse.

---

## 19. Referencia rápida de comandos

### Consultar ramas

```bash
git branch
```

### Crear una rama

```bash
git branch nombre-rama
```

### Crear y cambiar

```bash
git switch -c nombre-rama
```

### Cambiar de rama

```bash
git switch nombre-rama
```

### Fusionar

```bash
git switch rama-destino
git merge rama-origen
```

### Eliminar una rama local

```bash
git branch -d nombre-rama
```

### Publicar una rama

```bash
git push -u origin nombre-rama
```

### Ver la historia

```bash
git log --oneline
```

### Ver la historia gráficamente

```bash
git log --oneline --graph --all
```

### Comparar ramas

```bash
git diff rama-a..rama-b
```

---

## 20. Tabla de referencia

| Operación | Comando |
|---|---|
| Consultar ramas | `git branch` |
| Crear rama | `git branch nombre` |
| Crear y cambiar | `git switch -c nombre` |
| Cambiar de rama | `git switch nombre` |
| Fusionar | `git merge nombre` |
| Eliminar rama | `git branch -d nombre` |
| Publicar rama | `git push -u origin nombre` |
| Ver historial | `git log --oneline` |
| Ver gráfico | `git log --oneline --graph --all` |
| Comparar ramas | `git diff rama-a..rama-b` |

---

## 21. Material complementario

Una vez comprendidos los conceptos fundamentales, podés profundizar en:

- estrategias de branching;
- Git Flow;
- trunk-based development;
- Pull Requests;
- revisión de código;
- ramas protegidas;
- integración continua;
- automatización de workflows.

Estos temas exceden el núcleo de este módulo.

Su estudio queda como material complementario para quienes quieran profundizar en flujos de trabajo profesionales.

---

## 22. Qué estudiar y qué consultar

No es necesario memorizar toda la documentación.

Una estrategia razonable es:

```text
Necesidad
   ↓
Identificar operación
   ↓
Consultar documentación
   ↓
Probar
   ↓
Verificar
   ↓
Continuar
```

Por ejemplo:

> "Necesito crear una rama y cambiarme a ella."

Consultás:

```bash
git switch -c
```

> "Necesito integrar una rama."

Consultás:

```bash
git merge
```

> "Necesito saber qué pasó con la historia."

Consultás:

```bash
git log --graph
```

---

## 23. Recursos mínimos

Si necesitás conservar solamente las referencias esenciales de este módulo:

### Git

:contentReference[oaicite:0]{index=0}

### Pro Git

:contentReference[oaicite:1]{index=1}

### GitHub Docs

:contentReference[oaicite:2]{index=2}

### GitHub — Conflictos

:contentReference[oaicite:3]{index=3}

### Visual Studio Code — Git

:contentReference[oaicite:4]{index=4}

---

## 24. Estrategia de consulta

Los recursos de este módulo deben utilizarse como herramientas de trabajo.

No hace falta memorizar cada opción.

La competencia que buscamos desarrollar es:

```text
comprender el problema
        ↓
identificar la operación necesaria
        ↓
consultar la documentación
        ↓
ejecutar
        ↓
verificar
        ↓
explicar el resultado
```

La documentación oficial no es solamente un material de estudio.

Es una herramienta profesional que vas a seguir utilizando mucho después de terminar este curso.

---

> **No se espera que recuerdes todos los comandos de Git. Se espera que puedas comprender qué necesitás hacer, encontrar la operación adecuada y verificar que el resultado sea el esperado.**