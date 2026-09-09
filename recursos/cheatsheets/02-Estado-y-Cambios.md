# Cheatsheet — Estado y Cambios

> Referencia rápida para saber qué cambió, qué está preparado y qué se va a registrar.

---

## Ver el estado

```bash
git status
```

Usalo para conocer:

* rama actual;
* archivos modificados;
* archivos nuevos;
* cambios preparados;
* archivos sin seguimiento.

> Si no sabés qué está pasando, empezá por `git status`.

---

## Ver cambios

Cambios todavía no preparados:

```bash
git diff
```

Cambios preparados para el próximo commit:

```bash
git diff --staged
```

Flujo recomendado:

```text
modificar
   ↓
git status
   ↓
git diff
   ↓
git add
   ↓
git diff --staged
   ↓
git commit
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

Todo:

```bash
git add .
```

> Antes de usar `git add .`, revisá que no estés incorporando archivos que no correspondan.

---

## Preparar parcialmente

Para seleccionar cambios específicos:

```bash
git add -p
```

Es útil cuando un mismo archivo contiene modificaciones pertenecientes a tareas diferentes.

---

## Quitar del área de preparación

Si hiciste:

```bash
git add archivo.txt
```

y querés dejarlo fuera del próximo commit:

```bash
git restore --staged archivo.txt
```

El archivo sigue modificado.

```text
preparado
   ↓
git restore --staged
   ↓
modificado
```

---

## Descartar un cambio local

```bash
git restore archivo.txt
```

⚠️ Descarta modificaciones no registradas del archivo.

Antes:

```bash
git diff
```

---

## Archivos sin seguimiento

Si creás un archivo nuevo:

```text
notas.txt
```

consultá:

```bash
git status
```

Para incorporarlo:

```bash
git add notas.txt
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

Sirve para indicar archivos o directorios que no deberían formar parte del seguimiento.

> `.gitignore` no elimina automáticamente archivos que ya fueron registrados.

---

## ¿Por qué un archivo está ignorado?

```bash
git check-ignore -v archivo.txt
```

Permite identificar la regla que está provocando la exclusión.

---

## Verificar antes del commit

```bash
git status
git diff
git add .
git diff --staged
```

Comprobá:

```text
[ ] Cambios correctos
[ ] Archivos correctos
[ ] Sin secretos
[ ] Sin archivos innecesarios
[ ] Cambios coherentes
```

---

## Después del commit

```bash
git status
```

Para consultar el último commit:

```bash
git log --oneline -1
```

---

## Comandos esenciales

| Necesidad              | Comando                        |
| ---------------------- | ------------------------------ |
| Ver estado             | `git status`                   |
| Ver cambios            | `git diff`                     |
| Ver cambios preparados | `git diff --staged`            |
| Preparar archivo       | `git add archivo`              |
| Preparar todo          | `git add .`                    |
| Preparar parcialmente  | `git add -p`                   |
| Quitar preparación     | `git restore --staged archivo` |
| Descartar cambio local | `git restore archivo`          |
| Revisar `.gitignore`   | `git check-ignore -v archivo`  |

---

## Regla práctica

Antes de registrar:

```text
status
  ↓
diff
  ↓
add
  ↓
diff --staged
  ↓
commit
```

> **No alcanza con saber que modificaste algo. Tenés que saber exactamente qué estás a punto de registrar.**
