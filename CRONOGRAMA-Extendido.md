# Cronograma del Curso — Git y GitHub

## Implementación UNAHUR — 6 semanas

---

# 1. Datos generales

| Concepto                 |            Dedicación |
| ------------------------ | --------------------: |
| Duración                 |             6 semanas |
| Clases sincrónicas       |                     6 |
| Duración por clase       |                   4 h |
| Trabajo sincrónico total |                  24 h |
| Trabajo autónomo total   |                  26 h |
| Dedicación total         |              **50 h** |
| Módulos                  |             **00–09** |
| Modalidad                | Sincrónica + autónoma |

El recorrido comprende los **10 módulos del curso**, desde **00 — ¿Por qué Git?** hasta **09 — Proyecto final integrador**.

La reducción temporal no elimina módulos. **Reorganiza la profundidad y el lugar donde se desarrolla cada contenido.**

---

# 2. Principio de organización

La distribución se basa en una distinción:

```text
CONTENIDOS QUE NECESITAN
INTERACCIÓN PEDAGÓGICA

        ↓

SINCRÓNICO
```

y:

```text
CONTENIDOS QUE PUEDEN
DESARROLLARSE AUTÓNOMAMENTE

        ↓

TRABAJO AUTÓNOMO
```

La clase sincrónica prioriza:

* construcción conceptual;
* modelización;
* demostraciones;
* práctica guiada;
* interpretación;
* errores;
* situaciones problemáticas;
* decisiones;
* revisión;
* feedback;
* conflictos.

El trabajo autónomo prioriza:

* práctica repetida;
* ejercicios;
* profundización;
* lectura;
* experimentación;
* documentación;
* desafíos;
* producción;
* proyecto.

Por lo tanto:

> **No se reduce el curso simplemente quitando contenidos. Se decide qué necesita ser enseñado sincrónicamente y qué puede ser aprendido, practicado o profundizado autónomamente.**

---

# 3. Distribución general

| Semana    | Sincrónico | Trabajo autónomo | Módulos                                                      |
| --------- | ---------: | ---------------: | ------------------------------------------------------------ |
| 1         |        4 h |              4 h | **00 — ¿Por qué Git? + 01 — Mi primer repositorio**          |
| 2         |        4 h |              4 h | **02 — Guardar cambios + 03 — Historial**                    |
| 3         |        4 h |              4 h | **04 — GitHub + 05 — Markdown**                              |
| 4         |        4 h |              4 h | **06 — Ramas**                                               |
| 5         |        4 h |              5 h | **07 — Trabajo colaborativo**                                |
| 6         |        4 h |              5 h | **08 — Perfil profesional + 09 — Proyecto final integrador** |
| **Total** |   **24 h** |         **26 h** | **00–09**                                                    |


---

# 4. Distribución de M00 — ¿Por qué Git?

## Semana 1

### Modalidad

**Sincrónica + autónoma.**

### Dedicación orientativa

* **Sincrónica:** 1 h
* **Autónoma:** 2 h

### Función

M00 introduce el problema que da sentido a todo el curso:

```text
los proyectos cambian
        ↓
necesitamos registrar esos cambios
        ↓
necesitamos comprender su evolución
        ↓
Git
```

El módulo establece el marco conceptual sobre el que se construirá el resto del recorrido. Su función no es enseñar comandos exhaustivamente, sino construir una primera comprensión del problema y de la herramienta. 

### Sincrónico — 1 h

Se trabajará:

* problema del control de versiones;
* situaciones concretas de pérdida o modificación de archivos;
* diferencia entre una copia y un historial;
* qué es Git;
* qué es un repositorio;
* Git ≠ GitHub;
* visión general del recorrido.

Se mantiene el enfoque recomendado para el módulo:

```text
explicación
    ↓
situación problemática
    ↓
discusión
    ↓
demostración
    ↓
experimentación
    ↓
reflexión
```

Este enfoque está expresamente previsto para M00. 

### Autónomo — 2 h

* lectura del módulo;
* actividad introductoria;
* diagnóstico;
* ejemplos sobre control de versiones;
* preparación del entorno;
* instalación/verificación de Git;
* verificación de VS Code y terminal.

### Evidencia

El estudiante debería poder explicar:

> ¿Por qué utilizaría Git en un proyecto?

y distinguir:

```text
Git
≠
GitHub
```

---

# 5. Semana 1 — ¿Por qué Git + Mi primer repositorio

## Módulos

**00 — ¿Por qué Git?**

**01 — Mi primer repositorio**

### Dedicación

* **Sincrónica:** 4 h
* **Autónoma:** 4 h

---

## Clase sincrónica — 4 h

### Bloque 1 — M00: ¿Por qué Git?

**60 min**

Construcción del problema:

```text
archivos
 ↓
cambios
 ↓
versiones
 ↓
necesidad de historial
 ↓
Git
```

No se busca terminar M00 con dominio técnico.

Se busca que el estudiante comprenda **por qué existe la herramienta**.

---

### Bloque 2 — M01: Repositorio

**45 min**

Trabajar:

* Git;
* repositorio;
* carpeta de trabajo;
* `.git`;
* repositorio local.

Modelo:

```text
PROYECTO
├── archivos
│
└── .git
```

---

### Bloque 3 — Práctica guiada

**75 min**

Crear un repositorio real.

Trabajar:

```bash
git init
git status
```

Observar qué cambia antes y después de inicializar.

---

### Bloque 4 — Ejercicio

**45 min**

Crear un segundo repositorio con menor nivel de asistencia.

El estudiante debe reproducir el proceso comprendiendo qué está haciendo.

---

### Bloque 5 — Cierre

**15 min**

Situaciones rápidas:

* Git fuera de un repositorio;
* identificar `.git`;
* distinguir carpeta y repositorio;
* explicar por qué Git funciona sin GitHub.

---

## Trabajo autónomo — 4 h

### M00 — 2 h

* lectura;
* actividad introductoria;
* diagnóstico;
* preparación del entorno.

### M01 — 2 h

* práctica con repositorios;
* ejercicios con `git status`;
* creación de un repositorio propio;
* desafío sencillo.

### Evidencia

```text
repositorio
   ↓
archivos
   ↓
git status
   ↓
interpretación
```

---

# 6. Semana 2 — Guardar cambios e Historial

## Módulos

**02 — Guardar cambios**

**03 — Historial**

### Dedicación

* **Sincrónica:** 4 h
* **Autónoma:** 4 h

---

## Clase sincrónica — 4 h

### Bloque 1 — Recuperación

**20 min**

Partir del repositorio de la semana anterior.

Pregunta:

> ¿Cómo registramos ahora los cambios?

---

### Bloque 2 — M02: ciclo básico

**70 min**

Construir:

```text
modificar
   ↓
observar
   ↓
preparar
   ↓
registrar
```

Trabajar:

```bash
git status
git add
git commit
```

---

### Bloque 3 — Práctica

**60 min**

Modificar distintos archivos y observar los cambios de estado.

---

### Bloque 4 — M03: Historial

**40 min**

Trabajar:

```bash
git log
git log --oneline
```

Analizar:

* hash;
* autor;
* fecha;
* mensaje;
* secuencia.

---

### Bloque 5 — Interpretación y cierre

**50 min**

Presentar historiales.

Consigna:

> Reconstruí qué ocurrió en el proyecto solamente a partir del historial.

El objetivo es pasar de:

```text
ver commits
```

a:

```text
interpretar historia
```

---

## Trabajo autónomo — 4 h

### M02

* crear varios commits;
* experimentar con archivos preparados parcialmente;
* ejercicios de `status`;
* práctica de mensajes significativos.

### M03

* lectura de historiales;
* reconstrucción de secuencias;
* desafío de crear una historia comprensible.

### Evidencia

```text
modificación
   ↓
git add
   ↓
commit
   ↓
git log
   ↓
interpretación
```

---

# 7. Semana 3 — GitHub y Markdown

## Módulos

**04 — GitHub**

**05 — Markdown**

### Dedicación

* **Sincrónica:** 4 h
* **Autónoma:** 4 h

---

## Clase sincrónica — 4 h

### Bloque 1 — GitHub

**30 min**

Diferenciar:

```text
Git
↓
control de versiones

GitHub
↓
plataforma
↓
repositorios remotos
↓
colaboración
```

---

### Bloque 2 — Local y remoto

**45 min**

Construir:

```text
LOCAL
 ↓
commit
 ↓
push
 ↓
REMOTO
```

y:

```text
REMOTO
 ↓
pull
 ↓
LOCAL
```

---

### Bloque 3 — Práctica

**70 min**

* crear repositorio remoto;
* conectar local y remoto;
* identificar `origin`;
* realizar `push`;
* comprobar cambios.

---

### Bloque 4 — Diagnóstico

**35 min**

Situaciones:

* commit sin push;
* cambios locales;
* cambios remotos;
* diferencias entre local y remoto.

---

### Bloque 5 — Markdown

**20 min**

Introducir Markdown desde la comunicación:

```text
qué quiero comunicar
        ↓
cómo organizarlo
        ↓
qué sintaxis necesito
```

---

### Bloque 6 — Práctica inicial

**40 min**

* títulos;
* listas;
* énfasis;
* enlaces;
* código;
* bloques de código;
* tablas;
* citas.

---

### Bloque 7 — Cierre

**20 min**

Relacionar:

```text
Markdown
 ↓
README
 ↓
Git
 ↓
GitHub
```

---

## Trabajo autónomo — 4 h

### M04

* práctica de sincronización;
* ejercicios local/remoto;
* resolución de situaciones;
* profundización en `pull` y `fetch`.

### M05

* práctica Markdown;
* construcción de README;
* documentación de un repositorio.

### Evidencia

Repositorio remoto con:

```text
README.md
+
historial Git
+
GitHub
```

---

# 8. Semana 4 — Ramas

## Módulo

**06 — Ramas**

### Dedicación

* **Sincrónica:** 4 h
* **Autónoma:** 4 h

---

## Clase sincrónica — 4 h

### Bloque 1 — Necesidad de ramas

**35 min**

Situación:

> Necesitamos desarrollar algo nuevo sin modificar directamente la línea principal.

---

### Bloque 2 — Crear y cambiar ramas

**45 min**

Trabajar:

```bash
git branch
git switch
git switch -c
```

y utilizar:

```bash
git status
```

como hábito.

---

### Bloque 3 — Ramas y commits

**45 min**

Construir visualmente:

```text
A ── B ── C
          \
           D ── E
```

Introducir progresivamente `HEAD`.

---

### Bloque 4 — Práctica

**60 min**

* crear rama;
* modificar;
* commit;
* volver a `main`;
* modificar;
* observar divergencia.

---

### Bloque 5 — Merge

**35 min**

Trabajar:

```bash
git switch main
git merge feature
```

Enfatizar:

> La rama actual es la rama sobre la que se realiza la integración.

---

## Trabajo autónomo — 4 h

* crear y utilizar ramas;
* interpretar diagramas;
* practicar merges;
* explorar ramas locales/remotas;
* estudiar `HEAD`;
* resolver un desafío de desarrollo sin modificar directamente `main`.

### Evidencia

El estudiante debe poder explicar:

```text
main
 ↓
historia

feature
 ↓
otra línea de evolución
```

y cómo se integran ambas.

---

# 9. Semana 5 — Trabajo colaborativo

## Módulo

**07 — Trabajo colaborativo**

### Dedicación

* **Sincrónica:** 4 h
* **Autónoma:** 5 h

Esta semana concentra el principal salto conceptual:

```text
mi historia
   ↓
historia compartida
```

El módulo establece como prioridad presencial la diferencia Git/GitHub, ramas colaborativas, `push`, `pull`, Pull Requests, revisión, integración y conflictos básicos; mientras que `fetch`, documentación de colaboración y protección de ramas pueden profundizarse autónomamente. 

---

## Clase sincrónica — 4 h

### Bloque 1 — El problema colaborativo

**30 min**

Pregunta:

> ¿Qué cambia cuando otra persona también trabaja sobre este repositorio?

---

### Bloque 2 — Flujo colaborativo

**40 min**

```text
tarea
 ↓
rama
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

---

### Bloque 3 — Práctica colaborativa

**75 min**

Idealmente en parejas.

Cada participante:

* toma una tarea;
* crea una rama;
* realiza commits;
* publica la rama;
* crea una Pull Request.

---

### Bloque 4 — Revisión

**35 min**

El compañero revisa.

Se trabaja:

```text
observar
 ↓
comprender
 ↓
preguntar
 ↓
sugerir
```

La revisión debe entenderse como trabajo técnico, no como búsqueda de errores ajenos.

---

### Bloque 5 — Corrección e integración

**60 min**

```text
feedback
 ↓
corrección
 ↓
nuevo commit
 ↓
revisión
 ↓
merge
```

---

## Trabajo autónomo — 5 h

### Ejercicios

* Issue vs. Pull Request;
* commit vs. Pull Request;
* push vs. pull;
* pull vs. fetch.

### Práctica

Continuar un flujo colaborativo.

### Desafío

Diseñar el flujo para que dos personas trabajen sobre un mismo proyecto sin modificar directamente `main`.

### Conflicto

Resolver un conflicto controlado:

```text
dos cambios
   ↓
conflicto
   ↓
análisis
   ↓
decisión
   ↓
resolución
```

### Profundización

* `fetch`;
* convenciones;
* `CONTRIBUTING.md`;
* `CODE_OF_CONDUCT.md`;
* protección de ramas.

### Evidencia

```text
Issue
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
corrección
 ↓
merge
```

---

# 10. Semana 6 — Perfil profesional y Proyecto final integrador

## Módulos

**08 — Perfil profesional**

**09 — Proyecto final integrador**

### Dedicación

* **Sincrónica:** 4 h
* **Autónoma:** 5 h

La última semana cambia deliberadamente de lógica:

```text
aprender herramientas
        ↓
utilizar herramientas
        ↓
producir evidencia
```

---

# Parte A — Módulo 08 — Perfil profesional

## Clase sincrónica

### Bloque 1 — De conocimiento a evidencia

**25 min**

```text
conocimiento
 ↓
práctica
 ↓
proyecto
 ↓
documentación
 ↓
evidencia
```

---

### Bloque 2 — README como presentación

**35 min**

Analizar repositorios.

Preguntas:

* ¿Qué hace?
* ¿Para qué sirve?
* ¿Cómo se instala?
* ¿Cómo se utiliza?
* ¿Qué necesita saber alguien que llega por primera vez?

---

### Bloque 3 — Seguridad y `.gitignore`

**35 min**

Trabajar:

```text
secretos
tokens
claves
credenciales
```

y:

```text
.gitignore
```

Diferenciar claramente:

```text
prevenir
```

de:

```text
eliminar algo
que ya fue registrado
```

---

### Bloque 4 — Actividad de mejora

**45 min**

Seleccionar un proyecto y analizar:

```text
README
estructura
historial
documentación
.gitignore
```

Definir mejoras concretas.

---

# Parte B — Módulo 09 — Proyecto final integrador

## Clase sincrónica

### Bloque 5 — Definición

**30 min**

Cada estudiante determina:

```text
qué voy a hacer
        ↓
qué voy a demostrar
        ↓
qué evidencia voy a producir
```

---

### Bloque 6 — Planificación

**30 min**

Según corresponda:

```text
Issue
 ↓
rama
 ↓
tarea
 ↓
commits
 ↓
documentación
 ↓
Pull Request
```

---

### Bloque 7 — Desafío integrador

**30 min**

Consigna:

> Organizá y desarrollá una mejora o pequeño proyecto utilizando Git y GitHub. El resultado debe permitir reconstruir razonablemente cómo trabajaste.

El estudiante decide:

* qué hacer;
* cómo organizarlo;
* qué ramas utilizar;
* qué commits realizar;
* cómo documentarlo;
* cómo revisarlo.

---

### Bloque 8 — Cierre

**40 min**

Presentación de avances/proyectos.

Preguntas:

* ¿Qué problema resolviste?
* ¿Qué aprendiste?
* ¿Qué decisión fue difícil?
* ¿Qué evidencia quedó en Git?
* ¿Qué mejorarías?

---

## Trabajo autónomo — 5 h

Este constituye el principal bloque de producción del Proyecto Final.

### Etapa 1 — Organización

```text
repositorio
README
.gitignore
Issues
```

### Etapa 2 — Desarrollo

```text
ramas
commits
push
```

### Etapa 3 — Revisión

```text
Pull Request
```

cuando corresponda.

### Etapa 4 — Documentación

Mejorar README y documentación.

### Etapa 5 — Revisión final

Comprobar:

```bash
git status
```

y:

```bash
git log --oneline --graph --all
```

Revisar el repositorio publicado.

### Evidencia final

```text
Repositorio
    +
README
    +
.gitignore
    +
historial
    +
evidencia de trabajo
    +
presentación
```

---

# 11. Distribución definitiva de las 26 horas autónomas

| Semana    |    Horas | Trabajo autónomo principal |
| --------- | -------: | -------------------------- |
| 1         |  **4 h** | M00 + M01                  |
| 2         |  **4 h** | M02 + M03                  |
| 3         |  **4 h** | M04 + M05                  |
| 4         |  **4 h** | M06                        |
| 5         |  **5 h** | M07                        |
| 6         |  **5 h** | M08 + M09                  |
| **Total** | **26 h** |                            |

---

# 12. Distribución definitiva de las 24 horas sincrónicas

| Semana    |    Horas | Módulos                                                  |
| --------- | -------: | -------------------------------------------------------- |
| 1         |  **4 h** | 00 — ¿Por qué Git? + 01 — Mi primer repositorio          |
| 2         |  **4 h** | 02 — Guardar cambios + 03 — Historial                    |
| 3         |  **4 h** | 04 — GitHub + 05 — Markdown                              |
| 4         |  **4 h** | 06 — Ramas                                               |
| 5         |  **4 h** | 07 — Trabajo colaborativo                                |
| 6         |  **4 h** | 08 — Perfil profesional + 09 — Proyecto final integrador |
| **Total** | **24 h** | **00–09**                                                |

---

# 13. Mapa completo del recorrido

```text
00 — ¿Por qué Git?
        ↓
01 — Mi primer repositorio
        ↓
02 — Guardar cambios
        ↓
03 — Historial
        ↓
04 — GitHub
        ↓
05 — Markdown
        ↓
06 — Ramas
        ↓
07 — Trabajo colaborativo
        ↓
08 — Perfil profesional
        ↓
09 — Proyecto final integrador
```

Conceptualmente:

```text
problema
   ↓
repositorio
   ↓
cambio
   ↓
registro
   ↓
historia
   ↓
publicación
   ↓
documentación
   ↓
ramificación
   ↓
colaboración
   ↓
evidencia
   ↓
integración
```

---

# 14. Distribución metodológica

La metodología permanece intacta:

```text
CONCEPTO
   ↓
DEMOSTRACIÓN
   ↓
PRÁCTICA
   ↓
EJERCICIO
   ↓
DESAFÍO
   ↓
PROYECTO
```

Pero se distribuye entre las dos modalidades.

| Instancia      | Sincrónico                | Autónomo                 |
| -------------- | ------------------------- | ------------------------ |
| Concepto       | **Principal**             | Lectura/refuerzo         |
| Demostración   | **Principal**             | —                        |
| Práctica       | **Guiada**                | **Consolidación**        |
| Ejercicio      | Introducción / corrección | **Principal**            |
| Desafío        | Seleccionado              | **Principal**            |
| Proyecto       | Orientación / seguimiento | **Producción principal** |
| Errores        | **Principal**             | Experimentación          |
| Feedback       | **Principal**             | Aplicación               |
| Profundización | Complementaria            | **Principal**            |

---

# 15. Qué contenidos son prioritariamente sincrónicos

Dado que las horas son limitadas, se priorizan presencialmente los contenidos que forman el núcleo del curso:

```text
M00
modelo conceptual

M01
repositorio

M02
cambios
staging
commits

M03
historial

M04
local/remoto
GitHub
sincronización

M06
ramas
merge

M07
colaboración
Pull Requests
revisión
conflictos

M09
integración
```

Estos contenidos constituyen el núcleo que no conviene trasladar completamente al trabajo autónomo. 

---

# 16. Qué contenidos tienen mayor peso autónomo

Se desplazan hacia el trabajo autónomo, sin desaparecer:

```text
M00
lecturas y preparación

M03
ejercitación adicional sobre historial

M04
profundización de sincronización

M05
sintaxis y práctica extendida de Markdown

M06
HEAD
ramas remotas
variantes
exploración adicional

M07
fetch
CONTRIBUTING.md
CODE_OF_CONDUCT.md
protección de ramas

M08
portfolio
curaduría
mejora documental

M09
producción del proyecto
```

Esto respeta el criterio del proyecto de que los contenidos complementarios puedan desarrollarse mediante actividades autónomas sin eliminar el núcleo formativo. 

---

# 17. Progresión de autonomía

La distribución también busca producir una progresión deliberada.

### Semanas 1–2

```text
docente
  ↓
modela
  ↓
estudiante reproduce
```

### Semanas 3–4

```text
docente
  ↓
plantea situación
  ↓
estudiante aplica
```

### Semanas 5–6

```text
situación
   ↓
análisis
   ↓
decisión
   ↓
acción
   ↓
evidencia
```

Esto coincide con el criterio transversal establecido para el curso:

```text
seguir instrucciones
        ↓
reconocer qué herramienta utilizar
        ↓
diagnosticar
        ↓
decidir autónomamente
```

La meta no es que el estudiante memorice comandos, sino que pueda enfrentarse a un repositorio real y decidir cómo continuar. 

---

# 18. Hilo conductor de las seis semanas

```text
SEMANA 1
¿Por qué necesitamos Git?
        ↓
¿Cómo creo un repositorio?

SEMANA 2
¿Cómo registro un cambio?
        ↓
¿Cómo leo lo que ocurrió?

SEMANA 3
¿Cómo comparto el repositorio?
        ↓
¿Cómo comunico lo que contiene?

SEMANA 4
¿Cómo trabajo sin alterar
la línea principal?

SEMANA 5
¿Cómo trabajo con otras personas?

SEMANA 6
¿Cómo convierto todo esto
en evidencia de trabajo?
        ↓
¿Cómo integro lo aprendido
en un proyecto?
```

---

# 19. Resultado esperado

Al finalizar las seis semanas, el estudiante debería haber recorrido **los diez módulos**, sin convertir las 24 horas sincrónicas en una carrera de comandos.

Debería poder pasar de:

> **“Sé ejecutar algunos comandos de Git.”**

a:

> **“Puedo utilizar Git y GitHub para trabajar de manera organizada sobre la evolución de un proyecto.”**

Y, fundamentalmente, debería poder responder ante una situación nueva:

```text
Tengo un proyecto.

        ↓

Necesito modificarlo.

        ↓

Quiero registrar lo que hago.

        ↓

Necesito poder entender la historia.

        ↓

Quiero compartirlo.

        ↓

Necesito documentarlo.

        ↓

Quiero trabajar en una línea separada.

        ↓

Necesito coordinarme con otra persona.

        ↓

Quiero revisar e integrar cambios.

        ↓

Quiero poder mostrar evidencia
del trabajo realizado.
```

Ese es el recorrido que articula **00–09**.

---

# 20. Principio rector

> **Los diez módulos forman un único recorrido formativo. Las seis semanas no reemplazan módulos ni los sacan del curso: distribuyen sus contenidos entre instancias sincrónicas y autónomas según el valor pedagógico de cada modalidad.**

Y la regla operativa para UNAHUR queda:

> **24 horas para construir modelos, demostrar, practicar con acompañamiento, discutir, resolver problemas y revisar; 26 horas para practicar, ejercitar, profundizar, desafiar y producir.**

