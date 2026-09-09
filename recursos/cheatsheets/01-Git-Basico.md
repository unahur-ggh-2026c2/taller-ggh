# Cheatsheet — Git Básico

> Referencia rápida para las operaciones fundamentales de Git.

---

## Crear un repositorio

Inicializar Git en un proyecto:

```bash
git init
```

Comprobar el estado:

```bash
git status
```

---

## Flujo básico

```text
modificar
   ↓
git status
   ↓
git add
   ↓
git commit
```

Comandos:

```bash
git status
git add archivo
git commit -m "Describe el cambio"
```

---

## Preparar cambios

Un archivo:

```bash
git add archivo.txt
```

Varios:

```bash
git add archivo1.txt archivo2.txt
```

Todo lo correspondiente al directorio actual:

```bash
git add .
```

---

## Crear un commit

```bash
git commit -m "Agrega validación de entrada"
```

El mensaje debería describir el cambio.

### Mejor

```text
Agrega validación de entrada
Corrige cálculo de totales
Documenta instalación
```

### Evitar

```text
cambios
fix
cosas
final
```

---

## Consultar el historial

Historial completo:

```bash
git log
```

Historial resumido:

```bash
git log --oneline
```

Historial con ramas:

```bash
git log --oneline --graph --all
```

---

## Revisar cambios

Cambios todavía no preparados:

```bash
git diff
```

Cambios preparados:

```bash
git diff --staged
```

Ver un commit:

```bash
git show HEAD
```

---

## Trabajar con ramas

Crear una rama y cambiarse:

```bash
git switch -c feature-nombre
```

Cambiar de rama:

```bash
git switch nombre-de-la-rama
```

Listar ramas:

```bash
git branch
```

---

## Integrar una rama

Primero ubicarse en la rama que recibirá los cambios:

```bash
git switch main
```

Después:

```bash
git merge feature-nombre
```

---

## Repositorio remoto

Consultar remotos:

```bash
git remote -v
```

Publicar cambios:

```bash
git push
```

Obtener cambios:

```bash
git pull
```

Primera publicación de una rama:

```bash
git push -u origin nombre-de-la-rama
```

---

## `.gitignore`

Archivo:

```text
.gitignore
```

Ejemplo:

```gitignore
.env
.venv/
__pycache__/
*.log
```

Usalo para archivos que no deberían formar parte del seguimiento del proyecto.

> Agregar posteriormente un archivo a `.gitignore` no elimina automáticamente lo que ya fue registrado en Git.

---

## Deshacer una preparación

Si ejecutaste:

```bash
git add archivo.txt
```

y querés quitarlo del área de preparación:

```bash
git restore --staged archivo.txt
```

El cambio del archivo no se elimina.

---

## Descartar un cambio local

```bash
git restore archivo.txt
```

⚠️ Descarta las modificaciones no registradas del archivo.

Antes de hacerlo, revisá:

```bash
git diff
```

---

## Comandos esenciales

| Necesidad       | Comando         |
| --------------- | --------------- |
| Inicializar     | `git init`      |
| Estado          | `git status`    |
| Preparar        | `git add`       |
| Commit          | `git commit`    |
| Historial       | `git log`       |
| Cambios         | `git diff`      |
| Ver commit      | `git show`      |
| Ramas           | `git branch`    |
| Crear rama      | `git switch -c` |
| Cambiar rama    | `git switch`    |
| Integrar        | `git merge`     |
| Remotos         | `git remote -v` |
| Publicar        | `git push`      |
| Obtener cambios | `git pull`      |

---

## Flujo de trabajo

```text
Issue
  ↓
rama
  ↓
cambios
  ↓
commit
  ↓
push
  ↓
Pull Request
  ↓
revisión
  ↓
merge
```

---

## Si no sabés qué está pasando

Primero:

```bash
git status
```

Después, si necesitás ver los cambios:

```bash
git diff
```

Y para entender la historia:

```bash
git log --oneline --graph --all
```

> **No necesitás memorizar todos los comandos. Necesitás saber qué querés hacer y dónde consultar cuando no recuerdes cómo hacerlo.**
