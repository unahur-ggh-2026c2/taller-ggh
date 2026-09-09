# Cheatsheet — Ramas

> Referencia rápida para crear, cambiar, consultar e integrar ramas en Git.

---

## Ver ramas

Ramas locales:

```bash
git branch
```

Todas las ramas, incluyendo las remotas:

```bash id="4a9k2r"
git branch -a
```

La rama actual aparece marcada con `*`.

---

## Crear una rama

Crear una rama sin cambiarte:

```bash id="q7v3ne"
git branch nombre-de-la-rama
```

Crear una rama y cambiarte inmediatamente:

```bash id="t2m8xp"
git switch -c nombre-de-la-rama
```

Ejemplo:

```bash id="c5r1wf"
git switch -c feature-login
```

---

## Cambiar de rama

```bash id="m6x4qa"
git switch nombre-de-la-rama
```

Ejemplo:

```bash id="n8k2sd"
git switch main
```

Antes de cambiar de rama, revisá el estado:

```bash id="p4w7yz"
git status
```

---

## Rama actual

La forma más sencilla de identificarla:

```bash id="r9c3vt"
git status
```

También:

```bash id="e6j1mk"
git branch
```

---

## Flujo básico

Para una nueva funcionalidad:

```text
main
  ↓
crear rama
  ↓
trabajar
  ↓
commits
  ↓
push
  ↓
Pull Request
  ↓
merge
```

Por ejemplo:

```bash id="u3f8hb"
git switch main
git pull
git switch -c feature-login
```

---

## Trabajar en una rama

Una vez creada:

```bash id="s5q2dx"
git status
```

Realizá los cambios y registralos:

```bash id="a8m4kw"
git add .
git commit -m "Implementa inicio de sesión"
```

Publicá la rama:

```bash id="v7p3nc"
git push -u origin feature-login
```

---

## Integrar una rama

Primero ubicarse en la rama que recibirá los cambios:

```bash id="f2k8qm"
git switch main
```

Actualizarla:

```bash id="z6w1pr"
git pull
```

Integrar:

```bash id="h4n9tx"
git merge feature-login
```

---

## El sentido de `merge`

Si estás en:

```text
main
```

y ejecutás:

```bash id="j7c5mv"
git merge feature-login
```

estás diciendo:

> Integrá los cambios de `feature-login` en `main`.

La dirección importa.

```text
rama actual
    ↑
recibe
    ↑
rama indicada en merge
```

---

## Publicar una rama

Primera vez:

```bash id="x8v3ql"
git push -u origin feature-login
```

Después:

```bash id="k5r2nd"
git push
```

---

## Eliminar una rama local

Una vez integrada y cuando ya no sea necesaria:

```bash id="m4q7ws"
git branch -d feature-login
```

La opción `-d` evita eliminarla si Git considera que contiene cambios que todavía no fueron integrados.

Para forzar la eliminación existe:

```bash id="z3n6kp"
git branch -D feature-login
```

⚠️ Usalo solamente cuando entiendas qué cambios estás descartando.

---

## Eliminar una rama remota

Si necesitás eliminar una rama del remoto:

```bash id="q9t4cx"
git push origin --delete feature-login
```

---

## Ver historial de ramas

Para comprender cómo evolucionaron las ramas:

```bash id="v2m7fa"
git log --oneline --graph --all
```

Ejemplo:

```text
*   e81a123 Merge branch 'feature-login'
|\
| * a81f3c2 Agrega validación
| * c52a19e Implementa login
|/
* 81d4f90 Inicializa proyecto
```

---

## Nombres de ramas

Preferí nombres que indiquen el propósito:

```text
feature-login
feature-busqueda
fix-validacion
docs-readme
```

Evitá:

```text
rama1
prueba
cosas
nueva
final
```

El nombre debería permitir entender para qué existe la rama.

---

## Rama y tarea

Una relación habitual:

```text
Issue
  ↓
rama
  ↓
commits
  ↓
Pull Request
```

Ejemplo:

```text
Issue #15
"Agregar búsqueda de usuarios"
        ↓
feature-busqueda-usuarios
```

---

## Ramas y trabajo colaborativo

Una rama permite trabajar sobre una tarea sin modificar directamente la línea principal.

```text
main
 |
 A
 |
 B
 |\
 | \
 |  C
 |  D
 |  E
 | /
 F
```

La rama permite desarrollar el cambio de manera aislada hasta que esté listo para integrarse.

---

## Conflictos

Un `merge` puede producir conflictos.

Si ocurre:

```bash id="n3f7xp"
git status
```

Identificá los archivos afectados.

Después:

```text
resolver
   ↓
revisar
   ↓
probar
   ↓
continuar
```

No elijas una versión automáticamente sin comprender el cambio.

---

## Antes de cambiar de rama

Comprobá:

```bash id="b8k4zm"
git status
```

Si tenés cambios locales pendientes, decidí qué corresponde hacer antes de cambiar:

```text
registrar
descartar
guardar temporalmente
```

No cambies de rama a ciegas.

---

## Comandos esenciales

| Necesidad       | Comando                           |
| --------------- | --------------------------------- |
| Ver ramas       | `git branch`                      |
| Ver todas       | `git branch -a`                   |
| Crear rama      | `git branch rama`                 |
| Crear y cambiar | `git switch -c rama`              |
| Cambiar         | `git switch rama`                 |
| Integrar        | `git merge rama`                  |
| Publicar rama   | `git push -u origin rama`         |
| Eliminar local  | `git branch -d rama`              |
| Eliminar remoto | `git push origin --delete rama`   |
| Ver historia    | `git log --oneline --graph --all` |

---

## Flujo recomendado

```text
git switch main
git pull
git switch -c feature-nombre
```

Trabajar:

```text
cambios
  ↓
git status
  ↓
git add
  ↓
git commit
```

Publicar:

```bash id="r8m3vq"
git push -u origin feature-nombre
```

Después:

```text
Pull Request
  ↓
revisión
  ↓
merge
```

Finalmente:

```bash id="c6w9pt"
git switch main
git pull
```

> **Una rama no es una copia descartable del proyecto: es una línea de trabajo que permite desarrollar y revisar cambios antes de integrarlos.**
