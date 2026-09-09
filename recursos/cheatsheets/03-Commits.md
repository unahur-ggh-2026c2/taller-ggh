# Cheatsheet — Commits

> Referencia rápida para crear commits claros y útiles.

---

## Crear un commit

Preparar cambios:

```bash
git add archivo.txt
```

Registrar:

```bash
git commit -m "Agrega validación de entrada"
```

---

## Flujo recomendado

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

## Mensajes de commit

### Preferir

```text
Agrega validación de entrada
Corrige cálculo de totales
Implementa búsqueda de usuarios
Actualiza documentación de instalación
```

### Evitar

```text
cambios
fix
cosas
prueba
final
final2
ahora sí
```

La pregunta práctica es:

> ¿El mensaje permite entender qué cambio se registró?

---

## Unidad de trabajo

Un commit debería representar un cambio coherente.

### Bien

```text
Agrega validación de usuarios
```

### Puede ser demasiado amplio

```text
Agrega validación, cambia README, corrige
otro error y reorganiza todo el proyecto
```

### Puede ser demasiado artificial

```text
Agrega una línea
Agrega otra línea
Cambia una palabra
```

No existe una cantidad universal de commits correcta.

> **Buscá commits comprensibles, no una cantidad determinada.**

---

## Ver commits

Historial resumido:

```bash
git log --oneline
```

Último commit:

```bash
git log --oneline -1
```

Ver un commit:

```bash
git show HEAD
```

Ver un commit específico:

```bash
git show ID_DEL_COMMIT
```

---

## Revisar antes de confirmar

Estado:

```bash
git status
```

Cambios no preparados:

```bash
git diff
```

Cambios preparados:

```bash
git diff --staged
```

Después:

```bash
git commit -m "Describe el cambio"
```

---

## Commit y área de preparación

Recordá:

```text
git add
   ↓
prepara cambios
```

```text
git commit
   ↓
registra cambios preparados
```

Por eso un cambio modificado pero no preparado no forma parte del commit.

---

## Verificar después

```bash
git status
```

Y:

```bash
git log --oneline -1
```

Para revisar exactamente qué registraste:

```bash
git show HEAD
```

---

## Commits y ramas

Una rama contiene una línea de desarrollo formada por commits.

```text
main
 |
 A
 |
 B
 |\
 | \
 C  D
    |
    E
```

Los commits permiten reconstruir cómo evolucionó cada línea de trabajo.

---

## Commit y Pull Request

No son lo mismo:

| Elemento     | Función                                                |
| ------------ | ------------------------------------------------------ |
| Commit       | Registra un cambio                                     |
| Pull Request | Propone y permite revisar cambios antes de integrarlos |

Una Pull Request puede contener uno o varios commits.

---

## Commit y Issue

Flujo habitual:

```text
Issue
  ↓
tarea
  ↓
rama
  ↓
commits
  ↓
Pull Request
  ↓
revisión
  ↓
merge
```

La Issue representa el trabajo que debe realizarse.

Los commits registran cómo se realizó.

---

## Después de una revisión

Si una Pull Request recibe una observación:

```text
revisión
   ↓
corrección
   ↓
nuevo commit
   ↓
push
```

Ejemplo:

```bash
git add .
git commit -m "Corrige validación solicitada en revisión"
git push
```

---

## Historial como evidencia

Un buen historial puede mostrar:

```text
qué se hizo
cuándo
qué se corrigió
cómo evolucionó el proyecto
```

Debe complementarse con:

```text
Issues
Pull Requests
código
documentación
```

No alcanza con contar commits.

---

## Checklist

Antes de crear un commit:

```text
[ ] Revisé git status.
[ ] Revisé git diff.
[ ] Preparé solamente lo necesario.
[ ] Revisé git diff --staged.
[ ] No incluí información sensible.
[ ] El cambio representa una unidad coherente.
[ ] El mensaje describe el cambio.
```

---

## Comandos esenciales

| Necesidad      | Comando                   |
| -------------- | ------------------------- |
| Estado         | `git status`              |
| Ver cambios    | `git diff`                |
| Preparar       | `git add`                 |
| Ver preparados | `git diff --staged`       |
| Crear commit   | `git commit -m "mensaje"` |
| Historial      | `git log --oneline`       |
| Último commit  | `git log --oneline -1`    |
| Ver commit     | `git show HEAD`           |

> **Un commit útil deja una pista clara sobre la evolución del proyecto.**

