# Desafíos
## Módulo 08 — Perfil Profesional

Los desafíos de este módulo buscan llevar los conocimientos un paso más allá de los ejercicios.

No se trata solamente de completar tareas.

La propuesta es resolver situaciones donde sea necesario tomar decisiones, justificar criterios y producir evidencia técnica.

---

# Desafío 1 — Tu repositorio habla por vos

Elegí uno de tus repositorios.

Imaginá que una persona recibe únicamente este enlace y dispone de cinco minutos para evaluarlo.

Sin explicarle nada, pedile que responda:

```text
¿Qué hace este proyecto?

¿Para qué sirve?

¿Cómo se instala?

¿Cómo se utiliza?

¿Qué tecnologías utiliza?

¿Qué parece demostrar sobre quien lo desarrolló?
```

Después compará sus respuestas con lo que vos querías comunicar.

## Objetivo

Detectar la diferencia entre:

```text
lo que creemos que comunicamos
```

y:

```text
lo que realmente comunicamos.
```

---

# Desafío 2 — README desde cero

Elegí un proyecto cuyo README sea inexistente o insuficiente.

Sin mirar ejemplos externos, construí un README que permita a una persona nueva:

```text
comprender
   ↓
instalar
   ↓
ejecutar
   ↓
probar
```

Como mínimo debería incluir:

```text
nombre
descripción
objetivo
requisitos
instalación
uso
ejemplo
tecnologías
```

Después entregá el proyecto a otra persona.

No le expliques nada.

Si no puede utilizarlo, tenés una nueva tarea:

> mejorar la documentación.

---

# Desafío 3 — El proyecto que no parece profesional

Elegí uno de tus proyectos que actualmente no presentarías en un portafolio.

No lo descartes.

Analizá qué tendría que cambiar para hacerlo presentable.

Clasificá las mejoras:

```text
Documentación
Código
Organización
Seguridad
Presentación
```

Después implementá las mejoras más importantes.

## Resultado esperado

No necesariamente debe quedar terminado.

Debe poder explicarse:

```text
Antes
 ↓
Problemas detectados
 ↓
Mejoras
 ↓
Resultado
```

---

# Desafío 4 — Auditoría de publicación

Antes de publicar un repositorio, realizá una auditoría.

Buscá:

```text
contraseñas
tokens
claves
datos personales
archivos temporales
configuraciones locales
archivos generados
```

Revisá también:

```text
README.md
.gitignore
estructura
historial
```

Construí una lista:

```text
[ ] Revisado
```

para cada categoría.

## Pregunta clave

> ¿Qué información podría generar un problema si este repositorio fuera público mañana?

---

# Desafío 5 — El secreto ya fue publicado

Un integrante del equipo comete este error:

```bash
git add .
git commit -m "Agrega configuración"
git push
```

Dentro del commit quedó:

```text
API_KEY=123456789
```

Después se da cuenta del problema y agrega:

```text
.env
```

a `.gitignore`.

## Preguntas

1. ¿El secreto dejó de estar publicado?
2. ¿Por qué?
3. ¿Qué problema adicional existe?
4. ¿Qué acciones deberían evaluarse?

No alcanza con responder:

```text
agregar .env a .gitignore
```

Explicá qué ocurrió con la historia.

---

# Desafío 6 — Perfil profesional sin experiencia laboral

Imaginá que todavía no tenés experiencia profesional como desarrollador.

Sin inventar experiencia, construí una estrategia para presentar tu perfil utilizando:

```text
proyectos académicos
proyectos personales
ejercicios relevantes
contribuciones
documentación
aprendizajes
```

Respondé:

> ¿Qué evidencia concreta podría mostrar que estoy aprendiendo a desarrollar software?

---

# Desafío 7 — Tres proyectos, una historia

Elegí tres proyectos.

No tienen que ser los más grandes.

Organizalos para contar una evolución:

```text
Proyecto 1
   ↓
qué aprendí

Proyecto 2
   ↓
qué incorporé

Proyecto 3
   ↓
qué puedo hacer ahora
```

Después explicá:

> ¿Qué historia cuenta esta selección sobre tu aprendizaje?

---

# Desafío 8 — Una habilidad, tres evidencias

Elegí una habilidad.

Por ejemplo:

```text
Git
```

Buscá tres evidencias diferentes:

```text
1. Commit
2. Pull Request
3. Historial
```

Explicá qué demuestra cada una.

Repetí el desafío con:

```text
documentación
programación
colaboración
```

---

# Desafío 9 — Evidencia insuficiente

Una persona declara:

> "Sé trabajar con Git y GitHub."

Su repositorio contiene únicamente:

```text
README.md
```

sin historial visible de trabajo relevante.

Analizá:

1. ¿Qué evidencia falta?
2. ¿Qué podría incorporar?
3. ¿Qué actividades del curso podrían generar esa evidencia?

El objetivo no es producir actividad artificial.

La evidencia debe surgir de trabajo real.

---

# Desafío 10 — Revisar el historial como reclutador

Elegí un proyecto con varios commits.

Ejecutá:

```bash
git log --oneline --graph --all
```

Imaginá que nunca viste el código.

Intentá reconstruir:

```text
qué ocurrió primero
qué se agregó después
qué problemas aparecieron
qué se corrigió
```

Después respondé:

> ¿La historia permite entender el proceso?

Si no, explicá qué podría mejorarse en futuros proyectos.

---

# Desafío 11 — Pull Request profesional

Creá una Pull Request para una mejora real.

La descripción debe contener:

```md
## Qué hice

...

## Por qué

...

## Cómo lo probé

...

## Issue relacionada

...
```

Después pedile a otra persona que la revise.

No le expliques verbalmente qué hiciste.

La Pull Request debe ser suficiente para iniciar la revisión.

---

# Desafío 12 — Revisión crítica

Revisá la Pull Request de otra persona.

No escribas solamente:

```text
LGTM
```

o:

```text
Está bien.
```

Encontrá al menos:

```text
1 aspecto correcto
1 aspecto que podría mejorar
1 pregunta
```

Los comentarios deben ser concretos y respetuosos.

---

# Desafío 13 — El cambio solicitado

Pedile al revisor que encuentre una mejora que realmente requiera modificar el trabajo.

Después:

```text
Pull Request
      ↓
review
      ↓
request changes
      ↓
corrección
      ↓
commit
      ↓
push
      ↓
nueva revisión
```

Finalmente integrá el cambio.

## Objetivo

Demostrar que una revisión no termina necesariamente en:

```text
Approve
```

Puede producir una nueva iteración.

---

# Desafío 14 — Perfil en cinco minutos

Imaginá que una persona entra a tu perfil de GitHub durante cinco minutos.

Definí qué debería encontrar primero.

Por ejemplo:

```text
1. Presentación
2. Proyecto principal
3. Segundo proyecto
4. Tecnologías
5. Información adicional
```

Después revisá si tu perfil actual permite encontrar esa información.

Si no:

> ¿Qué cambiarías?

---

# Desafío 15 — Selección difícil

Tenés estos cinco proyectos:

```text
A — grande, incompleto y mal documentado

B — pequeño, terminado y muy bien documentado

C — grande, terminado pero difícil de entender

D — pequeño, experimental y con información sensible

E — mediano, terminado y con buen historial
```

Elegí entre uno y tres para un portafolio.

Justificá cada decisión.

No existe una única respuesta correcta.

Lo importante es el criterio.

---

# Desafío 16 — Proyecto con información sensible

Recibís un proyecto que contiene:

```text
código
README
.env
capturas
base de datos
```

La base de datos contiene información real de usuarios.

El proyecto funciona perfectamente.

## Pregunta

> ¿Lo publicarías tal como está?

Explicá:

```text
qué conservarías
qué eliminarías
qué modificarías
qué protegerías
```

El objetivo es comprender que:

```text
proyecto terminado ≠ proyecto automáticamente publicable
```

---

# Desafío 17 — README para dos públicos

Tomá un proyecto y pensá en dos lectores:

```text
Usuario
```

y:

```text
Desarrollador
```

Definí qué información necesita cada uno.

Después diseñá la estructura del README para atender a ambos sin hacerlo innecesariamente extenso.

---

# Desafío 18 — Documentación que se puede probar

Escribí una sección de instalación.

Después intentá demostrar que cada paso funciona.

Por ejemplo:

```text
Paso 1 → probado
Paso 2 → probado
Paso 3 → probado
```

Si encontrás una instrucción incorrecta, corregila.

## Idea central

> Una instrucción técnica debería poder verificarse.

---

# Desafío 19 — La tecnología no es el proyecto

Elegí un proyecto y escribí una descripción que no mencione ninguna tecnología.

Por ejemplo, no utilizar:

```text
Python
Git
JavaScript
SQL
```

La descripción debe explicar solamente:

```text
qué problema resuelve
qué hace
```

Después agregá las tecnologías en una sección separada.

## Objetivo

Aprender a distinguir:

```text
qué hace el proyecto
```

de:

```text
con qué está construido.
```

---

# Desafío 20 — Proyecto explicable

Elegí un proyecto que conozcas bien.

Prepará una explicación de tres minutos sin mirar el README.

Debés poder responder:

```text
¿Qué problema resuelve?

¿Cómo lo resolviste?

¿Por qué elegiste esa solución?

¿Qué fue difícil?

¿Qué mejorarías?
```

Si no podés explicar una parte del proyecto:

> identificá esa parte como un área de aprendizaje.

---

# Desafío 21 — Pregunta incómoda

Presentá tu proyecto a otra persona y pedile que formule una pregunta que no esté respondida en el README.

Ejemplos:

```text
¿Por qué elegiste esta estructura?

¿Qué pasa si el usuario ingresa un dato incorrecto?

¿Por qué utilizaste esta biblioteca?

¿Cómo probarías este comportamiento?
```

Respondé utilizando evidencia del proyecto.

Después evaluá si esa pregunta debería quedar respondida en la documentación.

---

# Desafío 22 — Portafolio mínimo viable

Construí un portafolio mínimo utilizando solamente:

```text
1 perfil
1 proyecto
1 README
1 presentación
```

No agregues elementos decorativos.

El objetivo es comprobar cuánto puede comunicarse utilizando evidencia concreta.

---

# Desafío 23 — Portafolio progresivo

Diseñá una estrategia para los próximos proyectos.

Por cada nuevo proyecto registrá:

```text
Problema
Solución
Tecnologías
Aprendizajes
Evidencia
```

El objetivo es que cada nuevo proyecto pueda incorporarse progresivamente al perfil profesional.

---

# Desafío 24 — Curaduría

Revisá todos tus repositorios.

Clasificalos:

```text
A — mostrar
B — mejorar
C — conservar privado
D — archivar
```

Justificá cada decisión.

No es necesario eliminar repositorios simplemente porque no sean presentables.

Archivar o mantener privado también son decisiones válidas.

---

# Desafío 25 — Repositorio archivado

Elegí un proyecto antiguo.

No lo modifiques.

Analizá:

```text
README
historial
estructura
tecnologías
calidad
```

Respondé:

> ¿Qué muestra este proyecto sobre cómo trabajabas en ese momento?

Después:

> ¿Qué muestra sobre tu evolución?

Este desafío busca convertir el historial de aprendizaje en parte de la narrativa profesional.

---

# Desafío 26 — Antes y después

Tomá un repositorio y registrá su estado inicial:

```text
README:
______

Estructura:
______

.gitignore:
______

Documentación:
______

Presentación:
______
```

Después realizá mejoras.

Volvé a completar la misma evaluación.

Compará:

```text
Antes
 ↓
Cambios
 ↓
Después
```

---

# Desafío 27 — Auditoría profesional

Realizá una auditoría completa de uno de tus proyectos.

Evaluá:

```text
Código
Documentación
Historia
Seguridad
Organización
Presentación
```

Asigná:

```text
Bueno
Aceptable
Necesita mejoras
```

Después elegí solamente tres mejoras prioritarias.

La limitación es intencional.

No se trata de mejorar todo al mismo tiempo.

---

# Desafío 28 — Perfil honesto

Escribí una descripción profesional que represente exactamente tu nivel actual.

Debe incluir:

```text
qué hacés
qué estás aprendiendo
qué herramientas utilizás
qué proyectos podés mostrar
```

No utilices:

```text
experto
especialista
senior
dominio absoluto
```

salvo que realmente puedas sostener esas afirmaciones.

---

# Desafío 29 — Evidencia contra afirmaciones

Tomá cinco afirmaciones profesionales.

Por ejemplo:

```text
Sé usar Git.
Sé programar en Python.
Sé documentar proyectos.
Sé trabajar colaborativamente.
Sé resolver problemas.
```

Para cada una completá:

```text
Afirmación:
__________

Evidencia:
__________

Proyecto:
__________

¿Puedo explicarlo?
__________
```

Si no existe evidencia:

> identificá qué proyecto o actividad podría generarla.

---

# Desafío 30 — Tu proyecto como caso de estudio

Convertí uno de tus proyectos en un pequeño caso de estudio.

Estructura sugerida:

```md
# Caso de estudio

## Problema

...

## Contexto

...

## Solución

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

No es necesario publicarlo todavía.

El objetivo es aprender a narrar técnicamente un proyecto.

---

# Desafío final — Defendé tu evidencia

Elegí el proyecto que consideres más representativo.

Prepará una presentación de entre:

```text
5 y 7 minutos
```

Deberás explicar:

```text
1. Qué problema resolvía.
2. Qué construiste.
3. Cómo lo organizaste.
4. Qué tecnologías utilizaste.
5. Qué decisiones tomaste.
6. Cómo utilizaste Git.
7. Cómo utilizaste GitHub.
8. Cómo documentaste.
9. Qué dificultad encontraste.
10. Qué aprendiste.
11. Qué mejorarías.
```

Después respondé preguntas sobre el proyecto.

La evaluación no se centra solamente en que el proyecto funcione.

Se centra en tu capacidad para:

```text
mostrar
   ↓
explicar
   ↓
justificar
   ↓
reflexionar
```

---

# Criterio general de los desafíos

En este módulo no buscamos una respuesta única para cada situación.

Buscamos desarrollar criterio.

Ante cada desafío preguntate:

```text
¿Qué decisión tomaría?
¿Por qué?
¿Qué evidencia tengo?
¿Qué consecuencias puede tener?
¿Cómo podría explicarlo?
```

Ese razonamiento es más importante que decorar un perfil.

---

# Cierre

Un perfil profesional técnico no se construye de un día para otro.

Se construye proyecto a proyecto.

```text
aprendizaje
   ↓
práctica
   ↓
proyecto
   ↓
documentación
   ↓
revisión
   ↓
mejora
   ↓
evidencia
```

Y el ciclo vuelve a comenzar.

> **La mejor presentación profesional que podés construir es un trabajo que puedas mostrar y defender con conocimiento.**