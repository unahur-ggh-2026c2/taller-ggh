# Ejemplo 02 — Historial

Ejemplo pequeño para observar cómo evoluciona un repositorio mediante varios commits.

---

## Estructura

```text
02-Historial/
├── README.md
└── notas.txt
```

---

## 1. Crear el proyecto

```bash
mkdir 02-Historial
cd 02-Historial
git init
```

---

## 2. Crear el primer estado

Crear `notas.txt`:

```text
Primera versión del archivo.
```

Registrar:

```bash
git add notas.txt
git commit -m "Agrega archivo de notas"
```

---

## 3. Crear un segundo estado

Modificar `notas.txt`:

```text
Primera versión del archivo.
Segunda versión del archivo.
```

Registrar:

```bash
git add notas.txt
git commit -m "Actualiza archivo de notas"
```

---

## 4. Crear un tercer estado

Modificar nuevamente `notas.txt`:

```text
Primera versión del archivo.
Segunda versión del archivo.
Tercera versión del archivo.
```

Registrar:

```bash
git add notas.txt
git commit -m "Agrega tercera versión de notas"
```

---

## 5. Consultar el historial

```bash
git log --oneline
```

Resultado esperado:

```text
<id> Agrega tercera versión de notas
<id> Actualiza archivo de notas
<id> Agrega archivo de notas
```

---

## 6. Ver el historial gráficamente

```bash
git log --oneline --graph --all
```

En este ejemplo no hay ramas, por lo que la historia será lineal:

```text
* <id> Agrega tercera versión de notas
* <id> Actualiza archivo de notas
* <id> Agrega archivo de notas
```

---

## 7. Ver un commit

Consultar el último:

```bash
git show HEAD
```

También podés indicar un commit específico:

```bash
git show <id>
```

---

## Resultado

El repositorio ahora tiene una historia de tres commits:

```text
estado 1
   ↓
estado 2
   ↓
estado 3
```

La finalidad del ejemplo es observar que Git conserva la evolución del proyecto, no solamente su estado actual.
