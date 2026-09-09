# Proyecto
## Módulo 06 — Ramas

---

## 1. Propósito

En este proyecto vas a integrar los conceptos fundamentales trabajados durante el módulo para desarrollar diferentes líneas de trabajo dentro de un mismo repositorio.

El proyecto busca que puedas pasar de una historia lineal:

```text
A ── B ── C
```

a una historia con diferentes líneas de evolución:

```text
             D ── E
            /
A ── B ── C
            \
             F
```

y posteriormente integrar esas líneas cuando corresponda.

El objetivo no es crear muchas ramas.

El objetivo es demostrar que podés **decidir cuándo una línea de trabajo merece estar separada**, desarrollarla mediante commits y posteriormente integrarla de manera controlada.

---

# 2. Proyecto a utilizar

Podés utilizar:

- el proyecto desarrollado durante módulos anteriores;
- un proyecto propio;
- un proyecto pequeño creado específicamente para esta actividad.

Se recomienda utilizar un proyecto que ya tenga:

- repositorio Git;
- varios commits;
- README;
- algún contenido que pueda modificarse.

El proyecto debe permitir observar claramente la evolución mediante ramas.

---

# 3. Situación planteada

Imaginá que tu proyecto continúa creciendo.

Necesitás realizar simultáneamente diferentes tipos de trabajo:

```text
Nueva funcionalidad
        +
Corrección
        +
Documentación
```

No querés mezclar inmediatamente todas esas modificaciones en la línea principal.

Por eso vas a organizar el trabajo utilizando ramas.

---

# 4. Objetivo general

Construir una historia de Git que permita evidenciar:

- una rama principal;
- una rama para una nueva funcionalidad;
- una rama para una corrección;
- commits independientes;
- divergencia entre líneas de trabajo;
- integración mediante merge;
- publicación de una rama en GitHub;
- análisis de la historia resultante.

---

# 5. Preparación

Antes de comenzar:

```bash
git status
```

El repositorio debería estar limpio.

Verificá también:

```bash
git branch
```

y:

```bash
git log --oneline
```

Registrá brevemente el estado inicial.

Por ejemplo:

```text
Rama principal: main

Último commit:
...

Cantidad aproximada de commits:
...
```

---

# 6. Etapa 1 — Punto de partida

Partimos de una historia similar a:

```text
A ── B ── C
          ↑
        main
```

El proyecto debe encontrarse en la rama principal.

Verificá:

```bash
git switch main
```

y:

```bash
git status
```

No continúes hasta comprobar que estás trabajando sobre la rama correcta.

---

# 7. Etapa 2 — Crear una funcionalidad

Imaginá que el proyecto necesita una nueva funcionalidad.

Creá una rama específica.

Podés utilizar un nombre como:

```text
feature-nueva-funcionalidad
```

Creala y cambiá a ella:

```bash
git switch -c feature-nueva-funcionalidad
```

Verificá:

```bash
git branch
```

La nueva rama debe ser la rama actual.

---

# 8. Etapa 3 — Desarrollar la funcionalidad

Realizá una modificación real sobre el proyecto.

No es necesario desarrollar una funcionalidad compleja.

Puede ser:

- agregar una pequeña característica;
- incorporar un nuevo ejemplo;
- mejorar una sección;
- agregar un componente;
- modificar documentación relacionada con la funcionalidad.

El cambio debe ser suficientemente significativo como para justificar una rama.

---

# 9. Primer commit de la funcionalidad

Registrá el primer avance:

```bash
git add .
git commit -m "Agrega nueva funcionalidad"
```

Verificá:

```bash
git log --oneline
```

La historia debería comenzar a verse conceptualmente así:

```text
A ── B ── C ── D
               ↑
      feature-nueva-funcionalidad
```

---

# 10. Segundo commit

Continuá desarrollando la funcionalidad.

Realizá una mejora adicional.

Por ejemplo:

- completar la implementación;
- corregir un detalle;
- agregar documentación;
- mejorar un ejemplo.

Registrá otro commit:

```bash
git add .
git commit -m "Completa nueva funcionalidad"
```

Ahora deberías tener:

```text
A ── B ── C ── D ── E
                    ↑
           feature-nueva-funcionalidad
```

---

# 11. Etapa 4 — Volver a `main`

Ahora simularemos otro trabajo que debe realizarse de manera independiente.

Volvé a:

```bash
git switch main
```

Verificá:

```bash
git status
```

La rama actual debe ser:

```text
main
```

---

# 12. Etapa 5 — Crear una rama de corrección

Supongamos que encontramos un problema independiente de la nueva funcionalidad.

Creá:

```bash
git switch -c fix-correccion
```

El nombre debe comunicar claramente el propósito de la rama.

---

# 13. Etapa 6 — Realizar la corrección

Realizá una modificación concreta.

Por ejemplo:

- corregir un error;
- solucionar un problema de documentación;
- ajustar un ejemplo;
- corregir una configuración;
- reparar un comportamiento sencillo.

Registrá el cambio:

```bash
git add .
git commit -m "Corrige problema"
```

La historia ahora puede representarse:

```text
             D ── E
            /
A ── B ── C
            \
             F
```

Las ramas representan líneas de trabajo diferentes.

---

# 14. Etapa 7 — Observar la divergencia

Antes de integrar nada, ejecutá:

```bash
git log --oneline --graph --all
```

Observá la historia.

Identificá:

- `main`;
- `feature-nueva-funcionalidad`;
- `fix-correccion`;
- los commits propios de cada línea;
- el punto donde comenzaron a separarse.

Documentá brevemente lo observado.

---

# 15. Etapa 8 — Publicar una rama

Elegí una de las ramas de trabajo.

Por ejemplo:

```text
feature-nueva-funcionalidad
```

Publicala:

```bash
git push -u origin feature-nueva-funcionalidad
```

Ingresá al repositorio en GitHub.

Comprobá que la rama exista.

---

# 16. Etapa 9 — Analizar GitHub

En GitHub verificá:

- que la rama esté publicada;
- que sus commits estén disponibles;
- que la rama `main` continúe separada;
- que los cambios de la rama todavía no formen parte de `main`.

Respondé:

> ¿Qué diferencia existe entre tener una rama local y tenerla publicada en GitHub?

---

# 17. Etapa 10 — Integrar la corrección

Ahora vamos a incorporar la corrección.

Ubicate en:

```bash
git switch main
```

Verificá:

```bash
git status
```

Después:

```bash
git merge fix-correccion
```

Observá el resultado.

---

# 18. Etapa 11 — Analizar el primer merge

Ejecutá:

```bash
git log --oneline --graph --all
```

Analizá:

```text
¿Qué rama estaba activa?
¿Qué rama fue incorporada?
¿Qué commits aparecieron ahora en main?
¿Cómo cambió la historia?
```

Documentá las respuestas.

---

# 19. Etapa 12 — Continuar el trabajo de la funcionalidad

La rama:

```text
feature-nueva-funcionalidad
```

todavía existe.

Podés volver a ella:

```bash
git switch feature-nueva-funcionalidad
```

Realizá una mejora adicional.

Registrá:

```bash
git add .
git commit -m "Mejora nueva funcionalidad"
```

Ahora la rama contiene un commit adicional.

---

# 20. Etapa 13 — Integrar la funcionalidad

Volvé a:

```bash
git switch main
```

Verificá:

```bash
git status
```

Después:

```bash
git merge feature-nueva-funcionalidad
```

Si Git puede realizar la integración automáticamente, observá el resultado.

Si aparece un conflicto, no lo evites.

Resolvelo siguiendo el procedimiento trabajado en el módulo.

---

# 21. Etapa 14 — Resolver un posible conflicto

Si aparece un conflicto:

```bash
git status
```

Identificá los archivos afectados.

Abrilos y analizá las diferencias.

Decidí qué contenido debe quedar.

Después:

```bash
git add archivo
```

y completá la integración:

```bash
git commit
```

Verificá:

```bash
git status
```

El repositorio debería quedar en un estado consistente.

---

# 22. Etapa 15 — Analizar la historia final

Ejecutá:

```bash
git log --oneline --graph --all
```

Estudiá el resultado.

Respondé:

1. ¿Dónde comenzó la historia?
2. ¿Dónde se separó cada rama?
3. ¿Qué trabajo se realizó en cada una?
4. ¿Cuál fue integrada primero?
5. ¿Cuál fue integrada después?
6. ¿Hubo conflictos?
7. ¿Cómo quedaron representados los merges?

---

# 23. Etapa 16 — Eliminar ramas terminadas

Una vez integradas y comprobadas las ramas, evaluá si siguen siendo necesarias.

Si ya cumplieron su propósito:

```bash
git branch -d fix-correccion
```

y:

```bash
git branch -d feature-nueva-funcionalidad
```

Antes de eliminarlas, asegurate de que su trabajo esté efectivamente integrado.

---

# 24. Etapa 17 — Verificar ramas

Ejecutá:

```bash
git branch
```

Debería quedar como mínimo:

```text
* main
```

Las ramas pueden continuar existiendo en el repositorio remoto si fueron publicadas.

Esto permite volver a observar la diferencia entre:

```text
rama local
```

y:

```text
rama remota
```

---

# 25. Etapa 18 — Estado final

Verificá:

```bash
git status
```

El repositorio debería quedar limpio.

Después:

```bash
git log --oneline --graph --all
```

y:

```bash
git branch
```

Registrá la salida o una captura para utilizarla como evidencia del proyecto.

---

# 26. Documentar el proyecto

Creá:

```text
docs/ramas.md
```

Utilizá como estructura mínima:

```md
# Estrategia de ramas

## Proyecto

Descripción breve.

## Rama principal

Propósito de `main`.

## Ramas utilizadas

### feature-nueva-funcionalidad

Propósito y cambios realizados.

### fix-correccion

Propósito y cambios realizados.

## Integración

Descripción de los merges.

## Conflictos

Indicar si se produjo alguno y cómo fue resuelto.

## Publicación

Indicar qué rama fue publicada en GitHub.

## Resultado

Descripción de la historia final.

## Aprendizajes

Reflexión sobre el trabajo con ramas.
```

---

# 27. Documentar la historia

En `docs/ramas.md` incorporá una representación simplificada de la historia.

Por ejemplo:

```text
             feature
            /       \
main ──────          ── merge
            \
             fix
```

Adaptala a la historia real de tu proyecto.

No inventes una historia diferente de la que realmente construiste.

---

# 28. Documentar los comandos

Incluí los comandos principales utilizados.

Por ejemplo:

```bash
git switch -c feature-nueva-funcionalidad
git add .
git commit -m "Agrega nueva funcionalidad"
git switch main
git merge feature-nueva-funcionalidad
git push -u origin feature-nueva-funcionalidad
```

Acompañá cada grupo de comandos con una explicación.

La documentación no debe convertirse simplemente en una lista de comandos.

---

# 29. Reflexión

Respondé:

### ¿Por qué decidiste utilizar ramas?

---

### ¿Qué problema resolvieron?

---

### ¿Qué diferencia observaste entre trabajar en `main` y trabajar en una rama?

---

### ¿Qué ocurrió con `main` mientras trabajabas en las ramas?

---

### ¿Qué aprendiste al realizar un merge?

---

### ¿Apareció algún conflicto?

Si apareció:

- ¿por qué ocurrió?
- ¿cómo lo resolviste?

Si no apareció:

- ¿qué situación podría haberlo provocado?

---

### ¿Qué importancia tuvo verificar la rama actual?

---

### ¿Qué diferencia observaste entre una rama local y una publicada en GitHub?

---

# 30. Evidencias

El proyecto deberá conservar evidencia de:

```text
[ ] Estado inicial del repositorio
[ ] Creación de ramas
[ ] Commits realizados
[ ] Historia divergente
[ ] Merge
[ ] Publicación de una rama
[ ] Historia final
[ ] Documentación
```

La evidencia puede consistir en:

- salida de comandos;
- capturas;
- documentación;
- historial Git.

---

# 31. Criterios de evaluación

El proyecto será considerado logrado cuando:

### Comprensión

Se comprende qué problema resuelven las ramas.

### Organización

Las ramas utilizadas tienen propósitos claros.

### Commits

Los cambios están registrados mediante commits coherentes.

### Integración

Las ramas pueden integrarse correctamente.

### Historia

Se puede interpretar la evolución del proyecto mediante Git.

### GitHub

Al menos una rama fue publicada y comprobada en el repositorio remoto.

### Documentación

El proceso está documentado de manera clara.

### Reflexión

Se pueden explicar las decisiones tomadas durante el proyecto.

---

# 32. Condición fundamental

No se evalúa la cantidad de ramas creadas.

Tampoco se evalúa la cantidad de comandos utilizados.

Se evalúa la capacidad de utilizar ramas como una herramienta para organizar la evolución del proyecto.

El criterio central es:

```text
necesidad
   ↓
decisión
   ↓
rama
   ↓
trabajo
   ↓
commit
   ↓
integración
   ↓
historia
```

---

# 33. Resultado esperado

Al finalizar deberías poder observar tu repositorio y comprender algo como:

```text
                    feature
                   /       \
                  /         \
A ── B ── C ─────             ── M
                  \
                   fix ────────/
```

y explicar qué representa cada parte.

No solamente:

> "Esto es un gráfico de Git."

Sino:

> "El proyecto llegó hasta este punto, desde allí se separaron dos líneas de trabajo, cada una evolucionó mediante commits y posteriormente sus cambios fueron integrados en `main`."

Ese es el aprendizaje central del proyecto.

---

# 34. Entrega final

La entrega deberá contener:

```text
Repositorio
│
├── README.md
│
├── docs/
│   └── ramas.md
│
└── resto del proyecto
```

Además, el historial Git deberá permitir comprobar el trabajo realizado.

La entrega deberá estar publicada en GitHub.

---

# 35. Cierre

Hasta este módulo trabajamos principalmente con la idea:

```text
cambio
   ↓
commit
   ↓
historia
```

Ahora incorporamos:

```text
cambio
   ↓
línea de trabajo
   ↓
rama
   ↓
commit
   ↓
historia
   ↓
integración
```

Este cambio conceptual es fundamental para avanzar hacia el trabajo colaborativo.

> **Una rama no es solamente una herramienta técnica. Es una forma de organizar el trabajo y hacer explícitas las distintas líneas de evolución de un proyecto.**