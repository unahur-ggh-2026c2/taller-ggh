# Recursos
## Módulo 08 — Perfil Profesional

Este documento reúne recursos para profundizar los contenidos trabajados durante el módulo.

La propuesta es utilizarlos como material de consulta y no como una lista obligatoria de lecturas.

---

# 1. Git

La documentación oficial de Git continúa siendo una referencia fundamental para comprender el funcionamiento del control de versiones.

https://git-scm.com/docs

En este módulo resulta especialmente útil para revisar:

```text
repositorios
commits
ramas
historial
.gitignore
```

---

# 2. Pro Git

El libro **Pro Git** ofrece una referencia más extensa sobre Git.

https://git-scm.com/book/es/v2

Puede utilizarse para profundizar en:

- fundamentos de Git;
- ramas;
- repositorios remotos;
- flujos de trabajo;
- colaboración.

No es necesario leerlo completo para trabajar con el módulo.

---

# 3. GitHub Docs

La documentación oficial de GitHub es la referencia principal para las funcionalidades utilizadas durante el curso.

https://docs.github.com/es

En particular:

```text
repositorios
perfiles
Issues
Pull Requests
ramas
colaboración
```

---

# 4. GitHub — Tu perfil

GitHub permite personalizar el perfil público mediante información profesional y repositorios destacados.

https://docs.github.com/es/account-and-profile/setting-up-and-managing-your-github-profile

Este recurso permite consultar las posibilidades actuales de configuración del perfil.

---

# 5. README de perfil

GitHub permite crear un repositorio especial cuyo README puede aparecer directamente en el perfil.

https://docs.github.com/es/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile

Este mecanismo puede utilizarse para presentar:

```text
presentación
intereses
proyectos
tecnologías
enlaces
```

Debe utilizarse como complemento de los proyectos, no como sustituto de ellos.

---

# 6. Repositorios destacados

GitHub permite seleccionar repositorios para destacarlos en el perfil.

La documentación sobre personalización del perfil:

https://docs.github.com/es/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile

puede consultarse para conocer las opciones disponibles.

La selección debería responder a una pregunta:

> ¿Qué proyectos representan mejor mi trabajo actual?

---

# 7. GitHub — README

GitHub muestra archivos `README.md` en los repositorios y utiliza Markdown para estructurar su contenido.

https://docs.github.com/es/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes

El README debería funcionar como puerta de entrada al proyecto.

---

# 8. Markdown

GitHub proporciona una referencia específica sobre Markdown:

https://docs.github.com/es/get-started/writing-on-github

Puede utilizarse para profundizar en:

- títulos;
- listas;
- enlaces;
- tablas;
- código;
- imágenes;
- organización documental.

---

# 9. GitHub Flavored Markdown

GitHub utiliza una variante de Markdown con funcionalidades adicionales.

https://github.github.com/gfm/

Es especialmente útil cuando se desea comprender con mayor precisión cómo GitHub interpreta determinados elementos de Markdown.

---

# 10. `.gitignore`

La documentación oficial de Git sobre `.gitignore`:

https://git-scm.com/docs/gitignore

explica cómo indicar archivos que Git debe ignorar.

Puede utilizarse para evitar incorporar:

```text
archivos temporales
archivos generados
configuraciones locales
entornos
```

La configuración concreta depende del proyecto.

---

# 11. Plantillas de `.gitignore`

GitHub mantiene una colección de plantillas de `.gitignore` para distintos lenguajes y herramientas.

https://github.com/github/gitignore

Pueden utilizarse como referencia al iniciar un proyecto.

No conviene copiar una plantilla completa sin analizarla.

La pregunta debería ser:

> ¿Qué archivos genera realmente mi proyecto y cuáles no deberían versionarse?

---

# 12. Seguridad en GitHub

GitHub proporciona documentación específica sobre seguridad.

https://docs.github.com/es/code-security

Puede utilizarse para profundizar en:

- secretos;
- dependencias;
- seguridad del repositorio;
- alertas;
- buenas prácticas.

En este módulo interesa especialmente comprender que un repositorio público requiere revisar qué información contiene.

---

# 13. Secretos

GitHub documenta específicamente el manejo de secretos.

https://docs.github.com/es/code-security/secret-scanning/introduction/about-secret-scanning

La idea fundamental es:

```text
secreto
   ↓
no debería quedar expuesto
```

Un secreto publicado accidentalmente debe tratarse como comprometido.

Agregar posteriormente el archivo a `.gitignore` no elimina automáticamente el secreto del historial.

---

# 14. GitHub Secret Scanning

GitHub puede detectar determinados secretos expuestos en repositorios.

https://docs.github.com/es/code-security/secret-scanning

Esta funcionalidad puede servir como una capa adicional de protección.

No reemplaza:

```text
criterio
revisión
prevención
```

La responsabilidad principal sigue siendo evitar publicar secretos.

---

# 15. GitHub — Seguridad de repositorios

La documentación de seguridad de GitHub permite conocer herramientas disponibles para proteger repositorios.

https://docs.github.com/es/code-security

No todas las funcionalidades son necesarias para un proyecto pequeño.

El objetivo del módulo es comprender primero los principios básicos.

---

# 16. GitHub — Contribuciones

Las contribuciones permiten observar parte de la actividad desarrollada en GitHub.

https://docs.github.com/es/account-and-profile/setting-up-and-managing-your-github-profile/viewing-contributions-on-your-profile

Las contribuciones pueden incluir diferentes tipos de actividad.

Sin embargo:

```text
actividad ≠ experiencia
```

No debería perseguirse actividad artificial solamente para mejorar la apariencia del perfil.

---

# 17. GitHub — Contribuir a proyectos

La documentación de GitHub sobre colaboración permite profundizar en diferentes formas de contribuir.

https://docs.github.com/es/get-started/exploring-projects-on-github/contributing-to-projects

Puede resultar útil para comprender cómo una persona puede comenzar a participar en proyectos de otras personas.

---

# 18. GitHub Skills

GitHub ofrece ejercicios prácticos mediante GitHub Skills.

https://skills.github.com/

Es un recurso útil para continuar practicando:

```text
GitHub
Issues
Pull Requests
colaboración
workflows
```

Puede utilizarse como continuación del curso.

---

# 19. GitHub Community

GitHub dispone de recursos para construir comunidades y proyectos saludables.

https://docs.github.com/es/communities

Puede resultar útil para profundizar en:

- colaboración;
- documentación;
- reglas;
- participación;
- contribuciones.

---

# 20. CONTRIBUTING.md

GitHub documenta distintas formas de establecer pautas para colaboradores.

https://docs.github.com/es/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors

El archivo:

```text
CONTRIBUTING.md
```

puede utilizarse para explicar:

```text
cómo contribuir
cómo crear Issues
cómo trabajar con ramas
cómo abrir Pull Requests
qué convenciones seguir
```

---

# 21. CODE_OF_CONDUCT.md

GitHub también proporciona documentación sobre códigos de conducta.

https://docs.github.com/es/communities/setting-up-your-project-for-healthy-contributions/adding-a-code-of-conduct-to-your-project

Este recurso puede utilizarse cuando un proyecto tenga una comunidad o equipo que necesite establecer pautas de participación.

No es un requisito técnico de Git.

---

# 22. GitHub Pages

GitHub Pages permite publicar sitios directamente desde determinados repositorios.

https://pages.github.com/

Puede ser una alternativa para construir una página sencilla de:

```text
portafolio
documentación
proyecto
sitio personal
```

No es necesario utilizar GitHub Pages para completar el módulo.

Es un recurso de profundización.

---

# 23. GitHub Pages — Documentación

La documentación oficial permite conocer las diferentes posibilidades de publicación.

https://docs.github.com/es/pages

Puede utilizarse como punto de partida para construir un portafolio web.

---

# 24. GitHub Discussions

GitHub permite utilizar Discussions para determinados proyectos.

https://docs.github.com/es/discussions

Puede ser útil cuando un proyecto necesita un espacio para:

```text
preguntas
ideas
debates
anuncios
```

No debe confundirse con Issues.

De manera simplificada:

```text
Issue
 ↓
trabajo concreto

Discussion
 ↓
conversación
```

---

# 25. GitHub Issues

Las Issues continúan siendo relevantes para construir evidencia del proceso.

https://docs.github.com/es/issues

Una Issue bien redactada puede mostrar:

```text
problema
objetivo
resultado esperado
```

Esto puede resultar útil tanto para organizar el trabajo como para documentar decisiones.

---

# 26. Pull Requests

La documentación oficial:

https://docs.github.com/es/pull-requests

permite profundizar en:

```text
propuestas de cambios
revisión
comentarios
integración
```

Las Pull Requests pueden aportar evidencia sobre cómo se trabaja colaborativamente.

---

# 27. Revisiones

GitHub documenta el proceso de revisión de Pull Requests.

https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests

Una revisión puede:

```text
aprobar
comentar
solicitar cambios
```

El valor de la revisión está en el feedback que permite mejorar el trabajo.

---

# 28. Conflictos

La documentación de GitHub sobre conflictos puede consultarse en:

https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts

Los conflictos permiten observar una situación importante:

```text
Git puede detectar el conflicto.
La decisión sobre el contenido corresponde a las personas.
```

---

# 29. Pro Git — Ramas

Para profundizar en ramas y desarrollo paralelo:

https://git-scm.com/book/es/v2/Ramificaciones-en-Git-Ramificaciones-en-Git

Este contenido conecta directamente con el trabajo realizado en los módulos anteriores.

---

# 30. Git Log

Documentación oficial:

https://git-scm.com/docs/git-log

Para analizar proyectos:

```bash
git log --oneline --graph --all
```

es especialmente útil.

Permite reconstruir la evolución del repositorio.

---

# 31. GitHub — Perfil como evidencia

La documentación sobre perfiles puede servir para estudiar qué información puede mostrarse públicamente.

https://docs.github.com/es/account-and-profile

La idea del módulo no es maximizar la cantidad de información.

Es seleccionar aquella que aporte contexto y evidencia.

---

# 32. Portafolio técnico

No existe una única estructura correcta para un portafolio.

Puede estar compuesto por:

```text
GitHub
README
proyectos
documentación
sitio web
CV
```

La selección depende del perfil y del objetivo.

Lo importante es que los elementos sean coherentes entre sí.

---

# 33. Documentación técnica

Un proyecto técnico puede necesitar diferentes tipos de documentación.

Por ejemplo:

```text
README
CONTRIBUTING
CODE_OF_CONDUCT
docs/
```

No todos los proyectos necesitan todos estos elementos.

La documentación debe responder a necesidades reales.

---

# 34. Recursos para profundizar en Git

### Documentación oficial

https://git-scm.com/docs

### Pro Git

https://git-scm.com/book/es/v2

### Git Reference

https://git-scm.com/docs

Estos recursos deben ser considerados referencias de consulta.

---

# 35. Recursos para profundizar en GitHub

### GitHub Docs

https://docs.github.com/es

### GitHub Skills

https://skills.github.com/

### GitHub Community

https://docs.github.com/es/communities

Estos recursos permiten continuar aprendiendo después del curso.

---

# 36. Recursos para documentación

### GitHub Docs — Writing on GitHub

https://docs.github.com/es/get-started/writing-on-github

### GitHub Flavored Markdown

https://github.github.com/gfm/

### README

https://docs.github.com/es/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes

---

# 37. Recursos para seguridad

### GitHub Code Security

https://docs.github.com/es/code-security

### Secret Scanning

https://docs.github.com/es/code-security/secret-scanning

### `.gitignore`

https://git-scm.com/docs/gitignore

La combinación de:

```text
prevención
+
revisión
+
herramientas
```

es más importante que depender de una única herramienta.

---

# 38. Recursos para continuar practicando

Si querés continuar después del curso:

```text
GitHub Skills
       ↓
ejercicios prácticos

Pro Git
       ↓
profundización conceptual

GitHub Docs
       ↓
consulta funcional

Git Docs
       ↓
referencia de comandos
```

La recomendación es volver a estos recursos cuando aparezca una necesidad concreta.

---

# 39. Cómo utilizar la documentación

No intentes memorizar todas las funcionalidades.

Utilizá la documentación como parte del trabajo.

El flujo recomendado es:

```text
necesidad
   ↓
identificar concepto
   ↓
buscar documentación
   ↓
leer
   ↓
probar
   ↓
verificar
```

Esta capacidad es parte de la formación técnica.

---

# 40. Recursos fundamentales del módulo

Si solamente vas a conservar algunos enlaces, priorizá:

### Git

:contentReference[oaicite:0]{index=0}

### Pro Git

:contentReference[oaicite:1]{index=1}

### GitHub Docs

:contentReference[oaicite:2]{index=2}

### GitHub Skills

:contentReference[oaicite:3]{index=3}

### GitHub Security

:contentReference[oaicite:4]{index=4}

---

# 41. Qué consultar según la necesidad

| Necesidad | Recurso |
|---|---|
| Git | Git Docs |
| Conceptos de Git | Pro Git |
| GitHub | GitHub Docs |
| Perfil | GitHub Profile Docs |
| README | GitHub README Docs |
| Markdown | GitHub Markdown Docs |
| `.gitignore` | Git Docs |
| Secretos | GitHub Code Security |
| Pull Requests | GitHub Docs |
| Issues | GitHub Docs |
| Colaboración | GitHub Community |
| Práctica | GitHub Skills |
| Portafolio web | GitHub Pages |

---

# 42. Criterio para seleccionar recursos

No todo recurso que aparece en Internet tiene el mismo valor.

Para contenidos técnicos conviene priorizar:

```text
documentación oficial
      ↓
fuentes reconocidas
      ↓
material especializado
      ↓
experiencias de terceros
```

Los tutoriales externos pueden ser útiles.

Pero ante una duda sobre el comportamiento de Git o GitHub, la documentación oficial debería ser el punto de referencia.

---

# 43. Cierre

El objetivo de estos recursos no es que memorices GitHub.

El objetivo es que puedas seguir aprendiendo de manera autónoma.

La competencia importante es:

```text
no sé
 ↓
sé qué necesito averiguar
 ↓
sé dónde buscar
 ↓
sé cómo probarlo
 ↓
sé cómo verificarlo
```

Eso también forma parte del perfil profesional.

> **Un buen profesional no es quien recuerda todos los comandos. Es quien sabe encontrar la información correcta y utilizarla con criterio.**