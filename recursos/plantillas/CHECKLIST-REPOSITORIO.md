# Checklist — Repositorio

> Revisión final antes de presentar, compartir o entregar un repositorio.

---

## Identidad y estructura

- [ ] El nombre del repositorio es claro.
- [ ] La descripción explica brevemente el propósito.
- [ ] La estructura de archivos es coherente.
- [ ] No hay archivos innecesarios.

---

## README

- [ ] Explica qué es el proyecto.
- [ ] Explica su objetivo.
- [ ] Indica las tecnologías principales.
- [ ] Indica los requisitos.
- [ ] Explica cómo instalarlo.
- [ ] Explica cómo utilizarlo.
- [ ] Los ejemplos funcionan.
- [ ] Los enlaces funcionan.
- [ ] La información está actualizada.

---

## Git

- [ ] El repositorio tiene una historia comprensible.
- [ ] Los commits tienen mensajes descriptivos.
- [ ] Los commits representan cambios coherentes.
- [ ] No hay información sensible en el historial.
- [ ] No quedaron cambios pendientes que deban registrarse.

Comprobar:

```bash
git status
git log --oneline --graph --all
```

---

## `.gitignore`

* [ ] Existe `.gitignore` cuando corresponde.
* [ ] Se excluyen archivos temporales.
* [ ] Se excluyen configuraciones locales.
* [ ] Se excluyen credenciales y secretos.
* [ ] No se están ignorando archivos necesarios para ejecutar el proyecto.

---

## GitHub

* [ ] El repositorio remoto es el correcto.
* [ ] La rama principal está actualizada.
* [ ] Las ramas de trabajo ya no necesarias fueron revisadas.
* [ ] Las Issues relevantes están identificadas.
* [ ] Las Pull Requests fueron revisadas.
* [ ] Los cambios pendientes fueron integrados cuando corresponde.

---

## Colaboración

* [ ] Las tareas están asociadas a Issues cuando corresponde.
* [ ] Las ramas tienen nombres claros.
* [ ] Las Pull Requests describen los cambios.
* [ ] Las revisiones fueron realizadas.
* [ ] Las observaciones fueron resueltas.
* [ ] Los conflictos fueron resueltos y probados.

---

## Seguridad

* [ ] No hay contraseñas.
* [ ] No hay tokens.
* [ ] No hay claves privadas.
* [ ] No hay credenciales.
* [ ] No hay datos personales o sensibles.
* [ ] Se revisó el historial si el repositorio tuvo información sensible anteriormente.

---

## Proyecto

* [ ] El proyecto funciona.
* [ ] La versión presentada corresponde al alcance definido.
* [ ] Las funcionalidades principales fueron probadas.
* [ ] Las instrucciones del README fueron verificadas desde cero.
* [ ] Las dependencias necesarias están documentadas.
* [ ] El estado del proyecto está indicado.

---

## Documentación adicional

Cuando corresponda:

* [ ] `CHANGELOG.md` actualizado.
* [ ] `CONTRIBUTING.md` actualizado.
* [ ] `CASO-DE-ESTUDIO.md` completo.
* [ ] Licencia indicada.
* [ ] Otros documentos relevantes actualizados.

---

## Presentación

* [ ] Los proyectos destacados están correctamente presentados.
* [ ] La información pública representa el estado actual del proyecto.
* [ ] Las capturas o evidencias son relevantes.
* [ ] Los enlaces externos funcionan.

---

## Revisión final

Ejecutar:

```bash
git status
```

El estado debe ser el esperado para la entrega.

Revisar el historial:

```bash
git log --oneline --graph --all
```

Comprobar el remoto:

```bash
git remote -v
```

---

## Resultado

```text
[ ] LISTO PARA PRESENTAR
[ ] REQUIERE CORRECCIONES
```

### Observaciones

* ...
* ...
* ...

---

> **La checklist no reemplaza una revisión: ayuda a no olvidar lo importante.**
