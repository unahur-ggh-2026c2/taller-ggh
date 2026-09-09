# Recursos
## Módulo 02 — Guardar cambios

Los recursos de este módulo están orientados a profundizar en el ciclo de trabajo básico de Git: observar cambios, prepararlos, registrarlos y consultar el historial.

No es necesario estudiar toda la documentación antes de realizar las actividades. Se recomienda utilizarla como material de consulta cuando aparezca una duda concreta.

---

## 1. Pro Git — versión en español

**Chacon, S., & Straub, B. — Pro Git**

Libro de referencia sobre Git, disponible gratuitamente.

https://git-scm.com/book/es/v2

Para este módulo resultan especialmente útiles los contenidos relacionados con:

- guardar cambios en el repositorio;
- registrar cambios;
- consultar el estado;
- trabajar con commits;
- consultar el historial.

No es necesario leer el libro completo.

---

## 2. Documentación oficial de Git

### Git

Sitio oficial del proyecto:

https://git-scm.com/

Documentación completa:

https://git-scm.com/docs

La documentación oficial debe utilizarse como referencia para comprender el comportamiento de los comandos y consultar sus diferentes opciones.

---

## 3. `git status`

Documentación oficial:

https://git-scm.com/docs/git-status

`git status` permite consultar el estado actual del repositorio.

Durante este módulo es especialmente importante utilizarlo:

- después de modificar archivos;
- después de preparar cambios;
- después de realizar un commit.

La información proporcionada por este comando debe interpretarse antes de decidir cuál será la siguiente acción.

---

## 4. `git add`

Documentación oficial:

https://git-scm.com/docs/git-add

`git add` permite agregar cambios al área de preparación.

En este módulo se trabaja especialmente con:

```bash
git add archivo.md
```

La utilización de archivos individuales permite observar con claridad qué cambios estamos seleccionando.

Más adelante se analizarán otras formas de utilizar `git add`.

---

## 5. `git commit`

Documentación oficial:

https://git-scm.com/docs/git-commit

`git commit` permite registrar en el historial los cambios que fueron preparados.

Un commit constituye un punto registrado en la evolución del proyecto.

La documentación permite consultar las diferentes opciones disponibles y comprender con mayor profundidad el funcionamiento del comando.

---

## 6. `git log`

Documentación oficial:

https://git-scm.com/docs/git-log

`git log` permite consultar el historial de commits.

En este módulo se utiliza principalmente:

```bash
git log
```

y:

```bash
git log --oneline
```

La primera forma permite observar información detallada.

La segunda presenta una vista resumida del historial.

---

## 7. Visual Studio Code

### Control de código fuente

Visual Studio Code incorpora herramientas gráficas para trabajar con Git.

https://code.visualstudio.com/docs/sourcecontrol/overview

Estas herramientas permiten observar, entre otras cosas:

- archivos modificados;
- cambios preparados;
- diferencias;
- commits;
- historial.

Durante el curso se recomienda comprender primero la operación y utilizar la interfaz gráfica como complemento.

---

## 8. El modelo de trabajo

Como referencia rápida:

```text
┌──────────────────────┐
│ Área de trabajo      │
│                      │
│ Archivos modificados │
└──────────┬───────────┘
           │
           │ git add
           ▼
┌──────────────────────┐
│ Área de preparación  │
│                      │
│ Cambios seleccionados│
└──────────┬───────────┘
           │
           │ git commit
           ▼
┌──────────────────────┐
│ Historial            │
│                      │
│ Commits              │
└──────────────────────┘
```

Este esquema representa el modelo conceptual que se busca incorporar durante el módulo.

---

## 9. Comandos trabajados

| Comando | Propósito |
|---|---|
| `git status` | Consultar el estado del repositorio |
| `git add archivo` | Preparar cambios de un archivo |
| `git commit -m "mensaje"` | Registrar los cambios preparados |
| `git log` | Consultar el historial |
| `git log --oneline` | Consultar una versión resumida del historial |

No es necesario memorizar la tabla.

El objetivo es poder determinar qué herramienta utilizar según la situación.

---

## 10. Investigar por cuenta propia

Una vez completadas las actividades del módulo, podés investigar:

- `git add .`;
- `git add -A`;
- `git commit -a`;
- opciones de `git status`;
- opciones de `git log`;
- diferencias entre commits;
- autores y fechas de los commits;
- referencias de commits;
- convenciones para mensajes de commit.

Estos contenidos pueden ampliar la comprensión del flujo de trabajo, pero no son necesarios para completar el recorrido principal del módulo.

---

## 11. Una práctica importante

Cuando algo no salga como esperabas, evitá ejecutar comandos al azar.

Utilizá este recorrido:

```text
¿Qué hice?
     ↓
¿Qué esperaba que ocurriera?
     ↓
¿Qué ocurrió realmente?
     ↓
¿Qué informa git status?
     ↓
¿Qué puedo inferir?
     ↓
¿Qué acción corresponde?
     ↓
¿El resultado confirma mi hipótesis?
```

Esta forma de trabajar es más importante que conocer una gran cantidad de comandos.

---

## 12. Para profundizar

Una vez comprendido el flujo básico, resulta útil investigar cómo Git representa internamente los cambios y los commits.

Podés comenzar por:

- objetos de Git;
- árboles;
- blobs;
- referencias;
- HEAD;
- hashes;
- snapshots.

Estos conceptos no forman parte del núcleo necesario para completar este módulo.

Se recomienda abordarlos después de comprender correctamente:

```text
modificar
   ↓
preparar
   ↓
commit
   ↓
historial
```

---

## 13. Recurso principal

Si necesitás consultar solamente tres referencias durante este módulo:

1. **Pro Git — versión en español**  
   https://git-scm.com/book/es/v2

2. **Documentación oficial de Git**  
   https://git-scm.com/docs

3. **Visual Studio Code — Control de código fuente**  
   https://code.visualstudio.com/docs/sourcecontrol/overview

El resto de los recursos puede utilizarse para profundizar según las necesidades de cada estudiante.