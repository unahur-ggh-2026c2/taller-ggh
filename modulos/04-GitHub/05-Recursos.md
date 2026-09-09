# Recursos
## Módulo 04 — GitHub

Los recursos de este módulo están orientados a comprender la relación entre Git y GitHub, trabajar con repositorios remotos y consultar las operaciones básicas de intercambio de cambios.

---

## 1. GitHub

### Sitio oficial

https://github.com/

GitHub es la plataforma que utilizaremos para alojar los repositorios remotos del curso.

Desde el sitio se puede:

- crear repositorios;
- consultar repositorios;
- visualizar archivos;
- consultar commits;
- acceder al historial;
- publicar documentación;
- colaborar sobre proyectos.

---

## 2. Documentación oficial de GitHub

### GitHub Docs

https://docs.github.com/es

La documentación oficial de GitHub está disponible en español.

Puede utilizarse como referencia para consultar:

- repositorios;
- configuración;
- autenticación;
- colaboración;
- GitHub en general;
- características de la plataforma.

No es necesario recorrerla de manera lineal.

Se recomienda utilizarla como material de consulta cuando aparezca una necesidad concreta.

---

## 3. Inicio rápido de GitHub

### Introducción a GitHub

https://docs.github.com/es/get-started/start-your-journey/hello-world

Este recurso presenta un recorrido inicial por GitHub.

Puede resultar útil para familiarizarse con:

- repositorios;
- ramas;
- commits;
- cambios;
- solicitudes de incorporación.

En este módulo nos concentraremos principalmente en repositorios, commits y comunicación con el repositorio remoto.

---

## 4. Git — documentación oficial

### Git

https://git-scm.com/

Sitio oficial del proyecto Git.

Permite acceder a:

- documentación;
- libro Pro Git;
- referencia de comandos;
- información del proyecto.

---

## 5. Pro Git — versión en español

**Chacon, S., & Straub, B. — Pro Git**

Libro de referencia sobre Git, disponible gratuitamente en español:

https://git-scm.com/book/es/v2

Para este módulo resultan especialmente relevantes los contenidos relacionados con:

- repositorios remotos;
- GitHub;
- obtención de cambios;
- envío de cambios;
- trabajo con repositorios remotos.

---

## 6. Repositorios remotos

La documentación oficial de Git permite consultar el funcionamiento de los repositorios remotos:

https://git-scm.com/book/es/v2/Git-en-el-servidor-Git-en-el-servidor

El concepto fundamental es:

```text
Repositorio local
       │
       │ comunicación
       ▼
Repositorio remoto
```

Git permite trabajar con repositorios remotos independientemente de la plataforma concreta que los aloje.

---

## 7. `git remote`

Referencia oficial:

https://git-scm.com/docs/git-remote

Este comando permite administrar los repositorios remotos asociados al repositorio local.

Durante el módulo utilizamos especialmente:

```bash
git remote -v
```

para consultar los remotos configurados.

---

## 8. `git push`

Referencia oficial:

https://git-scm.com/docs/git-push

`git push` permite enviar commits locales hacia un repositorio remoto.

El modelo conceptual trabajado es:

```text
Repositorio local
       │
       │ git push
       ▼
Repositorio remoto
```

Es importante recordar:

> `git push` no crea el commit.

El commit ya existe localmente.

`git push` permite publicar ese historial en el repositorio remoto.

---

## 9. `git pull`

Referencia oficial:

https://git-scm.com/docs/git-pull

`git pull` permite incorporar cambios provenientes de un repositorio remoto.

El modelo simplificado utilizado en este módulo es:

```text
Repositorio remoto
       │
       │ git pull
       ▼
Repositorio local
```

En situaciones de colaboración más complejas pueden aparecer diferentes escenarios de integración. Estos serán trabajados posteriormente.

---

## 10. `git clone`

Como recurso complementario:

https://git-scm.com/docs/git-clone

`git clone` permite crear una copia local de un repositorio existente.

Es especialmente útil cuando:

- comenzamos a trabajar sobre un repositorio que ya existe en GitHub;
- otra persona comparte un proyecto;
- necesitamos obtener localmente un repositorio remoto.

No es necesario profundizar todavía en todas sus opciones.

---

## 11. GitHub y repositorios públicos

Una de las características importantes de GitHub es que los repositorios pueden ser utilizados como espacios públicos de publicación.

Un repositorio público puede permitir que otras personas:

- consulten el proyecto;
- lean la documentación;
- observen el historial;
- estudien el código;
- realicen aportes según la configuración del proyecto.

Esto introduce una dimensión que no existía cuando trabajábamos únicamente con repositorios locales.

---

## 12. README

GitHub utiliza habitualmente `README.md` como documento inicial de presentación de un repositorio.

Referencia:

https://docs.github.com/es/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes

El README puede utilizarse para explicar:

- qué es el proyecto;
- para qué sirve;
- cómo utilizarlo;
- cómo colaborar;
- dónde encontrar información adicional.

El trabajo específico con Markdown será desarrollado posteriormente.

---

## 13. Autenticación

Para trabajar con repositorios remotos pueden ser necesarias credenciales o mecanismos de autenticación.

GitHub ofrece documentación específica:

https://docs.github.com/es/authentication

La autenticación es un aspecto técnico importante, pero no constituye el objetivo central de este módulo.

Si aparece un problema de autenticación durante las prácticas, utilizá la documentación oficial para identificar el mecanismo requerido.

---

## 14. HTTPS y SSH

Los repositorios de GitHub pueden utilizar diferentes mecanismos para establecer la comunicación.

Entre los más habituales se encuentran:

```text
HTTPS
SSH
```

En una primera aproximación alcanza con comprender que la URL utilizada para el remoto determina cómo se establece la conexión.

No es necesario convertir este módulo en un curso de administración de claves SSH.

La configuración específica puede abordarse como material complementario o según las necesidades del entorno de trabajo.

---

## 15. GitHub CLI

Como recurso complementario existe:

### GitHub CLI

https://cli.github.com/

GitHub CLI permite trabajar con GitHub desde la línea de comandos.

Puede utilizarse para:

- crear repositorios;
- consultar repositorios;
- administrar diferentes recursos de GitHub;
- automatizar tareas.

No es necesario utilizar GitHub CLI para completar este módulo.

La actividad principal se realizará utilizando Git y la interfaz web de GitHub.

---

## 16. GitHub en Visual Studio Code

Visual Studio Code ofrece integración con Git y herramientas adicionales para trabajar con repositorios.

Documentación:

https://code.visualstudio.com/docs/sourcecontrol/overview

Estas herramientas pueden resultar útiles para:

- consultar cambios;
- realizar commits;
- consultar ramas;
- administrar repositorios;
- visualizar información relacionada con Git.

Durante el curso se recomienda comprender primero las operaciones mediante Git y utilizar la interfaz gráfica como complemento.

---

## 17. Flujo de trabajo de referencia

El modelo básico trabajado durante el módulo puede resumirse así:

```text
             REPOSITORIO LOCAL
                    │
                    │
             git commit
                    │
                    ▼
              HISTORIAL LOCAL
                    │
                    │ git push
                    ▼
             REPOSITORIO REMOTO
                    │
                    ▼
                 GITHUB
```

En sentido inverso:

```text
                 GITHUB
                    │
                    ▼
             REPOSITORIO REMOTO
                    │
                    │ git pull
                    ▼
             REPOSITORIO LOCAL
```

---

## 18. Mapa conceptual

```text
Git
│
├── Repositorio local
│   ├── cambios
│   ├── preparación
│   └── commits
│
└── Repositorio remoto
    │
    └── GitHub
        ├── repositorios
        ├── documentación
        └── colaboración
```

Entre ambos repositorios:

```text
LOCAL ── git push ──→ REMOTO
LOCAL ←─ git pull ─── REMOTO
```

---

## 19. Recursos para profundizar

Una vez dominado el recorrido básico, se puede investigar:

- múltiples repositorios remotos;
- `git fetch`;
- diferencias entre `git fetch` y `git pull`;
- autenticación mediante SSH;
- GitHub CLI;
- configuración de repositorios;
- repositorios públicos y privados;
- permisos;
- colaboradores;
- GitHub Pages;
- GitHub Actions.

Estos temas amplían el uso de Git y GitHub, pero no son necesarios para completar el recorrido principal del módulo.

---

## 20. Qué conviene recordar

Si necesitás conservar solamente las referencias esenciales del módulo:

1. **GitHub**  
   https://github.com/

2. **GitHub Docs en español**  
   https://docs.github.com/es

3. **Pro Git en español**  
   https://git-scm.com/book/es/v2

4. **`git remote`**  
   https://git-scm.com/docs/git-remote

5. **`git push`**  
   https://git-scm.com/docs/git-push

6. **`git pull`**  
   https://git-scm.com/docs/git-pull

7. **`git clone`**  
   https://git-scm.com/docs/git-clone

---

## 21. Estrategia de consulta

Ante un problema con GitHub, no intentes memorizar soluciones aisladas.

Primero determiná:

```text
¿Qué quiero hacer?
        ↓
¿Dónde está actualmente el cambio?
        ↓
¿Repositorio local o remoto?
        ↓
¿Qué operación necesito?
        ↓
¿Qué documentación corresponde consultar?
```

La documentación oficial debe ser una herramienta habitual de trabajo.

Aprender a buscar y comprender la documentación forma parte de las competencias que se pretende desarrollar durante el curso.

---

> **GitHub no reemplaza a Git. Es el entorno remoto que nos permite compartir repositorios Git y construir sobre ellos nuevas formas de trabajo.**