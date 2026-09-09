# Ejemplo 04 — Pull Request

Ejemplo del flujo básico para publicar una rama y proponer sus cambios mediante una Pull Request.

---

## Objetivo

Mostrar este recorrido:

```text
rama
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

## 1. Partir de un repositorio

Este ejemplo supone que ya existe un repositorio en GitHub.

Clonarlo:

```bash
git clone URL_DEL_REPOSITORIO
cd NOMBRE_DEL_REPOSITORIO
```

Comprobar:

```bash
git status
```

---

## 2. Actualizar `main`

```bash
git switch main
git pull
```

---

## 3. Crear una rama

```bash
git switch -c feature-readme
```

---

## 4. Realizar el cambio

Modificar `README.md`.

Por ejemplo, agregar una sección:

```md
## Características

- Gestión de tareas.
- Registro de cambios.
```

Revisar:

```bash
git status
git diff
```

---

## 5. Crear el commit

```bash
git add README.md
git commit -m "Agrega características al README"
```

---

## 6. Publicar la rama

```bash
git push -u origin feature-readme
```

La rama ahora está disponible en GitHub.

---

## 7. Crear la Pull Request

En GitHub:

```text
feature-readme
      ↓
Pull Request
      ↓
main
```

La descripción puede seguir esta estructura:

```md
## Qué hice

Agregué la sección de características al README.

## Por qué

El proyecto necesitaba documentar sus funcionalidades principales.

## Cómo lo probé

Revisé el README y verifiqué los enlaces existentes.
```

---

## 8. Revisar

Antes de integrar, comprobar:

```text
[ ] El cambio resuelve la tarea.
[ ] La documentación es correcta.
[ ] No hay cambios innecesarios.
[ ] La descripción de la Pull Request es clara.
```

---

## 9. Integrar

Una vez aprobada la Pull Request:

```text
Pull Request
     ↓
Merge
     ↓
main
```

La integración se realiza desde GitHub.

---

## 10. Actualizar el repositorio local

Después del merge:

```bash
git switch main
git pull
```

Comprobar:

```bash
git status
```

---

## Resultado

El flujo completo fue:

```text
Issue
  ↓
feature-readme
  ↓
cambio
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
  ↓
main
```

La Pull Request permitió proponer y revisar el cambio antes de integrarlo en `main`.
