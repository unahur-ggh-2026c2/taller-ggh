# Recursos
## Módulo 01 — Mi primer repositorio

Los recursos de este módulo están orientados a acompañar la creación y exploración de repositorios Git.

La documentación debe utilizarse principalmente como material de consulta. No es necesario leerla completa antes de realizar las prácticas.

---

## 1. Git — sitio oficial

### Git

Sitio oficial del proyecto Git.

https://git-scm.com/

Desde este sitio se puede consultar:

- información general sobre Git;
- documentación;
- instalación;
- referencias de comandos;
- enlaces a otros recursos del proyecto.

---

## 2. Pro Git

**Chacon, S., & Straub, B. — Pro Git**

Libro de referencia sobre Git, disponible gratuitamente en línea.

### Versión en español

https://git-scm.com/book/es/v2

Para este módulo resultan especialmente útiles los contenidos relacionados con:

- primeros pasos con Git;
- configuración inicial;
- creación de repositorios;
- obtención de información sobre el estado del repositorio.

No es necesario avanzar por todo el libro de manera lineal.

Utilizalo como material de consulta cuando necesites comprender con mayor profundidad algún concepto.

---

## 3. Referencia de comandos de Git

La documentación oficial incluye una referencia completa de los comandos disponibles en Git.

https://git-scm.com/docs

Durante el curso no es necesario memorizar todos los comandos.

La capacidad importante es aprender a:

1. identificar qué problema necesitás resolver;
2. consultar la documentación;
3. interpretar las opciones disponibles;
4. probar de manera controlada;
5. verificar el resultado.

---

## 4. `git init`

Documentación oficial:

https://git-scm.com/docs/git-init

`git init` permite crear un nuevo repositorio Git en una carpeta existente.

En este módulo se utiliza para comprender la transformación:

```text
carpeta común
     ↓
git init
     ↓
repositorio Git
```

---

## 5. `git status`

Documentación oficial:

https://git-scm.com/docs/git-status

`git status` permite consultar el estado actual del repositorio.

Durante el curso será una de las herramientas de observación más utilizadas.

Es recomendable acostumbrarse a consultar el estado antes y después de realizar operaciones importantes.

---

## 6. `git add`

Documentación oficial:

https://git-scm.com/docs/git-add

`git add` permite incorporar cambios al área de preparación.

Este concepto será trabajado con mayor profundidad en el módulo 02.

Por ahora, utilizalo para comenzar a comprender que existe una etapa intermedia entre:

```text
modificar un archivo
        ↓
registrar un commit
```

---

## 7. `git commit`

Documentación oficial:

https://git-scm.com/docs/git-commit

`git commit` registra en el historial los cambios que fueron preparados.

El mensaje del commit debe permitir comprender qué cambio se registró.

---

## 8. `git log`

Documentación oficial:

https://git-scm.com/docs/git-log

`git log` permite consultar el historial de commits.

En este módulo se utiliza para comenzar a observar:

- commits;
- autores;
- fechas;
- mensajes;
- identificadores.

El historial será trabajado con mayor profundidad en el módulo 03.

---

## 9. Visual Studio Code

### Documentación de control de versiones

Visual Studio Code incorpora herramientas para trabajar con sistemas de control de versiones.

https://code.visualstudio.com/docs/sourcecontrol/overview

Estas herramientas pueden utilizarse como complemento de la terminal.

Durante el curso se recomienda conocer ambas formas de interacción:

```text
Visual Studio Code
        +
Terminal
        +
Git
```

El objetivo no es depender de una interfaz gráfica, sino comprender qué operaciones estamos realizando.

---

## 10. Recursos del repositorio

El directorio:

```text
recursos/
```

contiene materiales adicionales para acompañar las actividades del curso.

Dentro de él se encuentran:

```text
recursos/
├── imagenes/
├── plantillas/
├── cheatsheets/
└── ejemplos/
```

Estos recursos podrán ampliarse a medida que el curso evolucione.

---

## 11. Comandos trabajados en el módulo

Como referencia rápida:

| Comando | Propósito |
|---|---|
| `git --version` | Consultar la versión instalada de Git |
| `git config` | Configurar Git |
| `git init` | Inicializar un repositorio |
| `git status` | Consultar el estado |
| `git add` | Preparar cambios |
| `git commit` | Registrar cambios |
| `git log` | Consultar el historial |

No se espera que memorices esta tabla.

Lo importante es comprender **cuándo y por qué utilizar cada herramienta**.

---

## 12. Para investigar por cuenta propia

Una vez completadas las actividades del módulo, podés investigar:

- `git config`;
- configuración local y global;
- opciones de `git status`;
- opciones de `git log`;
- alias de Git;
- archivos `.git`;
- estructura interna de un repositorio.

Estos temas no son necesarios para completar el recorrido principal del módulo.

El objetivo es comenzar a desarrollar el hábito de investigar funcionalidades que todavía no conocemos.

---

## 13. Una buena práctica

Cuando no sepas qué hace un comando, no te limites a copiar una solución encontrada en Internet.

Intentá seguir este recorrido:

```text
¿Qué quiero hacer?
        ↓
¿Qué comando podría resolverlo?
        ↓
Consultar documentación
        ↓
Probar en un repositorio de práctica
        ↓
Observar el resultado
        ↓
Verificar que realmente ocurrió lo esperado
```

Esta forma de trabajar será cada vez más importante a medida que avancemos hacia situaciones más complejas.

---

## 14. Recurso principal del módulo

Si tuvieras que conservar solamente tres referencias para este módulo, deberían ser:

1. **Git — sitio oficial**
   https://git-scm.com/

2. **Pro Git — versión en español**
   https://git-scm.com/book/es/v2

3. **Documentación oficial de Git**
   https://git-scm.com/docs

El resto de los recursos funciona como material complementario.