# Práctica
## Módulo 02 — Guardar cambios

---

## 1. Objetivo

En esta práctica vamos a trabajar con el recorrido fundamental de un cambio en Git:

```text
Modificar
    ↓
Observar
    ↓
Preparar
    ↓
Registrar
    ↓
Observar nuevamente
```

La finalidad no es aprender una receta de comandos.

La finalidad es comprender qué ocurre con un cambio desde que modificamos un archivo hasta que queda registrado en el historial.

---

## 2. Preparar el repositorio

Utilizá el repositorio creado durante el módulo anterior.

Si no lo tenés disponible, creá uno nuevo llamado:

```text
laboratorio-cambios
```

Inicializalo con Git.

Creá un archivo:

```text
README.md
```

con:

```md
# Laboratorio de cambios

Este repositorio será utilizado para practicar el registro de cambios con Git.
```

Prepará el archivo y realizá un primer commit:

```bash
git add README.md
git commit -m "Crea documentación inicial"
```

Comprobá el estado:

```bash
git status
```

El repositorio debe encontrarse limpio antes de comenzar.

---

## 3. Realizar una modificación

Abrí:

```text
README.md
```

y agregá:

```md
## Objetivo

Aprender a registrar la evolución de un proyecto utilizando Git.
```

Guardá el archivo.

Ahora ejecutá:

```bash
git status
```

### Observá

Git debería informar que `README.md` fue modificado.

Antes de continuar, respondé:

> ¿El cambio ya forma parte del historial?

Todavía no.

---

## 4. Comprender qué ocurrió

Hasta este momento hicimos:

```text
README.md
    ↓
Modificar
    ↓
Guardar archivo
    ↓
git status
```

El archivo cambió en nuestra carpeta de trabajo.

Pero todavía no existe un nuevo commit.

Esta diferencia es fundamental:

```text
Guardar archivo
       ≠
Registrar cambio en Git
```

---

## 5. Preparar el cambio

Ahora ejecutá:

```bash
git add README.md
```

Después:

```bash
git status
```

Observá cuidadosamente la nueva información.

### Preguntas

1. ¿Qué cambió respecto del estado anterior?
2. ¿Dónde aparece ahora `README.md`?
3. ¿El cambio ya forma parte del historial?
4. ¿Qué significa que el cambio esté preparado?

No realices todavía el commit.

---

## 6. Registrar el cambio

Ahora ejecutá:

```bash
git commit -m "Agrega objetivo del laboratorio"
```

Después:

```bash
git status
```

Observá el resultado.

El repositorio debería volver a quedar limpio.

---

## 7. Reconstruir el recorrido

Completá:

```text
Modificar archivo
        ↓
        ?
        ↓
        ?
        ↓
Commit
```

Los dos pasos intermedios corresponden a operaciones que acabás de realizar.

Explicá con tus palabras qué ocurre en cada etapa.

---

## 8. Crear varios cambios

Ahora agregá al `README.md`:

```md
## Contenidos

- Repositorios
- Cambios
- Área de preparación
- Commits
```

Guardá el archivo.

Consultá:

```bash
git status
```

---

## 9. Preparar y observar

Prepará el cambio:

```bash
git add README.md
```

Antes de hacer el commit, ejecutá:

```bash
git status
```

Observá nuevamente el estado.

Ahora preguntate:

> ¿Qué información conoce Git que no conocía antes de ejecutar `git add`?

Escribí la respuesta en tus apuntes.

---

## 10. Registrar el segundo cambio

Realizá:

```bash
git commit -m "Agrega contenidos del laboratorio"
```

Después:

```bash
git status
```

El repositorio debería quedar limpio.

---

## 11. Trabajar con dos archivos

Creá:

```text
objetivos.md
```

con:

```md
# Objetivos

- Comprender el área de preparación.
- Crear commits significativos.
- Interpretar el estado del repositorio.
```

Y:

```text
notas.md
```

con:

```md
# Notas

Este archivo contiene observaciones sobre el trabajo realizado.
```

Ahora ejecutá:

```bash
git status
```

Git debería detectar ambos archivos como nuevos y sin seguimiento.

---

## 12. Preparar selectivamente

Esta vez no vamos a preparar los dos archivos.

Prepará solamente:

```bash
git add objetivos.md
```

Después:

```bash
git status
```

Observá la diferencia entre:

```text
objetivos.md
```

y:

```text
notas.md
```

### Pregunta

¿Por qué `notas.md` todavía no forma parte del próximo commit?

---

## 13. Crear un commit selectivo

Registrá el cambio preparado:

```bash
git commit -m "Agrega objetivos del laboratorio"
```

Ahora consultá:

```bash
git status
```

Debería quedar pendiente:

```text
notas.md
```

Esto demuestra que un commit no tiene por qué contener todos los cambios existentes en la carpeta de trabajo.

---

## 14. Registrar el cambio pendiente

Ahora prepará:

```bash
git add notas.md
```

Consultá:

```bash
git status
```

Después realizá:

```bash
git commit -m "Agrega notas del laboratorio"
```

Finalmente:

```bash
git status
```

El repositorio debería quedar limpio.

---

## 15. Modificar dos archivos

Ahora modificá:

```text
README.md
```

agregando:

```md
## Estado

El proyecto se encuentra en desarrollo.
```

Y modificá:

```text
objetivos.md
```

agregando:

```md
- Desarrollar hábitos de trabajo con Git.
```

Guardá ambos archivos.

Consultá:

```bash
git status
```

---

## 16. Registrar solamente uno

Prepará únicamente:

```bash
git add README.md
```

Consultá:

```bash
git status
```

Realizá el commit:

```bash
git commit -m "Agrega estado del proyecto"
```

Volvé a consultar:

```bash
git status
```

Ahora deberías observar que `objetivos.md` continúa modificado.

### Pregunta

¿Por qué?

Explicalo antes de continuar.

---

## 17. Registrar el cambio restante

Prepará:

```bash
git add objetivos.md
```

y registrá el cambio:

```bash
git commit -m "Amplia los objetivos del proyecto"
```

Consultá:

```bash
git status
```

El repositorio debería quedar limpio.

---

## 18. Observar el historial

Ahora tenemos varios commits.

Ejecutá:

```bash
git log
```

Observá la información disponible.

Después ejecutá:

```bash
git log --oneline
```

Compará ambas salidas.

Identificá:

- cantidad de commits;
- mensajes;
- autor;
- fechas;
- identificadores.

---

## 19. Leer la historia

Observá los mensajes que escribiste.

Deberían permitir reconstruir aproximadamente esta evolución:

```text
Crea documentación inicial
        ↓
Agrega objetivo del laboratorio
        ↓
Agrega contenidos del laboratorio
        ↓
Agrega objetivos del laboratorio
        ↓
Agrega notas del laboratorio
        ↓
Agrega estado del proyecto
        ↓
Amplia los objetivos del proyecto
```

Los nombres concretos dependerán de los mensajes que hayas utilizado.

### Pregunta

> ¿Una persona que no estuvo trabajando en el proyecto podría comprender su evolución leyendo solamente estos mensajes?

Si la respuesta es no, pensá qué podrías mejorar.

---

## 20. Una comparación

Imaginá dos historiales.

### Historial A

```text
cambios
cambios
update
arreglo
final
```

### Historial B

```text
Crea documentación inicial
Agrega objetivos del proyecto
Actualiza descripción
Corrige información de integrantes
Agrega instrucciones de uso
```

Respondé:

1. ¿Cuál resulta más útil?
2. ¿Por qué?
3. ¿Qué información debería transmitir un mensaje de commit?
4. ¿Qué problemas genera un historial poco descriptivo?

---

## 21. Guardar no es hacer commit

Realizá el siguiente experimento.

Modificá `README.md`.

Guardá el archivo con:

```text
Ctrl + S
```

No ejecutes ningún comando de Git.

Preguntate:

> ¿Existe ahora un nuevo commit?

Consultá:

```bash
git status
```

La respuesta debería resultar evidente.

---

## 22. Preparar no es hacer commit

Ahora ejecutá:

```bash
git add README.md
```

Consultá:

```bash
git status
```

Preguntate:

> ¿Existe ahora un nuevo commit?

Todavía no.

El cambio está preparado, pero todavía no está registrado en el historial.

---

## 23. Registrar el cambio

Ahora sí:

```bash
git commit -m "Actualiza documentación"
```

Consultá:

```bash
git status
```

Y después:

```bash
git log --oneline
```

Ahora deberías poder observar el nuevo commit.

---

## 24. El recorrido completo

Repetí mentalmente el recorrido:

```text
Modificar
   ↓
Guardar archivo
   ↓
git status
   ↓
git add
   ↓
git status
   ↓
git commit
   ↓
git status
   ↓
git log
```

No memorices la secuencia como una receta.

Intentá explicar qué problema resuelve cada paso.

---

## 25. Situación problemática

Supongamos que modificaste:

```text
README.md
objetivos.md
notas.md
```

y ejecutaste:

```bash
git add README.md
git add objetivos.md
git commit -m "Actualiza documentación"
```

Después ejecutaste:

```bash
git status
```

y `notas.md` continúa apareciendo como modificado.

### Pregunta

¿Git cometió un error?

Explicá por qué.

---

## 26. Segunda situación problemática

Supongamos que ejecutaste:

```bash
git add README.md
```

y después modificaste nuevamente `README.md`.

Ahora ejecutá:

```bash
git status
```

Observá qué informa Git.

### Pregunta

¿Por qué puede existir una diferencia entre lo que estaba preparado y el estado actual del archivo?

No intentes resolver todavía el problema.

Primero observá y explicá.

---

## 27. Crear un historial significativo

Realizá tres modificaciones diferentes sobre el proyecto.

Por ejemplo:

```text
1. Agregar una sección al README.
2. Ampliar los objetivos.
3. Agregar nuevas notas.
```

Registrá cada modificación en un commit separado.

Los mensajes deben describir claramente qué hiciste.

Después ejecutá:

```bash
git log --oneline
```

Analizá el resultado.

---

## 28. Estado final

Antes de terminar, ejecutá:

```bash
git status
```

El repositorio debe quedar limpio.

Después:

```bash
git log --oneline
```

Verificá que los commits estén registrados.

La estructura del proyecto debería ser similar a:

```text
laboratorio-cambios/
├── .git/
├── README.md
├── objetivos.md
└── notas.md
```

---

## 29. Reflexión final

Respondé:

### 1.

¿Qué diferencia existe entre guardar un archivo y registrar un cambio?

### 2.

¿Qué función cumple el área de preparación?

### 3.

¿Qué hace `git add`?

### 4.

¿Qué hace `git commit`?

### 5.

¿Por qué puede ser útil seleccionar qué cambios forman parte de cada commit?

### 6.

¿Qué información proporciona `git status`?

### 7.

¿Qué información proporciona `git log`?

### 8.

¿Qué características debería tener un buen mensaje de commit?

---

## 30. Cierre

Si podés realizar el siguiente recorrido y explicar qué ocurre en cada etapa:

```text
Modificar
   ↓
Observar
   ↓
Preparar
   ↓
Observar
   ↓
Registrar
   ↓
Observar
   ↓
Consultar historial
```

entonces ya incorporaste el núcleo del flujo de trabajo básico con Git.

En el próximo módulo vamos a concentrarnos específicamente en el **historial**, para aprender a leerlo, interpretarlo y utilizarlo para comprender cómo evolucionó un proyecto.