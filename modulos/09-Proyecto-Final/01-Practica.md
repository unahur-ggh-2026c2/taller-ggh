# Práctica
## Módulo 09 — Proyecto Final

---

## 1. Objetivo

En esta práctica vamos a preparar el Proyecto Final antes de comenzar su desarrollo.

La intención es aplicar de manera integrada lo trabajado durante el curso:

```text
planificar
   ↓
organizar
   ↓
versionar
   ↓
documentar
   ↓
colaborar
   ↓
revisar
   ↓
integrar
   ↓
presentar
```

No vamos a empezar escribiendo código.

Primero vamos a organizar el trabajo.

---

# 2. Elegir el proyecto

Seleccioná un proyecto que pueda desarrollarse durante el Proyecto Final.

Puede ser:

- un programa;
- una aplicación;
- una herramienta;
- un proyecto académico;
- un proyecto personal;
- material educativo;
- documentación técnica;
- otro proyecto acordado con el docente.

No hace falta que sea grande.

Debe ser suficientemente concreto como para poder completarlo y presentarlo.

---

# 3. Definir el problema

Antes de pensar en tecnologías, describí qué problema querés resolver.

Completá:

```text
Problema:

________________________________________

¿Quién tiene este problema?

________________________________________

¿Por qué vale la pena resolverlo?

________________________________________
```

Si se trata de un proyecto académico, explicá también el contexto.

---

# 4. Definir el objetivo

Escribí una descripción breve del resultado que querés alcanzar.

Completá:

```text
Objetivo:

________________________________________
```

El objetivo debe ser concreto.

Evitá formular objetivos demasiado amplios como:

```text
Crear una aplicación completa para gestionar todo.
```

Buscá algo que pueda ser desarrollado y evaluado durante el proyecto.

---

# 5. Definir el alcance

Ahora establecé qué va a formar parte del proyecto.

Completá:

```text
El proyecto incluirá:

- ______________________________
- ______________________________
- ______________________________
```

Después definí qué queda fuera:

```text
El proyecto NO incluirá:

- ______________________________
- ______________________________
- ______________________________
```

Definir lo que no vas a hacer también es parte de planificar.

---

# 6. Definir un resultado mínimo

Pensá en la versión más pequeña que permita considerar que el proyecto funciona.

Completá:

```text
Versión mínima:

________________________________________
```

Esta versión será tu referencia inicial.

Después podrás agregar mejoras.

---

# 7. Identificar tareas

Dividí el proyecto en tareas pequeñas.

Por ejemplo:

```text
1. Crear estructura inicial.
2. Implementar funcionalidad principal.
3. Agregar validaciones.
4. Documentar instalación.
5. Agregar ejemplo.
6. Revisar proyecto.
```

No intentes definir absolutamente todo desde el principio.

La planificación también puede evolucionar.

---

# 8. Crear el repositorio

Creá el repositorio Git.

Si el proyecto ya existe, verificá que se encuentre correctamente bajo control de versiones.

Inicializá Git cuando corresponda:

```bash
git init
```

Después verificá:

```bash
git status
```

---

# 9. Crear la estructura inicial

Organizá la estructura básica del proyecto.

Por ejemplo:

```text
proyecto/
├── README.md
├── .gitignore
└── src/
```

La estructura real dependerá del proyecto.

No agregues directorios solamente porque aparezcan en un ejemplo.

---

# 10. Crear el README inicial

Antes de comenzar el desarrollo, creá:

```text
README.md
```

Incluí como mínimo:

```md
# Nombre del proyecto

Descripción breve.

## Objetivo

...

## Estado

En desarrollo.
```

No es necesario completar todavía toda la documentación.

El README evolucionará junto con el proyecto.

---

# 11. Crear `.gitignore`

Identificá qué archivos o directorios no deberían incorporarse al repositorio.

Creá:

```text
.gitignore
```

Incluí solamente reglas necesarias para el proyecto.

Por ejemplo:

```gitignore
__pycache__/
.venv/
.env
*.log
```

Adaptá las reglas a las tecnologías realmente utilizadas.

---

# 12. Revisar seguridad

Antes de comenzar, establecé qué información nunca debería formar parte del repositorio.

Por ejemplo:

```text
contraseñas
tokens
claves
credenciales
datos personales
configuraciones sensibles
```

Si el proyecto necesita configuración local, pensá cómo manejarla sin publicar secretos.

---

# 13. Primer commit

Una vez preparada la estructura inicial:

```bash
git status
```

Revisá qué archivos serán registrados.

Después:

```bash
git add .
```

y:

```bash
git commit -m "Inicializa estructura del proyecto"
```

El primer commit debería representar realmente el inicio del proyecto.

---

# 14. Crear el repositorio remoto

Creá el repositorio correspondiente en GitHub.

Conectá el repositorio local con el remoto.

Verificá:

```bash
git remote -v
```

Después publicá la rama principal:

```bash
git push -u origin main
```

Si utilizás otro nombre para la rama principal, adaptá el comando.

---

# 15. Crear las primeras Issues

Transformá las tareas principales en Issues.

Por ejemplo:

```text
#1 Crear estructura inicial
#2 Implementar funcionalidad principal
#3 Agregar validaciones
#4 Documentar instalación
```

No es necesario convertir absolutamente cada tarea en una Issue.

La intención es utilizar Issues para organizar trabajo real.

---

# 16. Priorizar

Asigná una prioridad a las tareas.

Por ejemplo:

```text
Alta
Media
Baja
```

Identificá qué tarea debe realizarse primero.

La prioridad puede cambiar durante el desarrollo.

---

# 17. Crear una rama de trabajo

Elegí una tarea concreta.

Por ejemplo:

```text
Implementar funcionalidad principal
```

Creá una rama:

```bash
git switch -c feature-funcionalidad-principal
```

Verificá:

```bash
git branch
```

---

# 18. Trabajar en la rama

Realizá solamente los cambios relacionados con la tarea.

Durante el desarrollo utilizá:

```bash
git status
```

para revisar el estado del repositorio.

También podés utilizar:

```bash
git diff
```

para observar exactamente qué cambió.

---

# 19. Registrar avances

Cuando exista un cambio coherente:

```bash
git add .
git commit -m "Implementa funcionalidad principal"
```

El mensaje debe explicar qué cambio se registró.

No es necesario crear un commit por cada pequeña modificación.

Buscá unidades de trabajo coherentes.

---

# 20. Publicar la rama

Cuando corresponda:

```bash
git push -u origin feature-funcionalidad-principal
```

Verificá que la rama aparezca en GitHub.

---

# 21. Crear la Pull Request

Creá una Pull Request desde:

```text
feature-funcionalidad-principal
```

hacia:

```text
main
```

La descripción debería explicar:

```text
qué se hizo
por qué
cómo se verificó
```

Si corresponde, vinculá la Issue relacionada.

---

# 22. Revisar la Pull Request

La revisión debe buscar:

```text
¿El cambio resuelve la tarea?

¿Está correctamente implementado?

¿La documentación es suficiente?

¿Hay algo que pueda mejorarse?

¿El cambio afecta otra parte del proyecto?
```

Si el proyecto es individual, la revisión puede realizarla otro estudiante o el docente.

---

# 23. Incorporar feedback

Si recibís una observación, analizala.

No aceptes ni rechaces automáticamente una sugerencia.

Preguntate:

```text
¿Qué problema está señalando?

¿Por qué importa?

¿Cómo puedo resolverlo?
```

Después realizá la corrección.

---

# 24. Nuevo commit

Registrá la corrección:

```bash
git add .
git commit -m "Corrige observaciones de revisión"
```

Después:

```bash
git push
```

La Pull Request debería actualizarse automáticamente.

---

# 25. Integrar

Cuando la Pull Request esté revisada y aprobada:

```text
merge
```

Después actualizá el repositorio local:

```bash
git switch main
git pull
```

Verificá:

```bash
git status
```

---

# 26. Repetir el ciclo

Continuá desarrollando el proyecto mediante ciclos similares:

```text
Issue
 ↓
rama
 ↓
cambio
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

No es necesario que todas las tareas tengan exactamente la misma secuencia si la naturaleza del proyecto no lo requiere.

---

# 27. Mantener `main` estable

La rama principal debería representar un estado razonablemente estable del proyecto.

Evitá utilizarla como espacio de experimentación permanente.

La idea es:

```text
main
 ↓
versión integrada
```

mientras que las ramas permiten desarrollar cambios.

---

# 28. Resolver un conflicto

Si el proyecto es colaborativo, puede aparecer un conflicto durante una integración.

Cuando ocurra:

1. identificá el archivo afectado;
2. observá las diferentes versiones;
3. comprendé qué intentaba hacer cada cambio;
4. decidí qué resultado necesita el proyecto;
5. resolvé el conflicto;
6. verificá el resultado;
7. registrá la resolución.

No resuelvas un conflicto simplemente eligiendo una de las versiones sin analizarla.

---

# 29. Verificar después de un conflicto

Después de resolverlo:

```bash
git status
```

Revisá el archivo.

Después verificá el proyecto.

Finalmente registrá la resolución cuando corresponda.

La resolución de conflictos debe comprobarse, no solamente marcarse como terminada.

---

# 30. Actualizar el README

A medida que el proyecto avance, mantené actualizado:

```text
README.md
```

Si cambia:

```text
instalación
uso
estructura
dependencias
funcionalidades
```

la documentación también debe cambiar.

No esperes hasta el último día.

---

# 31. Agregar un ejemplo

Cuando el proyecto tenga una funcionalidad demostrable, incorporá un ejemplo al README.

Por ejemplo:

```text
Entrada
   ↓
ejecución
   ↓
resultado
```

El ejemplo debe poder reproducirse.

---

# 32. Revisar la documentación

Pedile a otra persona que intente utilizar el proyecto siguiendo solamente el README.

Registrá:

```text
qué pudo hacer
qué no pudo hacer
qué información faltaba
```

Después corregí la documentación.

---

# 33. Revisar el historial

Ejecutá:

```bash
git log --oneline --graph --all
```

Observá:

```text
commits
ramas
merges
evolución
```

Preguntate:

> ¿La historia permite comprender cómo evolucionó el proyecto?

---

# 34. Revisar los mensajes

Identificá commits poco claros.

Por ejemplo:

```text
cambios
fix
final
cosas
```

No es necesario reescribir la historia para este ejercicio.

El objetivo es reconocer cómo mejorar la calidad de futuros commits.

---

# 35. Revisar el repositorio

Ejecutá:

```bash
git status
```

Después revisá en GitHub:

```text
README
Issues
Pull Requests
ramas
historial
archivos
```

Buscá inconsistencias.

---

# 36. Auditoría de seguridad

Antes de publicar la versión final, revisá nuevamente:

```text
contraseñas
tokens
claves
credenciales
datos personales
archivos locales
archivos temporales
```

También verificá:

```text
.gitignore
```

No supongas que porque el proyecto funcionó localmente es seguro publicarlo.

---

# 37. Revisar archivos ignorados

Verificá que `.gitignore` cumpla su función.

Ejecutá:

```bash
git status
```

Si necesitás investigar por qué un archivo está siendo ignorado, podés utilizar:

```bash
git check-ignore -v archivo
```

Este comando permite identificar qué regla está provocando la exclusión.

---

# 38. Preparar la versión final

Definí qué significa:

```text
"terminado"
```

para tu proyecto.

Completá:

```text
La versión final deberá permitir:

- ______________________________
- ______________________________
- ______________________________
```

No agregues nuevas funcionalidades importantes después de definir el alcance final, salvo que sea necesario y pueda ser absorbido por el tiempo disponible.

---

# 39. Revisar requisitos

Compará el proyecto con los objetivos definidos al principio.

Completá:

| Objetivo | Estado |
|---|---|
| | Cumplido / Parcial / Pendiente |
| | Cumplido / Parcial / Pendiente |
| | Cumplido / Parcial / Pendiente |

Si algo quedó pendiente, documentalo.

No intentes ocultarlo.

---

# 40. Preparar la documentación final

El README debería incluir, cuando corresponda:

```text
nombre
descripción
objetivo
problema
solución
tecnologías
requisitos
instalación
uso
ejemplo
estructura
estado
próximos pasos
licencia
```

No es obligatorio utilizar todas las secciones.

La documentación debe adaptarse al proyecto.

---

# 41. Documentar decisiones

Identificá entre una y tres decisiones técnicas importantes.

Para cada una:

```text
Decisión:
____________________

¿Por qué?
____________________

Alternativas consideradas:
____________________

Resultado:
____________________
```

Esto permite demostrar que el proyecto no fue construido de manera completamente arbitraria.

---

# 42. Documentar dificultades

Registrá los principales problemas encontrados.

Por ejemplo:

```text
Problema:
____________________

Cómo lo investigué:
____________________

Solución:
____________________

Qué aprendí:
____________________
```

Esta información puede utilizarse posteriormente en la presentación.

---

# 43. Preparar el caso de estudio

Creá:

```text
CASO-DE-ESTUDIO.md
```

Incluí:

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

---

# 44. Preparar la presentación

La presentación debería poder explicar:

```text
1. Problema
2. Solución
3. Tecnologías
4. Organización
5. Git
6. GitHub
7. Dificultades
8. Resultado
9. Aprendizajes
10. Próximos pasos
```

No es necesario mostrar cada comando ejecutado.

Hay que mostrar el proceso de manera comprensible.

---

# 45. Practicar

Realizá una presentación de prueba.

Intentá explicar el proyecto sin leer el README.

Después verificá:

```text
¿Puedo explicar el problema?

¿Puedo explicar la solución?

¿Puedo justificar decisiones?

¿Puedo explicar cómo utilicé Git?

¿Puedo explicar cómo utilicé GitHub?

¿Puedo reconocer limitaciones?
```

---

# 46. Preparar la defensa

Pensá qué preguntas podría realizar otra persona.

Por ejemplo:

```text
¿Por qué elegiste esta tecnología?

¿Por qué utilizaste esta rama?

¿Qué representa este commit?

¿Por qué existe esta Issue?

¿Qué problema resolvió esta Pull Request?

¿Cómo resolviste este conflicto?

¿Qué mejorarías?
```

Prepará las respuestas utilizando evidencia del repositorio.

---

# 47. Auditoría final

Antes de entregar, ejecutá:

```bash
git status
```

```bash
git log --oneline --graph --all
```

Después revisá GitHub.

Comprobá:

```text
[ ] README actualizado.
[ ] .gitignore revisado.
[ ] Sin secretos.
[ ] Sin archivos innecesarios.
[ ] Historial comprensible.
[ ] Ramas integradas.
[ ] Issues relevantes.
[ ] Pull Requests revisadas.
[ ] Documentación completa.
[ ] Proyecto en estado consistente.
```

---

# 48. Entrega

La entrega deberá incluir:

```text
Repositorio GitHub
README.md
.gitignore
CASO-DE-ESTUDIO.md
```

Además, deberá existir evidencia del proceso de trabajo:

```text
Issues
ramas
commits
Pull Requests
revisiones
integraciones
```

según la modalidad del proyecto.

---

# 49. Reflexión final

Respondé:

### 1.

¿Qué aprendí durante el desarrollo que no sabía al comenzar?

### 2.

¿Qué parte del proyecto me resultó más difícil?

### 3.

¿Qué problema resolví utilizando Git?

### 4.

¿Qué problema resolví utilizando GitHub?

### 5.

¿Qué decisión técnica fue la más importante?

### 6.

¿Qué error cometí y cómo lo resolví?

### 7.

¿Qué parte del proyecto mejoraría?

### 8.

¿Qué aprendí sobre trabajar con otras personas?

### 9.

¿Qué evidencia puedo mostrar de mi trabajo?

### 10.

¿Qué aprendí sobre mi propia forma de trabajar?

---

# 50. Cierre

El Proyecto Final no termina cuando el código funciona.

Termina cuando podés:

```text
mostrarlo
   ↓
explicarlo
   ↓
justificarlo
   ↓
documentarlo
   ↓
reconocer sus limitaciones
```

El objetivo de todo el recorrido fue llegar a este punto.

No solamente saber ejecutar comandos.

Sino poder utilizar Git y GitHub como herramientas dentro de un proceso de trabajo real.

> **Un proyecto terminado no es solamente un conjunto de archivos. Es también una historia de decisiones, cambios, problemas, soluciones y aprendizajes.**