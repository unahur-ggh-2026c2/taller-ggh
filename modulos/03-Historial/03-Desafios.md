# Desafíos
## Módulo 03 — Historial

Estos desafíos buscan que puedas utilizar el historial de Git como una herramienta de lectura, análisis e investigación.

La consigna general es:

> **No mires el historial para saber qué comandos ejecutar. Miralo para descubrir qué ocurrió en el proyecto.**

---

## Desafío 1 — Leer una historia desconocida

Cloná o utilizá un repositorio de práctica que tenga varios commits.

Sin modificar nada, ejecutá:

```bash
git log --oneline
```

Intentá reconstruir la evolución del proyecto solamente a partir de los mensajes.

Después ejecutá:

```bash
git log
```

Compará la información obtenida.

### Preguntas

- ¿Qué pudiste descubrir inicialmente?
- ¿Qué información adicional apareció?
- ¿Qué cosas todavía no podés determinar?

---

## Desafío 2 — Reconstruir la evolución

Utilizá un repositorio con al menos ocho commits.

A partir de:

```bash
git log --oneline
```

escribí una explicación de la evolución del proyecto.

No copies los mensajes.

Transformalos en una historia coherente.

Por ejemplo:

```text
El proyecto comenzó con una estructura mínima.
Luego se incorporó la documentación principal.
Posteriormente se agregaron los objetivos.
Más adelante se realizaron correcciones...
```

La explicación debe basarse exclusivamente en la información disponible.

---

## Desafío 3 — El commit misterioso

Elegí un commit intermedio de la historia.

Registrá:

```text
Identificador:
Mensaje:
Autor:
Fecha:
```

Ahora respondé:

> ¿Qué información adicional necesitarías para saber exactamente qué cambió en ese commit?

No realices todavía ninguna operación adicional.

El objetivo es distinguir entre:

```text
información sobre el commit
```

e:

```text
información sobre los cambios concretos
```

---

## Desafío 4 — Historia pobre

Creá un repositorio con al menos cinco commits.

Utilizá deliberadamente mensajes poco descriptivos:

```text
cambios
update
arreglo
más
final
```

Después ejecutá:

```bash
git log --oneline
```

Intentá reconstruir la historia.

### Tu desafío

Explicá qué dificultades aparecen.

Después realizá una segunda historia con mensajes descriptivos.

Compará ambas.

---

## Desafío 5 — ¿Cuándo ocurrió?

Supongamos que alguien informa:

> "El proyecto comenzó a tener problemas después de que se modificó la documentación."

Tenés acceso al historial.

### Tu desafío

Diseñá una estrategia para investigar la afirmación.

Deberás indicar:

1. qué información buscarías;
2. qué commit intentarías identificar;
3. qué datos del historial utilizarías;
4. qué información necesitarías consultar después.

No es necesario resolver todavía el problema técnico.

El objetivo es aprender a formular una investigación a partir del historial.

---

## Desafío 6 — Encontrar el comienzo

En un repositorio desconocido, identificá el commit inicial.

Después respondé:

- ¿qué mensaje tiene?
- ¿quién lo realizó?
- ¿cuándo?
- ¿qué representa dentro de la historia?

Finalmente explicá:

> ¿Por qué resulta útil conocer el punto inicial de un proyecto?

---

## Desafío 7 — Encontrar un punto intermedio

Identificá un commit que se encuentre aproximadamente en la mitad de la historia.

Registrá su:

```text
hash
mensaje
autor
fecha
```

Después describí:

> ¿Qué había ocurrido antes de ese punto?

y:

> ¿Qué ocurrió después?

La respuesta debe basarse en el historial.

---

## Desafío 8 — El historial como mapa temporal

Construí un esquema temporal de un repositorio:

```text
Inicio
  ↓
Commit A
  ↓
Commit B
  ↓
Commit C
  ↓
Commit D
  ↓
Actualidad
```

Para cada punto incorporá:

- identificador;
- mensaje;
- fecha.

Después explicá qué información aporta el esquema que no resulta tan evidente al observar una lista sin analizarla.

---

## Desafío 9 — Investigar una afirmación

Un compañero sostiene:

> "El objetivo X estaba desde el comienzo del proyecto."

Tenés un repositorio con historial.

### Tu desafío

Determinar qué evidencia necesitarías para confirmar o refutar la afirmación.

Pensá en términos de:

```text
afirmación
    ↓
historial
    ↓
commit relevante
    ↓
evidencia
```

No alcanza con decir "miraría el log".

Explicá qué buscarías.

---

## Desafío 10 — ¿Qué podemos saber?

Observá únicamente:

```text
91f7a20 Agrega objetivos
a3d84f6 Crea documentación inicial
42bc8d1 Corrige descripción
7e3a91f Agrega instrucciones
```

Determiná todo lo que razonablemente puedas inferir.

Después escribí una segunda lista:

```text
No podemos saber solamente con esta información:
```

La segunda lista debe ser explícita.

---

## Desafío 11 — Mensajes como comunicación

Elegí un proyecto real o de práctica y analizá sus mensajes de commit.

Evaluá:

### Claridad

¿Se entiende qué ocurrió?

### Consistencia

¿Los mensajes mantienen un criterio similar?

### Utilidad

¿Servirían para investigar un problema?

### Contexto

¿Permiten comprender la intención del cambio?

Finalmente escribí una conclusión.

---

## Desafío 12 — Historia para una persona nueva

Imaginá que mañana se incorpora una nueva persona al proyecto.

No puede preguntarle nada al equipo.

Solamente dispone del repositorio.

Su primer paso es:

```bash
git log --oneline
```

### Tu desafío

Analizá tu propio historial desde esa perspectiva.

Respondé:

- ¿qué podría entender?
- ¿qué preguntas le surgirían?
- ¿qué información falta?
- ¿los mensajes ayudan o dificultan su incorporación?

---

## Desafío 13 — El historial como diagnóstico

Supongamos que el equipo detecta que una funcionalidad dejó de comportarse como antes.

No sabés todavía cuál fue la causa.

### Tu desafío

Explicá cómo utilizarías el historial para comenzar la investigación.

No es necesario encontrar la solución.

Diseñá solamente una estrategia:

```text
Problema detectado
       ↓
Consultar historial
       ↓
Identificar cambios relevantes
       ↓
Seleccionar puntos de interés
       ↓
Investigar
```

Explicá qué buscarías en cada etapa.

---

## Desafío 14 — Construir evidencia

Elegí una afirmación sobre un proyecto.

Por ejemplo:

> "La documentación fue incorporada después de los objetivos."

Utilizá el historial para determinar si la afirmación puede sostenerse.

Después escribí:

```text
Afirmación:
...

Evidencia:
...

Conclusión:
...
```

Si el historial no alcanza para determinarlo, indicá qué información adicional necesitarías.

---

## Desafío 15 — El historial engañoso

Construí una historia con cinco commits cuyos mensajes sean técnicamente válidos pero poco informativos.

Por ejemplo:

```text
Actualiza proyecto
Actualiza proyecto
Actualiza proyecto
Actualiza proyecto
Actualiza proyecto
```

Después intentá reconstruir la evolución.

### Pregunta

> ¿Los mensajes son incorrectos?

Probablemente no.

Entonces:

> ¿Por qué siguen siendo malos mensajes para un historial?

El objetivo es diferenciar **validez técnica** de **calidad comunicacional**.

---

## Desafío 16 — Una historia útil

Construí nuevamente una historia de cinco commits.

Esta vez cada mensaje debe comunicar una intención concreta.

Por ejemplo:

```text
Crea estructura inicial
Agrega documentación del proyecto
Incorpora objetivos
Corrige descripción
Agrega instrucciones de uso
```

Después compará ambas historias.

Escribí una conclusión sobre el valor de los mensajes.

---

## Desafío 17 — Estado e historia

Partí de un repositorio limpio.

Realizá una modificación y no hagas commit.

Ahora observá:

```bash
git status
```

y:

```bash
git log --oneline
```

### Tu desafío

Explicá qué responde cada comando.

Después respondé:

> ¿Por qué necesitamos ambas herramientas?

---

## Desafío 18 — La historia no es el estado actual

Imaginá:

```text
Último commit
     ↓
README.md decía:
"Proyecto en desarrollo."
```

Después modificaste el archivo y ahora dice:

```text
"Proyecto finalizado."
```

Pero todavía no hiciste commit.

### Pregunta

¿Qué representa el historial?

¿Qué representa el archivo actual?

¿Qué representa `git status`?

Explicá la diferencia.

---

## Desafío 19 — Historia deliberada

Creá un proyecto pequeño y construí una historia de al menos diez commits.

Condiciones:

- cada commit debe representar una intención concreta;
- los mensajes deben ser descriptivos;
- debe existir al menos una corrección;
- debe existir al menos una incorporación;
- debe existir al menos una modificación de documentación.

Después ejecutá:

```bash
git log --oneline
```

Intentá escribir la historia del proyecto sin abrir ningún archivo.

---

## Desafío 20 — Evaluación crítica

Analizá tu historia de diez commits.

Asignale una evaluación de 1 a 5 en:

| Criterio | Puntaje |
|---|:---:|
| Claridad de mensajes | |
| Coherencia de la evolución | |
| Identificación de cambios | |
| Utilidad para investigar | |
| Facilidad de comprensión | |

Después justificá cada puntuación.

---

## Desafío 21 — Resolver sin receta

Recibís un repositorio desconocido.

No se te indica qué comando utilizar.

La única consigna es:

> "Necesito entender cómo evolucionó este proyecto."

### Tu desafío

Decidí por dónde empezar.

Después:

1. observá el historial;
2. identificá puntos relevantes;
3. seleccioná commits;
4. construí una explicación;
5. indicá qué información falta.

El objetivo es evaluar tu autonomía.

---

## Desafío 22 — Enseñar el historial

Explicale a una persona que nunca utilizó Git qué es el historial.

No empieces por:

```bash
git log
```

Primero explicá:

- qué problema resuelve;
- qué relación tiene con los commits;
- qué información conserva;
- por qué puede ser útil.

Después mostrale cómo consultar esa información.

---

## Desafío 23 — El historial como memoria

Reflexioná sobre esta afirmación:

> **"Git conserva la memoria del proyecto."**

Explicá qué significa.

Después señalá también los límites de esa afirmación.

¿Qué información puede conservar?

¿Qué información podría no estar disponible?

---

## Desafío 24 — Integración

Utilizá un repositorio con al menos diez commits.

Sin modificarlo:

1. ejecutá `git log`;
2. ejecutá `git log --oneline`;
3. identificá el primer commit;
4. identificá el último;
5. seleccioná dos commits intermedios;
6. registrá sus identificadores;
7. analizá sus mensajes;
8. reconstruí la evolución;
9. indicá qué información falta;
10. explicá qué investigarías a continuación.

---

## Desafío final — La historia que cuenta tu proyecto

Construí un pequeño repositorio documental desde cero.

El proyecto debe tener una evolución real y al menos diez commits.

Al finalizar:

```bash
git log --oneline
```

debe permitir reconstruir una historia razonablemente clara.

Después escribí:

```md
# Historia del proyecto

## Comienzo

...

## Primeras modificaciones

...

## Evolución

...

## Correcciones

...

## Estado actual

...
```

La explicación debe basarse en el historial.

No agregues acontecimientos que no puedan sostenerse con la evidencia disponible.

Finalmente respondé:

> **¿Qué aprendiste sobre la diferencia entre conservar una historia y comprender una historia?**

---

## Criterio de superación

El desafío se considera logrado cuando podés utilizar el historial para:

```text
observar
   ↓
identificar
   ↓
interpretar
   ↓
formular hipótesis
   ↓
buscar evidencia
   ↓
explicar
```

Ese recorrido será cada vez más importante cuando el curso avance hacia ramas, trabajo colaborativo y resolución de problemas reales.