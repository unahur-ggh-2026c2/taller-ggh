# Desafíos
## Módulo 04 — GitHub

Estos desafíos buscan que puedas trabajar con GitHub comprendiendo la relación entre el repositorio local y el remoto, y que puedas diagnosticar situaciones sin depender de una secuencia memorizada de comandos.

La consigna general es:

> **Antes de ejecutar un comando, determiná dónde está el cambio y dónde debería estar.**

---

## Desafío 1 — ¿Dónde está el cambio?

Partí de un repositorio conectado con GitHub.

Realizá una modificación en `README.md`, pero no ejecutes ningún otro comando.

Respondé:

```text
¿Dónde existe el cambio?
```

Después ejecutá:

```bash
git status
```

Volvé a responder.

Ahora prepará el cambio:

```bash
git add README.md
```

Volvé a consultar:

```bash
git status
```

Continuá con:

```bash
git commit -m "..."
```

y:

```bash
git push
```

Después de cada etapa explicá dónde se encuentra el cambio.

---

## Desafío 2 — El commit que no aparece

Un compañero afirma:

> "Hice el commit, pero no aparece en GitHub."

No podés tocar su repositorio todavía.

### Tu desafío

Construí una estrategia de diagnóstico.

¿Qué preguntas harías?

¿Qué comandos utilizarías?

Una estrategia razonable debería permitir distinguir entre:

```text
cambio sin registrar
        ↓
commit local
        ↓
commit publicado
```

No ejecutes comandos al azar.

Primero formulá la hipótesis.

---

## Desafío 3 — El cambio que aparece en GitHub

Un compañero afirma:

> "En GitHub aparece un cambio que yo no tengo en mi computadora."

### Tu desafío

Explicá:

1. ¿Qué situación podría estar ocurriendo?
2. ¿Qué comando utilizarías para consultar el historial local?
3. ¿Qué operación podría permitir incorporar el cambio remoto?
4. ¿Qué verificarías después?

---

## Desafío 4 — Local adelantado

Imaginá:

```text
LOCAL

A
↓
B
↓
C
```

```text
GITHUB

A
↓
B
```

### Tu desafío

Sin ejecutar nada, respondé:

1. ¿Qué repositorio contiene un commit que el otro todavía no tiene?
2. ¿Cuál?
3. ¿Qué operación debería analizarse?
4. ¿Qué resultado esperarías?

Después construí esta situación realmente en un repositorio de práctica y resolvela.

---

## Desafío 5 — Remoto adelantado

Ahora:

```text
LOCAL

A
↓
B
```

```text
GITHUB

A
↓
B
↓
C
```

Respondé:

1. ¿Dónde existe el commit `C`?
2. ¿Dónde no existe?
3. ¿Qué operación podría ser necesaria?
4. ¿Qué deberías comprobar después?

Construí también esta situación de manera práctica.

---

## Desafío 6 — El remoto desconocido

Recibís un repositorio Git que otra persona configuró.

No sabés:

- si está conectado con GitHub;
- cuál es el remoto;
- qué nombre tiene;
- qué URL utiliza.

### Tu desafío

Sin modificar nada, investigá la configuración.

Deberás determinar:

```text
¿Existe un remoto?
¿Qué nombre tiene?
¿A qué URL apunta?
```

Después explicá cómo obtuviste cada dato.

---

## Desafío 7 — ¿Qué significa `origin`?

Un estudiante ejecuta:

```bash
git remote -v
```

y obtiene:

```text
origin  https://github.com/usuario/proyecto.git (fetch)
origin  https://github.com/usuario/proyecto.git (push)
```

El estudiante afirma:

> "`origin` es GitHub."

### Tu desafío

Explicá por qué la afirmación es imprecisa.

Después respondé:

> ¿Podría existir un remoto llamado `universidad`?

> ¿Podría existir más de un remoto?

No es necesario implementarlo todavía.

---

## Desafío 8 — Publicar conscientemente

Creá un repositorio local con varios commits.

Conectalo con GitHub.

Ahora realizá tres modificaciones independientes.

Registrá cada una mediante un commit.

No hagas `push` todavía.

### Tu desafío

Observá:

```bash
git log --oneline
```

y después publicá los cambios.

Finalmente comprobá que los tres commits estén disponibles en GitHub.

Explicá qué diferencia temporal existió entre:

```text
commit local
```

y:

```text
commit publicado
```

---

## Desafío 9 — El cambio fantasma

Un estudiante dice:

> "GitHub debería mostrar mi cambio porque guardé el archivo."

### Tu desafío

Explicale por qué guardar un archivo no implica necesariamente:

```text
commit
```

y mucho menos:

```text
push
```

Construí una demostración práctica que permita mostrar las cuatro situaciones:

```text
archivo modificado
commit local
commit publicado
```

---

## Desafío 10 — El `push` que falta

Construí esta situación:

```text
LOCAL

A
↓
B
↓
C
```

```text
GITHUB

A
↓
B
```

No ejecutes `git push` todavía.

### Tu desafío

Respondé:

> ¿Qué información te permite afirmar que el repositorio local tiene algo que todavía no está publicado?

Después resolvé la situación.

---

## Desafío 11 — El `pull` que falta

Construí:

```text
LOCAL

A
↓
B
```

y:

```text
GITHUB

A
↓
B
↓
C
```

### Tu desafío

Antes de resolverlo, explicá:

> ¿Por qué `git push` no sería la operación adecuada para esta situación?

Después incorporá el cambio y verificá el resultado.

---

## Desafío 12 — Dos repositorios, una historia

Creá un repositorio local con al menos cinco commits.

Publicalo en GitHub.

Después:

1. realizá un nuevo commit local;
2. no lo publiques;
3. realizá un cambio desde GitHub;
4. registralo en GitHub.

Ahora los repositorios tienen historias diferentes.

Representá la situación:

```text
LOCAL

...

GITHUB

...
```

### Pregunta

> ¿Qué cambió respecto de los desafíos anteriores?

No intentes resolverlo todavía.

El objetivo es reconocer que la situación es más compleja.

---

## Desafío 13 — Diagnóstico antes de actuar

Un repositorio presenta una situación desconocida.

El usuario solamente dice:

> "No está sincronizado."

No sabemos qué significa exactamente esa frase.

### Tu desafío

Definí qué información necesitás antes de decidir qué hacer.

Podés considerar:

```bash
git status
git log --oneline
git remote -v
```

Explicá qué pregunta responde cada uno.

---

## Desafío 14 — GitHub como fuente de información

Elegí un repositorio público en GitHub.

Sin modificarlo, investigá:

- nombre;
- README;
- archivos;
- historial;
- commits;
- evolución.

Después respondé:

> ¿Qué información de un repositorio Git puede visualizarse directamente desde GitHub?

Y:

> ¿Qué utilidad tiene que esa información esté disponible públicamente?

---

## Desafío 15 — Publicar un proyecto

Partí de uno de tus proyectos anteriores.

El repositorio debe:

- tener varios commits;
- contar con un README;
- estar limpio;
- tener una historia comprensible.

Publicalo en GitHub.

Después revisá el repositorio como si fueras una persona externa que acaba de encontrarlo.

Evaluá:

- ¿se entiende qué es?
- ¿se entiende para qué sirve?
- ¿se puede consultar su historial?
- ¿los mensajes son claros?
- ¿la documentación inicial es suficiente?

Registrá las conclusiones.

---

## Desafío 16 — Local y remoto como dos puntos de referencia

Construí deliberadamente una situación en la que:

```text
LOCAL ≠ GITHUB
```

No importa inicialmente cuál está adelantado.

Tu tarea es:

1. identificar la diferencia;
2. determinar dónde está el cambio;
3. explicar qué debería ocurrir;
4. elegir la operación adecuada;
5. verificar el resultado.

No se evalúa solamente que "funcione".

Se evalúa el razonamiento previo.

---

## Desafío 17 — El diagnóstico incorrecto

Un estudiante encuentra:

```text
LOCAL

A
↓
B
↓
C
```

```text
GITHUB

A
↓
B
```

y ejecuta inmediatamente:

```bash
git pull
```

### Tu desafío

Analizá la decisión.

¿Es necesariamente la operación que corresponde?

¿Qué debería haber determinado primero?

Explicá por qué.

---

## Desafío 18 — Explicar `push`

Explicale a una persona que nunca utilizó Git:

> ¿Qué ocurre cuando ejecutás `git push`?

No podés responder solamente:

> "Sube los archivos."

Tu explicación debe incluir:

- repositorio local;
- commits;
- repositorio remoto;
- GitHub;
- publicación de cambios.

---

## Desafío 19 — Explicar `pull`

Ahora explicá:

> ¿Qué ocurre cuando ejecutás `git pull`?

Tu explicación debe diferenciar claramente:

```text
obtener cambios remotos
```

de:

```text
crear un cambio nuevo localmente
```

No es necesario entrar todavía en profundidad sobre conflictos.

---

## Desafío 20 — El repositorio compartido

Imaginá que dos personas trabajan sobre el mismo repositorio.

```text
Persona A ──→ GitHub
Persona B ──→ GitHub
```

La persona A publica un commit.

La persona B todavía no lo tiene localmente.

### Tu desafío

Explicá qué debería hacer B para incorporar ese cambio.

Después preguntate:

> ¿Qué podría ocurrir si B también realizó cambios localmente?

No es necesario resolver el conflicto.

El objetivo es anticipar que la colaboración agrega complejidad.

---

## Desafío 21 — Construir una demostración

Prepará una demostración para una persona que nunca utilizó GitHub.

En no más de diez minutos deberías poder mostrar:

```text
1. Repositorio local
2. Commit
3. Repositorio remoto
4. Push
5. Cambio visible en GitHub
6. Cambio remoto
7. Pull
8. Cambio visible localmente
```

No expliques solamente los comandos.

Explicá qué está ocurriendo entre los dos repositorios.

---

## Desafío 22 — GitHub no es una carpeta compartida

Analizá la afirmación:

> "GitHub es como una carpeta de red donde todos guardamos los archivos."

Explicá qué tiene de útil la comparación y en qué aspectos resulta incorrecta.

Tu respuesta debería incluir:

- repositorio;
- historial;
- commits;
- remoto;
- publicación;
- colaboración.

---

## Desafío 23 — El flujo completo

Construí un proyecto documental pequeño.

Realizá:

```text
Repositorio local
      ↓
Primer commit
      ↓
GitHub
      ↓
Push
      ↓
Segundo commit local
      ↓
Push
      ↓
Cambio desde GitHub
      ↓
Pull
      ↓
Nuevo commit local
      ↓
Push
```

Documentá qué ocurrió en cada etapa.

---

## Desafío 24 — Autonomía

Recibís un repositorio local que ya está conectado con GitHub.

No recibís instrucciones adicionales.

La única consigna es:

> "Realizá una modificación, registrala y asegurate de que quede publicada en GitHub."

Decidí por tu cuenta:

- qué consultar;
- qué comandos utilizar;
- cómo verificar;
- cómo comprobar el resultado remoto.

Al finalizar explicá el razonamiento seguido.

---

## Desafío 25 — Resolver un problema realista

Un compañero te dice:

> "Ayer hice un commit. Hoy abrí GitHub y no aparece. Después modifiqué el archivo otra vez y tampoco aparece."

### Tu desafío

No le des inmediatamente una solución.

Primero formulá preguntas.

Intentá determinar si el problema está en:

```text
archivo
   ↓
preparación
   ↓
commit
   ↓
remoto
   ↓
push
```

Después diseñá una secuencia de diagnóstico.

---

## Desafío 26 — La pregunta clave

Ante cualquier problema de sincronización, empezá por esta pregunta:

> **¿Dónde existe actualmente el cambio?**

Construí tres situaciones diferentes:

### Situación A

El cambio existe solamente en el archivo local.

### Situación B

El cambio existe en el historial local.

### Situación C

El cambio existe en el repositorio remoto.

Para cada una indicá qué información te permitiría reconocerla.

---

## Desafío 27 — Publicación selectiva

Creá varios commits locales.

Después publicá solamente los commits correspondientes a una etapa del proyecto.

Observá qué ocurre con el repositorio remoto.

Analizá:

> ¿Qué significa que el repositorio local tenga una historia más avanzada que el remoto?

---

## Desafío 28 — Evaluar un repositorio

Elegí uno de tus repositorios publicados.

Evaluá:

| Criterio | 1–5 |
|---|:---:|
| README comprensible | |
| Historial claro | |
| Mensajes descriptivos | |
| Organización | |
| Identificación del proyecto | |
| Estado del repositorio | |

Después escribí tres mejoras concretas.

---

## Desafío 29 — Enseñarlo

Prepará una explicación de cinco minutos para responder:

> "¿Cómo paso de tener un proyecto Git en mi computadora a tenerlo publicado en GitHub?"

Tu explicación debería incluir:

```text
Repositorio local
       ↓
Repositorio remoto
       ↓
origin
       ↓
push
       ↓
GitHub
```

Después agregá:

> "¿Y cómo traigo cambios de GitHub a mi computadora?"

---

## Desafío final — La sincronización consciente

Construí un repositorio completo desde cero.

Debe:

- contener documentación;
- tener varios commits;
- estar publicado en GitHub;
- tener un historial comprensible.

Después realizá al menos dos ciclos completos:

### Ciclo local → remoto

```text
Modificar
   ↓
Preparar
   ↓
Commit
   ↓
Push
   ↓
Verificar GitHub
```

### Ciclo remoto → local

```text
Modificar desde GitHub
   ↓
Commit remoto
   ↓
Pull
   ↓
Verificar localmente
```

Finalmente escribí una explicación:

```md
# Análisis del proyecto

## ¿Qué diferencia existe entre Git y GitHub?

...

## ¿Qué diferencia existe entre local y remoto?

...

## ¿Qué hace commit?

...

## ¿Qué hace push?

...

## ¿Qué hace pull?

...

## ¿Qué representa origin?

...

## ¿Cómo diagnostico que local y remoto están desincronizados?

...

## ¿Qué aprendí sobre publicar cambios?

...
```

---

## Criterio de superación

El desafío se considera logrado cuando podés enfrentar una situación de sincronización siguiendo este razonamiento:

```text
¿Qué cambió?
      ↓
¿Dónde está el cambio?
      ↓
¿Está registrado?
      ↓
¿Está publicado?
      ↓
¿Dónde debería estar?
      ↓
¿Qué operación corresponde?
      ↓
¿Cómo verifico el resultado?
```

> **La meta no es saber ejecutar `push` y `pull`. La meta es entender cuándo, por qué y hacia dónde debe viajar un cambio.**