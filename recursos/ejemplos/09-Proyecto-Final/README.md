# Ejemplo 09 — Proyecto Final

Ejemplo de referencia para organizar un Proyecto Final utilizando Git y GitHub.

---

## Objetivo

Integrar en un único proyecto los principales elementos trabajados durante el curso:

```text
proyecto
  ↓
Issue
  ↓
rama
  ↓
commits
  ↓
push
  ↓
Pull Request
  ↓
revisión
  ↓
merge
  ↓
documentación
  ↓
presentación
```

---

## 1. Definir el proyecto

Ejemplo:

```text
Nombre:
Gestor de Tareas

Problema:
Necesidad de administrar tareas desde una aplicación sencilla.

Objetivo:
Permitir crear, consultar y completar tareas.

Tecnologías:
Python
Git
GitHub
```

---

## 2. Definir el alcance

### Versión mínima

```text
- Crear una tarea.
- Listar tareas.
- Marcar una tarea como completada.
```

### Fuera de alcance

```text
- Usuarios.
- Autenticación.
- Base de datos.
- Aplicación web.
```

El alcance evita que el proyecto crezca indefinidamente.

---

## 3. Crear el repositorio

Estructura inicial:

```text
gestor-de-tareas/
├── README.md
├── .gitignore
├── src/
│   └── tareas.py
└── CASO-DE-ESTUDIO.md
```

Inicializar:

```bash
git init
```

Primer commit:

```bash
git add .
git commit -m "Inicializa proyecto final"
```

---

## 4. Crear las Issues

Separar el trabajo en tareas:

```text
Issue #1
Crear estructura inicial

Issue #2
Implementar creación de tareas

Issue #3
Implementar listado de tareas

Issue #4
Implementar tareas completadas

Issue #5
Documentar proyecto
```

---

## 5. Desarrollar una tarea

Para la Issue #2:

```bash
git switch main
git pull
git switch -c feature-crear-tareas
```

Realizar el cambio y registrar:

```bash
git add .
git commit -m "Implementa creación de tareas"
```

Publicar:

```bash
git push -u origin feature-crear-tareas
```

---

## 6. Crear la Pull Request

Título:

```text
Implementa creación de tareas
```

Descripción:

```md
## Relacionado con

Issue #2

## Qué hice

Implementé la creación de nuevas tareas.

## Cómo lo probé

Probé la creación de varias tareas desde la aplicación.
```

---

## 7. Revisar

Comprobar:

```text
[ ] La funcionalidad cumple la Issue.
[ ] El código funciona.
[ ] El cambio está documentado cuando corresponde.
[ ] No hay archivos innecesarios.
[ ] No hay información sensible.
```

---

## 8. Integrar

Después de la revisión:

```text
Pull Request
     ↓
merge
     ↓
main
```

Actualizar:

```bash
git switch main
git pull
```

Repetir el proceso para las siguientes tareas.

---

## 9. Caso de estudio

Crear `CASO-DE-ESTUDIO.md`.

Estructura mínima:

```md
# Caso de Estudio

## Problema

...

## Objetivo

...

## Solución

...

## Tecnologías

...

## Decisiones

...

## Dificultades

...

## Resultado

...

## Aprendizajes

...

## Próximos pasos

...
```

---

## 10. Documentar el proyecto

El README final debe permitir que otra persona:

```text
entienda el proyecto
   ↓
instale lo necesario
   ↓
lo ejecute
   ↓
comprenda su funcionamiento
```

Probar las instrucciones siguiendo únicamente el README.

---

## 11. Revisar el historial

```bash
git log --oneline --graph --all
```

Buscar una historia comprensible:

```text
Inicializa proyecto final
Implementa creación de tareas
Implementa listado de tareas
Agrega tareas completadas
Documenta proyecto
```

---

## 12. Revisión final

Estado:

```bash
git status
```

Historial:

```bash
git log --oneline --graph --all
```

Remoto:

```bash
git remote -v
```

---

## 13. Checklist de entrega

```text
[ ] Proyecto terminado según el alcance.
[ ] Repositorio disponible.
[ ] README actualizado.
[ ] .gitignore revisado.
[ ] Sin información sensible.
[ ] Issues utilizadas para organizar tareas.
[ ] Ramas utilizadas.
[ ] Commits claros.
[ ] Pull Requests revisadas.
[ ] Cambios integrados.
[ ] Proyecto probado.
[ ] CASO-DE-ESTUDIO.md completo.
[ ] Presentación preparada.
```

---

## Resultado esperado

El repositorio debería permitir reconstruir el proceso:

```text
Problema
   ↓
Objetivo
   ↓
Issues
   ↓
Ramas
   ↓
Commits
   ↓
Pull Requests
   ↓
Revisión
   ↓
Merge
   ↓
Proyecto terminado
   ↓
Caso de estudio
```

La finalidad no es demostrar una cantidad determinada de comandos o commits.

El proyecto debe demostrar que Git y GitHub fueron utilizados como herramientas reales de trabajo.

> **El Proyecto Final cierra el recorrido del curso: no solamente muestra el resultado, sino también cómo se llegó hasta él.**
