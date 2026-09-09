# Práctica
## Módulo 07 — Trabajo Colaborativo

---

## 1. Objetivo

En esta práctica vamos a realizar un flujo de trabajo colaborativo completo utilizando Git y GitHub.

Vamos a trabajar sobre la idea:

```text
tarea
  ↓
rama
  ↓
commits
  ↓
push
  ↓
Pull Request
  ↓
revisión
  ↓
correcciones
  ↓
merge
```

El objetivo no es aprender una colección de comandos aislados.

Queremos comprender cómo se organiza un cambio cuando el repositorio es compartido con otras personas.

---

# 2. Antes de comenzar

Necesitás:

- Git instalado;
- una cuenta de GitHub;
- acceso a un repositorio;
- una terminal;
- Visual Studio Code.

Para esta práctica se recomienda utilizar un repositorio propio o uno creado específicamente para la actividad.

---

# 3. Verificar Git

Comprobá que Git esté instalado:

```bash
git --version
```

Después verificá tu identidad:

```bash
git config --global user.name
git config --global user.email
```

Si todavía no está configurada:

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
```

---

# 4. Crear o elegir el repositorio

Utilizá un repositorio de GitHub que puedas modificar.

Podés crear uno nuevo desde GitHub o utilizar un proyecto existente.

El repositorio debería tener como mínimo:

```text
README.md
```

Es recomendable que también tenga algunos archivos sobre los cuales podamos trabajar.

---

# 5. Clonar el repositorio

Desde GitHub obtené la dirección del repositorio.

Después ejecutá:

```bash
git clone URL_DEL_REPOSITORIO
```

Por ejemplo:

```bash
git clone https://github.com/usuario/proyecto.git
```

Ingresá al directorio:

```bash
cd proyecto
```

---

# 6. Comprobar el repositorio

Ejecutá:

```bash
git status
```

Después:

```bash
git remote -v
```

Deberías poder identificar el repositorio remoto asociado.

También consultá:

```bash
git branch
```

---

# 7. Comprender la situación

Ahora tenemos:

```text
GitHub
   ↑
   │
repositorio remoto
   │
   ↓
repositorio local
```

El repositorio remoto es compartido.

El repositorio local es nuestra copia de trabajo.

---

# 8. Crear una tarea

Vamos a simular un proyecto que necesita una nueva funcionalidad.

Antes de crear la rama, definí qué vas a desarrollar.

Por ejemplo:

```text
Agregar una sección de instalación al proyecto.
```

o:

```text
Agregar un ejemplo nuevo.
```

o:

```text
Agregar una pequeña funcionalidad al proyecto.
```

La tarea debe ser concreta.

---

# 9. Crear una Issue

Ingresá al repositorio en GitHub.

Creá una Issue que describa la tarea.

Por ejemplo:

```text
Título:

Agregar sección de instalación

Descripción:

Incorporar al README instrucciones claras
para instalar y ejecutar el proyecto.
```

La Issue representa la necesidad que queremos resolver.

---

# 10. Observar la diferencia

Tenemos:

```text
Issue
  ↓
¿Qué necesitamos hacer?
```

Todavía no realizamos el cambio.

La Issue funciona como referencia para el trabajo.

---

# 11. Crear la rama

Volvé a la terminal.

Partiendo de `main`:

```bash
git switch main
```

Después:

```bash
git switch -c docs-instalacion
```

Verificá:

```bash
git branch
```

Deberías observar:

```text
  main
* docs-instalacion
```

---

# 12. Relacionar mentalmente la rama con la tarea

Tenemos:

```text
Issue
  │
  ↓
docs-instalacion
  │
  ↓
trabajo
```

La rama representa la línea de trabajo destinada a resolver la tarea.

---

# 13. Realizar el primer cambio

Modificá el proyecto para comenzar a resolver la Issue.

Por ejemplo, agregá al `README.md` una sección:

```md
## Instalación

Instrucciones para instalar y preparar el proyecto.
```

Guardá el archivo.

---

# 14. Revisar el cambio

Ejecutá:

```bash
git status
```

Después:

```bash
git diff
```

Observá exactamente qué cambió.

No hagas el commit todavía.

Primero revisá el trabajo.

---

# 15. Crear el primer commit

Si el cambio es correcto:

```bash
git add README.md
```

Después:

```bash
git commit -m "Agrega instrucciones de instalación"
```

Consultá:

```bash
git log --oneline
```

---

# 16. Realizar un segundo cambio

Continuá trabajando sobre la misma tarea.

Mejorá las instrucciones.

Podés agregar, por ejemplo:

```md
### Requisitos

- Git
- Python
- Visual Studio Code
```

Registrá el segundo avance:

```bash
git add README.md
git commit -m "Documenta requisitos de instalación"
```

Ahora la rama tiene más de un commit relacionado con la misma tarea.

---

# 17. Revisar la historia

Ejecutá:

```bash
git log --oneline --graph --all
```

Deberías poder identificar:

```text
main
  \
   commits de docs-instalacion
```

La rama contiene el trabajo que todavía no fue incorporado a `main`.

---

# 18. Publicar la rama

Ahora queremos compartir el trabajo.

Ejecutá:

```bash
git push -u origin docs-instalacion
```

El flujo es:

```text
commits locales
      ↓
git push
      ↓
GitHub
```

---

# 19. Verificar GitHub

Ingresá al repositorio en GitHub.

Comprobá que exista:

```text
docs-instalacion
```

También verificá que sus commits estén disponibles.

---

# 20. Crear la Pull Request

GitHub debería ofrecerte la posibilidad de crear una Pull Request para la nueva rama.

También podés hacerlo desde la sección de Pull Requests.

La situación es:

```text
docs-instalacion
       ↓
Pull Request
       ↓
main
```

---

# 21. Escribir una buena descripción

No crees una Pull Request vacía o con una descripción como:

```text
Cambios.
```

Explicá:

```md
## Qué hice

Agregué instrucciones de instalación y requisitos
del proyecto.

## Por qué

La documentación no explicaba cómo preparar
el entorno.

## Issue relacionada

Resuelve la Issue correspondiente a la documentación
de instalación.
```

La descripción debe permitir que otra persona entienda qué está revisando.

---

# 22. Observar la Pull Request

La Pull Request permite observar:

- archivos modificados;
- commits;
- diferencias;
- descripción;
- comentarios;
- estado de revisión.

Explorá cada sección.

La Pull Request es el espacio donde vamos a revisar el cambio antes de integrarlo.

---

# 23. Revisar los cambios

Ingresá a la pestaña de archivos modificados.

Observá:

```text
antes
  ↓
cambios
  ↓
después
```

Preguntate:

- ¿El cambio resuelve la tarea?
- ¿La documentación es clara?
- ¿Falta información?
- ¿Hay cambios innecesarios?
- ¿Hay errores?

---

# 24. Simular una revisión

Si estás trabajando solo, podés realizar la revisión utilizando otro usuario o simplemente simular el rol de revisor mediante el análisis de la Pull Request.

Si trabajás con otra persona, intercambien roles.

Una persona propone:

```text
Pull Request
```

La otra revisa.

---

# 25. Realizar un comentario

Agregá una observación concreta.

Por ejemplo:

```text
Sería conveniente agregar un ejemplo del comando
utilizado para clonar el repositorio.
```

La observación debe referirse al trabajo.

Evitá comentarios vagos como:

```text
No me gusta.
```

---

# 26. Solicitar una corrección

Supongamos que el revisor detectó una mejora necesaria.

Por ejemplo:

> La documentación debería explicar también cómo verificar que Git quedó correctamente instalado.

La Pull Request todavía no debe integrarse.

Tenemos:

```text
Pull Request
      ↓
revisión
      ↓
cambio solicitado
```

---

# 27. Volver al trabajo local

Volvé a tu rama:

```bash
git switch docs-instalacion
```

Realizá la corrección solicitada.

Por ejemplo:

```md
### Verificar Git

Para comprobar que Git está instalado:

```bash
git --version
```
```

---

# 28. Registrar la corrección

Guardá el cambio:

```bash
git add README.md
git commit -m "Agrega verificación de Git"
```

La Pull Request se actualizará automáticamente cuando publiques el commit.

---

# 29. Publicar la corrección

Ejecutá:

```bash
git push
```

Volvé a GitHub.

La Pull Request debería mostrar el nuevo commit.

Esto demuestra una característica importante:

> Una Pull Request puede continuar evolucionando después de haber sido creada.

---

# 30. Nueva revisión

Volvé a revisar los cambios.

Comprobá que la observación haya sido atendida.

El flujo ahora fue:

```text
Pull Request
     ↓
revisión
     ↓
corrección
     ↓
push
     ↓
nueva revisión
```

---

# 31. Aprobar

Si el cambio está correcto, aprobá la Pull Request si estás utilizando un flujo con revisión formal.

La situación puede quedar:

```text
Pull Request
     ↓
Approved
```

La aprobación indica que el cambio fue revisado y puede continuar hacia la integración.

---

# 32. Integrar

Ahora incorporá la rama en `main` utilizando la opción correspondiente de GitHub.

La situación final será:

```text
docs-instalacion
       \
        → main
```

El trabajo de la rama pasó a formar parte de la línea principal.

---

# 33. Volver al repositorio local

Después de la integración, volvé a tu terminal.

Tu `main` local puede estar desactualizado.

Comprobá:

```bash
git status
```

y:

```bash
git branch
```

---

# 34. Actualizar `main`

Volvé a `main`:

```bash
git switch main
```

Después actualizá la información:

```bash
git pull
```

Ahora tu repositorio local debería incorporar el resultado de la integración.

---

# 35. Verificar el resultado

Comprobá:

```bash
git log --oneline --graph --all
```

y:

```bash
git status
```

Verificá que los cambios realizados en la rama ahora formen parte de `main`.

---

# 36. Eliminar la rama

Si la rama ya cumplió su propósito, podés eliminarla localmente:

```bash
git branch -d docs-instalacion
```

Si la rama remota ya no es necesaria, también puede eliminarse desde GitHub o mediante:

```bash
git push origin --delete docs-instalacion
```

Antes de hacerlo, asegurate de que la integración haya sido completada correctamente.

---

# 37. El flujo completo

Repasemos todo lo realizado:

```text
Issue
  ↓
crear rama
  ↓
realizar cambios
  ↓
commit
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
commit
  ↓
push
  ↓
nueva revisión
  ↓
aprobación
  ↓
merge
  ↓
pull
  ↓
main actualizado
```

Este flujo constituye el núcleo de la práctica.

---

# 38. Segunda situación — Trabajo paralelo

Ahora vamos a simular una situación más realista.

Mientras una persona trabaja sobre:

```text
docs-instalacion
```

otra persona trabaja sobre:

```text
feature-ejemplo
```

Ambas ramas parten de `main`.

Representalo:

```text
             docs-instalacion
            /
main ──────
            \
             feature-ejemplo
```

---

# 39. Crear la segunda rama

Partiendo de `main` actualizado:

```bash
git switch main
```

Creá:

```bash
git switch -c feature-ejemplo
```

Realizá una modificación independiente.

Registrala:

```bash
git add .
git commit -m "Agrega nuevo ejemplo"
```

Publicá:

```bash
git push -u origin feature-ejemplo
```

---

# 40. Crear una segunda Pull Request

Desde GitHub creá una Pull Request:

```text
feature-ejemplo
       ↓
main
```

Analizá:

- qué archivos cambia;
- qué commits contiene;
- si afecta las mismas partes modificadas por otras ramas.

---

# 41. Integrar cambios independientes

Si las modificaciones no generan conflictos, pueden integrarse en momentos diferentes.

Por ejemplo:

```text
docs-instalacion
       ↓
      main
       ↑
       │
feature-ejemplo
```

Cada Pull Request representa una propuesta independiente.

---

# 42. Observar el historial

Después de integrar ambas ramas:

```bash
git pull
```

y:

```bash
git log --oneline --graph --all
```

Intentá reconstruir la historia.

Preguntate:

```text
¿Qué tarea se realizó primero?
¿Qué tarea se realizó después?
¿Qué ramas existieron?
¿Qué commits produjo cada una?
```

---

# 43. Tercera situación — Conflicto

Ahora vamos a provocar deliberadamente un conflicto.

Partiendo de `main`, creá:

```text
feature-a
```

y:

```text
feature-b
```

Ambas ramas deben modificar la misma línea de un mismo archivo.

---

# 44. Cambio en `feature-a`

Creá:

```bash
git switch -c feature-a
```

Modificá una línea.

Por ejemplo:

```text
Descripción: Proyecto educativo
```

cambiala por:

```text
Descripción: Proyecto educativo colaborativo
```

Registrá:

```bash
git add .
git commit -m "Actualiza descripción"
```

Publicá la rama.

---

# 45. Cambio en `feature-b`

Volvé a `main`:

```bash
git switch main
```

Creá:

```bash
git switch -c feature-b
```

Modificá exactamente la misma línea.

Por ejemplo:

```text
Descripción: Proyecto educativo para aprender Git
```

Registrá:

```bash
git add .
git commit -m "Amplía descripción"
```

Publicá la rama.

---

# 46. Intentar integrar

Creá la Pull Request correspondiente.

Intentá integrar las ramas.

GitHub puede detectar un conflicto.

La situación conceptual es:

```text
feature-a
    \
     \ 
      main
     /
    /
feature-b
```

Ambas ramas modificaron la misma parte del proyecto.

---

# 47. Analizar el conflicto

Antes de resolverlo preguntate:

```text
¿Qué quería lograr feature-a?
¿Qué quería lograr feature-b?
¿Qué información contiene cada cambio?
```

No elijas automáticamente una versión.

Primero comprendé el problema.

---

# 48. Resolver el conflicto

Si GitHub permite resolverlo desde la interfaz, podés hacerlo allí.

También podés resolverlo localmente.

El archivo puede contener:

```text
<<<<<<< HEAD
versión A
=======
versión B
>>>>>>> feature-b
```

Decidí cuál debe ser el resultado final.

Puede ser:

```text
versión A
```

```text
versión B
```

o una combinación:

```text
versión combinada
```

---

# 49. Completar la resolución

Una vez corregido el archivo:

```bash
git add archivo
```

y completá la integración según el flujo utilizado.

Después verificá:

```bash
git status
```

y:

```bash
git log --oneline --graph --all
```

---

# 50. Reflexión sobre conflictos

Respondé:

> ¿Por qué Git no pudo resolver automáticamente el conflicto?

> ¿Qué información necesitaste para decidir el resultado?

> ¿Por qué la resolución del conflicto es una decisión sobre el proyecto y no solamente sobre Git?

---

# 51. Cuarta situación — `fetch`

Ahora vamos a observar una diferencia importante.

Ejecutá:

```bash
git fetch
```

Después:

```bash
git status
```

y:

```bash
git branch -a
```

Observá las ramas locales y las referencias remotas.

---

# 52. ¿Qué hizo `fetch`?

`git fetch` permite obtener información actualizada del repositorio remoto sin integrar automáticamente esos cambios en la rama actual.

Conceptualmente:

```text
GitHub
  ↓
fetch
  ↓
información actualizada
```

No significa:

```text
"actualicé automáticamente mi trabajo"
```

---

# 53. `pull`

Ahora observá:

```bash
git pull
```

Conceptualmente:

```text
GitHub
  ↓
pull
  ↓
actualización local
```

La diferencia entre:

```bash
git fetch
```

y:

```bash
git pull
```

será importante cuando trabajemos con repositorios donde otras personas realizan cambios.

---

# 54. Simular una actualización externa

Si trabajás con otra persona, pedile que realice un cambio y lo publique.

Después, en tu repositorio local:

```bash
git fetch
```

Observá qué información cambió.

Después:

```bash
git pull
```

Analizá qué ocurrió.

---

# 55. Revisión de un cambio ajeno

Elegí una Pull Request de otra persona.

Antes de aprobarla, revisá:

### Objetivo

¿El cambio resuelve el problema planteado?

### Alcance

¿Modifica solamente lo necesario?

### Claridad

¿Los cambios son comprensibles?

### Documentación

¿La documentación acompaña el cambio?

### Calidad

¿Observás algún problema?

---

# 56. Escribir una buena observación

Una observación útil debería indicar:

```text
qué se observó
+
por qué importa
+
qué alternativa podría considerarse
```

Por ejemplo:

> "Esta sección explica cómo instalar el proyecto, pero no indica los requisitos previos. Podríamos agregarlos para que una persona nueva pueda preparar el entorno sin buscar información adicional."

---

# 57. Evitar revisiones poco útiles

No son buenas observaciones:

```text
Está mal.
```

```text
No me gusta.
```

```text
Cambialo.
```

Sin contexto, no ayudan a mejorar el trabajo.

La revisión debe favorecer una conversación técnica.

---

# 58. Crear un `CONTRIBUTING.md`

Ahora agregá al proyecto:

```text
CONTRIBUTING.md
```

Incluí como mínimo:

```md
# Contribuir al proyecto

## Crear una rama

...

## Commits

...

## Pull Requests

...

## Revisión

...

## Issues

...
```

El objetivo es documentar cómo debería participar una persona nueva en el proyecto.

---

# 59. Crear un `CODE_OF_CONDUCT.md`

Como ejercicio complementario, creá:

```text
CODE_OF_CONDUCT.md
```

No es necesario elaborar un documento extenso.

El objetivo es comprender que los proyectos colaborativos pueden establecer pautas explícitas de participación.

---

# 60. Revisar el repositorio

Al finalizar, tu repositorio puede contener:

```text
README.md
CONTRIBUTING.md
CODE_OF_CONDUCT.md
```

Además de los archivos propios del proyecto.

Observá cómo estos documentos ayudan a una persona nueva a comprender:

```text
qué es el proyecto
cómo utilizarlo
cómo contribuir
cómo participar
```

---

# 61. Ejercicio de explicación

Explicá con tus palabras la diferencia entre:

```text
Issue
Commit
Branch
Pull Request
Merge
```

Una explicación posible debería poder representarse como:

```text
Issue
 ↓
tarea

Branch
 ↓
línea de trabajo

Commit
 ↓
registro de un cambio

Pull Request
 ↓
propuesta y revisión

Merge
 ↓
integración
```

---

# 62. Ejercicio de flujo

Dibujá el siguiente proceso:

```text
Persona A
    ↓
Issue
    ↓
rama
    ↓
commit
    ↓
push
    ↓
Pull Request
    ↓
Persona B
    ↓
revisión
    ↓
corrección
    ↓
merge
    ↓
main
```

Después explicalo oralmente.

---

# 63. Comprobación final

Sin consultar documentación, intentá realizar:

```bash
git clone
git switch -c
git add
git commit
git push
git pull
git fetch
```

Y desde GitHub:

```text
Issue
Pull Request
Review
Merge
```

No es necesario memorizar todas las opciones.

Lo importante es comprender cuándo utilizar cada herramienta.

---

# 64. Reflexión final

Respondé:

### 1.

¿Qué problema resuelve una rama dentro de un trabajo colaborativo?

### 2.

¿Qué diferencia existe entre una Issue y una Pull Request?

### 3.

¿Qué diferencia existe entre un commit y una Pull Request?

### 4.

¿Por qué una Pull Request puede recibir nuevos commits después de haber sido creada?

### 5.

¿Qué función cumple una revisión?

### 6.

¿Por qué es importante explicar claramente un cambio?

### 7.

¿Qué diferencia existe entre `push`, `pull` y `fetch`?

### 8.

¿Por qué aparecen conflictos?

### 9.

¿Por qué resolver un conflicto requiere comprender la intención de los cambios?

### 10.

¿Qué reglas establecerías para que un equipo trabaje ordenadamente sobre un repositorio?

---

# 65. Modelo mental final

Al terminar la práctica deberías poder visualizar el trabajo colaborativo de esta manera:

```text
                    Issue
                      ↓
                 crear rama
                      ↓
                   trabajo
                      ↓
                   commits
                      ↓
                    push
                      ↓
               Pull Request
                      ↓
                  revisión
                  ↙      ↘
          corrección    aprobación
               ↓             ↓
             push           merge
               └──────┬──────┘
                      ↓
                     main
```

El flujo puede variar según el proyecto y el equipo.

Lo importante es comprender la lógica:

> **Una tarea se transforma en cambios concretos, esos cambios quedan registrados, se publican, se revisan y finalmente se integran al proyecto.**

---

# 66. Cierre

Hasta ahora aprendimos a trabajar con Git principalmente como herramienta individual.

En esta práctica empezamos a utilizarlo como parte de un proceso social y técnico.

La diferencia fundamental es:

```text
"Yo hice un cambio."
```

frente a:

```text
"Propongo este cambio para el proyecto,
puede ser revisado, discutido y mejorado
antes de incorporarlo."
```

Ese cambio de perspectiva es el corazón del trabajo colaborativo.