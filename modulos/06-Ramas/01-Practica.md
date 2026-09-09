# Práctica
## Módulo 06 — Ramas

---

## 1. Objetivo

En esta práctica vamos a trabajar con ramas de Git de manera progresiva.

El objetivo principal es comprender qué sucede con la historia del repositorio cuando dejamos de trabajar sobre una única línea de evolución.

Vamos a pasar de:

```text
A ── B ── C
```

a situaciones como:

```text
          D ── E
         /
A ── B ── C
```

y posteriormente aprenderemos a integrar esas líneas de trabajo.

La idea central es:

> **Una rama permite desarrollar una línea de trabajo independiente sin modificar inmediatamente otra línea de evolución del proyecto.**

---

## 2. Preparar el entorno

Para esta práctica necesitás:

- Git;
- Visual Studio Code;
- una terminal;
- un repositorio Git.

Podés utilizar el repositorio que venís trabajando durante el curso.

Antes de comenzar, verificá que el repositorio esté limpio:

```bash
git status
```

Idealmente deberías obtener algo similar a:

```text
nothing to commit, working tree clean
```

Si tenés cambios pendientes, resolvelos antes de continuar.

---

## 3. Consultar la rama actual

Ejecutá:

```bash
git branch
```

Podrías obtener:

```text
* main
```

El símbolo:

```text
*
```

indica la rama actual.

También podés utilizar:

```bash
git status
```

Git indicará en qué rama estás trabajando.

---

## 4. Observar la historia

Consultá:

```bash
git log --oneline
```

Podrías tener:

```text
c3d45ab Agrega documentación
a8f21cd Agrega ejercicios
91b72ef Crea estructura del proyecto
```

Tu historia será diferente.

Lo importante es que exista una línea de commits:

```text
A ── B ── C
```

---

## 5. Crear una rama

Vamos a crear una rama para realizar una modificación independiente.

Ejecutá:

```bash
git branch prueba-ramas
```

Ahora consultá:

```bash
git branch
```

Deberías observar algo parecido a:

```text
* main
  prueba-ramas
```

Todavía estamos en `main`.

Esto es importante:

> Crear una rama no significa cambiarse automáticamente a ella.

---

## 6. Cambiar de rama

Ahora ejecutá:

```bash
git switch prueba-ramas
```

Consultá:

```bash
git branch
```

Deberías obtener:

```text
  main
* prueba-ramas
```

También podés verificar:

```bash
git status
```

La rama actual debería ser:

```text
prueba-ramas
```

---

## 7. Crear y cambiar en una sola operación

Existe una forma más práctica de crear una rama y cambiarse inmediatamente a ella:

```bash
git switch -c experimento
```

Esta operación equivale conceptualmente a:

```bash
git branch experimento
git switch experimento
```

Consultá:

```bash
git branch
```

Ahora deberías tener:

```text
  main
  prueba-ramas
* experimento
```

---

## 8. Crear un cambio sobre una rama

Estamos trabajando en:

```text
experimento
```

Creá un archivo:

```text
experimento.md
```

Escribí:

```md
# Experimento

Este archivo fue creado dentro de una rama independiente.
```

Guardalo.

Consultá:

```bash
git status
```

Git debería indicar que existe un archivo nuevo.

---

## 9. Registrar el cambio

Agregá el archivo:

```bash
git add experimento.md
```

Después:

```bash
git commit -m "Agrega archivo de experimento"
```

Ahora consultá:

```bash
git log --oneline
```

La historia de la rama debería ser conceptualmente:

```text
A ── B ── C ── D
               ↑
          experimento
```

---

## 10. Volver a `main`

Ahora ejecutá:

```bash
git switch main
```

Consultá:

```bash
git status
```

Y luego:

```bash
git branch
```

Deberías estar nuevamente en:

```text
* main
  experimento
```

---

## 11. Observar qué ocurrió

Buscá:

```text
experimento.md
```

¿Qué ocurrió?

El archivo puede no aparecer en la rama `main`.

Esto demuestra una característica fundamental de las ramas:

> Cada rama representa un estado diferente del proyecto.

En `experimento` existe el commit que creó el archivo.

En `main`, ese commit todavía no forma parte de la línea de trabajo.

---

## 12. Comparar las historias

En `main` ejecutá:

```bash
git log --oneline
```

Después:

```bash
git switch experimento
```

y nuevamente:

```bash
git log --oneline
```

Compará ambas historias.

Respondé:

> ¿Qué commit aparece en `experimento` pero no aparece en `main`?

---

## 13. Volver a `main`

Ejecutá:

```bash
git switch main
```

Ahora representá conceptualmente la situación:

```text
A ── B ── C
          ↑
        main
          \
           D
            ↑
        experimento
```

Respondé:

1. ¿Dónde está `main`?
2. ¿Dónde está `experimento`?
3. ¿En qué rama existe el commit `D`?
4. ¿Qué rama tiene el archivo `experimento.md`?

---

## 14. Crear una segunda línea de trabajo

Ahora vamos a generar otra rama.

Partiendo de `main`:

```bash
git switch -c documentacion
```

Creá:

```text
documentacion.md
```

con:

```md
# Documentación

Este archivo pertenece a una segunda línea de trabajo.
```

Registrá el cambio:

```bash
git add documentacion.md
git commit -m "Agrega documentación de prueba"
```

La historia ahora puede representarse:

```text
             D
            /
A ── B ── C
            \
             E
```

Las ramas representan líneas de trabajo diferentes.

---

## 15. Consultar las ramas

Ejecutá:

```bash
git branch
```

Deberías tener algo parecido a:

```text
  main
* documentacion
  experimento
```

Identificá:

- la rama actual;
- la rama principal;
- la rama del experimento.

---

## 16. Observar los archivos

Estando en `documentacion`:

```text
documentacion.md
```

debería existir.

Ahora cambiá:

```bash
git switch experimento
```

¿Qué ocurre con los archivos?

Observá que:

```text
experimento.md
```

aparece porque pertenece a esa línea de trabajo.

Volvé a:

```bash
git switch documentacion
```

y observá nuevamente.

---

## 17. Una rama avanza

Volvé a:

```bash
git switch experimento
```

Modificá:

```text
experimento.md
```

Agregá:

```md
## Segunda versión

La rama permite continuar trabajando sin modificar directamente `main`.
```

Registrá:

```bash
git add experimento.md
git commit -m "Actualiza experimento"
```

Ahora la historia de esa rama tiene dos commits propios.

Conceptualmente:

```text
A ── B ── C
          \
           D ── E
```

---

## 18. Comparar con `main`

Volvé a:

```bash
git switch main
```

Consultá:

```bash
git log --oneline
```

Después:

```bash
git switch experimento
git log --oneline
```

Compará.

Respondé:

> ¿Cuántos commits adicionales tiene `experimento` respecto de `main`?

---

## 19. Ver la diferencia entre ramas

Git permite consultar diferencias.

Estando en `main`, podés utilizar:

```bash
git diff main..experimento
```

Observá qué cambios existen entre ambas ramas.

Después probá:

```bash
git diff experimento..main
```

Compará los resultados.

No es necesario memorizar todavía todas las variantes de `git diff`.

El objetivo es comenzar a observar que Git puede comparar diferentes líneas de trabajo.

---

## 20. Fusionar una rama

Ahora vamos a integrar el trabajo de `experimento` en `main`.

Primero:

```bash
git switch main
```

Verificá:

```bash
git status
```

Después ejecutá:

```bash
git merge experimento
```

Git intentará integrar la historia de `experimento` en `main`.

---

## 21. Observar el resultado

Consultá:

```bash
git log --oneline
```

y:

```bash
git branch
```

Ahora `main` debería incluir el trabajo que estaba en `experimento`.

El archivo:

```text
experimento.md
```

debería estar disponible desde `main`.

---

## 22. Comprender qué ocurrió

Antes del merge:

```text
A ── B ── C
          \
           D ── E
```

Después del merge, dependiendo de la historia concreta, podemos obtener una historia lineal:

```text
A ── B ── C ── D ── E
```

o una historia con un commit de merge:

```text
          D ── E
         /     \
A ── B ── C ─── M
```

No te preocupes todavía por memorizar todas las variantes.

Lo importante es comprender:

> El trabajo de una línea de evolución fue incorporado a otra.

---

## 23. El orden del merge

Vamos a comprobar una regla fundamental.

Supongamos:

```text
main
feature
```

Si queremos incorporar `feature` a `main`, primero debemos estar en:

```text
main
```

y ejecutar:

```bash
git merge feature
```

La operación significa:

```text
Estoy en main
       ↓
Incorporo feature
```

No significa simplemente:

> "unir dos ramas sin importar dónde estoy".

---

## 24. Eliminar una rama

Después de integrar `experimento`, podemos eliminar la rama:

```bash
git branch -d experimento
```

Consultá:

```bash
git branch
```

La rama `experimento` ya no debería aparecer.

Sin embargo, los commits que fueron incorporados a `main` siguen formando parte de la historia.

Esto es importante:

> **Eliminar una rama no equivale a borrar automáticamente la historia integrada.**

---

## 25. Crear una rama para una corrección

Ahora vamos a simular una situación real.

En `main`, modificá un archivo existente.

Por ejemplo:

```text
README.md
```

Suponé que detectaste un problema que querés corregir.

En lugar de trabajar directamente sobre `main`, creá:

```bash
git switch -c fix-readme
```

Realizá la corrección.

Registrala:

```bash
git add README.md
git commit -m "Corrige README"
```

Ahora tenés:

```text
main
  │
  └── fix-readme
```

La corrección está separada de la línea principal.

---

## 26. Integrar la corrección

Volvé a `main`:

```bash
git switch main
```

Integrá:

```bash
git merge fix-readme
```

Verificá que la corrección esté disponible.

Después podés eliminar la rama:

```bash
git branch -d fix-readme
```

---

## 27. Publicar una rama en GitHub

Hasta ahora trabajamos localmente.

Creá una nueva rama:

```bash
git switch -c prueba-github
```

Realizá algún cambio.

Por ejemplo:

```text
rama-remota.md
```

Registralo:

```bash
git add rama-remota.md
git commit -m "Agrega prueba de rama remota"
```

Ahora publicá la rama:

```bash
git push -u origin prueba-github
```

---

## 28. Observar GitHub

Ingresá al repositorio en GitHub.

Buscá la sección de ramas.

Deberías poder encontrar:

```text
main
prueba-github
```

La rama que creaste localmente ahora también está disponible en el repositorio remoto.

---

## 29. Comparar local y remoto

La situación ahora puede representarse:

```text
Repositorio local

main
prueba-github
```

y:

```text
GitHub

main
prueba-github
```

Recordá:

> Crear una rama local no implica publicarla automáticamente.

La publicación requiere una operación como:

```bash
git push -u origin prueba-github
```

---

## 30. Eliminar una rama local

Si la rama ya no es necesaria:

```bash
git switch main
git branch -d prueba-github
```

Consultá:

```bash
git branch
```

Observá que desapareció localmente.

---

## 31. Observar la rama remota

La rama puede continuar existiendo en GitHub.

Esto permite distinguir:

```text
rama local
```

de:

```text
rama remota
```

En un contexto de trabajo real, la administración de ambas será importante.

---

## 32. Simular un trabajo paralelo

Ahora vamos a realizar una práctica más completa.

Partí de:

```text
main
```

Creá:

```bash
git switch -c feature-a
```

Realizá un cambio y commit.

Después volvé:

```bash
git switch main
```

Creá:

```bash
git switch -c feature-b
```

Realizá otro cambio y commit.

La historia debería parecerse a:

```text
             feature-a
                ↓
A ── B ── C ── D

             feature-b
                ↓
A ── B ── C ── E
```

Las dos ramas comenzaron desde el mismo punto pero evolucionaron de manera independiente.

---

## 33. Integrar una de las ramas

Volvé a `main`:

```bash
git switch main
```

Integrá:

```bash
git merge feature-a
```

Ahora:

```text
A ── B ── C ── D
```

`feature-a` quedó integrada.

La otra rama todavía representa una línea independiente.

---

## 34. Integrar la segunda rama

Ahora:

```bash
git merge feature-b
```

Git deberá determinar cómo integrar sus cambios.

Dependiendo de qué archivos hayas modificado, puede realizar la integración automáticamente o puede requerir intervención.

Este ejercicio sirve para comenzar a comprender por qué las ramas pueden producir situaciones más complejas.

---

## 35. Si aparece un conflicto

No te preocupes si Git informa un conflicto.

Es una situación esperable.

Git puede indicar que existen conflictos en determinados archivos.

Consultá:

```bash
git status
```

Git indicará qué archivos necesitan atención.

Abrí el archivo conflictivo.

Podés encontrar marcas similares a:

```text
<<<<<<< HEAD
contenido de una rama
=======
contenido de la otra rama
>>>>>>> feature-b
```

Estas marcas indican las diferentes versiones que Git no pudo combinar automáticamente.

---

## 36. Resolver un conflicto

La resolución consiste en decidir qué contenido debe quedar.

Podés:

- conservar una versión;
- conservar la otra;
- combinar ambas;
- escribir una nueva solución.

Después de resolver el archivo, agregalo:

```bash
git add archivo
```

Finalmente completá el merge:

```bash
git commit
```

Consultá:

```bash
git status
```

El repositorio debería quedar nuevamente sin operaciones pendientes.

---

## 37. No resolver conflictos a ciegas

Ante un conflicto, no conviene eliminar automáticamente las marcas y elegir cualquier contenido.

Primero preguntate:

```text
¿Qué cambio intentaba hacer cada línea de trabajo?
```

Después:

```text
¿Qué resultado necesita realmente el proyecto?
```

El conflicto no es solamente un problema técnico.

Es una decisión sobre el contenido del proyecto.

---

## 38. Visualizar la historia

Git permite visualizar una historia con ramas mediante:

```bash
git log --oneline --graph --all
```

Ejecutalo.

Podrías obtener algo parecido a:

```text
*   9ab1234 Merge branch 'feature'
|\
| * 7cd4567 Actualiza funcionalidad
| * 4ef8912 Agrega funcionalidad
|/
* 123abcd Actualiza README
* 456efgh Crea proyecto
```

La representación gráfica ayuda a comprender las diferentes líneas de evolución.

---

## 39. Interpretar el gráfico

Observá:

```bash
git log --oneline --graph --all
```

Intentá identificar:

- la rama principal;
- las ramas secundarias;
- los commits;
- el punto donde se separaron;
- el punto donde se integraron.

No busques memorizar el gráfico.

Intentá leerlo como una historia.

---

## 40. Ejercicio de interpretación

Observá esta historia:

```text
*   M
|\
| * E
| * D
|/
* C
* B
* A
```

Respondé:

1. ¿Cuántos commits existen?
2. ¿Dónde se separó la segunda línea?
3. ¿Qué commits pertenecen a ella?
4. ¿Dónde se produjo la integración?
5. ¿Qué representa `M`?

---

## 41. Ejercicio de predicción

Antes de ejecutar los comandos, observá:

```text
A ── B ── C
          ↑
        main
```

Si ejecutamos:

```bash
git switch -c feature
```

¿cómo quedará la historia?

Después de:

```bash
echo "nuevo" > archivo.txt
git add archivo.txt
git commit -m "Agrega archivo"
```

¿cómo quedará?

Intentá dibujarlo antes de consultar Git.

---

## 42. Ejercicio de seguimiento

Realizá esta secuencia sin mirar las respuestas:

```text
1. Crear rama feature.
2. Cambiar a feature.
3. Crear un archivo.
4. Hacer commit.
5. Volver a main.
6. Observar que el archivo no está.
7. Volver a feature.
8. Observar que el archivo sí está.
9. Volver a main.
10. Hacer merge.
11. Observar que el archivo ahora está.
```

Después explicá qué ocurrió en cada etapa.

---

## 43. Ejercicio de nombres

Creá ramas para representar:

```text
Nueva funcionalidad de búsqueda
Corrección del README
Prueba de una nueva configuración
Actualización de documentación
```

Proponé nombres claros.

Por ejemplo:

```text
feature-busqueda
fix-readme
experimento-configuracion
docs-actualizacion
```

Justificá tus decisiones.

---

## 44. Comprobación final

Antes de terminar la práctica deberías poder realizar sin ayuda:

```bash
git branch
git switch -c nombre-rama
git switch nombre-rama
git status
git log --oneline
git merge nombre-rama
git branch -d nombre-rama
git push -u origin nombre-rama
```

Pero más importante que recordar los comandos es comprender:

```text
qué hacen
```

y:

```text
cuándo tiene sentido utilizarlos
```

---

## 45. Reflexión final

Respondé:

### 1.

¿Qué problema resuelven las ramas?

### 2.

¿Qué diferencia existe entre crear una rama y cambiarse a ella?

### 3.

¿Qué sucede con `main` cuando realizamos commits sobre otra rama?

### 4.

¿Por qué es importante verificar la rama actual antes de realizar un merge?

### 5.

¿Qué diferencia existe entre una rama y un commit?

### 6.

¿Qué diferencia existe entre una rama local y una rama publicada en GitHub?

### 7.

¿Por qué pueden aparecer conflictos?

### 8.

¿Qué significa resolver un conflicto?

### 9.

¿Por qué una rama puede ser útil para experimentar?

### 10.

¿Qué relación existe entre ramas, commits e historial?

---

## 46. Idea de cierre

Durante esta práctica dejamos de pensar el repositorio como una única secuencia:

```text
A ── B ── C ── D
```

y comenzamos a trabajar con:

```text
             D ── E
            /
A ── B ── C
            \
             F ── G
```

Cada línea representa una evolución diferente.

Git nos permite desarrollar esas líneas, registrarlas y posteriormente integrarlas.

> **Las ramas no complican la historia: permiten representar una historia que ya es compleja.**