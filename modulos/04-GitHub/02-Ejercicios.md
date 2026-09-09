# Ejercicios
## Módulo 04 — GitHub

Estos ejercicios buscan consolidar la relación entre Git, el repositorio local, el repositorio remoto y GitHub.

La pregunta guía es:

> **¿Dónde está mi cambio y cómo sé si ya fue publicado?**

---

## Ejercicio 1 — Git y GitHub

Explicá con tus propias palabras:

1. ¿Qué es Git?
2. ¿Qué es GitHub?
3. ¿Qué relación existe entre ambos?
4. ¿Se puede utilizar Git sin GitHub?
5. ¿Qué aporta GitHub a un repositorio Git?

---

## Ejercicio 2 — Local y remoto

Completá:

```text
Repositorio local
        ↓
        ?
        ↓
Repositorio remoto
        ↓
        ?
```

Indicá qué herramientas u operaciones intervienen en cada sentido.

Después explicá el recorrido completo.

---

## Ejercicio 3 — ¿Dónde está el cambio?

Para cada situación indicá dónde existe el cambio:

### A

Modificaste `README.md`, pero todavía no hiciste `git add`.

```text
[ ] Área de trabajo
[ ] Área de preparación
[ ] Historial local
[ ] GitHub
```

### B

Ejecutaste:

```bash
git add README.md
```

pero todavía no hiciste commit.

```text
[ ] Área de trabajo
[ ] Área de preparación
[ ] Historial local
[ ] GitHub
```

### C

Hiciste:

```bash
git commit
```

pero todavía no hiciste `git push`.

```text
[ ] Área de trabajo
[ ] Área de preparación
[ ] Historial local
[ ] GitHub
```

### D

Hiciste:

```bash
git push
```

```text
[ ] Área de trabajo
[ ] Área de preparación
[ ] Historial local
[ ] GitHub
```

Justificá cada respuesta.

---

## Ejercicio 4 — `commit` y `push`

Explicá la diferencia entre:

```bash
git commit
```

y:

```bash
git push
```

Después completá:

> `git commit` sirve para...

> `git push` sirve para...

---

## Ejercicio 5 — El cambio que no aparece

Un estudiante dice:

> "Hice un cambio en README.md pero no aparece en GitHub."

Proponé una secuencia de preguntas para diagnosticar el problema.

Como mínimo deberías considerar:

```text
¿El archivo fue modificado?
¿Se hizo commit?
¿Se hizo push?
```

Explicá por qué cada pregunta es relevante.

---

## Ejercicio 6 — Observar el remoto

En un repositorio conectado con GitHub ejecutá:

```bash
git remote -v
```

Respondé:

1. ¿Qué nombre tiene el remoto?
2. ¿Qué URL tiene?
3. ¿Para qué sirve esta información?
4. ¿Qué significa `origin`?

---

## Ejercicio 7 — El significado de `origin`

Analizá esta configuración:

```text
origin → https://github.com/usuario/proyecto.git
```

Respondé:

1. ¿Qué representa `origin`?
2. ¿Qué representa la URL?
3. ¿Qué ocurriría si el remoto tuviera otro nombre?
4. ¿Cambiaría GitHub?

---

## Ejercicio 8 — Publicar un commit

Partí de un repositorio que ya esté conectado con GitHub.

Realizá:

1. una modificación;
2. `git status`;
3. `git add`;
4. `git commit`;
5. `git log --oneline`;
6. `git push`.

Después comprobá el resultado en GitHub.

Registrá qué observaste en cada etapa.

---

## Ejercicio 9 — Antes del `push`

Realizá una modificación y registrala:

```bash
git add .
git commit -m "..."
```

Antes de ejecutar:

```bash
git push
```

respondé:

> ¿Qué diferencia debería existir entre el repositorio local y el remoto?

Después ejecutá el `push` y comprobalo.

---

## Ejercicio 10 — El `push` no crea el commit

Analizá esta afirmación:

> "Cuando hago `git push`, Git crea el commit."

¿Es correcta?

Explicá qué ocurre realmente en:

```text
git commit
    ↓
historial local
    ↓
git push
    ↓
historial remoto
```

---

## Ejercicio 11 — Obtener cambios

Realizá una modificación directamente desde GitHub y registrá el cambio mediante la interfaz web.

Después, desde tu computadora, ejecutá:

```bash
git log --oneline
```

¿Aparece el nuevo commit?

Luego ejecutá:

```bash
git pull
```

Volvé a consultar:

```bash
git log --oneline
```

Explicá qué cambió.

---

## Ejercicio 12 — El flujo inverso

Completá:

```text
GitHub
   ↓
   ?
   ↓
Repositorio local
```

¿Qué operación utilizarías?

Después explicá qué diferencia existe entre ese recorrido y:

```text
Repositorio local
   ↓
   ?
   ↓
GitHub
```

---

## Ejercicio 13 — Diagnóstico de situaciones

Indicá qué operación podría ser necesaria en cada caso.

### Situación A

> Tengo un commit local que todavía no aparece en GitHub.

### Situación B

> Otra persona modificó el repositorio en GitHub y necesito incorporar ese cambio localmente.

### Situación C

> Modifiqué un archivo pero todavía no lo registré.

### Situación D

> Registré un commit localmente y quiero publicarlo.

No respondas solamente con comandos. Explicá el razonamiento.

---

## Ejercicio 14 — Secuencia correcta

Ordená estas operaciones:

```text
git push
git add
modificar archivo
git commit
git status
```

Construí una secuencia posible para publicar correctamente una modificación.

Después explicá por qué ese orden tiene sentido.

---

## Ejercicio 15 — ¿Qué está pasando?

Observá:

```text
README.md modificado
```

Todavía no hiciste nada más.

Completá:

```text
Área de trabajo: ______
Área de preparación: ______
Historial local: ______
GitHub: ______
```

Ahora ejecutá:

```bash
git add README.md
```

Volvé a completar.

Después ejecutá:

```bash
git commit -m "Actualiza README"
```

Volvé a completar.

Finalmente:

```bash
git push
```

Volvé a completar.

El objetivo es observar cómo se desplaza el cambio.

---

## Ejercicio 16 — Local adelantado

Imaginá:

```text
LOCAL

A
↓
B
↓
C
```

y:

```text
GITHUB

A
↓
B
```

Respondé:

1. ¿Cuál está adelantado?
2. ¿Qué operación podría utilizarse?
3. ¿Qué resultado esperarías después?

---

## Ejercicio 17 — Remoto adelantado

Ahora:

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

Respondé:

1. ¿Cuál está adelantado?
2. ¿Qué operación podría ser necesaria?
3. ¿Qué debería ocurrir después?

---

## Ejercicio 18 — Ambos repositorios

Imaginá:

```text
LOCAL

A
↓
B
↓
C
```

y:

```text
GITHUB

A
↓
B
↓
D
```

Respondé:

1. ¿Qué diferencia existe entre ambos?
2. ¿Se puede resolver simplemente pensando "subo C"?
3. ¿Qué concepto adicional aparece en esta situación?

No es necesario resolver todavía el problema de integración.

El objetivo es reconocer que el escenario es diferente de los anteriores.

---

## Ejercicio 19 — Verificar antes de actuar

Un compañero te dice:

> "GitHub no está actualizado."

Antes de ejecutar ningún comando, escribí una estrategia de diagnóstico.

Podés comenzar por:

```bash
git status
```

y:

```bash
git log --oneline
```

También podés consultar:

```bash
git remote -v
```

Explicá qué información buscarías en cada caso.

---

## Ejercicio 20 — La URL del remoto

Ejecutá:

```bash
git remote -v
```

Copiá la información obtenida.

Después respondé:

1. ¿A qué repositorio apunta?
2. ¿Es local o remoto?
3. ¿Cómo sabés que está relacionado con GitHub?
4. ¿Qué ocurriría si esa URL fuera incorrecta?

---

## Ejercicio 21 — Publicación consciente

Creá una pequeña modificación en un proyecto.

Antes de publicar:

```bash
git status
```

Después:

```bash
git log --oneline
```

Verificá que el cambio haya sido registrado.

Recién entonces:

```bash
git push
```

Finalmente comprobá GitHub.

Escribí una breve explicación del recorrido.

---

## Ejercicio 22 — Obtener conscientemente

Pedile a un compañero que modifique un archivo directamente desde GitHub.

Antes de hacer nada, observá:

```bash
git log --oneline
```

Después:

```bash
git pull
```

Volvé a consultar el historial.

Explicá qué información nueva apareció.

---

## Ejercicio 23 — GitHub como repositorio remoto

Visitá tu repositorio en GitHub.

Identificá:

- nombre del repositorio;
- README;
- archivos;
- historial;
- commits;
- información del proyecto.

Después compará con el repositorio local.

Respondé:

> ¿Qué información podemos observar desde GitHub que también forma parte del repositorio Git?

---

## Ejercicio 24 — La historia compartida

Realizá tres commits localmente.

Publicá solamente los dos primeros.

Representá la situación:

```text
LOCAL

...

GITHUB

...
```

Después publicá el tercero.

Volvé a representar la situación.

Explicá qué significa que el repositorio local tenga commits que todavía no están en el remoto.

---

## Ejercicio 25 — Integración

Partí de un repositorio conectado con GitHub.

Realizá el siguiente recorrido:

```text
1. Modificar localmente
2. Consultar estado
3. Preparar
4. Commit
5. Consultar historial
6. Push
7. Verificar GitHub
8. Modificar desde GitHub
9. Pull
10. Consultar historial
```

En cada etapa anotá qué repositorio contiene el cambio.

---

## Ejercicio 26 — Explicar sin comandos

Explicale a una persona que nunca utilizó Git qué significa:

> "Tengo un commit local que todavía no está publicado."

Después explicá:

> "Hay un commit en GitHub que todavía no tengo localmente."

No utilices inicialmente comandos.

Primero explicá el concepto.

Después indicá qué operación utilizarías en cada situación.

---

## Ejercicio 27 — Corregir afirmaciones

Indicá si las siguientes afirmaciones son correctas o incorrectas y justificá.

### A

> GitHub reemplaza a Git.

### B

> Un commit se publica automáticamente en GitHub.

### C

> `git push` envía cambios del repositorio local al remoto.

### D

> `git pull` permite incorporar cambios disponibles en el remoto.

### E

> `origin` es otro nombre para GitHub.

### F

> Un repositorio local puede estar conectado con un repositorio remoto.

---

## Ejercicio 28 — Construir el mapa conceptual

Completá:

```text
Git
 │
 ├── Repositorio local
 │       │
 │       ├── cambios
 │       ├── preparación
 │       └── commits
 │
 └── Repositorio remoto
         │
         └── GitHub
```

Agregá dónde ubicarías:

```text
git add
git commit
git push
git pull
```

Después explicá el esquema.

---

## Ejercicio 29 — Investigar un repositorio

Elegí un repositorio público de GitHub.

Observá:

- README;
- archivos;
- historial;
- commits;
- evolución.

Respondé:

1. ¿Qué información presenta el proyecto?
2. ¿Cómo se puede acceder a su historial?
3. ¿Qué información de Git está disponible desde GitHub?
4. ¿Qué utilidad tiene publicar un repositorio?

No es necesario analizar el código.

---

## Ejercicio 30 — Integración conceptual

Explicá el siguiente recorrido:

```text
Archivo
   ↓
git add
   ↓
git commit
   ↓
Historial local
   ↓
git push
   ↓
Repositorio remoto
   ↓
GitHub
```

Después explicá el recorrido inverso:

```text
GitHub
   ↓
Repositorio remoto
   ↓
git pull
   ↓
Repositorio local
```

Finalmente respondé:

> ¿Qué parte del proceso ocurre localmente y qué parte implica comunicación con el repositorio remoto?

---

## Comprobación final

Sin consultar documentación, respondé:

### 1.

¿Qué diferencia existe entre Git y GitHub?

### 2.

¿Qué diferencia existe entre repositorio local y remoto?

### 3.

¿Qué hace `git commit`?

### 4.

¿Qué hace `git push`?

### 5.

¿Qué hace `git pull`?

### 6.

¿Qué representa `origin`?

### 7.

Si un cambio está en tu computadora pero no aparece en GitHub, ¿qué deberías investigar?

### 8.

Si un cambio aparece en GitHub pero no en tu computadora, ¿qué deberías investigar?

### 9.

¿Por qué no debemos confundir "registrar un cambio" con "publicar un cambio"?

---

> **El objetivo no es memorizar tres comandos nuevos. Es poder determinar dónde está un cambio y qué operación corresponde para llevarlo al lugar que necesitamos.**