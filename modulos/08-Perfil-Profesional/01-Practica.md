# Práctica
## Módulo 08 — Perfil Profesional

---

## 1. Objetivo

En esta práctica vamos a transformar un proyecto técnico en una pieza que pueda ser presentada profesionalmente.

No vamos a inventar experiencia.

Vamos a trabajar sobre evidencia real:

```text
proyecto
   ↓
organización
   ↓
documentación
   ↓
seguridad
   ↓
presentación
```

La pregunta que guía toda la práctica es:

> **Si otra persona encuentra este repositorio, ¿puede entender qué hice, cómo funciona y qué demuestra sobre mi forma de trabajar?**

---

# 2. Elegir el proyecto

Elegí un proyecto propio que pueda utilizarse como pieza de portafolio.

Puede ser:

- un proyecto realizado durante este curso;
- un trabajo académico;
- un pequeño programa;
- un proyecto personal;
- un repositorio de documentación;
- otro proyecto técnico que puedas explicar.

No hace falta que sea un proyecto grande.

Es preferible elegir uno que conozcas bien y puedas mejorar.

---

# 3. Revisar el estado actual

Cloná el repositorio si todavía no lo tenés localmente:

```bash
git clone URL_DEL_REPOSITORIO
```

Ingresá al proyecto:

```bash
cd nombre-del-proyecto
```

Verificá:

```bash
git status
```

Después observá:

```bash
git log --oneline --graph --all
```

No modifiques nada todavía.

Primero vamos a analizar.

---

# 4. Mirar el proyecto como una persona externa

Imaginá que nunca viste este proyecto.

Abrí:

```text
README.md
```

y respondé:

```text
¿Qué hace el proyecto?

¿Para qué sirve?

¿Quién podría utilizarlo?

¿Cómo se instala?

¿Cómo se ejecuta?

¿Hay ejemplos?

¿Qué tecnologías utiliza?

¿Hay información que falta?
```

No consultes al autor del proyecto.

La idea es comprobar cuánto puede comprender una persona solamente a partir del repositorio.

---

# 5. Evaluar el README

Asignale un estado a cada aspecto:

| Aspecto | Estado |
|---|---|
| Descripción | ? |
| Objetivo | ? |
| Instalación | ? |
| Uso | ? |
| Ejemplos | ? |
| Tecnologías | ? |
| Estructura | ? |
| Contribución | ? |
| Licencia | ? |

Utilizá:

```text
Completo
Parcial
Falta
No aplica
```

---

# 6. Identificar al lector

Antes de modificar el README, definí quién podría leerlo.

Por ejemplo:

```text
estudiante
docente
desarrollador
colaborador
reclutador
usuario técnico
```

No todos necesitan la misma información.

Respondé:

> ¿Qué debería poder comprender esta persona después de leer el README?

---

# 7. Definir el objetivo del proyecto

Escribí una frase que explique claramente qué problema resuelve.

Evitá:

```text
Este proyecto es un programa hecho en Python.
```

Buscá algo más cercano a:

```text
Este proyecto permite __________________________
```

o:

```text
El objetivo de este proyecto es __________________
```

La descripción debe centrarse en el propósito, no solamente en la tecnología.

---

# 8. Mejorar la descripción

Reescribí la introducción del README.

Debería responder rápidamente:

```text
¿Qué es?
¿Para qué sirve?
```

Por ejemplo:

```md
# Nombre del proyecto

Descripción breve del proyecto.

Este proyecto permite...
```

No es necesario escribir varios párrafos.

La claridad es más importante que la extensión.

---

# 9. Documentar el problema

Agregá una sección que explique el contexto cuando resulte necesario.

Por ejemplo:

```md
## Problema

Este proyecto surge a partir de la necesidad de...
```

No inventes un problema para hacer que el proyecto parezca más importante.

Utilizá el contexto real.

---

# 10. Documentar la solución

Explicá qué construiste.

Por ejemplo:

```md
## Solución

El proyecto implementa...
```

La explicación debería permitir comprender la relación:

```text
problema
   ↓
solución
```

---

# 11. Identificar tecnologías

Agregá las tecnologías realmente utilizadas.

Por ejemplo:

```md
## Tecnologías

- Python
- Git
- GitHub
- Markdown
```

No agregues tecnologías que solamente conocés pero que no utilizaste en el proyecto.

La evidencia debe corresponder con la realidad.

---

# 12. Documentar requisitos

Identificá qué necesita una persona para utilizar el proyecto.

Por ejemplo:

```md
## Requisitos

- Git
- Python 3.x
- ...
```

Si el proyecto no requiere una herramienta determinada, no la incluyas.

---

# 13. Documentar instalación

Escribí instrucciones que otra persona pueda ejecutar.

Por ejemplo:

```md
## Instalación

Clonar el repositorio:

```bash
git clone URL_DEL_REPOSITORIO
```

Ingresar al proyecto:

```bash
cd nombre-del-proyecto
```
```

Las instrucciones deben corresponder con el proyecto real.

---

# 14. Probar las instrucciones

Esta parte es importante.

No alcanza con escribir:

```text
git clone ...
```

Probá las instrucciones desde un entorno limpio cuando sea posible.

La secuencia debe ser:

```text
documentar
   ↓
probar
   ↓
detectar errores
   ↓
corregir
```

---

# 15. Documentar el uso

Explicá cómo utilizar el proyecto.

Por ejemplo:

```md
## Uso

Ejecutar:

```bash
python programa.py
```
```

Si existen parámetros o condiciones particulares, documentalos.

---

# 16. Agregar un ejemplo

Un ejemplo concreto suele ser más útil que una explicación extensa.

Podés incluir:

```md
## Ejemplo

Entrada:

...

Resultado:

...
```

El ejemplo debe poder relacionarse con el comportamiento real del proyecto.

---

# 17. Documentar la estructura

Si el proyecto tiene varios archivos o directorios, explicá brevemente su organización.

Por ejemplo:

```text
proyecto/
├── README.md
├── src/
├── tests/
└── docs/
```

Después explicá las partes importantes.

No es necesario documentar cada archivo si eso no aporta valor.

---

# 18. Revisar la estructura del repositorio

Observá:

```bash
git status
```

y:

```bash
git ls-files
```

Identificá:

- archivos necesarios;
- archivos generados;
- archivos temporales;
- configuraciones locales;
- posibles secretos.

---

# 19. Buscar información sensible

Revisá los archivos del proyecto.

Buscá indicios de:

```text
password
passwd
token
api_key
secret
credential
```

También revisá archivos de configuración.

La pregunta es:

> ¿Hay información que no debería hacerse pública?

---

# 20. Si encontrás un secreto

No lo publiques.

Si todavía no fue registrado por Git:

1. eliminá la información;
2. reemplazala por una configuración segura;
3. agregá el archivo correspondiente a `.gitignore` si corresponde;
4. verificá el estado.

Por ejemplo:

```bash
git status
```

---

# 21. Crear `.gitignore`

Si el proyecto no tiene uno, evaluá si necesita:

```text
.gitignore
```

Crealo en la raíz del proyecto.

Ejemplo conceptual:

```gitignore
__pycache__/
.venv/
.env
*.log
```

La lista debe adaptarse al proyecto.

No copies reglas innecesarias.

---

# 22. Verificar `.gitignore`

Creá o identificá un archivo que deba ser ignorado.

Después ejecutá:

```bash
git status
```

Comprobá que Git no lo presente como un cambio pendiente.

La idea es verificar que la regla funciona realmente.

---

# 23. Una aclaración importante

Recordá:

```text
.gitignore
```

evita incorporar determinados archivos al seguimiento.

No borra información que ya haya sido registrada en la historia.

Por eso:

```text
secreto publicado
       ↓
.gitignore
```

no significa:

```text
secreto eliminado
```

---

# 24. Revisar el historial

Ejecutá:

```bash
git log --oneline --graph --all
```

Observá:

- mensajes;
- cantidad de commits;
- organización;
- evolución del proyecto.

Preguntate:

> ¿La historia permite comprender cómo evolucionó el proyecto?

---

# 25. Analizar los mensajes de commit

Buscá mensajes como:

```text
cambios
fix
cosas
final
prueba
```

Si aparecen, no necesariamente significa que debas reescribir toda la historia.

El objetivo de este ejercicio es reconocer qué información aporta un buen mensaje.

Compará con:

```text
Agrega validación de entrada
Corrige cálculo del promedio
Documenta instalación
Agrega ejemplo de uso
```

---

# 26. Revisar Issues

Si el repositorio utiliza Issues, observá:

```text
¿Las tareas están claras?
¿Los títulos son descriptivos?
¿Se puede entender el problema?
```

Si no tiene Issues, no es obligatorio inventar un historial.

Podés crear una Issue para una mejora real que quieras realizar.

---

# 27. Revisar Pull Requests

Si el proyecto tiene Pull Requests, observá:

```text
títulos
descripciones
revisiones
comentarios
cambios solicitados
```

Preguntate:

> ¿Qué evidencia aportan estas Pull Requests sobre el proceso de trabajo?

Si el proyecto es personal y no tiene Pull Requests, simplemente registrá esa situación.

No hace falta fabricar actividad.

---

# 28. Crear una mejora real

Elegí una mejora pequeña pero concreta.

Puede ser:

```text
mejorar README
agregar ejemplo
corregir documentación
agregar validación
mejorar estructura
agregar prueba
```

Creá una Issue para esa tarea.

---

# 29. Crear una rama

No realices la mejora directamente sobre `main`.

Creá una rama:

```bash
git switch main
```

Después:

```bash
git switch -c docs-mejora
```

El nombre debe representar el trabajo que vas a realizar.

---

# 30. Realizar el cambio

Implementá la mejora.

No agregues cambios que no estén relacionados con la tarea.

La intención es mantener una modificación enfocada.

---

# 31. Revisar

Antes del commit:

```bash
git status
```

Después:

```bash
git diff
```

Preguntate:

```text
¿Cambió solamente lo necesario?
¿El resultado funciona?
¿La documentación coincide con el proyecto?
```

---

# 32. Registrar el cambio

Realizá un commit claro:

```bash
git add .
git commit -m "Mejora documentación del proyecto"
```

El mensaje debe describir el cambio.

---

# 33. Publicar

Publicá la rama:

```bash
git push -u origin docs-mejora
```

Después verificá el repositorio en GitHub.

---

# 34. Crear una Pull Request

Creá una Pull Request hacia:

```text
main
```

La descripción debería explicar:

```text
qué se mejoró
por qué
cómo se verificó
```

Si el repositorio utiliza Issues, relacioná la Pull Request con la Issue correspondiente.

---

# 35. Revisar el propio cambio

Aunque trabajes individualmente, realizá una revisión final.

Observá:

```text
Files changed
Commits
Description
```

Preguntate:

> Si otra persona revisara esta Pull Request, ¿entendería qué hice?

---

# 36. Integrar

Una vez revisada, integrá la Pull Request.

Después actualizá tu repositorio local:

```bash
git switch main
git pull
```

Comprobá:

```bash
git status
```

---

# 37. Revisar nuevamente el README

Volvé al README y preguntate:

```text
¿Ahora entiendo mejor el proyecto?

¿Una persona nueva podría instalarlo?

¿Puede ejecutarlo?

¿Puede entender su objetivo?

¿Puede encontrar ejemplos?

¿Puede saber qué tecnologías utiliza?
```

Si alguna respuesta es "no", realizá otra mejora.

---

# 38. Construir la narrativa del proyecto

Ahora completá:

```text
## Proyecto

Nombre:
____________________

Problema:
____________________

Solución:
____________________

Tecnologías:
____________________

Decisiones importantes:
____________________

Dificultades:
____________________

Aprendizajes:
____________________
```

Esto será la base para presentar el proyecto.

---

# 39. Identificar habilidades

Relacioná cada aspecto del proyecto con una capacidad demostrable.

Por ejemplo:

| Evidencia | Capacidad |
|---|---|
| Código | Programación |
| Git | Control de versiones |
| README | Documentación |
| Issues | Organización |
| Pull Request | Colaboración |
| Revisión | Comunicación técnica |
| Tests | Verificación |

No agregues habilidades que el proyecto no permita demostrar.

---

# 40. Preparar una presentación breve

Prepará una explicación de entre:

```text
3 y 5 minutos
```

Debería responder:

```text
¿Qué problema resolví?

¿Qué construí?

¿Qué tecnologías utilicé?

¿Qué decisión técnica importante tomé?

¿Qué dificultad encontré?

¿Qué aprendí?
```

---

# 41. Practicar la presentación

Explicá el proyecto en voz alta.

No leas el README palabra por palabra.

Utilizalo como apoyo.

El objetivo es poder explicar:

```text
problema
 ↓
solución
 ↓
decisiones
 ↓
resultado
```

---

# 42. Revisar la presentación

Después de explicarlo, preguntate:

```text
¿Fui claro?

¿Expliqué el problema?

¿Expliqué por qué elegí esa solución?

¿Dije algo que no puedo demostrar?

¿Pude explicar las decisiones?
```

La última pregunta es especialmente importante.

---

# 43. Revisar el perfil profesional

Ahora observá tu perfil de GitHub como si fueras una persona externa.

Preguntate:

```text
¿Qué proyecto veo primero?

¿Qué impresión produce?

¿Entiendo qué estoy aprendiendo?

¿Hay proyectos que debería destacar?

¿Hay repositorios que deberían ser privados?

¿Hay información que debería eliminar?
```

---

# 44. Seleccionar proyectos destacados

Elegí:

```text
1 a 3 proyectos
```

que representen mejor tu trabajo actual.

Para cada uno escribí:

```text
¿Por qué lo seleccioné?

¿Qué demuestra?

¿Qué aprendí?

¿Qué podría mejorar?
```

No es necesario que sean los proyectos más grandes.

---

# 45. Mejorar la descripción del perfil

Prepará una breve presentación profesional.

Debe indicar, de manera honesta:

```text
qué estudiás o hacés
qué tecnologías estás trabajando
qué temas te interesan
```

Evitá afirmaciones exageradas.

Por ejemplo:

```text
Desarrollador experto en todo.
```

es menos útil que una presentación concreta y verificable.

---

# 46. Revisar la coherencia

Compará:

```text
perfil
README
repositorios
proyectos
CV
```

Preguntate:

> ¿Todos cuentan una historia coherente?

No tienen que ser idénticos.

Pero deberían representar de manera consistente tu recorrido actual.

---

# 47. Crear una pequeña página de portafolio

Como ejercicio opcional, creá un documento:

```text
PORTFOLIO.md
```

que contenga:

```md
# Mi portafolio

## Sobre mí

...

## Proyectos

### Proyecto 1

...

### Proyecto 2

...

## Tecnologías

...

## Aprendizajes

...
```

El objetivo es practicar la selección y presentación de evidencia.

---

# 48. Revisar la información pública

Antes de considerar terminado el trabajo, revisá nuevamente:

```text
repositorios públicos
README
issues
pull requests
archivos
configuración
```

Preguntate:

> ¿Publicaría todo esto tal como está?

Si la respuesta es no, corregilo.

---

# 49. Crear una lista de mejoras futuras

No intentes resolver todo ahora.

Creá:

```text
MEJORAS.md
```

o una Issue con las próximas mejoras.

Por ejemplo:

```text
- agregar tests
- mejorar documentación
- agregar ejemplo
- reorganizar estructura
- mejorar mensajes
```

Esto también demuestra capacidad para reconocer trabajo pendiente.

---

# 50. Estado final

Al finalizar la práctica, deberías tener:

```text
proyecto
   ↓
README mejorado
   ↓
.gitignore revisado
   ↓
mejora real
   ↓
Issue
   ↓
rama
   ↓
commit
   ↓
Pull Request
   ↓
integración
   ↓
presentación
```

---

# 51. Comprobación final

Ejecutá:

```bash
git status
```

Después:

```bash
git branch
```

Y finalmente:

```bash
git log --oneline --graph --all
```

Verificá que el repositorio se encuentre en un estado coherente.

---

# 52. Reflexión

Respondé:

### 1.

¿Qué proyecto elegiste y por qué?

### 2.

¿Qué problema resuelve?

### 3.

¿Qué parte del README necesitaba mayor trabajo?

### 4.

¿Qué información faltaba?

### 5.

¿Qué información decidiste no publicar?

### 6.

¿Qué función cumple `.gitignore` en tu proyecto?

### 7.

¿Qué mejora realizaste?

### 8.

¿Qué evidencia existe de esa mejora?

### 9.

¿Qué habilidad técnica demuestra tu proyecto?

### 10.

¿Qué habilidad de comunicación demuestra?

### 11.

¿Qué mejorarías si tuvieras una semana más?

---

# 53. Cierre

El resultado de esta práctica no es solamente un README mejor.

Tampoco es solamente un perfil más ordenado.

El objetivo es comenzar a construir una relación entre:

```text
lo que aprendés
      ↓
lo que hacés
      ↓
lo que documentás
      ↓
lo que podés mostrar
      ↓
lo que podés explicar
```

Esa relación es la base de una evidencia profesional genuina.

> **No construyas un perfil para parecer que sabés. Construí proyectos que te permitan demostrar lo que sabés.**