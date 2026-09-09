# Ejercicios
## Módulo 03 — Historial

Estos ejercicios buscan desarrollar la capacidad de **leer e interpretar el historial de Git**, no solamente ejecutar comandos.

La pregunta guía es:

> **¿Qué puedo averiguar sobre la evolución de un proyecto a partir de su historial?**

---

## Ejercicio 1 — Primer vistazo

En un repositorio que tenga varios commits, ejecutá:

```bash
git log
```

Identificá:

- el commit más reciente;
- el commit más antiguo;
- el autor de cada uno;
- la fecha;
- el mensaje;
- el identificador.

Respondé:

1. ¿Cuántos commits aparecen?
2. ¿En qué orden se muestran?
3. ¿Qué información se repite en cada commit?

---

## Ejercicio 2 — Historial resumido

Ejecutá:

```bash
git log --oneline
```

Compará el resultado con:

```bash
git log
```

Completá:

| Información | `git log` | `git log --oneline` |
|---|:---:|:---:|
| Identificador | | |
| Mensaje | | |
| Autor | | |
| Fecha | | |

Explicá qué ventaja ofrece cada representación.

---

## Ejercicio 3 — Identificar un commit

Elegí un commit intermedio del historial.

Anotá su identificador.

Por ejemplo:

```text
a84f9c2
```

Respondé:

1. ¿Qué mensaje tiene?
2. ¿Quién lo creó?
3. ¿Cuándo fue creado?
4. ¿Qué commits aparecen antes?
5. ¿Qué commits aparecen después?

---

## Ejercicio 4 — Orden temporal

Observá:

```bash
git log --oneline
```

Copiá los commits en una lista y ordenalos desde el más antiguo hasta el más reciente.

Después escribí una breve descripción de la evolución del proyecto.

Por ejemplo:

```text
1. Se crea la estructura inicial.
2. Se incorpora la documentación.
3. Se agregan los objetivos.
4. Se corrige la descripción.
5. Se agregan instrucciones.
```

Utilizá únicamente información que pueda inferirse razonablemente del historial.

---

## Ejercicio 5 — Leer los mensajes

Analizá los mensajes de los últimos commits.

Clasificalos según indiquen:

- creación;
- incorporación;
- modificación;
- corrección;
- documentación;
- otro tipo de cambio.

Después respondé:

> ¿Los mensajes permiten reconstruir una evolución coherente?

---

## Ejercicio 6 — Historial claro o confuso

Compará:

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
Agrega objetivos
Actualiza descripción
Corrige instrucciones
Agrega información de uso
```

Respondé:

1. ¿Cuál es más fácil de interpretar?
2. ¿Por qué?
3. ¿Qué información falta en el historial A?
4. ¿Qué información aporta el historial B?

---

## Ejercicio 7 — Estado actual versus historial

Partí de un repositorio limpio.

Ejecutá:

```bash
git status
```

y:

```bash
git log --oneline
```

Compará ambas salidas.

Después modificá un archivo sin realizar un commit.

Volvé a ejecutar:

```bash
git status
```

y:

```bash
git log --oneline
```

Respondé:

1. ¿Qué cambio detectó `git status`?
2. ¿Aparece ese cambio en `git log`?
3. ¿Por qué?
4. ¿Qué diferencia existe entre el estado actual y la historia registrada?

---

## Ejercicio 8 — Construir una historia

Creá un repositorio nuevo.

Realizá al menos cinco commits que representen una evolución deliberada.

Por ejemplo:

```text
Commit 1 — documentación inicial
Commit 2 — descripción
Commit 3 — objetivos
Commit 4 — características
Commit 5 — corrección
```

Los mensajes deben ser propios y descriptivos.

Después:

```bash
git log --oneline
```

Intentá reconstruir la historia sin mirar los archivos.

---

## Ejercicio 9 — El commit más reciente

Utilizando únicamente:

```bash
git log
```

respondé:

1. ¿Cuál es el commit más reciente?
2. ¿Quién lo realizó?
3. ¿Cuándo?
4. ¿Qué mensaje tiene?
5. ¿Qué identificador posee?

Después explicá cómo encontraste cada respuesta.

---

## Ejercicio 10 — El commit inicial

Identificá el commit más antiguo del repositorio.

Respondé:

1. ¿Cuál es su identificador?
2. ¿Cuál es su mensaje?
3. ¿Quién lo realizó?
4. ¿Qué representa dentro de la historia?

Explicá por qué ese commit tiene una importancia particular.

---

## Ejercicio 11 — Un commit intermedio

Elegí un commit que no sea ni el primero ni el último.

Registrá:

```text
Identificador:
Mensaje:
Autor:
Fecha:
```

Después describí:

- qué ocurrió antes;
- qué ocurrió después;
- qué lugar ocupa ese commit en la evolución.

---

## Ejercicio 12 — El historial como relato

Leé todos los mensajes mediante:

```bash
git log --oneline
```

Ahora escribí un relato breve de la evolución del proyecto.

No copies los mensajes uno detrás de otro.

Transformalos en una explicación coherente.

Por ejemplo:

> "El proyecto comenzó con una estructura documental básica. Luego se incorporaron los objetivos y posteriormente se amplió la descripción. Finalmente se corrigió una parte de la documentación."

---

## Ejercicio 13 — ¿Qué sabemos y qué no sabemos?

Observá un historial real.

Separá la información en dos grupos.

### Podemos inferir:

- ...
- ...
- ...

### No podemos determinar solamente con el historial:

- ...
- ...
- ...

La segunda lista es tan importante como la primera.

El objetivo es reconocer los límites de la información disponible.

---

## Ejercicio 14 — El historial como evidencia

Supongamos que alguien afirma:

> "La descripción del proyecto siempre fue la misma."

Tenés acceso al historial.

Respondé:

1. ¿El historial puede ayudarte a investigar la afirmación?
2. ¿Qué información buscarías?
3. ¿Qué necesitarías consultar además del listado de commits?
4. ¿Qué diferencia existe entre una hipótesis y una evidencia?

---

## Ejercicio 15 — Identificadores

Observá los identificadores de varios commits.

Respondé:

1. ¿Se repiten?
2. ¿Tienen todos la misma estructura?
3. ¿Parecen números consecutivos?
4. ¿Para qué puede servir identificar un commit de manera única?

No es necesario investigar todavía cómo se generan internamente.

---

## Ejercicio 16 — Una historia problemática

Creá deliberadamente un pequeño repositorio con mensajes poco descriptivos:

```text
cambios
update
arreglo
más cosas
final
```

Después observá:

```bash
git log --oneline
```

Intentá reconstruir la evolución.

Escribí qué dificultades encontraste.

Después creá otro repositorio o una nueva historia utilizando mensajes descriptivos.

Compará ambas experiencias.

---

## Ejercicio 17 — Mejorar el criterio

Para cada mensaje, proponé una alternativa más útil:

```text
cambios
```

```text
update
```

```text
arreglo
```

```text
cosas nuevas
```

```text
final
```

Después explicá qué información agregaste y por qué.

---

## Ejercicio 18 — Leer sin ejecutar nada más

Observá solamente:

```text
7e3a91f Agrega instrucciones de uso
42bc8d1 Corrige descripción del proyecto
91f7a20 Incorpora objetivos
a3d84f6 Crea documentación inicial
```

Respondé:

1. ¿Cuál es el commit más reciente?
2. ¿Cuál es el inicial?
3. ¿Qué ocurrió entre ambos?
4. ¿Cuál parece ser una corrección?
5. ¿Qué información no podemos conocer solamente a partir de estos mensajes?

---

## Ejercicio 19 — `git log` como herramienta de consulta

Imaginá que alguien te pregunta:

> "¿Quién realizó el último cambio registrado?"

Sin modificar nada del repositorio, determiná qué herramienta utilizarías y dónde buscarías la información.

Después hacelo realmente.

---

## Ejercicio 20 — Buscar una modificación conceptual

Supongamos que el historial contiene:

```text
Crea estructura inicial
Agrega documentación
Agrega objetivos
Actualiza descripción
Corrige documentación
Agrega instrucciones
```

Te preguntan:

> "¿Cuándo apareció por primera vez la documentación?"

¿Qué commit revisarías?

Explicá el razonamiento.

---

## Ejercicio 21 — Construir una historia significativa

Elegí un pequeño proyecto documental.

Realizá al menos seis commits.

Cada commit debe tener:

- una intención concreta;
- cambios relacionados;
- un mensaje descriptivo.

Después ejecutá:

```bash
git log --oneline
```

Escribí una explicación de la historia que pueda ser entendida por alguien que nunca vio el proyecto.

---

## Ejercicio 22 — Evaluar tu propio historial

Leé tu historial como si fueras una persona externa.

Respondé:

### Claridad

¿Los mensajes son comprensibles?

### Secuencia

¿Se puede reconocer la evolución?

### Intención

¿Se entiende por qué se realizó cada cambio?

### Utilidad

¿El historial sería útil para investigar un problema?

### Mejora

¿Qué cambiarías si tuvieras que volver a construirlo?

---

## Ejercicio 23 — El historial y el trabajo en equipo

Imaginá que te incorporás a un proyecto desarrollado durante varios meses.

No conocés a quienes lo desarrollaron.

La primera herramienta que tenés disponible es:

```bash
git log --oneline
```

Respondé:

1. ¿Qué información te puede proporcionar?
2. ¿Qué preguntas podrías empezar a responder?
3. ¿Qué información necesitarías investigar posteriormente?
4. ¿Por qué un historial bien construido facilita la incorporación de nuevas personas?

---

## Ejercicio 24 — Reconstrucción

A partir del historial de un repositorio real, escribí:

```md
# Evolución del proyecto

## Inicio

...

## Desarrollo inicial

...

## Cambios posteriores

...

## Estado actual

...
```

La explicación debe basarse en información observable.

No agregues acontecimientos que no puedas justificar.

---

## Ejercicio 25 — Integración

Partí de un repositorio con varios commits.

Realizá:

```bash
git log
```

y:

```bash
git log --oneline
```

Después:

1. identificá el commit inicial;
2. identificá el más reciente;
3. elegí uno intermedio;
4. anotá su identificador;
5. identificá autor y fecha;
6. interpretá su mensaje;
7. reconstruí la evolución general;
8. indicá qué información no puede determinarse solamente con el historial.

---

## Comprobación final

Sin consultar documentación, explicá:

> **¿Qué información puedo obtener de un commit?**

Después:

> **¿Qué diferencia existe entre `git log` y `git log --oneline`?**

Y finalmente:

> **¿Por qué un historial bien construido puede convertirse en una herramienta de investigación?**

Si podés responder estas preguntas y demostrarlo sobre un repositorio real, el objetivo principal del módulo está cumplido.