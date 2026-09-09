# Recursos
## Módulo 03 — Historial

Los recursos de este módulo están orientados a consultar, interpretar y analizar el historial de un repositorio Git.

La documentación debe utilizarse principalmente como material de consulta. No es necesario leerla completa antes de realizar las actividades.

---

## 1. Pro Git — versión en español

**Chacon, S., & Straub, B. — Pro Git**

Libro de referencia sobre Git, disponible gratuitamente en español.

https://git-scm.com/book/es/v2

Para este módulo resultan especialmente útiles los contenidos relacionados con:

- visualización del historial;
- commits;
- referencias;
- recuperación de información;
- trabajo con el historial.

No es necesario recorrer el libro de manera lineal.

---

## 2. Documentación oficial de Git

### Git

Sitio oficial:

https://git-scm.com/

Documentación:

https://git-scm.com/docs

La documentación oficial permite consultar el comportamiento detallado de los comandos y sus diferentes opciones.

---

## 3. `git log`

Documentación oficial:

https://git-scm.com/docs/git-log

`git log` permite consultar el historial de commits.

Es el comando principal trabajado durante este módulo.

La información mostrada permite observar, entre otros datos:

- identificador del commit;
- autor;
- fecha;
- mensaje;
- relación temporal entre commits.

---

## 4. `git log --oneline`

La opción:

```bash
git log --oneline
```

permite obtener una representación resumida del historial.

Resulta especialmente útil para:

- observar rápidamente muchos commits;
- identificar commits;
- analizar la secuencia de evolución;
- revisar los mensajes.

La forma resumida no reemplaza a `git log`.

Ambas representaciones permiten observar aspectos diferentes del mismo historial.

---

## 5. Identificación de commits

Cada commit posee un identificador único.

En una vista resumida puede observarse una representación abreviada:

```text
a84f9c2
```

Este identificador permite referirse a un punto concreto de la historia.

En este módulo no es necesario profundizar en los mecanismos internos mediante los cuales Git genera estos identificadores.

El objetivo es comprender su función dentro del historial.

---

## 6. Visual Studio Code

### Control de código fuente

Visual Studio Code incluye herramientas para trabajar con Git:

https://code.visualstudio.com/docs/sourcecontrol/overview

Estas herramientas permiten consultar diferentes aspectos del repositorio y del historial.

Durante el curso se recomienda comprender primero los conceptos y operaciones mediante Git y utilizar la interfaz gráfica como complemento.

---

## 7. Modelo conceptual

Como referencia rápida:

```text
Proyecto
   │
   ├── Commit 1
   │      ↓
   ├── Commit 2
   │      ↓
   ├── Commit 3
   │      ↓
   ├── Commit 4
   │      ↓
   └── Estado actual
```

Cada commit representa un punto registrado de la evolución del proyecto.

El historial permite recorrer esos puntos y analizar cómo se llegó hasta el estado actual.

---

## 8. Comandos trabajados

| Comando | Propósito |
|---|---|
| `git log` | Consultar el historial detallado |
| `git log --oneline` | Consultar una versión resumida del historial |
| `git status` | Consultar el estado actual del repositorio |

En este módulo `git status` continúa siendo importante porque permite contrastar:

```text
estado actual
```

con:

```text
historial registrado
```

---

## 9. Investigar por cuenta propia

Una vez comprendidos los contenidos principales del módulo, podés investigar:

- opciones de formato de `git log`;
- cantidad de commits mostrados;
- filtros por autor;
- filtros temporales;
- búsqueda dentro de mensajes;
- diferencias entre commits;
- `git show`.

Estos contenidos amplían las posibilidades de consulta del historial.

No son necesarios para completar el recorrido principal del módulo.

---

## 10. `git show`

Como extensión del trabajo con el historial, podés investigar:

```bash
git show
```

Este comando permite profundizar sobre un commit concreto.

Mientras:

```bash
git log
```

responde principalmente:

> ¿Qué commits existen?

`git show` permite comenzar a investigar:

> ¿Qué contiene este commit?

Este recurso constituye un puente natural hacia el trabajo posterior con diferencias y recuperación de información.

---

## 11. Estrategia de investigación

Cuando necesites investigar cómo evolucionó algo, evitá comenzar ejecutando comandos al azar.

Podés utilizar este recorrido:

```text
¿Qué quiero averiguar?
        ↓
¿Qué información ya tengo?
        ↓
Consultar historial
        ↓
Identificar commits relevantes
        ↓
Seleccionar un punto de interés
        ↓
Investigar el commit
        ↓
Verificar la evidencia
        ↓
Formular una conclusión
```

La herramienta es importante, pero el razonamiento que guía la investigación lo es todavía más.

---

## 12. Recurso principal

Si necesitás conservar solamente tres referencias para este módulo:

1. **Pro Git — versión en español**  
   https://git-scm.com/book/es/v2

2. **Documentación oficial de Git**  
   https://git-scm.com/docs

3. **Referencia de `git log`**  
   https://git-scm.com/docs/git-log

El resto de los recursos puede utilizarse para profundizar según las necesidades de cada estudiante.