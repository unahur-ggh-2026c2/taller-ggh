# Filosofía del Curso
## Git y GitHub

> **Git no se aprende memorizando comandos. Se aprende trabajando con versiones, cometiendo errores, recuperando cambios y colaborando con otras personas.**

---

## 1. Una herramienta para trabajar, no un contenido para memorizar

Git y GitHub son herramientas utilizadas para resolver problemas concretos del desarrollo de software.

Por este motivo, el curso no se estructura como un catálogo de comandos ni como un recorrido exhaustivo por todas las funcionalidades disponibles.

El propósito es que los estudiantes comprendan qué problema resuelve cada herramienta, qué información administra y qué alternativas ofrece ante las situaciones habituales de un proyecto.

Los comandos aparecen como consecuencia de esa necesidad.

La secuencia pedagógica buscada es:

**problema → concepto → herramienta → práctica → comprensión**

y no:

**comando → memorización → repetición.**

---

## 2. Comprender antes que memorizar

Una persona puede memorizar una secuencia de comandos y, aun así, no comprender qué está haciendo Git.

Ese aprendizaje resulta frágil.

Ante una situación diferente de la practicada, el estudiante queda sin herramientas para decidir qué hacer.

Por eso el curso prioriza la construcción de un modelo mental que permita interpretar el estado de un repositorio y tomar decisiones.

El estudiante debe poder responder preguntas como:

- ¿Dónde está mi cambio?
- ¿Qué versión estoy viendo?
- ¿Qué cambios están preparados para confirmar?
- ¿Qué quedó registrado en el historial?
- ¿Qué ocurrió entre dos versiones?
- ¿Puedo recuperar lo que hice?
- ¿Dónde está el repositorio remoto?
- ¿Qué cambios tengo localmente y cuáles están publicados?
- ¿Qué sucede cuando otra persona modificó lo mismo que yo?
- ¿Qué estrategia puedo utilizar para integrar ambos trabajos?

Cuando el estudiante comprende estas preguntas, los comandos dejan de ser instrucciones aisladas y pasan a formar parte de un sistema coherente.

---

## 3. Aprender haciendo

Git es una herramienta eminentemente práctica.

Su comprensión requiere utilizarla, observar sus efectos, equivocarse y volver a intentar.

Por esta razón, cada concepto importante deberá estar acompañado por una experiencia práctica que permita observar qué ocurre en el repositorio.

La explicación teórica debe ser breve y funcional a la práctica.

No se busca eliminar la teoría, sino utilizarla en la medida necesaria para comprender lo que se está haciendo.

La práctica no es una instancia posterior a la explicación.

**La práctica es parte del proceso mediante el cual se construye el conocimiento.**

---

## 4. El error como herramienta pedagógica

Los errores son parte natural del trabajo con Git.

Un archivo eliminado accidentalmente, un commit realizado en un momento inadecuado, una rama mal utilizada o un conflicto entre cambios pueden convertirse en situaciones de aprendizaje mucho más significativas que una explicación teórica sobre el mismo problema.

Por este motivo, el curso no debe enseñar únicamente el camino correcto.

También debe enseñar:

- cómo reconocer que algo salió mal;
- cómo interpretar lo que Git informa;
- cómo determinar qué ocurrió;
- cómo recuperar el trabajo;
- cómo corregir la situación;
- cómo evitar repetir el mismo problema.

El objetivo no es que el estudiante nunca se equivoque.

El objetivo es que **sepa qué hacer cuando se equivoca**.

---

## 5. Los conflictos no son una falla del proceso

En un entorno colaborativo, los conflictos no son necesariamente errores.

Son una consecuencia posible de que diferentes personas trabajen sobre un mismo proyecto y, en determinados casos, sobre los mismos archivos o partes de ellos.

Por eso el curso debe presentar los conflictos como una situación normal del trabajo colaborativo.

Los estudiantes deben experimentar deliberadamente situaciones en las que dos personas realizan cambios incompatibles sobre un mismo archivo y luego resolverlas.

La resolución de conflictos constituye una de las experiencias prácticas centrales del curso porque permite comprender que Git no elimina los problemas derivados de la colaboración: proporciona herramientas para identificarlos, analizarlos y resolverlos.

---

## 6. Un entorno deliberadamente simple

El curso utilizará principalmente carpetas y archivos Markdown para las actividades prácticas.

Esta decisión no responde a una limitación técnica.

Responde a una decisión pedagógica.

Trabajar con Markdown permite concentrar la atención en Git y GitHub sin incorporar simultáneamente la complejidad sintáctica, de compilación, ejecución o depuración de un lenguaje de programación.

Un archivo Markdown puede:

- crearse;
- modificarse;
- compararse;
- confirmarse;
- revertirse;
- compartir sus cambios;
- entrar en conflicto;
- fusionarse;
- documentar un proyecto.

Por lo tanto, permite reproducir una gran parte de las situaciones que posteriormente aparecerán sobre archivos de código.

El objetivo es desarrollar primero el **músculo de trabajar con versiones y colaborar**, para luego transferirlo a proyectos de programación.

---

## 7. Del entorno controlado al proyecto real

Las actividades del curso utilizan situaciones simplificadas y controladas para facilitar el aprendizaje.

Sin embargo, el estudiante debe comprender desde el principio que los procedimientos practicados no son exclusivos de Markdown.

La misma lógica se aplica posteriormente sobre:

- archivos fuente;
- proyectos completos;
- configuraciones;
- documentación;
- scripts;
- archivos de datos;
- proyectos desarrollados en diferentes lenguajes.

El repositorio utilizado durante el curso funciona como un laboratorio.

Lo aprendido en ese laboratorio debe poder trasladarse posteriormente a proyectos reales.

---

## 8. El trabajo colaborativo se aprende colaborando

No alcanza con explicar qué es un repositorio remoto, una rama o un Pull Request.

Para comprender realmente el trabajo colaborativo, los estudiantes deben experimentar situaciones en las que:

- dos personas trabajan sobre el mismo proyecto;
- los cambios deben sincronizarse;
- diferentes ramas evolucionan en paralelo;
- una modificación debe integrarse;
- aparecen conflictos;
- alguien debe revisar un cambio realizado por otra persona.

El curso debe generar estas situaciones de manera progresiva y controlada.

La dificultad debe crecer junto con la comprensión de los estudiantes.

---

## 9. El docente como guía, no como operador remoto

Durante las actividades prácticas, el docente no debe convertirse en la persona que ejecuta los comandos por los estudiantes.

Cuando aparece un problema, la intervención docente debe favorecer el razonamiento:

> ¿Qué estado tiene el repositorio?

> ¿Qué cambió?

> ¿Qué información nos está dando Git?

> ¿Qué queremos conseguir?

> ¿Qué alternativas tenemos?

La asistencia debe orientarse a que el estudiante aprenda a diagnosticar y resolver la situación por sí mismo.

El objetivo es desarrollar autonomía.

Un estudiante que necesita que el docente le diga permanentemente qué comando ejecutar todavía no domina la herramienta, aunque pueda completar correctamente una secuencia de pasos.

---

## 10. La documentación forma parte del desarrollo

Un proyecto no está completo solamente porque funciona.

También debe poder ser comprendido por otras personas.

Por este motivo, la documentación mediante Markdown forma parte del ecosistema del curso.

Los estudiantes trabajarán progresivamente sobre:

- README;
- estructura de documentos;
- instrucciones de uso;
- presentación de proyectos;
- organización de información;
- referencias;
- elementos visuales;
- badges;
- documentación orientada a otros desarrolladores.

Markdown constituye además una oportunidad para introducir una práctica profesional transversal:

> **documentar el trabajo para que otra persona pueda entenderlo, utilizarlo y continuarlo.**

---

## 11. GitHub como espacio de trabajo y no solamente como almacenamiento

GitHub no debe presentarse únicamente como un lugar donde "subir el código".

El estudiante debe comprenderlo como un entorno de colaboración y exposición de proyectos.

Su utilización permite trabajar progresivamente sobre:

- repositorios remotos;
- sincronización;
- colaboración;
- revisión de cambios;
- documentación;
- Pull Requests;
- proyectos compartidos;
- presentación profesional.

Esta perspectiva permite comprender por qué Git y GitHub son herramientas complementarias, pero no equivalentes.

---

## 12. La profundidad es más importante que la cantidad

El curso no pretende enseñar todo Git.

Tampoco pretende recorrer todos los comandos disponibles ni todas las funcionalidades de GitHub.

Existe una diferencia entre:

**conocer que una funcionalidad existe**

y

**ser capaz de utilizar una herramienta fundamental con autonomía.**

El curso priorizará siempre la segunda.

Cuando una funcionalidad no sea necesaria para alcanzar los objetivos formativos principales, podrá ser mencionada y derivada hacia material complementario.

La existencia de material complementario no implica que todo deba ser evaluado ni que todo deba ser explicado durante las instancias de interacción pedagógica.

---

## 13. Trabajo presencial y trabajo autónomo

El aprendizaje del curso se construye mediante la combinación de interacción pedagógica y trabajo autónomo.

Las instancias con el docente deben concentrarse especialmente en aquellos contenidos que requieren:

- demostración;
- acompañamiento;
- interacción;
- resolución de problemas;
- discusión;
- trabajo colaborativo;
- corrección de errores;
- experimentación.

El trabajo autónomo debe utilizarse para:

- repetir procedimientos;
- consolidar conocimientos;
- resolver ejercicios;
- completar desafíos;
- consultar documentación;
- profundizar contenidos;
- avanzar en proyectos;
- explorar funcionalidades complementarias.

Esta distribución permite adaptar el curso a diferentes cargas horarias sin alterar su estructura de contenidos.

---

## 14. El curso completo y sus distintas implementaciones

El curso se concibe como un recorrido completo.

Las distintas implementaciones pueden seleccionar diferentes niveles de profundidad según:

- carga horaria;
- modalidad;
- perfil de los estudiantes;
- objetivos institucionales;
- experiencia previa;
- tiempo disponible para trabajo autónomo.

Una implementación reducida no constituye un curso diferente.

Constituye una **forma diferente de recorrer el mismo curso**.

Por esta razón, el material pedagógico general debe conservar su amplitud, mientras que las guías docentes determinan qué contenidos se priorizan, cuáles se trabajan autónomamente y cuáles quedan como material complementario.

---

## 15. La autonomía como resultado formativo

Una de las metas principales del curso es que el estudiante pueda continuar aprendiendo después de finalizarlo.

Git y GitHub tienen una profundidad que excede ampliamente los contenidos abordados durante cualquier curso introductorio.

Por eso, además de enseñar las herramientas fundamentales, se busca desarrollar la capacidad de:

- consultar documentación;
- interpretar mensajes de Git;
- investigar una funcionalidad desconocida;
- experimentar en un entorno seguro;
- identificar la causa de un problema;
- buscar una solución;
- verificar el resultado.

El curso debe enseñar también **cómo seguir aprendiendo Git**.

---

## 16. La transferencia es el verdadero objetivo

El estudiante no necesita recordar indefinidamente cada comando trabajado durante el curso.

Necesita poder enfrentarse a un proyecto nuevo y reconocer que los problemas son similares.

Un repositorio de programación, un proyecto académico, un trabajo colaborativo o un proyecto personal pueden utilizar tecnologías completamente diferentes y, sin embargo, compartir los mismos problemas:

- registrar cambios;
- conservar versiones;
- trabajar en paralelo;
- compartir avances;
- integrar modificaciones;
- recuperar estados anteriores;
- colaborar con otras personas.

La herramienta puede cambiar.

El modelo de trabajo permanece.

---

## 17. Criterio final

Todo contenido, actividad o recurso del curso debe poder responder afirmativamente a al menos una de estas preguntas:

1. ¿Ayuda a comprender cómo funciona Git?
2. ¿Permite practicar una situación real de trabajo?
3. ¿Desarrolla autonomía?
4. ¿Mejora la capacidad de colaborar?
5. ¿Favorece la documentación y organización de proyectos?
6. ¿Facilita la transferencia hacia proyectos reales?

Si la respuesta es negativa, su incorporación debe ser reconsiderada.

El objetivo no es construir el curso más extenso posible.

El objetivo es construir el **curso que mejor prepare al estudiante para trabajar con Git y GitHub sin dolor y sin depender permanentemente de otra persona para resolver problemas que debería poder resolver por sí mismo**.