# Desafíos
## Módulo 09 — Proyecto Final

Los desafíos de este módulo buscan llevar el Proyecto Final hacia situaciones que requieran criterio, análisis y toma de decisiones.

No se trata de cumplir mecánicamente una cantidad de comandos.

La propuesta es resolver problemas similares a los que pueden aparecer durante un proyecto real.

---

# Desafío 1 — Elegir un proyecto viable

Tenés tres propuestas:

```text
A — Aplicación completa de gestión para una organización.

B — Programa pequeño que resuelve una necesidad concreta.

C — Plataforma web con autenticación, base de datos,
    usuarios, permisos y panel administrativo.
```

El tiempo disponible para el Proyecto Final es limitado.

Elegí una propuesta y justificá:

```text
¿Qué puedo terminar?
¿Qué puedo documentar?
¿Qué puedo explicar?
¿Qué evidencia puedo generar?
```

El objetivo no es elegir el proyecto más grande.

Es elegir el proyecto que permita realizar un trabajo completo.

---

# Desafío 2 — Reducir el alcance

Tomá un proyecto demasiado grande.

Por ejemplo:

```text
Sistema de gestión de biblioteca completo.
```

Reducilo hasta obtener una primera versión razonable.

Por ejemplo:

```text
Registrar libros.
Consultar libros.
Registrar préstamos.
```

Después definí:

```text
Versión mínima
Mejoras futuras
```

Explicá qué problema resuelve reducir el alcance.

---

# Desafío 3 — El proyecto sin planificación

Un estudiante comienza directamente a programar.

Después de varios días tiene:

```text
muchos archivos
varios commits
ninguna Issue
README vacío
main con todos los cambios
```

Analizá la situación.

Respondé:

1. ¿Qué problemas puede generar?
2. ¿Qué debería haber definido antes?
3. ¿Qué puede corregirse todavía?
4. ¿Qué no conviene intentar reconstruir artificialmente?

---

# Desafío 4 — Diseñar el flujo de trabajo

Definí un flujo de trabajo para tu proyecto.

Debe incluir:

```text
Issue
 ↓
rama
 ↓
trabajo
 ↓
commit
 ↓
push
 ↓
Pull Request
 ↓
revisión
 ↓
corrección
 ↓
merge
```

Después explicá qué función cumple cada etapa.

---

# Desafío 5 — Elegir una estrategia de ramas

Tenés un proyecto pequeño.

Proponé una estructura de ramas.

Después tenés un proyecto grupal con varias funcionalidades simultáneas.

Proponé otra.

Compará:

```text
Proyecto pequeño
vs.
Proyecto grupal
```

Respondé:

> ¿Por qué no necesariamente conviene utilizar la misma estrategia en ambos casos?

---

# Desafío 6 — Commit artificial

El docente establece como requisito:

```text
"El proyecto debe tener 30 commits."
```

Un estudiante comienza a crear commits como:

```text
cambio 1
cambio 2
cambio 3
cambio 4
...
```

Analizá el problema.

Respondé:

> ¿Por qué la cantidad de commits no debería ser un objetivo en sí mismo?

Después proponé un criterio mejor.

---

# Desafío 7 — Historia comprensible

Compará estos historiales:

### Proyecto A

```text
inicio
cambios
fix
cosas
prueba
final
final2
```

### Proyecto B

```text
Inicializa estructura del proyecto
Agrega validación de entrada
Implementa búsqueda de libros
Documenta instalación
Corrige error en consulta
```

¿Cuál permite comprender mejor la evolución?

¿Por qué?

---

# Desafío 8 — El README engañoso

El README dice:

```text
## Instalación

1. Clonar el repositorio.
2. Ejecutar el programa.
```

Pero para ejecutar el proyecto realmente hace falta:

```text
Python 3.12
dependencia X
archivo de configuración
variable de entorno
```

Analizá el problema.

Respondé:

> ¿Qué debería hacer el autor?

---

# Desafío 9 — README que no fue probado

Un estudiante escribe instrucciones de instalación y dice:

> "Seguramente funcionan."

No las prueba.

Otra persona intenta utilizar el proyecto y falla.

Analizá:

```text
documentación
 ↓
suposición
```

versus:

```text
documentación
 ↓
prueba
 ↓
corrección
```

Explicá por qué la segunda secuencia es preferible.

---

# Desafío 10 — Pull Request demasiado grande

Una Pull Request contiene:

```text
25 archivos modificados
8 funcionalidades
cambios de documentación
cambios de estructura
correcciones varias
```

El título es:

```text
"Actualización"
```

Analizá:

1. ¿Qué dificultades tendrá el revisor?
2. ¿Qué podría hacerse diferente?
3. ¿Cómo dividirías el trabajo?

---

# Desafío 11 — Pull Request demasiado pequeña

Ahora tenés una Pull Request que solamente cambia:

```text
un espacio
```

pero está acompañada por:

```text
Issue
rama
Pull Request
tres comentarios
merge
```

¿Es necesariamente una mala práctica?

Justificá.

El objetivo es comprender que el tamaño del cambio debe evaluarse según su contexto.

---

# Desafío 12 — Revisión superficial

Un revisor responde:

```text
LGTM
```

sin mirar el código.

¿Qué problemas puede generar?

Después definí qué debería comprobar mínimamente antes de aprobar una Pull Request.

---

# Desafío 13 — Revisión útil

Transformá este comentario:

```text
"Esto está mal."
```

en un comentario técnico más útil.

Debe indicar:

```text
qué observaste
por qué importa
qué proponés
```

---

# Desafío 14 — Feedback rechazado

Un estudiante recibe una observación en una Pull Request y responde:

> "Funciona, así que está bien."

Analizá la respuesta.

¿Que funcione alcanza para cerrar una revisión?

¿Qué otros aspectos podrían ser relevantes?

---

# Desafío 15 — Conflicto

Dos integrantes modificaron la misma parte del README.

### Rama A

```text
El proyecto requiere Python 3.11.
```

### Rama B

```text
El proyecto requiere Python 3.12.
```

Se produce un conflicto.

No resuelvas simplemente eligiendo una línea.

Definí:

```text
¿Qué información debería verificarse?
¿Qué versión utiliza realmente el proyecto?
¿Qué debería quedar documentado?
```

---

# Desafío 16 — Conflicto con código

Dos ramas modifican la misma función.

Una agrega:

```text
validación
```

y la otra agrega:

```text
nuevo comportamiento
```

El merge produce un conflicto.

Explicá qué debería analizar el desarrollador antes de resolverlo.

---

# Desafío 17 — Resolver sin comprender

Un estudiante resuelve todos los conflictos utilizando:

```text
Accept Current Change
```

sin leer el contenido.

¿Por qué es peligroso?

¿Qué debería hacer en cambio?

---

# Desafío 18 — Conflicto resuelto, proyecto roto

El conflicto desapareció.

Pero después del merge el programa deja de funcionar.

Respondé:

> ¿Qué faltó hacer?

Definí un procedimiento posterior a la resolución.

Por ejemplo:

```text
resolver
 ↓
revisar
 ↓
probar
 ↓
corregir
```

---

# Desafío 19 — El secreto publicado

Un integrante publica:

```text
.env
```

y dentro hay:

```text
API_KEY=abc123
```

Una hora después lo agrega a `.gitignore`.

Analizá la situación.

Respondé:

```text
¿Qué pasó?
¿Qué sigue siendo visible?
¿Por qué .gitignore no alcanza?
¿Qué debería evaluarse ahora?
```

---

# Desafío 20 — Información sensible en un proyecto académico

Un proyecto académico utiliza datos reales de personas.

El estudiante quiere publicarlo para mostrarlo en su perfil.

¿Lo publicarías tal como está?

Definí:

```text
qué podría conservarse
qué debería eliminarse
qué debería anonimizarse
qué debería mantenerse privado
```

---

# Desafío 21 — `.gitignore` incorrecto

Un proyecto tiene:

```gitignore
*
```

Todo está siendo ignorado.

El estudiante dice:

> "Perfecto, ya no puedo subir archivos innecesarios."

Analizá el problema.

¿Qué consecuencias tiene esta configuración?

---

# Desafío 22 — `.gitignore` demasiado amplio

Un estudiante agrega:

```gitignore
*.json
```

porque quiere evitar publicar archivos de configuración.

Pero el proyecto también necesita versionar:

```text
config/default.json
```

Analizá el problema.

Diseñá una regla más precisa.

---

# Desafío 23 — Repositorio público

Antes de publicar un proyecto, un estudiante revisa solamente:

```text
README
```

No revisa el historial.

¿Por qué esto puede ser insuficiente?

¿Qué debería analizar además?

---

# Desafío 24 — Código heredado

Te entregan un proyecto que ya tiene:

```text
código
commits
ramas
README
```

pero no conocés su historia.

Antes de modificarlo, ¿qué revisarías?

Construí una secuencia:

```text
1.
2.
3.
4.
5.
```

---

# Desafío 25 — Proyecto existente

El proyecto ya tenía:

```text
README
.gitignore
10 commits
```

antes de comenzar el Proyecto Final.

Definí cómo demostrarías qué trabajo realizaste durante esta etapa.

---

# Desafío 26 — Proyecto grupal

Un equipo tiene cuatro integrantes.

Uno realiza todos los commits.

Los otros tres solamente dicen:

> "Trabajamos juntos."

Analizá:

1. ¿Qué problema aparece?
2. ¿Qué evidencia falta?
3. ¿Cómo podría organizarse mejor el trabajo?

---

# Desafío 27 — Participación desigual

En un proyecto grupal:

```text
Integrante A → código
Integrante B → documentación
Integrante C → revisión
Integrante D → pruebas
```

¿Significa necesariamente que A trabajó más que todos?

Justificá por qué la cantidad de commits no permite determinar por sí sola la contribución real.

---

# Desafío 28 — Issue mal definida

Una Issue dice:

```text
"Mejorar aplicación."
```

Transformala en una Issue útil.

Debe contener:

```text
Problema
Objetivo
Resultado esperado
```

---

# Desafío 29 — Issue que no representa trabajo real

Un estudiante crea diez Issues solamente para demostrar que utilizó GitHub.

Analizá la situación.

¿Qué sería preferible?

```text
10 Issues artificiales
```

o:

```text
3 Issues reales
```

Justificá.

---

# Desafío 30 — GitHub como almacenamiento

Un estudiante dice:

> "GitHub sirve para guardar mi proyecto en Internet."

La afirmación no es completamente incorrecta, pero es insuficiente.

Explicá qué otras funciones trabajadas durante el curso puede cumplir GitHub.

---

# Desafío 31 — Git como backup

Un estudiante dice:

> "Uso Git solamente porque es una copia de seguridad."

Explicá qué conceptos del curso permiten demostrar que Git es mucho más que un backup.

---

# Desafío 32 — Proyecto sin historial

Recibís un proyecto que funciona perfectamente, pero tiene:

```text
un único commit
```

No sabés cómo evolucionó.

¿Qué información perdiste?

¿Qué podría haber aportado un historial mejor construido?

---

# Desafío 33 — Historia extensa pero inútil

Ahora recibís un proyecto con:

```text
500 commits
```

pero todos dicen:

```text
cambio
```

¿Es necesariamente mejor que el proyecto anterior?

Explicá.

---

# Desafío 34 — Documentación desactualizada

El proyecto cambió:

```text
Python 3.11 → Python 3.12
```

pero el README sigue diciendo:

```text
Python 3.11
```

¿Qué problema genera?

¿Quién debería detectar este error?

---

# Desafío 35 — Documentación y código

El README dice que existe:

```text
comando A
```

pero el programa actualmente utiliza:

```text
comando B
```

¿Qué debería considerarse la fuente de verdad?

¿Qué debería hacer el desarrollador?

---

# Desafío 36 — Proyecto terminado sin próximos pasos

El estudiante dice:

> "El proyecto está terminado."

Pero todavía existen:

```text
errores conocidos
funcionalidades pendientes
documentación incompleta
```

¿Puede considerarse terminado?

Diferenciá:

```text
alcance definido
```

de:

```text
perfección absoluta
```

---

# Desafío 37 — Presentación de cinco minutos

Tenés cinco minutos para presentar tu proyecto.

Definí cómo distribuirías el tiempo.

Por ejemplo:

```text
Problema      → 1 min
Solución      → 1 min
Proceso       → 1 min
Evidencia     → 1 min
Aprendizajes  → 1 min
```

Justificá tu distribución.

---

# Desafío 38 — Pregunta inesperada

Durante la defensa te preguntan:

> "¿Por qué no utilizaste otra tecnología?"

No existe una respuesta única.

Construí una respuesta basada en:

```text
contexto
requisitos
aprendizaje
simplicidad
```

No respondas solamente:

```text
"porque elegí esta."
```

---

# Desafío 39 — Defender una decisión

Elegí una decisión real de tu proyecto.

Prepará una defensa utilizando:

```text
Problema
Alternativas
Decisión
Motivo
Resultado
```

---

# Desafío 40 — Admitir una limitación

Durante la presentación te preguntan algo que no implementaste.

Por ejemplo:

> "¿Qué ocurre si ingresamos datos inválidos?"

La respuesta correcta no tiene que ser inventada.

Construí una respuesta profesional que distinga:

```text
lo que funciona
```

de:

```text
lo que todavía no está implementado.
```

---

# Desafío 41 — El proyecto que no funciona

El proyecto presenta un error el día de la presentación.

¿Qué harías?

Definí una estrategia:

```text
identificar
 ↓
explicar
 ↓
mostrar evidencia
 ↓
proponer solución
```

El objetivo es evaluar también la capacidad de comunicar una limitación.

---

# Desafío 42 — README versus presentación

El README tiene veinte secciones.

La presentación dura cinco minutos.

¿Qué información mostrarías oralmente?

¿Qué dejarías en el README?

Explicá la diferencia entre:

```text
documentación de referencia
```

y:

```text
presentación oral
```

---

# Desafío 43 — Proyecto como portafolio

Una vez terminado el Proyecto Final, decidí si lo presentarías públicamente.

Evaluá:

```text
Calidad
Documentación
Seguridad
Originalidad
Comprensión
Estado
```

Después clasificá:

```text
Publicar
Mejorar antes de publicar
Mantener privado
```

Justificá.

---

# Desafío 44 — Evidencia profesional

Elegí tres capacidades demostradas durante el Proyecto Final.

Por ejemplo:

```text
Git
documentación
colaboración
```

Para cada una indicá:

```text
Capacidad
↓
Evidencia
↓
Dónde puede verificarse
```

---

# Desafío 45 — Auditoría completa

Realizá una auditoría del repositorio final.

Evaluá:

```text
Proyecto
Git
GitHub
Documentación
Seguridad
Presentación
```

Para cada categoría asigná:

```text
Bueno
Aceptable
Necesita mejoras
```

Después elegí las tres mejoras más importantes.

---

# Desafío 46 — Proyecto bajo presión

Imaginá que quedan:

```text
24 horas
```

para entregar.

Todavía faltan:

```text
una funcionalidad
README
pruebas
presentación
```

Definí prioridades.

No intentes terminar todo simultáneamente.

Explicá:

```text
qué terminarías
qué simplificarías
qué dejarías documentado como pendiente
```

---

# Desafío 47 — Cambio de alcance

A mitad del proyecto aparece una nueva necesidad:

> "También necesitamos usuarios con autenticación."

Analizá si incorporarías esa funcionalidad.

Considerá:

```text
tiempo
complejidad
objetivo
alcance
riesgo
```

Si decidís no incorporarla, explicá cómo registrarías la decisión.

---

# Desafío 48 — Replanificar

Una funcionalidad resulta mucho más compleja de lo esperado.

El plan original era:

```text
Tarea A
Tarea B
Tarea C
Tarea D
```

Pero Tarea B consume demasiado tiempo.

Proponé una nueva planificación.

La idea es comprender que:

```text
planificar
```

no significa:

```text
seguir ciegamente un plan.
```

---

# Desafío 49 — Proyecto profesionalmente defendible

Respondé:

> ¿Qué tendría que poder mostrar una persona para defender que realmente trabajó en un proyecto?

Construí una lista de evidencias.

Por ejemplo:

```text
código
commits
Issues
Pull Requests
documentación
decisiones
presentación
```

---

# Desafío 50 — El proyecto completo

Tomá tu Proyecto Final y reconstruí el recorrido:

```text
Problema
 ↓
Objetivo
 ↓
Planificación
 ↓
Issue
 ↓
Rama
 ↓
Desarrollo
 ↓
Commit
 ↓
Pull Request
 ↓
Revisión
 ↓
Corrección
 ↓
Merge
 ↓
Documentación
 ↓
Presentación
```

Para cada etapa indicá dónde está la evidencia.

---

# Desafío final — Defendé el proceso

Prepará una presentación donde no muestres solamente el resultado.

Mostrá también cómo llegaste hasta él.

Deberías poder responder:

```text
¿Qué problema elegiste?

¿Por qué elegiste ese alcance?

¿Cómo organizaste el trabajo?

¿Cómo utilizaste Git?

¿Cómo utilizaste GitHub?

¿Cómo registraste los cambios?

¿Cómo revisaste el trabajo?

¿Cómo resolviste los problemas?

¿Cómo documentaste?

¿Qué aprendiste?
```

La presentación debe permitir reconstruir:

```text
intención
   ↓
trabajo
   ↓
evidencia
   ↓
resultado
```

---

# Criterio general

Los desafíos del Proyecto Final buscan desarrollar una competencia central:

> **tomar decisiones técnicas y poder justificarlas.**

No existe una única estrategia correcta para todos los proyectos.

Una solución puede ser adecuada en un proyecto y excesiva en otro.

Por eso, ante cada decisión preguntate:

```text
¿Qué necesito?
¿Qué alternativas tengo?
¿Qué costo tiene cada alternativa?
¿Qué riesgo implica?
¿Qué resultado espero?
```

---

# Cierre

El Proyecto Final es la instancia donde Git deja de ser el tema principal y pasa a convertirse en una herramienta dentro de un proceso.

El objetivo es llegar a:

```text
proyecto real
      ↓
trabajo organizado
      ↓
historial
      ↓
colaboración
      ↓
documentación
      ↓
evidencia
      ↓
presentación
```

> **El desafío final no es terminar un proyecto perfecto. Es demostrar que sabés trabajar sobre un proyecto de manera consciente, organizada y defendible.**