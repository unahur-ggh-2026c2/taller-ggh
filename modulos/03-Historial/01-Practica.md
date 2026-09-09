# Práctica
## Módulo 03 — Historial

---

## 1. Objetivo

En esta práctica vamos a aprender a consultar y leer el historial de un repositorio Git.

Hasta ahora aprendimos a crear commits.

Ahora vamos a observar esos registros y utilizarlos para comprender la evolución del proyecto.

El recorrido será:

```text
Crear commits
     ↓
Consultar historial
     ↓
Identificar commits
     ↓
Interpretar información
     ↓
Reconstruir evolución
```

---

## 2. Preparar el repositorio

Utilizá el repositorio desarrollado durante el módulo anterior.

Si no lo tenés disponible, creá uno nuevo llamado:

```text
laboratorio-historial
```

Inicializalo con Git.

Creá:

```text
README.md
```

con:

```md
# Laboratorio de historial

Este repositorio será utilizado para practicar la consulta
y análisis del historial de Git.
```

Realizá un primer commit:

```bash
git add README.md
git commit -m "Crea documentación inicial"
```

---

## 3. Construir una historia

Ahora vamos a generar varios cambios.

Modificá `README.md` agregando:

```md
## Propósito

Aprender a consultar y comprender el historial de un repositorio.
```

Registrá el cambio:

```bash
git add README.md
git commit -m "Agrega propósito del laboratorio"
```

---

## 4. Segundo cambio

Agregá:

```md
## Contenidos

- Commits
- Historial
- Identificación de cambios
```

Registrá:

```bash
git add README.md
git commit -m "Agrega contenidos del laboratorio"
```

---

## 5. Tercer cambio

Agregá:

```md
## Estado

El laboratorio se encuentra en desarrollo.
```

Registrá:

```bash
git add README.md
git commit -m "Agrega estado del laboratorio"
```

---

## 6. Cuarto cambio

Corregí o modificá alguna parte del contenido.

La modificación debe ser concreta.

Después registrala mediante un nuevo commit.

Elegí un mensaje que permita comprender qué modificaste.

Por ejemplo:

```text
Corrige descripción del laboratorio
```

---

## 7. Consultar el historial

Ahora ejecutá:

```bash
git log
```

No ejecutes todavía ningún otro comando.

Observá cuidadosamente la información.

Intentá identificar:

- commit;
- autor;
- fecha;
- mensaje;
- identificador.

---

## 8. Leer la salida

Tomá uno de los commits mostrados por Git.

Identificá:

```text
commit:
Author:
Date:
mensaje:
```

Respondé:

1. ¿Qué información representa cada elemento?
2. ¿Cuál permite identificar el commit?
3. ¿Cuál indica quién realizó el registro?
4. ¿Cuál indica cuándo fue realizado?
5. ¿Cuál describe la intención del cambio?

---

## 9. Observar el orden

Mirando la salida de:

```bash
git log
```

respondé:

1. ¿Qué commit aparece primero?
2. ¿Es el más antiguo o el más reciente?
3. ¿Qué relación existe entre los commits mostrados?
4. ¿Podés reconstruir el orden en el que fueron realizados?

Explicalo con tus palabras.

---

## 10. Vista resumida

Ahora ejecutá:

```bash
git log --oneline
```

Compará el resultado con:

```bash
git log
```

Respondé:

1. ¿Qué información desapareció?
2. ¿Qué información se mantiene?
3. ¿Qué ventaja tiene esta representación?
4. ¿En qué situación preferirías utilizarla?

---

## 11. Identificar commits

En la salida de:

```bash
git log --oneline
```

deberías observar algo similar a:

```text
a84f9c2 Agrega estado del laboratorio
b71d4e8 Agrega contenidos del laboratorio
c92ab31 Agrega propósito del laboratorio
f10c842 Crea documentación inicial
```

Los identificadores serán diferentes en tu repositorio.

Identificá:

- el commit más reciente;
- el commit inicial;
- el commit correspondiente a la incorporación de contenidos.

---

## 12. El identificador

Elegí uno de tus commits y observá su identificador.

Por ejemplo:

```text
a84f9c2
```

Respondé:

1. ¿Es una numeración secuencial?
2. ¿Permite identificar un commit?
3. ¿Es igual al identificador de otro commit?
4. ¿Por qué resulta útil disponer de un identificador?

No es necesario investigar todavía cómo se genera internamente.

---

## 13. Leer la historia

A partir de:

```bash
git log --oneline
```

intentá reconstruir la evolución del proyecto.

Escribila en lenguaje natural.

Por ejemplo:

```text
Primero se creó la documentación inicial.
Después se agregó el propósito.
Luego se incorporaron los contenidos.
Finalmente se agregó información sobre el estado.
```

No copies este ejemplo.

Construí la historia de tu propio repositorio.

---

## 14. La importancia de los mensajes

Ahora analizá tus propios mensajes.

Respondé:

> ¿Podrías comprender la evolución del proyecto si solamente tuvieras los mensajes de los commits?

Si la respuesta es negativa, identificá cuáles mensajes podrían mejorar.

No modifiques todavía el historial.

El objetivo es aprender a evaluarlo.

---

## 15. Comparar dos historiales

Observá:

### Historial A

```text
cambios
update
arreglo
cosas
final
```

### Historial B

```text
Crea documentación inicial
Agrega propósito del proyecto
Actualiza objetivos
Corrige descripción
Agrega instrucciones
```

Respondé:

1. ¿Cuál permite reconstruir mejor la evolución?
2. ¿Qué información aporta el segundo?
3. ¿Qué problemas presenta el primero?
4. ¿Por qué los mensajes forman parte de la calidad del historial?

---

## 16. El historial como evidencia

Imaginá que alguien afirma:

> "La documentación siempre tuvo esta estructura."

Tenés un historial con varios commits.

### Pregunta

¿El historial puede ayudarte a investigar esa afirmación?

Explicá qué información podrías buscar y qué información todavía necesitarías consultar.

---

## 17. Una modificación más

Realizá una nueva modificación significativa en `README.md`.

Registrala mediante un commit descriptivo.

Por ejemplo:

```text
Agrega instrucciones de uso
```

Después ejecutá:

```bash
git log --oneline
```

Observá cómo cambió la historia.

---

## 18. Comparar antes y después

Recordá cómo se veía el historial antes del último commit.

Ahora observá nuevamente:

```bash
git log --oneline
```

Respondé:

1. ¿Qué elemento nuevo apareció?
2. ¿Dónde aparece?
3. ¿Qué información conserva respecto de los commits anteriores?
4. ¿Qué relación tiene con el commit anterior?

---

## 19. Crear una historia deliberada

Ahora creá una segunda rama de documentación dentro del mismo proyecto conceptual, sin utilizar todavía ramas de Git.

Simplemente agregá contenido relacionado con:

```text
Descripción
Objetivos
Características
Estado
Notas
```

Realizá varias modificaciones pequeñas.

Registrá cada una en commits separados.

Los mensajes deben permitir reconstruir la evolución.

Después:

```bash
git log --oneline
```

Leé tu propia historia.

---

## 20. Analizar el resultado

Respondé:

### ¿Qué ocurrió primero?

...

### ¿Qué ocurrió después?

...

### ¿Qué commit representa la incorporación de una nueva característica?

...

### ¿Qué commit representa una corrección?

...

### ¿Cuál es el commit más reciente?

...

### ¿Cuál es el commit inicial?

...

---

## 21. Diferenciar estado actual e historial

Partí de un repositorio limpio.

Después modificá `README.md`, pero no hagas commit.

Ejecutá:

```bash
git status
```

y:

```bash
git log --oneline
```

Compará ambas salidas.

Respondé:

> ¿Qué información muestra `git status` que todavía no aparece en el historial?

Y:

> ¿Qué información muestra `git log` que no proporciona `git status`?

Esta diferencia es fundamental.

---

## 22. El pasado y el presente

Podemos pensar:

```text
git status
    ↓
¿Qué está ocurriendo ahora?

git log
    ↓
¿Qué quedó registrado antes?
```

Explicá con tus palabras esta diferencia.

---

## 23. Limpiar el repositorio

Registrá el cambio pendiente mediante un commit.

Después ejecutá:

```bash
git status
```

El repositorio debería quedar limpio.

Finalmente:

```bash
git log --oneline
```

Observá nuevamente la historia.

---

## 24. Construir un historial útil

Ahora realizá al menos cinco commits adicionales.

Cada uno debe representar una modificación concreta.

Evitá mensajes genéricos.

Al finalizar deberías tener una secuencia similar a:

```text
Commit 1 — documentación inicial
Commit 2 — descripción
Commit 3 — objetivos
Commit 4 — características
Commit 5 — corrección
Commit 6 — instrucciones
...
```

Los mensajes concretos deben surgir de tus propios cambios.

---

## 25. Leer como otra persona

Imaginá que mañana otra persona recibe tu repositorio.

No puede preguntarte qué ocurrió.

Solamente puede consultar:

```bash
git log --oneline
```

Leé tu historial desde esa perspectiva.

Respondé:

1. ¿Puede comprender la evolución?
2. ¿Hay mensajes ambiguos?
3. ¿Hay commits demasiado generales?
4. ¿Los cambios parecen seguir una lógica?
5. ¿Qué mejorarías?

---

## 26. Investigar un momento concreto

Elegí un commit intermedio de tu historial.

Anotá su identificador.

Por ejemplo:

```text
a84f9c2
```

Respondé:

- ¿qué mensaje tiene?
- ¿qué lugar ocupa en la historia?
- ¿qué ocurrió antes?
- ¿qué ocurrió después?

Todavía no necesitamos modificar ni recuperar nada.

El objetivo es aprender a identificar un punto concreto de la historia.

---

## 27. El historial como mapa

Pensá el historial como un mapa temporal:

```text
Pasado
  │
  ▼
Commit 1
  │
  ▼
Commit 2
  │
  ▼
Commit 3
  │
  ▼
Commit 4
  │
  ▼
Presente
```

Explicá:

> ¿Qué información aporta este mapa?

Y:

> ¿Qué información necesitaríamos para saber exactamente qué cambió entre dos puntos?

La segunda pregunta será importante en actividades posteriores.

---

## 28. Comprobación práctica

Sin consultar las prácticas anteriores, ejecutá:

```bash
git log
```

y:

```bash
git log --oneline
```

Después identificá:

- el commit más reciente;
- el commit inicial;
- un commit intermedio;
- el identificador de ese commit;
- su autor;
- su fecha;
- su mensaje.

Si podés realizarlo sin asistencia, ya estás utilizando el historial de manera autónoma.

---

## 29. Reflexión final

Respondé:

### 1.

¿Qué información contiene un commit?

### 2.

¿Qué diferencia existe entre `git log` y `git log --oneline`?

### 3.

¿Qué función cumple el identificador de un commit?

### 4.

¿Por qué los mensajes son importantes para el historial?

### 5.

¿Qué diferencia existe entre el estado actual y el historial registrado?

### 6.

¿Cómo puede ayudarnos el historial a investigar un problema?

### 7.

¿Qué información podemos obtener del historial y cuál necesitamos buscar en otros lugares?

---

## 30. Cierre

El objetivo de esta práctica no es simplemente saber ejecutar:

```bash
git log
```

El objetivo es poder mirar el resultado y **entender qué nos está contando Git**.

Cuando puedas observar un historial y reconstruir razonablemente la evolución de un proyecto, habrás dado el paso necesario para comenzar a trabajar con herramientas más potentes de investigación y comparación.

> **El historial no es solamente una lista de commits. Es la memoria registrada del proyecto.**