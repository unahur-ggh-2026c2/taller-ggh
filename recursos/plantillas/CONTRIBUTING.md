# Contribuir al proyecto

Gracias por tu interés en contribuir a este proyecto.

Este documento describe las pautas básicas para proponer cambios y colaborar de manera ordenada.

---

## Antes de comenzar

Revisá:

- el `README.md`;
- las Issues abiertas;
- las Pull Requests existentes;
- las pautas específicas del proyecto.

Si no encontrás una Issue relacionada con tu propuesta, evaluá crear una antes de comenzar el desarrollo.

---

## Flujo de trabajo

Para una nueva tarea:

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

Evitá realizar cambios directamente sobre `main` cuando el proyecto utilice este flujo.

---

## Crear una rama

Partir de una versión actualizada de `main`:

```bash
git switch main
git pull
```

Crear una rama descriptiva:

```bash
git switch -c feature-nombre
```

Ejemplos:

```text
feature-busqueda
feature-exportacion
fix-validacion
docs-readme
```

---

## Commits

Los commits deberían representar cambios coherentes.

Preferir mensajes descriptivos:

```text
Agrega búsqueda de usuarios
Corrige validación de entrada
Actualiza documentación de instalación
```

Evitar mensajes ambiguos:

```text
cambios
fix
cosas
final
```

---

## Pull Requests

La Pull Request debería explicar:

```text
qué cambió
por qué
cómo fue probado
```

Antes de crearla:

* revisar los propios cambios;
* comprobar que el proyecto funciona;
* verificar que no haya información sensible;
* actualizar la documentación cuando corresponda.

---

## Revisión

Las Pull Requests pueden recibir comentarios y solicitudes de cambios.

El feedback debería ser:

* claro;
* respetuoso;
* relacionado con el cambio;
* orientado a mejorar el proyecto.

Las observaciones deben revisarse y resolverse antes de integrar el cambio cuando corresponda.

---

## Pruebas

Antes de solicitar la integración:

```text
[ ] El proyecto funciona.
[ ] Las funcionalidades modificadas fueron probadas.
[ ] No se introdujeron errores conocidos.
[ ] La documentación corresponde al comportamiento actual.
```

Indicar en la Pull Request cómo se realizaron las pruebas.

---

## Documentación

Si un cambio modifica:

* instalación;
* uso;
* comportamiento;
* configuración;
* estructura;

actualizá la documentación correspondiente.

---

## Código

Mantener el estilo y la organización utilizados por el proyecto.

Antes de introducir cambios importantes:

```text
comprender
   ↓
proponer
   ↓
implementar
   ↓
probar
   ↓
documentar
```

Evitá cambios que no estén relacionados con la tarea.

---

## Información sensible

No incorporar al repositorio:

```text
contraseñas
tokens
claves
credenciales
datos sensibles
archivos de configuración privados
```

Revisá `.gitignore` antes de publicar cambios.

---

## Reportar problemas

Para informar un problema, utilizar una Issue cuando el proyecto disponga de este mecanismo.

Incluir:

```text
qué ocurrió
qué se esperaba
cómo reproducirlo
```

Ejemplo:

```md
## Problema

La aplicación no permite guardar una tarea vacía.

## Resultado esperado

Debe mostrar un mensaje indicando que la tarea es obligatoria.

## Pasos para reproducir

1. Ejecutar la aplicación.
2. Seleccionar "Nueva tarea".
3. Dejar el campo vacío.
4. Confirmar.
```

---

## Código de conducta

Si el proyecto cuenta con un `CODE_OF_CONDUCT.md`, todas las contribuciones deben respetar sus pautas.

Mantener siempre una comunicación respetuosa y profesional.

---

## Licencia

Las contribuciones realizadas al proyecto quedan sujetas a la licencia indicada en el repositorio.

Consultar el archivo `LICENSE` cuando corresponda.

---

## Resumen

```text
1. Revisar la Issue.
2. Actualizar main.
3. Crear una rama.
4. Realizar cambios.
5. Probar.
6. Crear commits claros.
7. Publicar la rama.
8. Crear Pull Request.
9. Atender la revisión.
10. Integrar.
```

---

> **Contribuir no es solamente modificar código: es hacer que el cambio pueda comprenderse, revisarse y mantenerse.**

