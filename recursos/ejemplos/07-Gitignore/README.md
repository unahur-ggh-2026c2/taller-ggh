# Ejemplo 07 — Gitignore

Ejemplo pequeño para observar cómo `.gitignore` evita incorporar archivos que no deberían formar parte del repositorio.

---

## Estructura

```text
07-Gitignore/
├── README.md
├── .gitignore
└── src/
    └── programa.py
```

---

## 1. Crear el repositorio

```bash
mkdir 07-Gitignore
cd 07-Gitignore
git init
```

---

## 2. Crear `.gitignore`

Crear:

```text
.gitignore
```

Contenido:

```gitignore
.env
__pycache__/
*.log
```

Estas reglas indican que Git debe ignorar:

```text
.env
directorios __pycache__
archivos .log
```

---

## 3. Crear archivos

Crear:

```text
src/programa.py
.env
registro.log
```

Por ejemplo:

```python
print("Hola, Git")
```

---

## 4. Revisar el estado

```bash
git status
```

Los archivos ignorados no deberían aparecer como archivos sin seguimiento.

El archivo `src/programa.py`, en cambio, sí debería aparecer.

---

## 5. Preparar y registrar

```bash
git add .
git commit -m "Agrega programa y configuración de Gitignore"
```

---

## 6. Verificar

```bash
git status
```

El repositorio debería quedar limpio.

---

## 7. Investigar un archivo ignorado

Para saber por qué un archivo está siendo ignorado:

```bash
git check-ignore -v .env
```

Git indicará la regla de `.gitignore` que se aplica.

---

## Importante

`.gitignore` evita que archivos no deseados sean incorporados al seguimiento.

No elimina archivos del disco.

Tampoco elimina automáticamente archivos que ya fueron registrados en commits anteriores.

---

## Resultado

```text
.gitignore
    ↓
define reglas
    ↓
Git ignora determinados archivos
    ↓
git add .
    ↓
solo se preparan los archivos correspondientes
```

> **`.gitignore` forma parte del repositorio y debe diseñarse como parte de la configuración del proyecto, no agregarse como un parche al final.**
