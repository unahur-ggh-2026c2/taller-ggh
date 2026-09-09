# Proyecto
## Módulo 02 — Guardar cambios

---

## 1. Propósito

En este proyecto vas a construir la evolución de un pequeño proyecto documental utilizando Git.

La actividad integra los conceptos centrales del módulo:

- modificación de archivos;
- consulta del estado;
- área de preparación;
- selección de cambios;
- commits;
- mensajes descriptivos;
- historial;
- repositorio limpio.

El objetivo no es producir una aplicación.

El objetivo es construir un **historial de cambios coherente y comprensible**.

---

## 2. El proyecto

Creá un repositorio llamado:

```text
proyecto-documental
```

El tema puede ser elegido libremente.

Algunas posibilidades:

- una aplicación ficticia;
- un proyecto académico;
- una herramienta informática;
- una biblioteca;
- un juego;
- una organización;
- una idea de emprendimiento.

El proyecto deberá contener inicialmente:

```text
proyecto-documental/
├── README.md
├── objetivos.md
└── notas.md
```

---

## 3. Primera versión

### `README.md`

Debe contener:

```md
# Nombre del proyecto

Descripción breve del proyecto.

## Propósito

Explicación del propósito general.
```

### `objetivos.md`

Debe contener:

```md
# Objetivos

- Objetivo 1
- Objetivo 2
- Objetivo 3
```

### `notas.md`

Debe contener:

```md
# Notas

Notas iniciales del proyecto.
```

El contenido concreto debe ser desarrollado por vos.

---

## 4. Crear el primer commit

Inicializá el repositorio.

Consultá el estado:

```bash
git status
```

Prepará los archivos necesarios y realizá un primer commit.

El mensaje debe describir correctamente lo que estás registrando.

Por ejemplo:

```bash
git commit -m "Crea documentación inicial del proyecto"
```

No es obligatorio utilizar exactamente ese mensaje.

---

## 5. Primera evolución

Ahora ampliá el proyecto.

Modificá `README.md` incorporando una sección:

```md
## Características

Descripción de las principales características del proyecto.
```

Modificá también `objetivos.md` agregando al menos un nuevo objetivo.

Consultá:

```bash
git status
```

Analizá los cambios antes de prepararlos.

---

## 6. Segundo commit

Decidí si los cambios realizados deberían formar parte del mismo commit.

En este caso representan una misma evolución documental, por lo que pueden registrarse juntos.

Prepará los cambios y realizá un segundo commit.

El mensaje debe expresar la intención del cambio.

Por ejemplo:

```text
Amplia descripción y objetivos del proyecto
```

Después:

```bash
git status
```

El repositorio debería quedar limpio.

---

## 7. Segunda evolución

Ahora modificá solamente:

```text
notas.md
```

Agregá información relacionada con el desarrollo del proyecto.

Por ejemplo:

```md
## Decisiones

- Decisión 1
- Decisión 2
```

Consultá:

```bash
git status
```

Prepará el cambio y realizá un nuevo commit.

El mensaje debe describir qué incorporaste.

---

## 8. Cambios simultáneos

Ahora realizá modificaciones independientes en:

```text
README.md
objetivos.md
notas.md
```

Los cambios deben representar tres intenciones diferentes.

Por ejemplo:

```text
README.md
    Corrección de una descripción.

objetivos.md
    Incorporación de un objetivo.

notas.md
    Nueva decisión del proyecto.
```

No hagas ningún commit todavía.

Consultá:

```bash
git status
```

---

## 9. Seleccionar los cambios

Ahora vas a tomar una decisión.

El próximo commit deberá contener solamente:

```text
README.md
```

Prepará ese archivo.

Consultá:

```bash
git status
```

Verificá que los otros dos cambios continúen pendientes.

---

## 10. Registrar el cambio seleccionado

Realizá un commit que describa la modificación realizada en `README.md`.

Por ejemplo:

```bash
git commit -m "Corrige descripción del proyecto"
```

Después:

```bash
git status
```

Deberían continuar pendientes los cambios de:

```text
objetivos.md
notas.md
```

---

## 11. Segundo cambio pendiente

Ahora prepará únicamente:

```text
objetivos.md
```

Consultá nuevamente:

```bash
git status
```

Realizá un commit descriptivo.

Después:

```bash
git status
```

Debería quedar pendiente solamente:

```text
notas.md
```

---

## 12. Registrar el último cambio

Prepará:

```text
notas.md
```

y realizá un nuevo commit.

Después:

```bash
git status
```

El repositorio debe quedar limpio.

---

## 13. Construir una historia

Ahora consultá:

```bash
git log --oneline
```

Observá todos los commits realizados.

Tu historial debería representar aproximadamente una evolución como:

```text
Documentación inicial
        ↓
Ampliación del proyecto
        ↓
Agrega decisiones
        ↓
Corrige descripción
        ↓
Actualiza objetivos
        ↓
Agrega nueva nota
```

Los mensajes concretos dependerán de tus decisiones.

---

## 14. Evaluar el historial

Ahora leé tu historial como si fueras una persona que nunca trabajó en el proyecto.

Preguntate:

- ¿qué ocurrió primero?
- ¿qué cambios se realizaron después?
- ¿qué modificaciones fueron independientes?
- ¿los mensajes permiten comprender las intenciones?
- ¿hay commits demasiado generales?
- ¿hay mensajes que no aportan información?

Registrá tus observaciones en:

```text
evaluacion-historial.md
```

---

## 15. Mejorar el proyecto

Realizá ahora una modificación que consideres necesaria para mejorar la documentación.

Antes de hacer nada:

```bash
git status
```

Después:

1. modificá;
2. observá;
3. prepará;
4. registrá;
5. verificá.

El mensaje del commit debe ser específico.

---

## 16. Simular una tarea real

Imaginá que recibís esta tarea:

> "Actualizar la descripción del proyecto y agregar información sobre sus objetivos."

Realizá las modificaciones necesarias.

Consultá el estado.

Decidí qué cambios forman parte de la tarea.

Preparalos.

Creá un commit que represente esa tarea.

Después comprobá:

```bash
git status
```

y:

```bash
git log --oneline
```

---

## 17. Simular una segunda tarea

Ahora imaginá:

> "Agregar una nueva decisión de diseño al proyecto."

Modificá solamente `notas.md`.

Registrá la tarea en un nuevo commit.

El historial debería permitir distinguir esta tarea de la anterior.

---

## 18. Verificación del estado

Antes de finalizar, ejecutá:

```bash
git status
```

El repositorio debe quedar limpio.

Si no está limpio, no continúes.

Primero determiná:

- qué archivo cambió;
- por qué cambió;
- si el cambio debe registrarse;
- si debe formar parte de un commit nuevo.

---

## 19. Verificación del historial

Ejecutá:

```bash
git log --oneline
```

Comprobá que:

- existan varios commits;
- los mensajes sean descriptivos;
- los commits representen cambios concretos;
- el orden permita comprender la evolución.

---

## 20. Producto final

El proyecto debe contener como mínimo:

```text
proyecto-documental/
├── .git/
├── README.md
├── objetivos.md
├── notas.md
└── evaluacion-historial.md
```

Además, deberá contar con un historial compuesto por varios commits significativos.

No se evalúa la cantidad de commits por sí misma.

Se evalúa que representen una evolución coherente.

---

## 21. Reflexión final

Completá `evaluacion-historial.md`:

```md
# Evaluación del historial

## ¿Qué aprendí sobre el registro de cambios?

...

## ¿Qué diferencia existe entre guardar un archivo y registrar un cambio?

...

## ¿Qué función cumple el área de preparación?

...

## ¿Por qué decidí separar algunos cambios en diferentes commits?

...

## ¿Qué características tienen mis mensajes de commit?

...

## ¿Qué podría mejorar de mi historial?

...

## ¿Qué parte del proceso todavía necesito practicar?

...
```

Las respuestas deben reflejar tu experiencia durante el proyecto.

---

## 22. Criterios de finalización

El proyecto se considera completo cuando:

- existe un repositorio correctamente inicializado;
- contiene documentación propia;
- existen varios commits;
- los commits representan cambios concretos;
- los mensajes son descriptivos;
- se practicó la selección de cambios;
- se realizaron commits independientes;
- se consultó el estado durante el proceso;
- se consultó el historial;
- el repositorio termina limpio;
- la reflexión final está completa.

---

## 23. Pregunta final

Sin consultar documentación, respondé:

> **Si modifico cinco archivos, ¿estoy obligado a incluir los cinco en el próximo commit?**

Después explicá:

> **¿Por qué puede ser útil decidir qué cambios forman parte de cada commit?**

Finalmente:

> **¿Qué características debería tener un historial para resultar útil a otra persona que se incorpora al proyecto?**

Si podés responder estas preguntas y demostrarlo mediante tu repositorio, completaste el objetivo principal del módulo.