# Cheatsheet — Historial

> Referencia rápida para consultar y analizar la historia de un repositorio.

---

## Ver el historial

Historial completo:

```bash
git log
```

Historial resumido:

```bash id="7c8n2r"
git log --oneline
```

Historial con ramas:

```bash id="p3g8kx"
git log --oneline --graph --all
```

---

## Ver el último commit

```bash id="t7q4mz"
git log --oneline -1
```

Detalle:

```bash id="v9j2sf"
git show HEAD
```

---

## Ver un commit

Con su identificador:

```bash id="h5m3wd"
git show ID_DEL_COMMIT
```

Ejemplo:

```bash id="q1r8bc"
git show a81f3c2
```

---

## Entender el historial

Una vista especialmente útil:

```bash id="e6k4pn"
git log --oneline --graph --all
```

Permite observar:

```text
commits
ramas
ramificaciones
integraciones
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

## Historial de una rama

```bash id="n4w6hs"
git log --oneline nombre-de-la-rama
```

Ejemplo:

```bash id="k8m2vx"
git log --oneline feature-login
```

---

## Historial de un archivo

```bash id="r5t9cp"
git log --oneline -- README.md
```

Para ver también los cambios:

```bash id="f2x7qa"
git log -p -- README.md
```

Esto permite investigar cómo evolucionó un archivo.

---

## Buscar commits por mensaje

```bash id="m6z3yt"
git log --grep="texto"
```

Ejemplo:

```bash id="j9c4wb"
git log --oneline --grep="validación"
```

Útil en repositorios con muchos commits.

---

## Comparar ramas

Para consultar diferencias entre dos ramas:

```bash id="w3n8pk"
git diff main..feature-login
```

Esto muestra los cambios entre ambas referencias.

---

## Investigar una línea

```bash id="c6r2mv"
git blame archivo.txt
```

Permite identificar el commit asociado a cada línea.

Usalo para investigar la historia del código, no para buscar culpables.

---

## Investigar un problema

Cuando aparece un comportamiento inesperado:

```text
problema
   ↓
identificar archivo
   ↓
consultar historial
   ↓
identificar commit
   ↓
git show
   ↓
analizar cambio
```

Comandos útiles:

```bash id="f7k3sd"
git log --oneline -- archivo.txt
git show ID_DEL_COMMIT
```

---

## Historial y ramas

Conceptualmente:

```text
main
 |
 A
 |
 B
 |\
 | \
 |  C
 |  |
 |  D
 | /
 E
```

La historia permite reconstruir:

```text
qué se hizo
en qué rama
cómo evolucionó
cómo se integró
```

---

## Historial y Pull Requests

Una Pull Request puede contener varios commits:

```text
rama
 ↓
commit
 ↓
commit
 ↓
Pull Request
 ↓
revisión
 ↓
merge
```

El historial permite analizar la evolución del cambio antes de su integración.

---

## Historial útil

Ejemplo:

```text
Inicializa estructura del proyecto
Implementa búsqueda
Agrega validación
Corrige error de consulta
Documenta instalación
```

Permite reconstruir razonablemente la evolución.

---

## Historial poco útil

Ejemplo:

```text
cambios
fix
prueba
cosas
final
final2
```

El problema no es la cantidad de commits.

Es la dificultad para interpretar qué ocurrió.

---

## Antes de entregar

Ejecutá:

```bash id="u4p7mz"
git log --oneline --graph --all
```

Revisá:

```text
[ ] Los commits son comprensibles.
[ ] Las ramas tienen sentido.
[ ] Las integraciones son identificables.
[ ] La historia refleja el proceso real.
```

---

## Comandos esenciales

| Necesidad            | Comando                           |
| -------------------- | --------------------------------- |
| Historial            | `git log`                         |
| Historial resumido   | `git log --oneline`               |
| Historial gráfico    | `git log --oneline --graph --all` |
| Último commit        | `git log --oneline -1`            |
| Ver commit           | `git show ID`                     |
| Historial de archivo | `git log --oneline -- archivo`    |
| Cambios históricos   | `git log -p -- archivo`           |
| Buscar por mensaje   | `git log --grep="texto"`          |
| Comparar ramas       | `git diff rama1..rama2`           |
| Investigar líneas    | `git blame archivo`               |

---

## Regla práctica

```text
¿Qué pasó?
    ↓
git log

¿Qué cambió?
    ↓
git show

¿Cómo evolucionó este archivo?
    ↓
git log -- archivo

¿Cómo se relacionan las ramas?
    ↓
git log --oneline --graph --all
```

> **El historial no está solamente para mirar hacia atrás: también es una herramienta para entender, investigar y explicar el proyecto.**
