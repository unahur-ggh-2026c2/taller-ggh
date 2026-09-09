# Proyecto Final
## Módulo 09 — Proyecto Final

---

# 1. Propósito

El Proyecto Final integra los conocimientos trabajados durante todo el curso.

La propuesta no consiste en demostrar que conocés una lista de comandos.

Consiste en demostrar que podés utilizar Git y GitHub dentro de un proceso completo de trabajo.

El proyecto debe permitir observar:

```text
planificación
   ↓
organización
   ↓
desarrollo
   ↓
versionado
   ↓
documentación
   ↓
colaboración
   ↓
revisión
   ↓
integración
   ↓
presentación
```

---

# 2. Consigna general

Desarrollá un proyecto utilizando Git y GitHub como herramientas de trabajo.

El proyecto puede ser:

- un programa;
- una aplicación;
- una herramienta;
- un proyecto académico;
- un proyecto personal;
- material educativo;
- documentación técnica;
- otro proyecto acordado con el docente.

No se busca construir el sistema más grande posible.

Se busca construir un proyecto que pueda ser:

```text
terminado
documentado
versionado
revisado
explicado
```

---

# 3. Objetivo

Al finalizar el proyecto deberás poder demostrar que sos capaz de:

```text
crear un repositorio
        ↓
organizar el trabajo
        ↓
registrar cambios
        ↓
trabajar con ramas
        ↓
utilizar GitHub
        ↓
documentar
        ↓
revisar cambios
        ↓
integrar
        ↓
presentar el resultado
```

---

# 4. Elección del proyecto

Elegí un proyecto que tenga un alcance razonable.

Antes de comenzar, completá:

```text
Nombre del proyecto:

________________________________________

Problema que resuelve:

________________________________________

Objetivo:

________________________________________

Usuario o destinatario:

________________________________________
```

---

# 5. Alcance

Definí claramente qué incluirá el proyecto.

```text
El proyecto incluirá:

- ______________________________
- ______________________________
- ______________________________
```

Y qué quedará fuera:

```text
El proyecto no incluirá:

- ______________________________
- ______________________________
- ______________________________
```

Definir límites es parte del proyecto.

---

# 6. Versión mínima

Definí cuál será la versión mínima que permita considerar terminado el proyecto.

```text
La versión mínima permitirá:

- ______________________________
- ______________________________
- ______________________________
```

Las funcionalidades adicionales pueden quedar como mejoras futuras.

---

# 7. Planificación

Dividí el proyecto en tareas.

Por ejemplo:

```text
1. Crear estructura inicial.
2. Implementar funcionalidad principal.
3. Agregar validaciones.
4. Documentar instalación.
5. Agregar ejemplos.
6. Realizar pruebas.
7. Preparar presentación.
```

Las tareas deben representar trabajo real.

---

# 8. Issue

Creá una Issue para cada tarea relevante.

La Issue debe contener como mínimo:

```md
## Problema

...

## Objetivo

...

## Resultado esperado

...
```

No es necesario crear Issues artificialmente para aumentar la cantidad.

---

# 9. Repositorio

Creá el repositorio Git.

Si el proyecto todavía no utiliza Git:

```bash
git init
```

Verificá:

```bash
git status
```

Después prepará la estructura inicial.

---

# 10. Estructura inicial

Creá una estructura coherente con el proyecto.

Como referencia:

```text
proyecto/
├── README.md
├── .gitignore
└── src/
```

La estructura final dependerá de las características del proyecto.

---

# 11. README inicial

Creá:

```text
README.md
```

Incluí inicialmente:

```md
# Nombre del proyecto

Descripción breve.

## Objetivo

...

## Estado

En desarrollo.
```

La documentación deberá evolucionar junto con el proyecto.

---

# 12. `.gitignore`

Creá:

```text
.gitignore
```

Incluí los archivos que no deban formar parte del repositorio.

Por ejemplo:

```gitignore
.env
.venv/
__pycache__/
*.log
```

Las reglas deben adaptarse al proyecto.

---

# 13. Primer commit

Revisá:

```bash
git status
```

Después:

```bash
git add .
```

y:

```bash
git commit -m "Inicializa estructura del proyecto"
```

El commit debe representar el estado inicial.

---

# 14. GitHub

Creá el repositorio remoto y vinculalo con el repositorio local.

Verificá:

```bash
git remote -v
```

Después publicá la rama principal:

```bash
git push -u origin main
```

---

# 15. Rama de trabajo

Seleccioná una tarea concreta.

Creá una rama:

```bash
git switch -c feature-nombre
```

Trabajá sobre esa rama.

La rama debe representar un cambio o conjunto de cambios relacionados.

---

# 16. Desarrollo

Implementá la tarea.

Durante el trabajo utilizá:

```bash
git status
```

y:

```bash
git diff
```

para revisar el estado y los cambios.

---

# 17. Commits

Registrá cambios coherentes.

Por ejemplo:

```bash
git add .
git commit -m "Implementa búsqueda de libros"
```

Los mensajes deben permitir comprender qué se modificó.

Evitá mensajes como:

```text
cambios
cosas
final
fix
```

cuando no aporten información útil.

---

# 18. Publicar la rama

Publicá la rama:

```bash
git push -u origin feature-nombre
```

Verificá que aparezca en GitHub.

---

# 19. Pull Request

Creá una Pull Request hacia:

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
```

Si corresponde, vinculá la Issue relacionada.

---

# 20. Revisión

La Pull Request debe ser revisada.

El revisor debe considerar:

```text
objetivo
alcance
funcionamiento
claridad
documentación
posibles mejoras
```

No alcanza con comprobar solamente que el programa funcione.

---

# 21. Corrección

Si la revisión produce observaciones, realizá las correcciones necesarias.

El flujo será:

```text
revisión
   ↓
feedback
   ↓
corrección
   ↓
commit
   ↓
push
```

La Pull Request debe actualizarse con los nuevos cambios.

---

# 22. Integración

Una vez aprobada la Pull Request:

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

# 23. Repetir el ciclo

Continuá el desarrollo utilizando ciclos similares:

```text
Issue
 ↓
rama
 ↓
desarrollo
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

No es necesario que todos los cambios tengan exactamente la misma estructura.

El flujo debe adaptarse al proyecto.

---

# 24. Colaboración

Si el proyecto es grupal, cada integrante debe participar de manera real.

El trabajo puede distribuirse mediante:

```text
Issues
ramas
commits
Pull Requests
revisiones
```

La actividad debe corresponder con trabajo efectivo.

No se debe generar actividad artificial para mejorar las métricas del repositorio.

---

# 25. Conflictos

Durante el trabajo colaborativo puede producirse un conflicto.

Si ocurre:

1. identificá el archivo;
2. analizá las modificaciones;
3. comprendé qué intentaba hacer cada rama;
4. decidí el resultado correcto;
5. resolvé el conflicto;
6. verificá el resultado;
7. continuá el proceso.

No elijas automáticamente una de las versiones.

---

# 26. Prueba después del conflicto

Después de resolver un conflicto:

```text
revisar
   ↓
probar
   ↓
verificar
```

La ausencia de marcas de conflicto no garantiza que el resultado sea correcto.

---

# 27. Documentación

A medida que el proyecto avance, actualizá el README.

Cuando cambie:

```text
instalación
uso
dependencias
estructura
funcionalidades
```

también deberá actualizarse la documentación.

---

# 28. README final

El README debería incluir, cuando corresponda:

```text
Nombre
Descripción
Objetivo
Problema
Solución
Tecnologías
Requisitos
Instalación
Uso
Ejemplo
Estructura
Estado
Próximos pasos
Licencia
```

No es obligatorio utilizar todas las secciones.

---

# 29. Ejemplo reproducible

Agregá al README al menos un ejemplo que pueda ser reproducido.

Debe permitir observar:

```text
entrada
   ↓
ejecución
   ↓
resultado
```

El resultado documentado debe coincidir con el comportamiento real del proyecto.

---

# 30. Prueba de documentación

Pedile a otra persona que intente instalar y utilizar el proyecto siguiendo únicamente el README.

No le des instrucciones adicionales.

Registrá:

```text
Paso
Resultado
Problema
Corrección
```

Después actualizá la documentación.

---

# 31. Seguridad

Antes de la entrega revisá:

```text
contraseñas
tokens
claves
credenciales
datos personales
información confidencial
```

El repositorio no debe contener información sensible que no corresponda publicar.

---

# 32. Revisión del `.gitignore`

Comprobá que `.gitignore` contemple los archivos apropiados para el proyecto.

Podés utilizar:

```bash
git check-ignore -v archivo
```

para investigar por qué un archivo está siendo ignorado.

---

# 33. Revisar el historial

Ejecutá:

```bash
git log --oneline --graph --all
```

Analizá:

```text
commits
ramas
merges
evolución
```

Preguntate:

> ¿La historia permite comprender cómo evolucionó el proyecto?

---

# 34. Revisar el estado

Ejecutá:

```bash
git status
```

Antes de entregar, el repositorio debería encontrarse en un estado conocido y coherente.

No debería haber cambios pendientes que hayas olvidado registrar.

---

# 35. Caso de estudio

Creá:

```text
CASO-DE-ESTUDIO.md
```

Utilizá:

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

# 36. Decisiones

Documentá entre una y tres decisiones importantes.

Para cada una:

```text
Decisión:
________________________

Alternativas:
________________________

Elección:
________________________

Motivo:
________________________

Resultado:
________________________
```

---

# 37. Dificultades

Documentá problemas importantes encontrados durante el desarrollo.

```text
Problema:
________________________

Investigación:
________________________

Solución:
________________________

Aprendizaje:
________________________
```

No hace falta ocultar los problemas.

Los problemas también forman parte de la historia del proyecto.

---

# 38. Resultado

Describí qué quedó funcionando al finalizar.

Separá:

```text
Implementado
```

de:

```text
Pendiente
```

Esto permite presentar el estado real del proyecto.

---

# 39. Próximos pasos

Definí mejoras futuras.

Por ejemplo:

```text
1. ______________________
2. ______________________
3. ______________________
```

No es necesario implementarlas para completar el proyecto si quedan fuera del alcance definido.

---

# 40. Preparar la presentación

Prepará una presentación de entre:

```text
5 y 10 minutos
```

Deberías poder explicar:

```text
1. Problema.
2. Objetivo.
3. Solución.
4. Tecnologías.
5. Organización.
6. Git.
7. GitHub.
8. Dificultades.
9. Resultado.
10. Aprendizajes.
```

---

# 41. Defensa oral

Durante la presentación deberás poder responder preguntas sobre:

```text
proyecto
Git
GitHub
ramas
commits
Issues
Pull Requests
revisión
conflictos
documentación
seguridad
```

Las respuestas deben basarse en el trabajo realizado.

---

# 42. Evidencias

El proyecto debe permitir encontrar evidencia de:

```text
trabajo
   ↓
decisiones
   ↓
cambios
   ↓
revisión
   ↓
resultado
```

Las evidencias pueden encontrarse en:

```text
repositorio
historial
Issues
Pull Requests
README
caso de estudio
```

---

# 43. Entrega final

La entrega deberá incluir como mínimo:

```text
Repositorio GitHub
README.md
.gitignore
CASO-DE-ESTUDIO.md
```

Y, según la modalidad:

```text
Issues
ramas
commits
Pull Requests
revisiones
integraciones
```

---

# 44. Checklist

Antes de entregar, verificá:

```text
[ ] El proyecto tiene un objetivo claro.
[ ] El alcance está definido.
[ ] El repositorio está disponible.
[ ] README está actualizado.
[ ] .gitignore fue revisado.
[ ] No hay secretos publicados.
[ ] Las tareas relevantes están registradas.
[ ] Las ramas fueron utilizadas cuando correspondía.
[ ] Los commits son comprensibles.
[ ] Las Pull Requests necesarias fueron revisadas.
[ ] Los cambios fueron integrados.
[ ] El proyecto fue probado.
[ ] La documentación coincide con el proyecto.
[ ] El caso de estudio está completo.
[ ] La presentación está preparada.
```

---

# 45. Evaluación

Se evaluarán cinco dimensiones principales.

## Proyecto

```text
claridad
organización
coherencia
resultado
```

## Git

```text
commits
ramas
historial
integración
```

## GitHub

```text
repositorio
Issues
Pull Requests
revisiones
```

## Documentación

```text
README
instrucciones
ejemplos
caso de estudio
```

## Presentación

```text
comprensión
comunicación
justificación
reflexión
```

---

# 46. No se evalúa cantidad

No se evaluará como objetivo:

```text
cantidad de commits
cantidad de ramas
cantidad de Issues
cantidad de Pull Requests
```

El criterio será:

```text
¿Son necesarias?
¿Son coherentes?
¿Representan trabajo real?
¿Permiten observar el proceso?
```

---

# 47. Proyecto individual

Si el proyecto es individual, no es necesario fabricar una dinámica de equipo.

Puede utilizarse un flujo como:

```text
Issue
 ↓
rama
 ↓
commit
 ↓
Pull Request
 ↓
revisión
 ↓
corrección
 ↓
merge
```

La revisión puede realizarla el docente o un compañero.

---

# 48. Proyecto grupal

Si el proyecto es grupal, el equipo debe poder demostrar colaboración real.

Se recomienda utilizar:

```text
Issues
ramas
Pull Requests
revisiones
```

Cada integrante debe conocer el funcionamiento general del proyecto y poder explicar su participación.

---

# 49. Reflexión final

Respondé:

```text
¿Qué aprendí durante el proyecto?

¿Qué parte fue más difícil?

¿Qué decisión fue más importante?

¿Qué problema resolví utilizando Git?

¿Qué problema resolví utilizando GitHub?

¿Qué aprendí trabajando con otras personas?

¿Qué mejoraría?

¿Qué quiero seguir aprendiendo?
```

---

# 50. Cierre

El Proyecto Final representa el cierre del recorrido.

Durante el curso aprendimos:

```text
Git
 ↓
repositorios
 ↓
cambios
 ↓
historial
 ↓
GitHub
 ↓
Markdown
 ↓
ramas
 ↓
colaboración
 ↓
perfil profesional
```

Ahora integramos todo en una experiencia completa.

El resultado esperado no es un proyecto perfecto.

Es un proyecto que pueda ser:

```text
mostrado
explicado
documentado
revisado
defendido
```

> **El objetivo final no es demostrar que sabés usar Git. Es demostrar que podés trabajar con Git.**