# Desafíos
## Módulo 01 — Mi primer repositorio

Los desafíos de este módulo buscan que puedas trabajar con Git con mayor autonomía.

No se trata solamente de repetir una secuencia de comandos.

El objetivo es que puedas **observar el estado de un repositorio, interpretar lo que Git informa y decidir qué acción corresponde realizar**.

---

## Desafío 1 — Crear un repositorio desde cero

Sin consultar la práctica anterior, creá un repositorio llamado:

```text
desafio-repositorio
```

El proyecto debe contener:

```text
README.md
objetivos.md
notas.md
```

Realizá las acciones necesarias para:

1. convertir la carpeta en un repositorio;
2. comprobar que Git reconoce el proyecto;
3. preparar los archivos;
4. registrar un primer commit;
5. comprobar el estado final.

### Condición

No copies una secuencia de comandos de la práctica.

Pensá qué necesita ocurrir en cada etapa.

---

## Desafío 2 — El repositorio que no existe

Abrís una terminal y ejecutás:

```bash
git status
```

Git responde indicando que la carpeta actual no es un repositorio.

### Tu desafío

Sin buscar inmediatamente la solución en Internet:

1. interpretá el mensaje;
2. explicá qué significa;
3. determiná qué debería existir para que `git status` funcione;
4. proponé una solución.

Después comprobá tu hipótesis.

---

## Desafío 3 — Encontrar el repositorio

Tenés esta estructura:

```text
cursos/
├── git/
│   └── laboratorio/
│       ├── README.md
│       └── .git/
│
├── python/
│   ├── README.md
│   └── .git/
│
└── apuntes/
    └── comandos.md
```

Estás ubicado en:

```text
cursos/
```

### Preguntas

1. ¿Es `cursos/` un repositorio?
2. ¿Es `git/` un repositorio?
3. ¿Es `laboratorio/` un repositorio?
4. ¿Es `python/` un repositorio?
5. ¿Qué ocurriría si ejecutaras `git status` desde `laboratorio/`?
6. ¿Qué ocurriría desde `apuntes/`?

Explicá tus respuestas.

---

## Desafío 4 — El archivo que Git no conoce

Tenés un repositorio con un commit inicial.

Después creás:

```text
README.md
objetivos.md
notas.md
```

y Git informa que los tres archivos no están siendo rastreados.

### Tu desafío

Prepará solamente:

```text
README.md
```

Después consultá el estado.

Ahora prepará:

```text
notas.md
```

y volvé a consultar el estado.

### Pregunta

¿Qué información te proporciona `git status` que no podrías obtener simplemente mirando la carpeta con el explorador de archivos?

---

## Desafío 5 — Algo quedó afuera

Partís de un repositorio limpio.

Modificás:

```text
README.md
objetivos.md
notas.md
```

Preparás solamente dos de ellos y realizás un commit.

Después ejecutás:

```bash
git status
```

### Tu desafío

Sin abrir el historial todavía:

1. identificá qué cambio quedó fuera;
2. explicá por qué;
3. prepará el cambio pendiente;
4. registralo en un segundo commit.

### Pregunta

¿Por qué Git permite que un commit contenga solamente algunos de los cambios realizados?

---

## Desafío 6 — El commit demasiado grande

Imaginá que durante una tarde realizaste estos cambios:

```text
README.md
    Corrección de una descripción.

objetivos.md
    Incorporación de nuevos objetivos.

integrantes.md
    Actualización de integrantes.

notas.md
    Nuevas notas personales.
```

Todos fueron preparados y registrados en un único commit:

```text
Actualiza proyecto
```

### Tu desafío

Analizá si considerás que fue una buena decisión.

Después proponé cómo dividirías los cambios en commits más significativos.

No existe una única solución.

Lo importante es justificar la decisión.

---

## Desafío 7 — Mensajes que cuentan una historia

Tenés este historial:

```text
cambios
cambios2
arreglos
cosas
update
final
final2
ahora-si
```

Y otro:

```text
Crea estructura inicial del proyecto
Agrega objetivos de la documentación
Actualiza integrantes
Corrige descripción del proyecto
Agrega instrucciones de instalación
```

### Tu desafío

Compará ambos historiales.

Respondé:

1. ¿Cuál permite comprender mejor la evolución del proyecto?
2. ¿Qué información aporta un buen mensaje?
3. ¿Qué debería poder reconstruir una persona leyendo el historial?
4. ¿Un mensaje de commit debería describir cada línea modificada?

Justificá.

---

## Desafío 8 — Recuperar el control

Estás trabajando sobre un repositorio.

Realizaste modificaciones en varios archivos y ya no estás seguro de qué cambiaste.

Antes de hacer cualquier otra cosa:

### Tu desafío

Determiná qué herramienta o información de Git utilizarías para observar la situación actual.

No busques todavía cómo deshacer cambios.

Primero respondé:

> **¿Qué necesito saber antes de decidir qué hacer?**

Después consultá el estado del repositorio y compará la información obtenida con tu hipótesis.

---

## Desafío 9 — El commit que no aparece

Un estudiante afirma:

> "Hice `git add` y mi cambio desapareció."

Le pedís que ejecute:

```bash
git status
```

y observás que el archivo aparece como preparado.

### Tu desafío

Explicale qué ocurrió.

Tu explicación debe distinguir claramente:

```text
modificación
     ↓
preparación
     ↓
commit
```

El objetivo es que puedas detectar el error conceptual de la afirmación.

---

## Desafío 10 — El commit que no contiene lo esperado

Un estudiante ejecutó:

```bash
git add README.md
git commit -m "Actualiza documentación"
```

Pero había modificado:

```text
README.md
objetivos.md
notas.md
```

Después se sorprende porque los otros dos archivos siguen apareciendo como modificados.

### Tu desafío

Explicá exactamente por qué ocurrió.

Después indicá qué debería hacer para registrar los otros cambios.

---

## Desafío 11 — Dos repositorios

Creá:

```text
proyecto-a/
proyecto-b/
```

Inicializá ambos como repositorios Git.

En `proyecto-a` creá:

```text
README.md
```

y realizá un commit.

En `proyecto-b` creá:

```text
README.md
```

pero no realices ningún commit.

### Tu desafío

Compará:

```bash
git status
```

en ambos repositorios.

Explicá por qué el mismo nombre de archivo puede encontrarse en situaciones diferentes.

---

## Desafío 12 — El repositorio contaminado

Por error inicializaste Git en una carpeta demasiado alta:

```text
mis-proyectos/
├── curso-git/
├── proyecto-python/
├── apuntes/
└── pruebas/
```

La carpeta `mis-proyectos/` ahora contiene:

```text
.git/
```

### Tu desafío

Analizá el problema.

Respondé:

1. ¿Qué proyectos quedaron dentro de ese repositorio?
2. ¿Por qué puede ser una mala idea?
3. ¿Qué deberías haber hecho?
4. ¿Cómo comprobarías dónde está realmente el repositorio?

No elimines nada hasta comprender qué ocurrió.

---

## Desafío 13 — Detectar un error de procedimiento

Un compañero realiza:

```bash
git init
git commit -m "Primer commit"
```

Git informa que no hay nada para registrar.

### Tu desafío

Explicá por qué puede ocurrir esto.

Pensá en la secuencia completa:

```text
crear/modificar archivos
        ↓
preparar cambios
        ↓
registrar cambios
```

¿Qué paso falta?

---

## Desafío 14 — La prueba de autonomía

Creá un repositorio nuevo llamado:

```text
desafio-autonomia
```

No mires las prácticas anteriores.

El proyecto debe contener:

```text
README.md
objetivos.md
historia.md
```

Realizá:

1. inicialización;
2. creación de archivos;
3. consulta del estado;
4. preparación;
5. primer commit;
6. modificación de un archivo;
7. nueva consulta del estado;
8. preparación del cambio;
9. segundo commit;
10. consulta final del estado.

### Condición

Si aparece un problema, no copies inmediatamente la solución.

Primero:

1. leé el mensaje;
2. identificá qué te está diciendo Git;
3. formulá una hipótesis;
4. probá una solución;
5. verificá el resultado.

---

## Desafío 15 — Explicar sin comandos

Explicale a una persona que nunca utilizó Git qué significa:

> "El archivo está modificado, pero el cambio todavía no está preparado."

No podés utilizar comandos.

La explicación debe utilizar una situación cotidiana o una analogía.

Después explicá:

> "El cambio está preparado, pero todavía no forma parte del historial."

Nuevamente, sin comandos.

---

## Desafío 16 — El mapa mental

Construí un mapa que relacione:

```text
carpeta
repositorio
archivo
cambio
estado
staging
commit
historial
```

Podés utilizar Markdown, un diagrama o una herramienta visual.

El mapa debe mostrar las relaciones entre los conceptos.

No se evalúa el diseño.

Se evalúa que las relaciones sean correctas.

---

## Desafío 17 — ¿Qué sabe Git?

Para cada situación indicá qué información puede conocer Git:

| Situación | ¿Git puede saberlo? | ¿Por qué? |
|---|:---:|---|
| Existe un archivo en la carpeta | | |
| El archivo fue modificado | | |
| El archivo fue preparado | | |
| El cambio fue registrado en un commit | | |
| Quién realizó un commit | | |
| Cuándo se registró un commit | | |
| Qué decía el archivo antes del commit | | |

Justificá cada respuesta.

---

## Desafío 18 — El recorrido completo

Explicá este esquema como si estuvieras enseñándoselo a un compañero:

```text
┌─────────────────────┐
│ Carpeta de trabajo  │
└──────────┬──────────┘
           │
           │ modificar
           ▼
┌─────────────────────┐
│ Cambio              │
└──────────┬──────────┘
           │
           │ preparar
           ▼
┌─────────────────────┐
│ Área de preparación │
└──────────┬──────────┘
           │
           │ registrar
           ▼
┌─────────────────────┐
│ Commit              │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Historial           │
└─────────────────────┘
```

Tu explicación debe responder:

- ¿qué ocurre en cada etapa?
- ¿por qué existen etapas intermedias?
- ¿qué información conserva Git?
- ¿qué diferencia existe entre trabajar y registrar?

---

## Desafío 19 — Resolver sin receta

Un compañero te entrega un repositorio y te dice:

> "No sé qué hice. Git me muestra cosas en rojo y verde."

No sabés exactamente qué comandos ejecutó.

### Tu desafío

No ejecutes comandos al azar.

Construí una estrategia de diagnóstico.

La estrategia debe comenzar por:

```text
¿Qué necesito saber?
```

y continuar con:

```text
¿Qué información puedo obtener?
```

hasta llegar a:

```text
¿Qué acción corresponde realizar?
```

El objetivo es desarrollar una forma de trabajar que pueda utilizarse también cuando los problemas sean más complejos.

---

## Desafío 20 — El primer repositorio profesional

Creá un repositorio llamado:

```text
mi-primer-repositorio
```

Debe contener:

```text
README.md
objetivos.md
notas.md
```

El `README.md` deberá explicar:

- qué es el proyecto;
- para qué fue creado;
- quién lo realiza.

Realizá al menos tres commits significativos.

Los mensajes deben permitir reconstruir la evolución del proyecto.

Al finalizar, el repositorio debe quedar limpio.

### Condición final

Sin mirar documentación, deberías poder explicar:

> ¿Qué diferencia existe entre el estado actual de los archivos y el historial del repositorio?

Si podés responderlo y demostrarlo con tu repositorio, estás listo para avanzar.