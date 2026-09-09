# Ejercicios
## Módulo 09 — Proyecto Final

Los ejercicios de este módulo acompañan el desarrollo del Proyecto Final.

La propuesta es utilizarlos para practicar las decisiones y situaciones que aparecen durante el desarrollo de un proyecto real.

---

# Ejercicio 1 — Definir el proyecto

Completá:

```text
Nombre:
________________________

Problema:
________________________

Objetivo:
________________________

Usuario:
________________________

Resultado esperado:
________________________
```

Después explicá el proyecto en no más de cinco líneas.

---

# Ejercicio 2 — Alcance

Definí:

```text
El proyecto incluirá:

- ______________________
- ______________________
- ______________________
```

y:

```text
El proyecto no incluirá:

- ______________________
- ______________________
- ______________________
```

Explicá por qué es importante definir también lo que queda fuera del proyecto.

---

# Ejercicio 3 — Versión mínima

Definí cuál sería la versión mínima funcional del proyecto.

Respondé:

```text
¿Qué tiene que poder hacer obligatoriamente?

____________________________________
```

Después separá:

```text
Obligatorio
Opcional
```

---

# Ejercicio 4 — Dividir el trabajo

Tomá el proyecto y dividilo en tareas.

Por ejemplo:

```text
1. Crear estructura.
2. Implementar funcionalidad principal.
3. Agregar validaciones.
4. Documentar instalación.
5. Agregar ejemplo.
6. Revisar.
```

No intentes definir todas las tareas posibles.

El objetivo es obtener una primera planificación razonable.

---

# Ejercicio 5 — Crear Issues

Transformá las principales tareas en Issues.

Para cada una indicá:

```text
Título:
________________________

Problema:
________________________

Objetivo:
________________________

Resultado esperado:
________________________
```

---

# Ejercicio 6 — Priorizar Issues

Tomá las Issues creadas y asignales:

```text
Alta
Media
Baja
```

Después respondé:

> ¿Qué tarea debería realizarse primero y por qué?

---

# Ejercicio 7 — Crear el repositorio

Creá un repositorio local:

```bash
git init
```

Después:

```bash
git status
```

Respondé:

> ¿Qué información muestra `git status` en este momento?

---

# Ejercicio 8 — Estructura inicial

Creá una estructura inicial para el proyecto.

Por ejemplo:

```text
proyecto/
├── README.md
├── .gitignore
└── src/
```

Adaptala al proyecto real.

Después explicá por qué elegiste esa estructura.

---

# Ejercicio 9 — Primer README

Creá un README inicial con:

```md
# Nombre del proyecto

Descripción.

## Objetivo

...

## Estado

En desarrollo.
```

No intentes documentar todavía todo el proyecto.

La documentación evolucionará junto con el desarrollo.

---

# Ejercicio 10 — Primer `.gitignore`

Creá:

```text
.gitignore
```

Incluí los archivos que no deberían formar parte del repositorio.

Después ejecutá:

```bash
git status
```

y verificá el resultado.

---

# Ejercicio 11 — Primer commit

Prepará el estado inicial:

```bash
git add .
```

y registralo:

```bash
git commit -m "Inicializa estructura del proyecto"
```

Después:

```bash
git log --oneline
```

Respondé:

> ¿Qué representa este commit?

---

# Ejercicio 12 — Analizar el primer commit

Ejecutá:

```bash
git show HEAD
```

Identificá:

```text
archivos incorporados
cambios realizados
mensaje
```

Explicá por qué este commit representa una unidad de trabajo coherente.

---

# Ejercicio 13 — Crear una rama

Elegí una tarea concreta.

Creá una rama:

```bash
git switch -c feature-nombre
```

Después verificá:

```bash
git branch
```

Respondé:

> ¿En qué rama estás trabajando?

---

# Ejercicio 14 — Primer cambio

Realizá una modificación pequeña pero concreta.

Después:

```bash
git status
```

y:

```bash
git diff
```

Respondé:

```text
¿Qué cambió?

¿Qué archivo fue modificado?

¿El cambio corresponde a la tarea?
```

---

# Ejercicio 15 — Commit de una tarea

Registrá el cambio:

```bash
git add .
git commit -m "Implementa funcionalidad principal"
```

Después:

```bash
git log --oneline
```

Explicá qué información aporta el mensaje.

---

# Ejercicio 16 — Commit poco claro

Analizá:

```text
cambios
fix
final
cosas
```

¿Por qué estos mensajes dificultan comprender la historia?

Proponé una alternativa para cada uno.

---

# Ejercicio 17 — Diferentes unidades de trabajo

Considerá estos cambios:

```text
Agregar validación
Corregir README
Agregar ejemplo
Corregir cálculo
```

¿Conviene registrarlos en un único commit o en varios?

Justificá la decisión.

No existe una cantidad universal de commits correcta.

---

# Ejercicio 18 — Publicar la rama

Publicá la rama:

```bash
git push -u origin feature-nombre
```

Después verificá en GitHub que exista.

---

# Ejercicio 19 — Crear una Pull Request

Creá una Pull Request hacia:

```text
main
```

La descripción debe responder:

```text
¿Qué hice?

¿Por qué?

¿Cómo lo probé?
```

---

# Ejercicio 20 — Revisar una Pull Request

Revisá una Pull Request de otro estudiante.

Encontrá:

```text
1 aspecto correcto
1 aspecto mejorable
1 pregunta
```

Los comentarios deben ser concretos.

---

# Ejercicio 21 — Solicitar cambios

Sobre una Pull Request, realizá una observación que requiera una corrección real.

El autor debe:

```text
analizar
 ↓
corregir
 ↓
commit
 ↓
push
```

Después revisá nuevamente.

---

# Ejercicio 22 — Integrar

Una vez aprobada la Pull Request, realizá el merge.

Después:

```bash
git switch main
git pull
```

Verificá:

```bash
git status
```

Respondé:

> ¿Qué cambió en `main` después de la integración?

---

# Ejercicio 23 — Analizar el historial

Ejecutá:

```bash
git log --oneline --graph --all
```

Identificá:

```text
commit inicial
rama de trabajo
commits de la rama
merge
```

Intentá reconstruir la secuencia de trabajo.

---

# Ejercicio 24 — Historial como narrativa

Escribí una breve explicación de la evolución del proyecto utilizando solamente el historial.

Por ejemplo:

```text
Primero...
Después...
Luego...
Finalmente...
```

Respondé:

> ¿La historia permite comprender el proceso?

---

# Ejercicio 25 — Actualizar una rama

Imaginá que `main` avanzó mientras trabajabas en otra rama.

Representá:

```text
main
 ↓
nuevo cambio

feature
 ↓
trabajo pendiente
```

Explicá por qué puede ser necesario actualizar tu rama antes de integrarla.

---

# Ejercicio 26 — Conflicto

Trabajá con otra persona.

Ambos deben modificar deliberadamente una misma línea de un archivo.

Después intenten integrar los cambios.

Observá el conflicto.

No resuelvas todavía.

Identificá:

```text
¿Qué líneas están en conflicto?

¿Qué intentaba hacer cada cambio?
```

---

# Ejercicio 27 — Resolver el conflicto

Resolvé el conflicto analizando las dos versiones.

Después verificá el archivo resultante.

Ejecutá:

```bash
git status
```

y comprobá que no queden conflictos pendientes.

Finalmente registrá la resolución cuando corresponda.

---

# Ejercicio 28 — Verificar una resolución

Después de resolver un conflicto:

```text
¿El proyecto sigue funcionando?

¿Se conservaron los cambios necesarios?

¿Se perdió información?

¿El resultado tiene sentido?
```

La resolución no termina cuando Git deja de mostrar el conflicto.

---

# Ejercicio 29 — README durante el desarrollo

Revisá el README mientras el proyecto todavía está en desarrollo.

Identificá qué información ya debería estar documentada y cuál todavía no.

Separá:

```text
Ya documentable
Pendiente
No aplica todavía
```

---

# Ejercicio 30 — README final

Completá el README con las secciones que correspondan:

```text
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

No agregues secciones solamente para completar una lista.

---

# Ejercicio 31 — Probar la instalación

Pedile a otra persona que instale el proyecto siguiendo solamente el README.

No le des instrucciones adicionales.

Registrá:

```text
Paso
Resultado
Problema
Corrección
```

Después actualizá el README.

---

# Ejercicio 32 — Probar el uso

Realizá una prueba de uso desde cero.

Documentá:

```text
entrada
ejecución
resultado
```

Verificá que el ejemplo del README coincida con el comportamiento real.

---

# Ejercicio 33 — Auditoría de seguridad

Revisá el repositorio en busca de:

```text
contraseñas
tokens
claves
credenciales
datos personales
información confidencial
```

Marcá:

```text
[ ] Revisado
```

para cada categoría.

---

# Ejercicio 34 — `.gitignore`

Identificá tres archivos o directorios que deberían ser ignorados.

Completá:

| Elemento | ¿Por qué ignorarlo? |
|---|---|
| | |
| | |
| | |

Después incorporá las reglas necesarias.

---

# Ejercicio 35 — Verificar un archivo ignorado

Creá un archivo que deba ser ignorado.

Después:

```bash
git status
```

Verificá que no aparezca como cambio pendiente.

Si necesitás investigar la regla utilizada:

```bash
git check-ignore -v archivo
```

Explicá qué regla lo está ignorando.

---

# Ejercicio 36 — Secreto publicado

Analizá esta situación:

```bash
git add .env
git commit -m "Agrega configuración"
git push
```

Después se agrega:

```text
.env
```

a `.gitignore`.

Respondé:

1. ¿El archivo dejó de existir en la historia?
2. ¿Qué información continúa disponible?
3. ¿Por qué `.gitignore` no soluciona por sí solo el problema?

---

# Ejercicio 37 — Estado del repositorio

Ejecutá:

```bash
git status
```

antes y después de:

```text
modificar
agregar
commitear
cambiar de rama
```

Registrá cómo cambia la información mostrada.

---

# Ejercicio 38 — Remoto

Ejecutá:

```bash
git remote -v
```

Respondé:

```text
¿Qué remoto está configurado?

¿Qué URL utiliza?

¿Qué función cumple `origin`?
```

---

# Ejercicio 39 — Sincronización

Realizá:

```bash
git pull
```

y:

```bash
git push
```

Explicá con tus palabras la diferencia entre ambas operaciones.

---

# Ejercicio 40 — Commit y Pull Request

Compará:

```text
commit
```

y:

```text
Pull Request
```

Completá:

| | Commit | Pull Request |
|---|---|---|
| ¿Qué representa? | | |
| ¿Dónde ocurre? | | |
| ¿Para qué sirve? | | |
| ¿Quién puede revisarlo? | | |

---

# Ejercicio 41 — Issue y Pull Request

Compará:

```text
Issue
```

y:

```text
Pull Request
```

Explicá:

```text
¿Qué problema representa una Issue?

¿Qué representa una Pull Request?

¿Cómo pueden relacionarse?
```

---

# Ejercicio 42 — Rama y commit

Explicá la relación entre:

```text
rama
```

y:

```text
commit
```

Utilizá un ejemplo de tu propio proyecto.

---

# Ejercicio 43 — Documentar una decisión

Elegí una decisión técnica importante.

Completá:

```text
Decisión:
________________________

Problema:
________________________

Alternativas:
________________________

Elección:
________________________

Motivo:
________________________
```

---

# Ejercicio 44 — Documentar una dificultad

Elegí un problema que hayas encontrado.

Completá:

```text
Problema:
________________________

Cómo lo investigué:
________________________

Solución:
________________________

Qué aprendí:
________________________
```

---

# Ejercicio 45 — Revisión final

Revisá:

```text
README
.gitignore
estructura
historial
Issues
Pull Requests
```

Marcá:

```text
[ ] Todo está actualizado.
[ ] No hay información sensible.
[ ] La documentación coincide con el proyecto.
[ ] El historial es comprensible.
[ ] Las tareas relevantes están cerradas.
[ ] Las Pull Requests necesarias están integradas.
```

---

# Ejercicio 46 — Estado final

Ejecutá:

```bash
git status
```

Después:

```bash
git log --oneline --graph --all
```

Describí el estado final del repositorio.

---

# Ejercicio 47 — Caso de estudio

Completá:

```text
Problema:
________________________

Solución:
________________________

Tecnologías:
________________________

Decisiones:
________________________

Dificultades:
________________________

Resultado:
________________________

Aprendizajes:
________________________
```

Después transformá esta información en:

```text
CASO-DE-ESTUDIO.md
```

---

# Ejercicio 48 — Presentación

Prepará una presentación de entre tres y cinco minutos.

Debe responder:

```text
¿Qué problema resolví?

¿Qué construí?

¿Cómo trabajé?

¿Cómo utilicé Git?

¿Cómo utilicé GitHub?

¿Qué dificultad tuve?

¿Qué aprendí?
```

---

# Ejercicio 49 — Preguntas de defensa

Prepará respuestas para:

> ¿Por qué elegiste este proyecto?

> ¿Por qué utilizaste esta tecnología?

> ¿Qué representa este commit?

> ¿Por qué creaste esta rama?

> ¿Qué función cumple esta Issue?

> ¿Qué se revisó en esta Pull Request?

> ¿Cómo resolviste el conflicto?

> ¿Qué mejorarías?

---

# Ejercicio 50 — Revisión externa

Entregale el repositorio a otra persona.

No expliques el proyecto.

Pedile que responda:

```text
¿Qué hace?

¿Cómo se instala?

¿Cómo se utiliza?

¿Qué está bien documentado?

¿Qué resulta confuso?

¿Qué mejorarías?
```

Compará sus respuestas con tus objetivos.

---

# Ejercicio 51 — Antes y después

Compará el estado inicial y final del proyecto.

Completá:

| Aspecto | Antes | Después |
|---|---|---|
| README | | |
| Estructura | | |
| Git | | |
| GitHub | | |
| Seguridad | | |
| Documentación | | |
| Presentación | | |

Después escribí una breve conclusión.

---

# Ejercicio 52 — Evidencia

Para cada afirmación, buscá una evidencia dentro del proyecto.

```text
Sé utilizar Git.
```

Evidencia:

```text
________________________
```

```text
Sé utilizar GitHub.
```

Evidencia:

```text
________________________
```

```text
Sé documentar proyectos.
```

Evidencia:

```text
________________________
```

```text
Sé trabajar colaborativamente.
```

Evidencia:

```text
________________________
```

---

# Ejercicio 53 — Limitaciones

Escribí tres aspectos que el proyecto todavía no resuelve.

```text
1. ______________________
2. ______________________
3. ______________________
```

Después explicá:

> ¿Por qué no los resolviste?

Reconocer el alcance real del proyecto es parte de una buena presentación técnica.

---

# Ejercicio 54 — Próximos pasos

Definí tres mejoras futuras:

```text
1. ______________________
2. ______________________
3. ______________________
```

Asignales:

```text
Alta
Media
Baja
```

---

# Ejercicio 55 — Checklist final

Antes de entregar:

```text
[ ] Proyecto definido.
[ ] Alcance definido.
[ ] Repositorio creado.
[ ] README actualizado.
[ ] .gitignore revisado.
[ ] Issues creadas cuando corresponde.
[ ] Ramas utilizadas.
[ ] Commits claros.
[ ] Pull Requests utilizadas cuando corresponde.
[ ] Revisiones realizadas.
[ ] Conflictos resueltos cuando corresponde.
[ ] Proyecto probado.
[ ] Documentación verificada.
[ ] Sin secretos publicados.
[ ] Caso de estudio preparado.
[ ] Presentación preparada.
```

---

# Ejercicio 56 — Reflexión final

Respondé:

### 1.

¿Qué aprendí sobre Git?

### 2.

¿Qué aprendí sobre GitHub?

### 3.

¿Qué aprendí sobre trabajar con ramas?

### 4.

¿Qué aprendí sobre revisar cambios?

### 5.

¿Qué aprendí sobre documentar?

### 6.

¿Qué aprendí sobre trabajar con otras personas?

### 7.

¿Qué haría diferente si volviera a comenzar?

### 8.

¿Qué quiero seguir aprendiendo después de este curso?

---

# Cierre

Los ejercicios de este módulo no buscan que completes una lista de comandos.

Buscan ayudarte a comprobar que podés integrar las herramientas dentro de un proyecto.

La secuencia fundamental es:

```text
planificar
   ↓
trabajar
   ↓
registrar
   ↓
revisar
   ↓
mejorar
   ↓
integrar
   ↓
documentar
   ↓
presentar
```

> **El Proyecto Final no es el último ejercicio de Git. Es la primera oportunidad de utilizar todo lo aprendido como parte de un proceso completo de trabajo.**