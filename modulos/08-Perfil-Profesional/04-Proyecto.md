# Proyecto
## Módulo 08 — Perfil Profesional

---

## 1. Propósito

En este proyecto vamos a integrar los conocimientos desarrollados durante el curso para transformar un proyecto técnico en una pieza de presentación profesional.

No se trata de crear una aplicación compleja.

El objetivo es construir una **evidencia concreta de trabajo técnico** que pueda ser comprendida, utilizada y explicada por otra persona.

El proyecto integra:

```text
Git
 ↓
GitHub
 ↓
Markdown
 ↓
documentación
 ↓
organización
 ↓
seguridad
 ↓
presentación profesional
```

---

# 2. Situación

Imaginá que terminaste un proyecto que querés presentar como parte de tu trayectoria técnica.

Una persona recibe solamente el enlace al repositorio.

No te conoce.

No conoce el contexto.

No sabe qué hiciste.

Debe poder descubrir:

```text
qué es
 ↓
qué problema resuelve
 ↓
cómo utilizarlo
 ↓
cómo está organizado
 ↓
qué tecnologías utiliza
 ↓
qué demuestra sobre vos
```

Tu tarea será preparar el repositorio para esa situación.

---

# 3. Objetivo general

Construir un repositorio técnicamente presentable que permita demostrar:

- capacidad para organizar un proyecto;
- utilización de Git;
- utilización de GitHub;
- documentación técnica;
- criterios básicos de seguridad;
- capacidad de explicar decisiones;
- capacidad de presentar evidencia de aprendizaje.

---

# 4. Modalidad

El proyecto puede realizarse:

### Individual

Es la modalidad recomendada.

Cada estudiante selecciona un proyecto propio y lo transforma en una pieza de portafolio.

### En equipo

Puede realizarse sobre un proyecto grupal.

En ese caso debe quedar claramente identificado:

```text
qué hizo el equipo
```

y:

```text
qué hizo cada integrante.
```

No debe atribuirse individualmente trabajo realizado por otras personas.

---

# 5. Elegir el proyecto

Seleccioná un proyecto que cumpla al menos una de estas condiciones:

- fue desarrollado durante el curso;
- fue realizado como trabajo académico;
- es un proyecto personal;
- representa un aprendizaje técnico importante;
- permite demostrar una capacidad concreta.

No es necesario comenzar un proyecto desde cero.

Una mejora profunda de un proyecto existente puede ser una excelente opción.

---

# 6. Criterio de selección

Antes de comenzar, respondé:

```text
¿Qué demuestra este proyecto?

¿Por qué quiero mostrarlo?

¿Qué aprendí realizándolo?

¿Puedo explicar cómo funciona?

¿Puedo explicar las decisiones importantes?
```

Si no podés responder estas preguntas, considerá elegir otro proyecto.

---

# 7. Estado inicial

Antes de realizar cambios, documentá el estado inicial.

Completá:

```text
Proyecto:
________________________

Objetivo:
________________________

Estado del README:
________________________

Estado del .gitignore:
________________________

Documentación:
________________________

Estructura:
________________________

Seguridad:
________________________

Presentación:
________________________
```

Este registro permitirá comparar:

```text
antes
 ↓
trabajo realizado
 ↓
después
```

---

# 8. Repositorio

El proyecto debe encontrarse en un repositorio Git.

El repositorio deberá contener como mínimo:

```text
README.md
.gitignore
```

Además, deberá contener los archivos propios del proyecto.

La estructura concreta dependerá del proyecto elegido.

---

# 9. README

El README será la principal puerta de entrada al proyecto.

Debe permitir comprender rápidamente:

```text
qué es
para qué sirve
cómo instalarlo
cómo utilizarlo
```

También debería proporcionar contexto suficiente para entender qué demuestra el proyecto.

---

# 10. Estructura sugerida del README

La siguiente estructura puede utilizarse como referencia:

```md
# Nombre del proyecto

Descripción breve.

## Objetivo

...

## Problema

...

## Solución

...

## Tecnologías

...

## Requisitos

...

## Instalación

...

## Uso

...

## Ejemplo

...

## Estructura

...

## Próximos pasos

...

## Licencia

...
```

No es obligatorio utilizar todas las secciones.

La estructura debe adaptarse al proyecto real.

---

# 11. Descripción

La descripción inicial debe responder:

> ¿Qué es este proyecto?

Evitar descripciones que solamente indiquen una tecnología.

Por ejemplo:

```text
Proyecto desarrollado en Python.
```

es insuficiente.

Debe explicarse qué hace el proyecto.

---

# 12. Objetivo

Incluir una sección que explique:

```text
¿Para qué se construyó?
```

El objetivo debe corresponder con el proyecto real.

No es necesario exagerar su alcance.

---

# 13. Problema

Explicar el problema o necesidad que originó el proyecto.

Puede tratarse de:

```text
una necesidad concreta
un ejercicio académico
un problema de aprendizaje
una automatización
una necesidad personal
```

Si el proyecto es principalmente educativo, indicarlo.

---

# 14. Solución

Explicar brevemente qué se construyó para abordar el problema.

Debe existir una relación clara:

```text
Problema
   ↓
Solución
```

---

# 15. Tecnologías

Indicar únicamente las tecnologías realmente utilizadas.

Por ejemplo:

```text
Python
Git
GitHub
Markdown
```

No incorporar tecnologías solamente porque sean conocidas o populares.

---

# 16. Requisitos

Documentar qué necesita una persona para utilizar el proyecto.

Por ejemplo:

```text
Python 3.x
Git
```

o cualquier otra dependencia real.

---

# 17. Instalación

Escribir instrucciones completas.

Por ejemplo:

```bash
git clone URL_DEL_REPOSITORIO
cd nombre-del-proyecto
```

Si existen dependencias, documentar cómo instalarlas.

Las instrucciones deben poder ser verificadas.

---

# 18. Prueba de instalación

La instalación debe probarse.

Siempre que sea posible, utilizar un entorno limpio.

El objetivo es verificar:

```text
README
 ↓
instalación
 ↓
ejecución
```

sin depender de conocimientos que no estén documentados.

---

# 19. Uso

Explicar cómo utilizar el proyecto.

Incluir comandos, parámetros o pasos cuando corresponda.

Por ejemplo:

```bash
python programa.py
```

La documentación debe corresponder con la versión actual del proyecto.

---

# 20. Ejemplo

Incluir al menos un ejemplo concreto cuando el proyecto lo permita.

Por ejemplo:

```text
Entrada
   ↓
procesamiento
   ↓
resultado
```

Un ejemplo debe ser verificable.

No incluir resultados ficticios.

---

# 21. Estructura

Si el proyecto posee varios archivos o directorios, documentar brevemente su organización.

Por ejemplo:

```text
proyecto/
├── README.md
├── src/
├── tests/
└── docs/
```

Explicar solamente las partes relevantes.

---

# 22. `.gitignore`

Revisar el archivo:

```text
.gitignore
```

Debe impedir el seguimiento de archivos que no correspondan al repositorio.

Por ejemplo:

```text
archivos temporales
entornos virtuales
configuraciones locales
archivos generados
```

Las reglas deben adaptarse al proyecto.

---

# 23. Seguridad

Antes de publicar el repositorio, verificar que no contenga:

```text
contraseñas
tokens
claves
credenciales
datos personales innecesarios
información confidencial
```

Esta revisión es obligatoria.

---

# 24. Información sensible

Si se encuentra información sensible:

```text
NO PUBLICARLA.
```

Analizar:

```text
qué información es
si ya fue registrada
si ya fue publicada
qué acciones corresponden
```

Agregar un archivo a `.gitignore` no elimina información que ya haya sido registrada en la historia.

---

# 25. Revisar el historial

Ejecutar:

```bash
git log --oneline --graph --all
```

Analizar:

```text
commits
ramas
mensajes
evolución
```

El objetivo es comprender qué evidencia existe sobre el proceso de desarrollo.

---

# 26. Crear una mejora

El proyecto debe incorporar al menos una mejora concreta.

Puede ser:

```text
documentación
código
estructura
ejemplo
prueba
organización
```

La mejora debe resolver una necesidad real.

---

# 27. Issue

Crear una Issue para la mejora.

Debe contener:

```md
## Problema

...

## Objetivo

...

## Resultado esperado

...
```

El título debe describir claramente la tarea.

---

# 28. Rama

Crear una rama específica para la mejora.

Por ejemplo:

```bash
git switch main
git switch -c docs-mejora
```

No realizar directamente el trabajo sobre `main`.

---

# 29. Trabajo

Realizar la mejora.

Mantener el cambio enfocado.

No aprovechar esta tarea para modificar arbitrariamente todo el proyecto.

El objetivo es poder identificar claramente:

```text
Issue
 ↓
rama
 ↓
cambio
```

---

# 30. Commit

Registrar el trabajo mediante un commit claro.

Por ejemplo:

```bash
git add .
git commit -m "Mejora documentación del proyecto"
```

El mensaje debe permitir comprender qué cambió.

---

# 31. Push

Publicar la rama:

```bash
git push -u origin docs-mejora
```

Verificar que la rama esté disponible en GitHub.

---

# 32. Pull Request

Crear una Pull Request hacia:

```text
main
```

La descripción debe explicar:

```md
## Qué hice

...

## Por qué

...

## Cómo lo probé

...

## Issue

...
```

---

# 33. Revisión

La Pull Request debe ser revisada.

Si el proyecto es individual, la revisión puede realizarla otro estudiante o el docente.

La revisión debe buscar:

```text
claridad
alcance
funcionamiento
documentación
calidad
```

---

# 34. Cambio solicitado

La Pull Request deberá recibir al menos una observación que implique una mejora.

El autor deberá responder realizando la modificación correspondiente.

El flujo será:

```text
Pull Request
      ↓
revisión
      ↓
observación
      ↓
corrección
      ↓
commit
      ↓
push
      ↓
nueva revisión
```

---

# 35. Integración

Una vez aprobada la Pull Request:

```text
merge
```

Después actualizar el repositorio local:

```bash
git switch main
git pull
```

Verificar:

```bash
git status
```

---

# 36. Revisar el resultado

Después de integrar el cambio, volver a revisar:

```text
README
.gitignore
estructura
historial
proyecto
```

Comprobar que la documentación continúa coincidiendo con el estado real.

---

# 37. Presentación profesional

El proyecto debe poder presentarse en pocos minutos.

Preparar una explicación de:

```text
3 a 5 minutos
```

Debe responder:

```text
¿Qué problema resuelve?

¿Qué construí?

¿Qué tecnologías utilicé?

¿Qué decisión importante tomé?

¿Qué dificultad encontré?

¿Qué aprendí?
```

---

# 38. Caso de estudio

Crear un archivo:

```text
CASO-DE-ESTUDIO.md
```

con la siguiente estructura:

```md
# Caso de estudio

## Problema

...

## Contexto

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

No es necesario que sea extenso.

Debe ser concreto y honesto.

---

# 39. Habilidades demostradas

Agregar al caso de estudio una sección:

```md
## Habilidades demostradas
```

Relacionar cada capacidad con evidencia real.

Por ejemplo:

```text
Git → historial y commits
GitHub → Pull Request
Markdown → documentación
Programación → código
Colaboración → revisión
```

No incluir capacidades que el proyecto no permita demostrar.

---

# 40. Perfil profesional

Revisar el perfil de GitHub.

El objetivo es seleccionar información relevante.

Definir:

```text
proyecto principal
proyectos secundarios
tecnologías
presentación
```

No es obligatorio modificar todos los elementos del perfil.

---

# 41. Curaduría

Revisar los repositorios existentes.

Clasificarlos:

```text
Mostrar
Mejorar
Privado
Archivar
```

No es necesario eliminar repositorios.

La intención es aprender a seleccionar qué evidencia resulta relevante.

---

# 42. Coherencia

Comparar:

```text
perfil
README
proyectos
CASO-DE-ESTUDIO.md
```

Preguntarse:

> ¿Todos representan de manera coherente mi nivel y mi recorrido actual?

No deben existir afirmaciones que no puedan sostenerse con evidencia.

---

# 43. Entrega

La entrega debe contener:

```text
Repositorio GitHub
README.md
.gitignore
CASO-DE-ESTUDIO.md
```

Además debe existir evidencia de:

```text
Issue
rama
commit
Pull Request
revisión
corrección
merge
```

---

# 44. Presentación

Durante la presentación, el estudiante deberá mostrar:

1. el proyecto;
2. el README;
3. la estructura;
4. la evidencia de Git;
5. la Issue;
6. la Pull Request;
7. la revisión;
8. la corrección;
9. la integración;
10. el caso de estudio.

No es necesario mostrar absolutamente cada archivo.

La presentación debe centrarse en las decisiones y evidencias principales.

---

# 45. Preguntas de defensa

El docente puede preguntar:

> ¿Por qué elegiste este proyecto?

> ¿Qué problema resuelve?

> ¿Qué parte fue más difícil?

> ¿Por qué elegiste esa tecnología?

> ¿Qué información decidiste no publicar?

> ¿Qué función cumple `.gitignore`?

> ¿Qué evidencia existe de tu trabajo?

> ¿Qué aprendiste?

> ¿Qué mejorarías?

> ¿Qué cambiarías si otra persona tuviera que colaborar en el proyecto?

---

# 46. Requisitos mínimos

Para considerar completo el proyecto deberán cumplirse:

### Repositorio

- repositorio Git;
- repositorio disponible en GitHub;
- README actualizado;
- `.gitignore` revisado.

### Documentación

- descripción;
- objetivo;
- instalación;
- uso;
- ejemplo;
- tecnologías;
- caso de estudio.

### Git

- rama de trabajo;
- commits claros;
- historial verificable.

### GitHub

- Issue;
- Pull Request;
- revisión;
- corrección;
- merge.

### Seguridad

- sin secretos publicados;
- sin información confidencial innecesaria.

### Presentación

- explicación oral;
- capacidad para justificar decisiones.

---

# 47. Criterios de evaluación

## 1. Proyecto

Se evaluará:

- claridad;
- coherencia;
- funcionamiento cuando corresponda;
- organización.

## 2. Documentación

Se evaluará:

- claridad;
- precisión;
- utilidad;
- correspondencia con el proyecto real.

## 3. Git y GitHub

Se evaluará:

- uso de ramas;
- commits;
- Issues;
- Pull Requests;
- revisión;
- integración.

## 4. Seguridad

Se evaluará:

- identificación de información sensible;
- utilización adecuada de `.gitignore`;
- criterio de publicación.

## 5. Comunicación

Se evaluará:

- capacidad para explicar;
- capacidad para justificar decisiones;
- honestidad técnica;
- claridad de la presentación.

---

# 48. No se evalúa la cantidad

No se evaluará:

```text
cantidad de commits
cantidad de repositorios
cantidad de seguidores
cantidad de estrellas
```

El foco está puesto en:

```text
calidad
evidencia
comprensión
documentación
criterio
```

---

# 49. Resultado esperado

Al finalizar el proyecto debería existir una pieza que pueda resumirse así:

```text
Proyecto real
      ↓
repositorio organizado
      ↓
documentación clara
      ↓
seguridad revisada
      ↓
historial comprensible
      ↓
mejora registrada
      ↓
Pull Request revisada
      ↓
integración
      ↓
caso de estudio
      ↓
presentación
```

El resultado no tiene que parecer un proyecto empresarial.

Tiene que ser **real, comprensible, defendible y técnicamente honesto**.

---

# 50. Reflexión final

Respondé:

### 1.

¿Qué demuestra este proyecto sobre mi forma de trabajar?

### 2.

¿Qué evidencia concreta puedo mostrar?

### 3.

¿Qué aprendí durante el proceso?

### 4.

¿Qué parte del proyecto todavía necesita mejorar?

### 5.

¿Qué haría diferente si comenzara nuevamente?

### 6.

¿Qué otro proyecto debería construir para continuar mi recorrido?

---

# 51. Cierre

Este proyecto representa el cierre del recorrido inicial del curso.

Comenzamos aprendiendo a controlar versiones.

Después aprendimos a trabajar con ramas, GitHub, Markdown y colaboración.

Ahora damos un paso más:

```text
trabajo técnico
      ↓
evidencia
      ↓
presentación
```

El objetivo no es terminar con un perfil perfecto.

El objetivo es terminar sabiendo cómo transformar el trabajo que hacemos en una evidencia que otras personas puedan comprender.

> **Tu perfil profesional se construye con el trabajo que hacés, pero también con la capacidad de explicarlo, documentarlo y mostrarlo.**