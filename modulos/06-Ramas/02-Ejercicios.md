# Ejercicios
## Módulo 06 — Ramas

Estos ejercicios buscan consolidar la comprensión de las ramas mediante situaciones concretas.

La prioridad no está en ejecutar comandos mecánicamente, sino en poder anticipar y explicar qué sucede con la historia del repositorio.

---

## Ejercicio 1 — Reconocer una rama

Observá:

```text
A ── B ── C
```

Respondé:

1. ¿Qué representa cada letra?
2. ¿Qué representa la secuencia completa?
3. ¿Dónde podría estar apuntando `main`?
4. ¿Qué información necesitarías para saber cuál es la rama actual?

---

## Ejercicio 2 — Crear una rama

Partiendo de:

```text
A ── B ── C
          ↑
        main
```

Indicá qué comando utilizarías para crear una rama llamada:

```text
feature-login
```

Después indicá qué comando utilizarías para cambiarte a ella.

---

## Ejercicio 3 — Crear y cambiar

¿Qué diferencia existe entre:

```bash
git branch feature
```

y:

```bash
git switch -c feature
```

Explicalo con tus palabras.

---

## Ejercicio 4 — Predecir la historia

Partimos de:

```text
A ── B ── C
          ↑
        main
```

Ejecutamos:

```bash
git switch -c feature
```

Dibujá cómo queda la historia.

---

## Ejercicio 5 — Primer commit en una rama

Partimos de:

```text
A ── B ── C
          ↑
        main
        feature
```

Realizamos un commit sobre `feature`.

Representá la historia resultante.

---

## Ejercicio 6 — ¿Dónde está el commit?

Observá:

```text
A ── B ── C
          \
           D
```

Suponiendo que:

```text
main → C
feature → D
```

Respondé:

1. ¿En qué rama existe `D`?
2. ¿`main` contiene `D`?
3. ¿`feature` contiene `C`?
4. ¿Qué rama avanzó?

---

## Ejercicio 7 — Cambiar de rama

Partimos de:

```text
A ── B ── C
          \
           D
```

Ejecutamos:

```bash
git switch main
```

Respondé:

1. ¿En qué commit queda posicionada la rama actual?
2. ¿Qué sucede con los archivos propios de `D`?
3. ¿El commit `D` desapareció?

---

## Ejercicio 8 — Verificar la rama actual

Indicá dos comandos que permitan comprobar en qué rama estamos trabajando.

Explicá qué información proporciona cada uno.

---

## Ejercicio 9 — Crear un archivo en una rama

Partimos de:

```text
A ── B ── C
          ↑
        main
```

Creamos:

```bash
git switch -c documentacion
```

Después creamos:

```text
documentacion.md
```

y realizamos:

```bash
git add documentacion.md
git commit -m "Agrega documentación"
```

Representá la historia.

---

## Ejercicio 10 — ¿Por qué el archivo desaparece?

Después del ejercicio anterior ejecutamos:

```bash
git switch main
```

El archivo `documentacion.md` ya no aparece.

Respondé:

> ¿Por qué?

Y, fundamentalmente:

> ¿Se perdió el archivo?

Explicá qué ocurre realmente.

---

## Ejercicio 11 — Dos líneas de trabajo

Partimos de:

```text
A ── B ── C
```

Creamos dos ramas:

```text
feature-a
feature-b
```

Sobre `feature-a` hacemos un commit `D`.

Sobre `feature-b` hacemos un commit `E`.

Dibujá la historia completa.

---

## Ejercicio 12 — Identificar ramas

Observá:

```text
A ── B ── C ── D
          \
           E ── F
```

Suponiendo que:

```text
main → D
feature → F
```

Respondé:

1. ¿Dónde se separaron las ramas?
2. ¿Qué commits son exclusivos de `feature`?
3. ¿Qué commits pertenecen a la historia compartida?
4. ¿Cuál es la rama más avanzada?
5. ¿Qué ocurriría si hacemos `git switch main`?

---

## Ejercicio 13 — `HEAD`

Observá:

```text
A ── B ── C
          \
           D
```

Si estamos trabajando en `feature` y:

```text
feature → D
```

¿Dónde se encuentra conceptualmente `HEAD`?

Representalo:

```text
HEAD
 ↓
 ?
 ↓
 ?
```

---

## Ejercicio 14 — Cambiar `HEAD`

Partimos de:

```text
A ── B ── C
          \
           D
```

Estamos en `feature`.

Ejecutamos:

```bash
git switch main
```

Representá ahora:

```text
HEAD
 ↓
 ?
 ↓
 ?
```

Explicá qué cambió y qué no cambió.

---

## Ejercicio 15 — Merge

Observá:

```text
A ── B ── C
          \
           D ── E
```

Queremos incorporar `feature` a `main`.

Respondé:

1. ¿En qué rama debemos ubicarnos?
2. ¿Qué comando debemos ejecutar?
3. ¿Qué rama estamos incorporando?
4. ¿Sobre qué rama se realiza la integración?

---

## Ejercicio 16 — Orden incorrecto

Un estudiante hace:

```bash
git switch feature
git merge main
```

pero quería incorporar `feature` a `main`.

### Preguntas

1. ¿Qué operación realizó realmente?
2. ¿Por qué no es equivalente a incorporar `feature` en `main`?
3. ¿Qué debería haber hecho?

---

## Ejercicio 17 — Merge conceptual

Observá:

```text
A ── B ── C
          \
           D ── E
```

Después de integrar `feature` en `main`, dibujá una posible historia resultante.

Podés representar:

```text
A ── B ── C ── D ── E
```

o una historia con merge:

```text
          D ── E
         /     \
A ── B ── C ─── M
```

Explicá qué representa cada caso.

---

## Ejercicio 18 — Eliminar una rama

Después de integrar:

```text
feature
```

en:

```text
main
```

ya no necesitamos la rama.

¿Qué comando utilizarías para eliminarla localmente?

Explicá por qué eliminar la rama no significa necesariamente eliminar los commits que fueron integrados.

---

## Ejercicio 19 — Rama para una corrección

Tenés un proyecto funcionando en `main`.

Detectás un error en:

```text
README.md
```

Querés corregirlo sin trabajar directamente sobre `main`.

Respondé:

1. ¿Qué nombre le darías a la rama?
2. ¿Cómo la crearías?
3. ¿Dónde realizarías el commit?
4. ¿Cómo incorporarías la corrección a `main`?

---

## Ejercicio 20 — Elegir nombres

Proponé nombres adecuados para ramas destinadas a:

### A

Agregar un sistema de búsqueda.

### B

Corregir un error de instalación.

### C

Actualizar la documentación.

### D

Experimentar con una nueva configuración.

Evitá nombres genéricos como:

```text
rama1
prueba
cosas
nueva
```

Justificá al menos dos de tus decisiones.

---

## Ejercicio 21 — Rama o `main`

Para cada situación indicá si trabajarías directamente sobre `main` o crearías una rama.

### A

Corregir una palabra en un README personal.

### B

Desarrollar una funcionalidad importante.

### C

Experimentar con una solución que podría descartarse.

### D

Realizar una modificación que otra persona deberá revisar.

No existe necesariamente una única respuesta correcta.

Justificá tus decisiones.

---

## Ejercicio 22 — Leer una historia

Observá:

```text
*  M
|\
| * E
| * D
|/
* C
* B
* A
```

Respondé:

1. ¿Cuántos commits aparecen?
2. ¿Dónde se produjo la separación?
3. ¿Qué commits pertenecen a la línea secundaria?
4. ¿Qué representa `M`?
5. ¿Qué operación pudo haber producido `M`?

---

## Ejercicio 23 — Construir la historia

Realizá en un repositorio real:

```text
1. Crear un commit inicial.
2. Crear una rama llamada feature.
3. Realizar un cambio.
4. Hacer commit.
5. Volver a main.
6. Realizar otro cambio.
7. Hacer commit.
8. Observar la divergencia.
```

Después ejecutá:

```bash
git log --oneline --graph --all
```

Compará el gráfico con tu representación previa.

---

## Ejercicio 24 — `git diff` entre ramas

Partiendo de dos ramas con cambios diferentes, ejecutá:

```bash
git diff main..feature
```

y después:

```bash
git diff feature..main
```

Respondé:

1. ¿Qué diferencias aparecen?
2. ¿Por qué los resultados pueden ser diferentes?
3. ¿Qué información aporta comparar dos ramas?

---

## Ejercicio 25 — Merge en un repositorio real

Creá:

```text
feature
```

Realizá uno o más commits.

Después:

```bash
git switch main
git merge feature
```

Consultá:

```bash
git log --oneline --graph --all
```

Explicá qué ocurrió.

---

## Ejercicio 26 — Conflicto

Creá dos ramas desde el mismo punto.

Modificá la misma línea de un archivo de manera diferente en cada rama.

Realizá commits en ambas.

Después intentá fusionarlas.

Si Git genera un conflicto:

```bash
git status
```

Identificá los archivos afectados.

---

## Ejercicio 27 — Resolver un conflicto

Sobre el archivo conflictivo identificá:

```text
<<<<<<< HEAD
versión actual
=======
otra versión
>>>>>>> nombre-rama
```

Decidí qué contenido debe quedar.

Eliminá las marcas de conflicto.

Después:

```bash
git add archivo
git commit
```

Consultá:

```bash
git status
```

Finalmente:

```bash
git log --oneline --graph --all
```

Explicá cómo quedó la historia.

---

## Ejercicio 28 — ¿Quién decide?

Ante un conflicto, Git no puede decidir automáticamente entre:

```text
versión A
```

y:

```text
versión B
```

Respondé:

> ¿Por qué la resolución del conflicto requiere una decisión humana?

> ¿Qué información deberías analizar antes de elegir qué contenido conservar?

---

## Ejercicio 29 — Publicar una rama

Creá:

```bash
git switch -c feature-github
```

Realizá un cambio y commit.

Publicá:

```bash
git push -u origin feature-github
```

Después ingresá a GitHub y verificá que la rama exista.

---

## Ejercicio 30 — Local vs. remoto

Respondé:

> ¿Qué diferencia existe entre:

```text
feature-github
```

y:

```text
origin/feature-github
```

No hace falta describir internamente todos los mecanismos de Git.

Explicá conceptualmente la diferencia entre una referencia local y una referencia asociada al repositorio remoto.

---

## Ejercicio 31 — El error del push

Un estudiante ejecuta:

```bash
git switch -c feature
```

y después trabaja durante varias horas.

Finalmente pregunta:

> "¿Por qué no veo mi rama en GitHub?"

¿Qué le responderías?

---

## Ejercicio 32 — Flujo completo

Realizá el siguiente flujo:

```text
main
 ↓
crear feature
 ↓
trabajar
 ↓
commit
 ↓
publicar
 ↓
GitHub
 ↓
volver a main
 ↓
merge
 ↓
eliminar rama local
```

Registrá los comandos utilizados.

---

## Ejercicio 33 — Interpretar una situación

Un proyecto tiene:

```text
main
feature-login
fix-readme
```

`feature-login` tiene tres commits propios.

`fix-readme` tiene un commit propio.

Ninguna de las dos ramas fue integrada.

Respondé:

1. ¿Cuántas líneas de trabajo existen?
2. ¿Qué tienen en común las ramas?
3. ¿Qué podría ocurrir si ambas modificaron el mismo archivo?
4. ¿Qué operación permitiría integrar cada una?

---

## Ejercicio 34 — Diseñar un flujo

Imaginá que vas a desarrollar una nueva funcionalidad.

Diseñá un flujo utilizando:

```text
main
feature
commit
merge
```

Representalo gráficamente.

Después escribí los comandos que utilizarías.

---

## Ejercicio 35 — Detectar un error conceptual

Un compañero afirma:

> "Cuando creo una rama, Git crea otra copia independiente del repositorio."

¿Estás de acuerdo?

Explicá qué modelo conceptual utilizarías en su lugar.

---

## Ejercicio 36 — Detectar otro error conceptual

Otro compañero afirma:

> "Si borro una rama, borro todos los commits que hice en ella."

¿Es necesariamente cierto?

Explicá qué diferencia existe entre una rama y los commits.

---

## Ejercicio 37 — ¿Qué rama estoy modificando?

Imaginá que ejecutás:

```bash
git switch feature
```

y después modificás:

```text
README.md
```

Antes de hacer el commit:

```bash
git status
```

¿Qué información deberías comprobar?

¿Por qué es importante?

---

## Ejercicio 38 — Recuperar una rama

Suponé que tenés:

```text
main
feature
```

y olvidaste en qué rama realizaste un cambio.

Utilizá:

```bash
git branch
```

y:

```bash
git log --oneline --all
```

para investigar.

Explicá cómo determinarías dónde quedó registrado el cambio.

---

## Ejercicio 39 — Graficar una historia

Construí una historia que tenga:

- cinco commits comunes;
- una rama secundaria;
- dos commits en esa rama;
- un commit adicional en `main`;
- un merge.

Representala gráficamente.

Después describí la historia en palabras.

---

## Ejercicio 40 — Comparar dos historias

### Historia A

```text
A ── B ── C ── D
```

### Historia B

```text
A ── B ── C
          \
           D ── E
```

Respondé:

1. ¿Cuál representa una única línea de evolución?
2. ¿Cuál representa líneas divergentes?
3. ¿Qué ventaja ofrece la segunda?
4. ¿Qué operación podría volver a integrar las líneas?

---

## Ejercicio 41 — Rama experimental

Creá una rama:

```text
experimento
```

sobre la cual realices una modificación que deliberadamente pueda descartarse.

Después:

1. realizá varios commits;
2. volvé a `main`;
3. compará;
4. decidí no integrar la rama;
5. eliminá la rama.

Reflexioná:

> ¿Qué ventaja tuvo utilizar una rama para experimentar?

---

## Ejercicio 42 — Rama de documentación

Creá:

```text
docs-readme
```

Realizá mejoras en:

```text
README.md
```

Registrá los cambios.

Después integrá la rama en `main`.

Analizá si separar la documentación en una rama facilitó el trabajo.

---

## Ejercicio 43 — Rama de funcionalidad

Creá:

```text
feature-ejemplo
```

Desarrollá una pequeña funcionalidad del proyecto.

Utilizá varios commits pequeños.

Después consultá:

```bash
git log --oneline --graph --all
```

Observá cómo la rama representa el proceso de desarrollo.

---

## Ejercicio 44 — Revisar antes de integrar

Antes de hacer:

```bash
git merge feature
```

consultá:

```bash
git status
git log --oneline
git diff main..feature
```

Respondé:

> ¿Qué información aporta cada comando antes de realizar la integración?

---

## Ejercicio 45 — Ejercicio integrador

Construí un repositorio que tenga esta evolución:

```text
A ── B ── C
          \
           D ── E
```

Después:

1. creá la rama;
2. realizá dos commits;
3. volvé a `main`;
4. realizá un cambio adicional;
5. observá la divergencia;
6. compará las ramas;
7. integrá la rama;
8. observá el resultado;
9. eliminá la rama;
10. verificá la historia final.

Utilizá:

```bash
git log --oneline --graph --all
```

para analizar el resultado.

---

## Comprobación final

Sin consultar documentación, intentá responder:

### 1.

¿Cómo se crea una rama?

### 2.

¿Cómo se crea y cambia a una rama en una sola operación?

### 3.

¿Cómo se cambia de rama?

### 4.

¿Cómo se consulta la rama actual?

### 5.

¿Cómo se realiza un commit sobre una rama?

### 6.

¿Cómo se integra una rama?

### 7.

¿Por qué importa la rama actual al hacer un merge?

### 8.

¿Cómo se elimina una rama local?

### 9.

¿Cómo se publica una rama en GitHub?

### 10.

¿Qué diferencia existe entre una rama y un commit?

### 11.

¿Qué diferencia existe entre una rama local y una rama remota?

### 12.

¿Por qué pueden aparecer conflictos?

### 13.

¿Qué significa resolver un conflicto?

### 14.

¿Cómo podés visualizar gráficamente una historia con ramas?

---

## Criterio de resolución

No alcanza con ejecutar correctamente los comandos.

En cada ejercicio se busca desarrollar la capacidad de:

```text
observar
   ↓
predecir
   ↓
ejecutar
   ↓
verificar
   ↓
explicar
```

Si podés anticipar cómo debería quedar la historia antes de ejecutar los comandos y después comprobar que Git produjo ese resultado, estás construyendo el modelo mental correcto.

> **Una rama se aprende realmente cuando podés mirar una historia de commits y entender qué pasó.**