# Ejercicios
## Módulo 08 — Perfil Profesional

Los siguientes ejercicios buscan ayudarte a transformar conocimientos y trabajos técnicos en evidencia concreta de aprendizaje.

La propuesta es avanzar desde el análisis de proyectos existentes hacia la construcción y presentación de un perfil profesional técnico.

---

# Ejercicio 1 — Mirar un repositorio como visitante

Elegí un repositorio que no conozcas.

Puede ser propio o ajeno.

Sin ejecutar el proyecto, respondé:

1. ¿Qué entendés que hace?
2. ¿Cuál parece ser su objetivo?
3. ¿Quién podría utilizarlo?
4. ¿Qué tecnologías utiliza?
5. ¿Cómo se instala?
6. ¿Cómo se ejecuta?
7. ¿Dónde encontraste esa información?
8. ¿Qué información falta?

### Reflexión

¿Cuánto pudiste comprender solamente a partir del repositorio?

---

# Ejercicio 2 — Evaluar un README

Elegí un proyecto propio.

Completá:

| Aspecto | Completo | Parcial | Falta | No aplica |
|---|---|---|---|---|
| Descripción | | | | |
| Objetivo | | | | |
| Instalación | | | | |
| Uso | | | | |
| Ejemplos | | | | |
| Tecnologías | | | | |
| Estructura | | | | |
| Contribución | | | | |
| Licencia | | | | |

Después seleccioná los tres aspectos que más necesitan mejorar.

---

# Ejercicio 3 — Descripción del proyecto

Tomá la descripción actual de un proyecto y respondé:

> ¿Explica claramente qué hace el proyecto o solamente qué tecnología utiliza?

Compará:

```text
Proyecto realizado en Python.
```

con:

```text
Aplicación que permite registrar y consultar
las tareas pendientes de un usuario.
```

Explicá cuál comunica mejor el propósito y por qué.

---

# Ejercicio 4 — Problema y solución

Para uno de tus proyectos completá:

```text
Problema:

________________________________________

Solución:

________________________________________
```

Después explicá la relación:

```text
problema
   ↓
solución
```

No inventes un problema que el proyecto nunca intentó resolver.

---

# Ejercicio 5 — Tecnologías utilizadas

Elaborá una lista de las tecnologías realmente utilizadas en tu proyecto.

Por ejemplo:

```text
Python
Git
GitHub
Markdown
```

Después, para cada una, indicá:

```text
Tecnología
↓
¿Dónde la utilicé?
↓
¿Qué demuestra?
```

No incluyas tecnologías que solamente conozcas pero que no hayas utilizado en el proyecto.

---

# Ejercicio 6 — Requisitos

Analizá un proyecto y determiná qué necesita una persona para utilizarlo.

Completá:

```text
Sistema operativo:
________________

Software:
________________

Versiones:
________________

Dependencias:
________________
```

Si algún dato no aplica, indicá:

```text
No aplica.
```

---

# Ejercicio 7 — Instalación

Escribí las instrucciones de instalación de tu proyecto.

Deben poder seguirse desde cero.

Incluí, cuando corresponda:

```bash
git clone ...
cd ...
...
```

Después pedile a otra persona que intente seguirlas sin recibir explicaciones adicionales.

Registrá:

```text
¿Qué pudo hacer?
¿Qué no pudo hacer?
¿Qué información faltó?
```

---

# Ejercicio 8 — Probar la documentación

Una persona que no conoce tu proyecto debe intentar instalarlo utilizando únicamente el README.

No la ayudes durante la primera prueba.

Después registrá:

```text
Paso 1 → OK
Paso 2 → Problema
Paso 3 → OK
...
```

Finalmente corregí la documentación.

---

# Ejercicio 9 — Ejemplo de uso

Agregá al README un ejemplo concreto.

Debe incluir, cuando corresponda:

```text
entrada
   ↓
ejecución
   ↓
resultado
```

Por ejemplo:

```md
## Ejemplo

Entrada:

...

Resultado:

...
```

Verificá que el ejemplo corresponda con el comportamiento real del proyecto.

---

# Ejercicio 10 — Estructura del proyecto

Representá la estructura de un proyecto:

```text
proyecto/
├── README.md
├── src/
├── tests/
└── docs/
```

Después explicá el propósito de cada directorio.

No agregues directorios que el proyecto no tenga.

---

# Ejercicio 11 — Archivos que deberían ignorarse

Analizá los archivos de tu proyecto.

Identificá cuáles son:

```text
necesarios
temporales
generados
locales
sensibles
```

Después proponé qué debería incluir `.gitignore`.

---

# Ejercicio 12 — Crear un `.gitignore`

Creá un archivo:

```text
.gitignore
```

adecuado para tu proyecto.

Incluí solamente reglas necesarias.

Después ejecutá:

```bash
git status
```

y verificá el comportamiento.

---

# Ejercicio 13 — Verificar `.gitignore`

Creá deliberadamente un archivo que debería ser ignorado.

Por ejemplo:

```text
archivo-temporal.log
```

Agregá una regla apropiada a `.gitignore`.

Después ejecutá:

```bash
git status
```

Respondé:

> ¿Por qué el archivo no aparece como cambio pendiente?

---

# Ejercicio 14 — `.gitignore` no es un borrador de historia

Supongamos que alguien realizó:

```bash
git add .env
git commit -m "Agrega configuración"
git push
```

Después agregó:

```text
.env
```

a:

```text
.gitignore
```

Respondé:

1. ¿El secreto dejó de existir en la historia?
2. ¿Por qué?
3. ¿Qué diferencia existe entre evitar un seguimiento futuro y eliminar información ya registrada?

---

# Ejercicio 15 — Detectar información sensible

Analizá estos ejemplos:

```text
API_KEY=123456
```

```text
PASSWORD=secreto
```

```text
TOKEN=abcdef
```

```text
DATABASE_URL=...
```

Indicá:

```text
¿Debe publicarse?
¿Por qué?
¿Qué debería hacerse?
```

---

# Ejercicio 16 — Revisar un repositorio antes de publicarlo

Antes de hacer público un proyecto, elaborá una lista de comprobación.

Como mínimo:

```text
[ ] No hay contraseñas.
[ ] No hay tokens.
[ ] No hay claves.
[ ] No hay datos personales innecesarios.
[ ] README actualizado.
[ ] .gitignore revisado.
[ ] Proyecto identificable.
```

Agregá cinco comprobaciones propias.

---

# Ejercicio 17 — Analizar el historial

Ejecutá:

```bash
git log --oneline --graph --all
```

Respondé:

1. ¿Cuántos commits tiene el proyecto?
2. ¿Los mensajes son comprensibles?
3. ¿Existen ramas?
4. ¿La historia permite reconocer etapas?
5. ¿Hay commits cuyo propósito resulte difícil de identificar?

---

# Ejercicio 18 — Mensajes de commit

Clasificá los siguientes mensajes como:

```text
claro
```

o:

```text
poco claro
```

### A

```text
cambios
```

### B

```text
Agrega validación de entrada
```

### C

```text
fix
```

### D

```text
Documenta instalación
```

### E

```text
final
```

### F

```text
Corrige cálculo del promedio
```

Justificá tus respuestas.

---

# Ejercicio 19 — Mejorar commits

Transformá estos mensajes:

```text
cambios
fix
cosas
prueba
final
```

en mensajes más descriptivos.

No es necesario que sean idénticos a los utilizados en un proyecto real.

El objetivo es aprender a comunicar el propósito del cambio.

---

# Ejercicio 20 — Issue como evidencia

Creá una Issue para una mejora real de uno de tus proyectos.

Debe contener:

```md
# Título

...

## Problema

...

## Objetivo

...

## Resultado esperado

...
```

Después explicá qué capacidad demuestra esta Issue.

---

# Ejercicio 21 — Pull Request como evidencia

Elegí una Pull Request de uno de tus proyectos.

Analizá:

```text
Título
Descripción
Commits
Archivos modificados
Comentarios
Revisión
Resultado
```

Respondé:

> ¿Qué puede aprender una persona externa sobre tu forma de trabajar a partir de esta Pull Request?

---

# Ejercicio 22 — Mejorar una Pull Request

Imaginá esta Pull Request:

```text
Título:
Cambios

Descripción:
Hice varias cosas.
```

Reescribila utilizando:

```md
## Qué hice

...

## Por qué

...

## Cómo lo probé

...

## Issue relacionada

...
```

---

# Ejercicio 23 — Proyecto académico

Elegí un trabajo práctico que hayas realizado.

Respondé:

```text
¿Qué problema resolvía?

¿Qué construí?

¿Qué aprendí?

¿Qué decisiones tomé?

¿Qué dificultad encontré?

¿Qué mejoraría?
```

Después explicá:

> ¿Qué tendría que cambiar para que este trabajo pueda presentarse como un proyecto de portafolio?

---

# Ejercicio 24 — Del trabajo práctico al proyecto

Partimos de:

```text
trabajo práctico
```

Diseñá el proceso:

```text
trabajo práctico
      ↓
?
      ↓
?
      ↓
?
      ↓
proyecto presentable
```

Utilizá conceptos trabajados durante el módulo.

---

# Ejercicio 25 — Selección de proyectos

Elegí entre uno y tres proyectos para destacar.

Para cada uno completá:

```text
Proyecto:
__________

¿Por qué lo selecciono?
__________

¿Qué demuestra?
__________

¿Qué aprendí?
__________

¿Qué debería mejorar?
__________
```

---

# Ejercicio 26 — Proyecto que no conviene mostrar

Elegí un proyecto que actualmente no presentarías profesionalmente.

Explicá por qué.

Podés considerar:

- falta de documentación;
- código incompleto;
- información sensible;
- falta de contexto;
- proyecto demasiado pequeño;
- resultado experimental.

Después indicá qué debería mejorar para convertirse en una pieza presentable.

---

# Ejercicio 27 — Cantidad versus calidad

Compará:

### Perfil A

```text
40 repositorios
10 seguidores
muchos commits
README mínimos
```

### Perfil B

```text
4 repositorios
README completos
proyectos explicados
historial comprensible
```

¿Cuál considerás más útil para conocer el trabajo de la persona?

Justificá.

---

# Ejercicio 28 — Tecnología y evidencia

Una persona afirma:

```text
"Conozco Python, Git, GitHub, SQL y Docker."
```

Pero su perfil solamente contiene:

```text
un repositorio vacío
```

Analizá la afirmación.

¿Qué podría hacer para generar evidencia concreta?

---

# Ejercicio 29 — Habilidad y proyecto

Completá:

| Habilidad | Proyecto que la demuestra | Evidencia |
|---|---|---|
| Programación | | |
| Git | | |
| GitHub | | |
| Documentación | | |
| Colaboración | | |
| Comunicación técnica | | |

No es obligatorio completar todas las filas si no existe evidencia real.

---

# Ejercicio 30 — Perfil profesional

Redactá una presentación breve.

Debe responder:

```text
¿Quién soy?
¿Qué estoy aprendiendo o haciendo?
¿Qué tecnologías estoy trabajando?
¿Qué temas me interesan?
```

Evitá afirmaciones que no puedas sostener con evidencia.

---

# Ejercicio 31 — Comparar presentaciones

Analizá:

### Perfil A

```text
Soy experto en programación,
Git, Python, bases de datos,
DevOps, inteligencia artificial
y muchas tecnologías más.
```

### Perfil B

```text
Estoy aprendiendo programación con Python
y trabajando en proyectos donde practico
Git, GitHub y documentación técnica.
```

¿Cuál te parece más creíble?

¿Por qué?

---

# Ejercicio 32 — Coherencia profesional

Compará:

```text
CV
GitHub
README
Portafolio
```

Para cada uno respondé:

```text
¿Presentan información consistente?
¿Existen contradicciones?
¿Hay tecnologías declaradas sin evidencia?
```

---

# Ejercicio 33 — CV y GitHub

Tomá una experiencia o proyecto que figure en tu CV.

Buscá su correspondiente evidencia en GitHub.

Completá:

```text
CV:
________________

GitHub:
________________

Evidencia:
________________
```

Si no existe evidencia, explicá qué podrías construir para generarla.

---

# Ejercicio 34 — README como presentación

Imaginá que una persona recibe el enlace de tu repositorio y dispone solamente de un minuto.

¿Qué debería poder descubrir durante ese minuto?

Elaborá una lista de prioridades.

Por ejemplo:

```text
1. Qué es.
2. Para qué sirve.
3. Cómo probarlo.
4. Qué tecnologías utiliza.
```

---

# Ejercicio 35 — Presentación técnica

Prepará una presentación oral de tres minutos sobre un proyecto.

Debe contener:

```text
Problema
Solución
Tecnologías
Decisiones
Resultado
Aprendizajes
```

No leas el README.

Explicá el proyecto.

---

# Ejercicio 36 — Preguntas del público

Después de presentar un proyecto, respondé:

> ¿Por qué elegiste esa tecnología?

> ¿Qué fue lo más difícil?

> ¿Qué cambiarías?

> ¿Cómo probarías el proyecto?

> ¿Cómo podría contribuir otra persona?

> ¿Qué aprendiste?

La intención es comprobar que comprendés el proyecto y no solamente que podés describirlo.

---

# Ejercicio 37 — Revisión externa

Pedile a otra persona que observe tu repositorio durante cinco minutos.

No le expliques nada.

Pedile que responda:

```text
¿Qué entendiste que hace?

¿Qué tecnología utiliza?

¿Cómo se ejecuta?

¿Qué te resultó confuso?

¿Qué mejorarías?
```

Compará sus respuestas con tus intenciones.

---

# Ejercicio 38 — Mejorar a partir de feedback

Utilizando las observaciones anteriores:

1. identificá los problemas;
2. priorizalos;
3. corregí los más importantes;
4. actualizá el README;
5. repetí la prueba.

Documentá qué cambió.

---

# Ejercicio 39 — Revisión del perfil

Observá tu perfil de GitHub como si fueras una persona externa.

Respondé:

```text
¿Qué proyecto aparece primero?

¿Qué información encuentro?

¿Qué proyecto destacaría?

¿Qué repositorio debería mejorar?

¿Hay algo que debería ocultar o eliminar?
```

---

# Ejercicio 40 — Repositorios públicos y privados

Clasificá estos casos:

| Caso | Público | Privado | Depende |
|---|---|---|---|
| Proyecto personal terminado | | | |
| Trabajo con datos sensibles | | | |
| Ejercicio académico simple | | | |
| Proyecto profesional confidencial | | | |
| Proyecto de portafolio | | | |

Justificá las decisiones.

---

# Ejercicio 41 — Información que no debería publicarse

Analizá:

```text
nombre del proyecto
README
código
archivo .env
contraseña
token
capturas
datos de usuarios
```

Indicá cuáles podrían ser apropiados para publicar y cuáles requieren cuidado.

No todas las respuestas son necesariamente absolutas.

Justificá.

---

# Ejercicio 42 — Crear un `PORTFOLIO.md`

Creá:

```text
PORTFOLIO.md
```

con:

```md
# Mi portafolio

## Sobre mí

...

## Proyectos

...

## Tecnologías

...

## Aprendizajes

...
```

El contenido debe basarse en experiencia real.

---

# Ejercicio 43 — Mejorar un proyecto existente

Elegí un proyecto que ya tengas.

Realizá al menos tres mejoras:

```text
1. Documentación.
2. Organización.
3. Evidencia técnica.
```

Podés incluir:

- README;
- `.gitignore`;
- ejemplo;
- tests;
- estructura;
- Issues;
- Pull Request.

Documentá las mejoras.

---

# Ejercicio 44 — Construir evidencia

Elegí una capacidad que quieras demostrar.

Por ejemplo:

```text
programación
```

Diseñá:

```text
capacidad
   ↓
proyecto
   ↓
evidencia
   ↓
explicación
```

Repetí el ejercicio con:

```text
Git
documentación
colaboración
```

---

# Ejercicio 45 — Perfil sin exageraciones

Reescribí estas afirmaciones para hacerlas más concretas:

```text
"Soy experto en Git."
```

```text
"Domino Python."
```

```text
"Soy especialista en bases de datos."
```

Transformalas en afirmaciones que puedan respaldarse con proyectos o experiencia real.

---

# Ejercicio 46 — Próximas mejoras

Creá una lista de mejoras para tu perfil.

Por ejemplo:

```text
- mejorar README del proyecto A
- agregar proyecto B
- documentar proyecto C
- completar CONTRIBUTING.md
- revisar .gitignore
```

Priorizalas:

```text
Alta
Media
Baja
```

---

# Ejercicio 47 — Analizar un proyecto desde afuera

Elegí un repositorio de otra persona.

Intentá reconstruir:

```text
qué problema resuelve
qué tecnologías utiliza
cómo evolucionó
cómo trabaja la persona
```

Después indicá:

> ¿Qué conclusiones pudiste obtener solamente a partir de la evidencia disponible?

---

# Ejercicio 48 — La historia del proyecto

Tomá:

```bash
git log --oneline --graph --all
```

y escribí una breve narración de la evolución del proyecto.

Por ejemplo:

```text
Primero se creó la estructura básica.
Después se incorporó...
Luego se corrigió...
Finalmente se documentó...
```

La narración debe surgir de la historia real.

---

# Ejercicio 49 — Auditoría final

Realizá una revisión completa:

```text
[ ] Proyecto identificable.
[ ] README claro.
[ ] Instalación documentada.
[ ] Uso documentado.
[ ] Ejemplo disponible.
[ ] Tecnologías reales.
[ ] .gitignore revisado.
[ ] No hay secretos visibles.
[ ] Historial comprensible.
[ ] Proyecto seleccionable para portafolio.
```

Agregá tres criterios propios.

---

# Ejercicio 50 — Proyecto presentable

Elegí un proyecto y preparalo para que otra persona pueda conocerlo sin tu intervención.

Debe contener como mínimo:

```text
README.md
.gitignore
código o material técnico
```

Además:

```text
objetivo
instalación
uso
tecnologías
ejemplo
```

Finalmente prepará una presentación oral de tres a cinco minutos.

---

# Comprobación final

Sin consultar el material, respondé:

### 1.

¿Qué diferencia existe entre tener un proyecto y tener evidencia de un proyecto?

### 2.

¿Qué función cumple un README?

### 3.

¿Por qué la documentación forma parte del trabajo técnico?

### 4.

¿Qué información no debería publicarse en un repositorio?

### 5.

¿Qué función cumple `.gitignore`?

### 6.

¿Por qué `.gitignore` no elimina un secreto que ya fue registrado?

### 7.

¿Qué puede mostrar el historial de Git sobre un proyecto?

### 8.

¿Qué puede aportar una Pull Request como evidencia?

### 9.

¿Cómo seleccionarías proyectos para un portafolio?

### 10.

¿Qué relación existe entre una habilidad y la evidencia que la demuestra?

### 11.

¿Qué diferencia existe entre un CV y GitHub?

### 12.

¿Qué debería poder comprender una persona al entrar a tu repositorio?

---

# Criterio de resolución

Los ejercicios no se consideran completamente resueltos solamente por producir un archivo o ejecutar un comando.

La resolución debería permitir explicar:

```text
qué hice
   ↓
por qué lo hice
   ↓
qué problema resolví
   ↓
qué evidencia quedó
   ↓
qué puedo explicar sobre ella
```

El objetivo del módulo no es construir una apariencia profesional.

Es aprender a convertir el trabajo técnico real en una evidencia clara, organizada y comprensible.

> **No se trata de decir "sé". Se trata de poder mostrar, explicar y sostener lo que decís que sabés.**