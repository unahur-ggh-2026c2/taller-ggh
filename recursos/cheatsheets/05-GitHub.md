# Cheatsheet — GitHub

> Referencia rápida para trabajar con repositorios y colaborar mediante GitHub.

---

## Repositorio remoto

Consultar los remotos configurados:

```bash
git remote -v
```

Publicar cambios:

```bash id="m3x8qk"
git push
```

Obtener cambios:

```bash id="8y7w2p"
git pull
```

Primera publicación de una rama:

```bash id="k4n6rz"
git push -u origin nombre-de-la-rama
```

---

## Flujo local → GitHub

```text
cambios
   ↓
commit
   ↓
push
   ↓
GitHub
```

Para una tarea desarrollada en una rama:

```text
Issue
   ↓
rama
   ↓
commit
   ↓
push
   ↓
Pull Request
```

---

## Issue

Una **Issue** permite registrar y organizar trabajo.

Puede representar:

```text
tarea
problema
mejora
idea
```

Una Issue útil debería dejar claro:

```text
qué problema existe
qué se quiere lograr
qué resultado se espera
```

Evitá títulos demasiado vagos:

```text
Mejorar aplicación
Cambios
Arreglar cosas
```

---

## Relacionar trabajo

Un flujo habitual:

```text
Issue #12
    ↓
feature-validacion
    ↓
commits
    ↓
Pull Request
    ↓
revisión
    ↓
merge
```

La Issue representa la necesidad.

Los commits registran el trabajo.

La Pull Request propone integrar ese trabajo.

---

## Pull Request

Una Pull Request permite:

```text
proponer cambios
revisarlos
comentar
solicitar correcciones
integrarlos
```

Flujo:

```text
rama de trabajo
      ↓
push
      ↓
Pull Request
      ↓
review
      ↓
correcciones
      ↓
merge
```

---

## Descripción de una Pull Request

Como mínimo debería explicar:

```md
## Qué hice

...

## Por qué

...

## Cómo lo probé

...
```

Evitá descripciones como:

```text
"Actualización"
"Changes"
"Listo"
```

---

## Revisar una Pull Request

Antes de aprobar, preguntate:

```text
[ ] ¿Resuelve el objetivo?
[ ] ¿El cambio es coherente?
[ ] ¿Está probado?
[ ] ¿La documentación corresponde?
[ ] ¿Hay algo que deba corregirse?
```

Una revisión no consiste solamente en comprobar si "funciona".

---

## Feedback

Un comentario útil debería indicar:

```text
qué observaste
+
por qué importa
+
qué podría mejorarse
```

### Poco útil

```text
Esto está mal.
```

### Más útil

```text
Esta validación no contempla entradas vacías.
Conviene verificarlas antes de procesar el valor.
```

---

## Solicitar cambios

Cuando una revisión requiere una corrección:

```text
Pull Request
   ↓
feedback
   ↓
corrección
   ↓
commit
   ↓
push
   ↓
nueva revisión
```

No hace falta crear otra Pull Request para cada corrección.

---

## Merge

Cuando una Pull Request está lista:

```text
Pull Request
      ↓
aprobación
      ↓
merge
      ↓
main
```

Después de integrar:

```bash id="7h3v0m"
git switch main
git pull
```

---

## Ramas en GitHub

Para consultar las ramas localmente:

```bash id="z1h4ws"
git branch
```

Para crear una rama:

```bash id="v8f6pt"
git switch -c feature-nombre
```

Para publicarla:

```bash id="q5m2ya"
git push -u origin feature-nombre
```

---

## GitHub no reemplaza a Git

```text
Git
 ↓
control de versiones
```

```text
GitHub
 ↓
repositorios remotos
colaboración
Issues
Pull Requests
revisiones
```

Git puede utilizarse sin GitHub.

---

## Antes de publicar

Revisá:

```bash id="x6r9ce"
git status
```

Y asegurate de no publicar:

```text
contraseñas
tokens
claves
credenciales
datos sensibles
archivos locales
```

Revisá también:

```text
.gitignore
```

---

## Después de publicar

Comprobá en GitHub:

```text
[ ] Repositorio correcto.
[ ] Rama correcta.
[ ] Commits visibles.
[ ] README actualizado.
[ ] Issues relevantes.
[ ] Pull Requests correctas.
[ ] Sin información sensible.
```

---

## Flujo colaborativo completo

```text
Issue
  ↓
rama
  ↓
desarrollo
  ↓
commit
  ↓
push
  ↓
Pull Request
  ↓
revisión
  ↓
corrección
  ↓
merge
  ↓
main
```

---

## Comandos esenciales

| Necesidad       | Comando                   |
| --------------- | ------------------------- |
| Ver remoto      | `git remote -v`           |
| Publicar        | `git push`                |
| Obtener cambios | `git pull`                |
| Crear rama      | `git switch -c rama`      |
| Cambiar de rama | `git switch rama`         |
| Ver ramas       | `git branch`              |
| Publicar rama   | `git push -u origin rama` |

---

## Regla práctica

```text
Git
 ↓
registra el trabajo

GitHub
 ↓
permite compartirlo, revisarlo
y colaborar sobre él
```

> **GitHub no es solamente el lugar donde subís el proyecto: es el espacio donde el trabajo versionado puede organizarse, revisarse y compartirse.**
