# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

### 5.1.1. Software Development Environment Configuration

En esta sección se detallan las herramientas, frameworks y plataformas utilizadas por el equipo para el desarrollo colaborativo durante todo el ciclo de vida del producto digital. Se han considerado actividades de Project Management, Requirements Management, UX/UI Design, Software Development, Documentation y Deployment.

**Project Management**

<table>
  <thead>
    <tr>
      <th>Producto</th>
      <th>Propósito de uso</th>
      <th>Ruta de Referencia / Descarga</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Jira</strong></td>
      <td>Herramienta principal para la gestión del proyecto, administración del Product Backlog y seguimiento de Sprints bajo metodología ágil.</td>
      <td><a href="https://www.atlassian.com/software/jira">https://www.atlassian.com/software/jira</a></td>
    </tr>
  </tbody>
</table>

**Requirements Management**

<table>
  <thead>
    <tr>
      <th>Producto</th>
      <th>Propósito de uso</th>
      <th>Ruta de Referencia / Descarga</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>UXPressia</strong></td>
      <td>Utilizado para la gestión de requerimientos, específicamente para la creación de User Personas, Empathy Maps e Impact Maps.</td>
      <td><a href="https://uxpressia.com/">https://uxpressia.com/</a></td>
    </tr>
  </tbody>
</table>

**Product UX/UI Design**

<table>
  <thead>
    <tr>
      <th>Producto</th>
      <th>Propósito de uso</th>
      <th>Ruta de Referencia / Descarga</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Figma</strong></td>
      <td>Herramienta de diseño UX/UI para la elaboración de Wireframes, Mock-ups y Prototipos interactivos.</td>
      <td><a href="https://www.figma.com/">https://www.figma.com/</a></td>
    </tr>
    <tr>
      <td><strong>Miro</strong></td>
      <td>Plataforma de colaboración visual empleada en las sesiones de EventStorming (Big Picture y Design-Level) para el modelado del dominio.</td>
      <td><a href="https://miro.com/">https://miro.com/</a></td>
    </tr>
  </tbody>
</table>

**Software Development**

<table>
  <thead>
    <tr>
      <th>Producto</th>
      <th>Propósito de uso</th>
      <th>Ruta de Referencia / Descarga</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Structurizr</strong></td>
      <td>Herramienta para el diseño y documentación de la arquitectura de software siguiendo el modelo C4 (Context, Container, Component, Code).</td>
      <td><a href="https://structurizr.com/">https://structurizr.com/</a></td>
    </tr>
    <tr>
      <td><strong>MySQL Workbench</strong></td>
      <td>Utilizado para el diseño de base de datos, permitiendo la creación de diagramas entidad-relación y la gestión de la persistencia de datos.</td>
      <td><a href="https://www.mysql.com/products/workbench/">https://www.mysql.com/products/workbench/</a></td>
    </tr>
    <tr>
      <td><strong>Visual Studio Code</strong></td>
      <td>Entorno de desarrollo (IDE) principal para la implementación de la Landing Page y la aplicación Frontend.</td>
      <td><a href="https://code.visualstudio.com/">https://code.visualstudio.com/</a></td>
    </tr>
    <tr>
      <td><strong>GitHub Desktop</strong></td>
      <td>Cliente de Git utilizado para facilitar el Source Code Management y la implementación del flujo de trabajo GitFlow en el equipo.</td>
      <td><a href="https://desktop.github.com/">https://desktop.github.com/</a></td>
    </tr>
    <tr>
      <td><strong>ASP.NET Core / C#</strong></td>
      <td>Framework y lenguaje principal para el desarrollo de los RESTful Web Services que conforman el Backend de la aplicación, siguiendo la arquitectura, el estilo de codificación y la organización por bounded context del proyecto de referencia <strong>learning-center-platform</strong>.</td>
      <td><a href="https://dotnet.microsoft.com/apps/aspnet">https://dotnet.microsoft.com/apps/aspnet</a></td>
    </tr>
    <tr>
      <td><strong>.NET SDK</strong></td>
      <td>Kit de desarrollo requerido para compilar, ejecutar y publicar el proyecto de Web Services en C#, junto con Entity Framework Core para la capa de persistencia.</td>
      <td><a href="https://dotnet.microsoft.com/download">https://dotnet.microsoft.com/download</a></td>
    </tr>
    <tr>
      <td><strong>Vue 3 / JavaScript</strong></td>
      <td>Framework y lenguaje utilizados para la construcción de la Frontend Web Application de la plataforma, empleando Single File Components y JavaScript como lenguaje de programación.</td>
      <td><a href="https://vuejs.org/">https://vuejs.org/</a></td>
    </tr>
    <tr>
      <td><strong>PrimeVue</strong></td>
      <td>Biblioteca de componentes de UI para Vue basada en Material Design, utilizada para construir las vistas del dashboard de forma consistente con el Design System.</td>
      <td><a href="https://primevue.org/">https://primevue.org/</a></td>
    </tr>
    <tr>
      <td><strong>Node.js / Vite</strong></td>
      <td>Entorno de ejecución JavaScript y herramienta de build requeridos para ejecutar el servidor de desarrollo de Vue, gestionar dependencias y generar el bundle de producción del Frontend.</td>
      <td><a href="https://nodejs.org/">https://nodejs.org/</a></td>
    </tr>
    <tr>
      <td><strong>Pinia</strong></td>
      <td>Biblioteca oficial de gestión de estado para Vue, utilizada para centralizar el estado compartido entre bounded contexts del Frontend mediante stores por dominio.</td>
      <td><a href="https://pinia.vuejs.org/">https://pinia.vuejs.org/</a></td>
    </tr>
    <tr>
      <td><strong>Tailwind CSS</strong></td>
      <td>Framework CSS utility-first empleado para el estilo del Landing Page, compilando <code>src/input.css</code> hacia <code>styles.css</code> mediante su CLI.</td>
      <td><a href="https://tailwindcss.com/">https://tailwindcss.com/</a></td>
    </tr>
    <tr>
      <td><strong>Docker</strong></td>
      <td>Plataforma de containerización utilizada para empaquetar el RESTful Web Services (ASP.NET Core) en una imagen reproducible, construida con Cloud Build, publicada en Google Artifact Registry y desplegada en Google Cloud Run.</td>
      <td><a href="https://www.docker.com/">https://www.docker.com/</a></td>
    </tr>
  </tbody>
</table>

**Software Documentation**

<table>
  <thead>
    <tr>
      <th>Producto</th>
      <th>Propósito de uso</th>
      <th>Ruta de Referencia / Descarga</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Swagger / OpenAPI</strong></td>
      <td>Empleado para la documentación técnica de los endpoints del RESTful API, permitiendo su exploración y prueba interactiva.</td>
      <td><a href="https://swagger.io/">https://swagger.io/</a></td>
    </tr>
    <tr>
      <td><strong>Markdown</strong></td>
      <td>Lenguaje de marcado utilizado para la elaboración y mantenimiento de la documentación general del proyecto alojada en GitHub.</td>
      <td><a href="https://www.markdownguide.org/">https://www.markdownguide.org/</a></td>
    </tr>
  </tbody>
</table>

**Software Deployment**

<table>
  <thead>
    <tr>
      <th>Producto</th>
      <th>Propósito de uso</th>
      <th>Ruta de Referencia / Descarga</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Google Cloud Platform</strong></td>
      <td>Proveedor de infraestructura cloud utilizado para el despliegue y hospedaje de los servicios Backend y aplicaciones en producción.</td>
      <td><a href="https://cloud.google.com/">https://cloud.google.com/</a></td>
    </tr>
    <tr>
      <td><strong>GitHub Pages</strong></td>
      <td>Servicio de hosting estático utilizado para el despliegue continuo de la Landing Page del producto.</td>
      <td><a href="https://pages.github.com/">https://pages.github.com/</a></td>
    </tr>
  </tbody>
</table>

### 5.1.2. Source Code Management

Para la gestión del código fuente y el seguimiento de modificaciones, el equipo utiliza GitHub como plataforma principal y Git como sistema de control de versiones distribuido. Se han establecido repositorios independientes para cada producto de la solución, asegurando que el repositorio de Web Services incluya tanto el proyecto como los archivos de pruebas unitarias, de integración y de aceptación.

**Repositorios del Proyecto**

| Producto                     | URL del Repositorio                                     |
| :--------------------------- | :------------------------------------------------------ |
| **Landing Page**             | https://github.com/Kauflink/ap-entreprenly-landing      |
| **Web Services**             | https://github.com/Kauflink/ap-entreprenly-web-services |
| **Frontend Web Application** | https://github.com/Kauflink/ap-entreprenly-frontend     |

**Estrategia de Flujo de Trabajo: GitFlow**

El equipo implementa el modelo GitFlow como workflow de control de versiones para organizar el desarrollo colaborativo de forma estructurada. Este flujo permite trabajar en múltiples funcionalidades en paralelo sin afectar la estabilidad de la rama principal.

Se han definido las siguientes ramas fundamentales:

- **main**: Es la rama principal que contiene el código fuente en estado de producción. Cada versión integrada aquí debe estar etiquetada con un número de versión.

- **develop**: Rama base para el desarrollo donde se integran todas las funcionalidades completadas para pruebas antes de un lanzamiento.

- **feature**: Ramas temporales creadas para desarrollar nuevas funcionalidades o historias de usuario específicas.

- **release**: Ramas utilizadas para preparar un nuevo lanzamiento oficial, permitiendo realizar ajustes menores y correcciones de errores finales.

- **hotfix**: Ramas de emergencia creadas directamente desde main para solucionar errores críticos detectados en el entorno de producción.

**Convenciones de Nombres para Ramas**

Para mantener la trazabilidad y el orden en los repositorios, se aplican las siguientes convenciones de nomenclatura:

- **Feature Branches**: feature/US-[ID-Historia]-[Nombre]
- **Release Branches**: release/v[Major.Minor.Patch]
- **Hotfix Branches**: hotfix/[Descripcion-Error]

**Versionamiento Semántico**

El equipo adopta el estándar Semantic Versioning 2.0.0 para el nombramiento de los lanzamientos. Las versiones se estructuran siguiendo el formato MAJOR.MINOR.PATCH:

1. MAJOR: Incrementado cuando se realizan cambios incompatibles en la API.
2. MINOR: Incrementado cuando se añade funcionalidad de manera retrocompatible.
3. PATCH: Incrementado cuando se realizan correcciones de errores retrocompatibles.

**Estándar de Mensajes de Commit**

Para asegurar un historial de cambios legible y facilitar la automatización, se utiliza la especificación de Conventional Commits para todos los mensajes de commit. La estructura utilizada es [tipo]:[descripción breve], empleando los siguientes prefijos:

- feat: Incorporación de una nueva funcionalidad.
- fix: Corrección de un error o bug.
- docs: Modificaciones exclusivamente en la documentación.
- style: Cambios de formato o estética que no afectan la lógica del código.
- refactor: Reestructuración de código que no añade funciones ni corrige errores.
- test: Adición o actualización de pruebas

### 5.1.3. Source Code Style Guide & Conventions

En esta sección se establecen las guías de estilo y convenciones de codificación adoptadas por el equipo de Kauflink para el desarrollo de los productos digitales que conforman la solución **Entreprenly**. El objetivo es garantizar que el código fuente sea legible, mantenible y coherente entre todos los miembros del equipo, independientemente del componente o capa de la arquitectura en la que se trabaje. Como regla general, **toda nomenclatura de elementos en el código fuente se redacta en inglés**, incluyendo nombres de variables, clases, métodos, componentes, atributos y comentarios técnicos.

Las referencias adoptadas para cada lenguaje y tecnología utilizada en la solución se detallan a continuación.

#### HTML

Para el desarrollo del Landing Page de Entreprenly, el equipo adopta como referencia principal la **HTML Style Guide and Coding Conventions** de W3Schools y la **Google HTML/CSS Style Guide**.

Las convenciones aplicadas son las siguientes:

- Se utiliza **HTML5** como estándar de marcado, declarando siempre el `DOCTYPE` al inicio del documento: `<!DOCTYPE html>`.
- Los nombres de los elementos y atributos se escriben en **minúsculas** (`<section>`, `<article>`, `class="hero-section"`).
- Los atributos se encierran siempre entre **comillas dobles**: `<img src="logo.png" alt="Entreprenly logo">`.
- Se incluyen los atributos `lang` en la etiqueta `<html>` para indicar el idioma de la página: `<html lang="en">`.
- Todas las imágenes incluyen el atributo `alt` con una descripción significativa, como parte del enfoque de accesibilidad (a11y) del proyecto.
- Se utiliza **indentación de 2 espacios** para mantener la legibilidad del árbol de elementos.
- Los elementos de bloque se escriben en líneas separadas; los elementos en línea pueden mantenerse en una misma línea si el resultado es conciso.
- Se evita el uso de estilos en línea (`style=""`); el estilo visual se aplica mediante **clases utilitarias de Tailwind CSS** directamente en el marcado.
- Los comentarios se utilizan para delimitar secciones principales del documento: `<!-- Hero Section -->`.

#### CSS

Para el estilo visual del Landing Page de Entreprenly, el equipo utiliza **Tailwind CSS** (enfoque utility-first), tomando como referencia complementaria la **Google HTML/CSS Style Guide**. Las hojas de estilo finales se generan a partir de un archivo fuente (`src/input.css`) compilado con la CLI de Tailwind hacia `styles.css`.

Las convenciones aplicadas son las siguientes:

- El estilo se compone aplicando **clases utilitarias de Tailwind** sobre los elementos HTML (p. ej. `flex`, `gap-4`, `text-center`, `rounded-lg`), en lugar de escribir reglas CSS personalizadas para cada componente.
- La generación de la hoja de estilos se realiza con la CLI de Tailwind: `tailwindcss -i ./src/input.css -o ./styles.css` (con `--watch` en desarrollo y `--minify` para producción, según los scripts `dev` y `build` de `package.json`).
- Los **tokens del Design System** (colores de marca, tipografía, espaciado) se centralizan en la configuración/capa de tema de Tailwind, garantizando consistencia con los demás productos digitales.
- La tipografía principal es **Reddit Sans**, cargada desde Google Fonts.
- El soporte de **tema claro/oscuro** se gestiona mediante las variantes de Tailwind y un script (`app.js`) que alterna la clase de tema en la raíz del documento.
- Las clases personalizadas residuales, cuando se requieren, se escriben en **kebab-case** dentro de `src/input.css` usando las directivas de Tailwind (`@layer`, `@apply`).

#### JavaScript

El Landing Page de Entreprenly utiliza JavaScript para comportamientos de interacción básicos. El equipo adopta las convenciones establecidas en la **Google HTML/CSS Style Guide** para los aspectos de scripting complementarios al marcado.

Las convenciones aplicadas son las siguientes:

- Se utiliza `const` para valores que no cambian y `let` para valores que pueden reasignarse; se evita el uso de `var`.
- Los nombres de variables y funciones se escriben en **camelCase**: `getUserData`, `handleButtonClick`.
- Las funciones se declaran como **arrow functions** cuando no requieren su propio contexto `this`: `const fetchData = () => { ... }`.
- Los strings se definen usando **template literals** cuando se requiere interpolación: `` `Hello, ${userName}` ``.
- El código se organiza en funciones con una única responsabilidad, evitando bloques de lógica demasiado extensos.
- Se incluyen comentarios descriptivos en funciones no triviales, explicando el propósito y no el mecanismo.

#### Vue Framework

Para el desarrollo del Frontend Web Application de Entreprenly con **Vue 3**, el equipo adopta la **Vue Style Guide** oficial como referencia principal para la organización y estructura de los Single File Components (SFC), complementada con la **Google JavaScript Style Guide** y las **MDN JavaScript guidelines** para el código de lógica.

Las convenciones aplicadas son las siguientes:

- Los componentes se desarrollan como **Single File Components** (`.vue`) empleando la **Composition API** con `<script setup>`.
- Los nombres de **archivos de componentes** se escriben en **PascalCase**: `DashboardLayout.vue`, `ProductCard.vue`, `SubscriptionPanel.vue`.
- Los nombres de **componentes con múltiples palabras** evitan colisiones con elementos HTML nativos, conforme a la Vue Style Guide (regla de prioridad esencial).
- Las **props** se declaran con su tipo y, cuando aplica, con valores por defecto y la marca de obligatoriedad: `defineProps({ productId: { type: Number, required: true } })`.
- El estado reactivo local se gestiona con `ref` y `reactive`, y los valores derivados con `computed`, en lugar de mutaciones manuales del DOM.
- El estado compartido entre vistas y bounded contexts se gestiona con **Pinia** (stores por dominio), evitando el prop-drilling y centralizando la lógica de acceso a datos.
- Los nombres de **variables, funciones y métodos** se escriben en **camelCase**: `isLoggedIn`, `fetchProducts()`.
- Los nombres de **constantes globales** se escriben en **UPPER_SNAKE_CASE**: `MAX_RETRY_ATTEMPTS`.
- Las vistas y los componentes se organizan **por bounded context** (`auth/`, `inventory/`, `sales/`, `subscription/`, `profile/`, `chatbot/`, además de `shared/`), evitando una estructura monolítica, y la navegación se resuelve con **Vue Router** mediante lazy-loading por BC.
- Las operaciones asíncronas (consumo de la API) se manejan con `async/await` sobre **axios**, encapsuladas en servicios por bounded context; las rutas base y los endpoints se parametrizan mediante variables de entorno de Vite (`VITE_*`).
- La internacionalización (i18n) se gestiona con **vue-i18n**, manteniendo las claves de traducción organizadas por bounded context.

#### C# y ASP.NET Core

Para el desarrollo de los RESTful Web Services de Entreprenly, el equipo adopta las **C# Coding Conventions** de Microsoft y las **Microsoft ASP.NET Core Coding Guidelines** como referencias principales, tomando como base la arquitectura y organización del proyecto de referencia **learning-center-platform**.

Las convenciones aplicadas son las siguientes:

- Los nombres de **clases, interfaces, métodos y propiedades públicas** se escriben en **PascalCase**: `ProductController`, `IProductRepository`, `FindProductById()`. Las interfaces se prefijan con `I`.
- Los nombres de **variables locales y parámetros** se escriben en **camelCase**: `currentUser`, `productId`.
- Los nombres de **constantes** se escriben en **PascalCase**: `DefaultPageSize`.
- Los **namespaces** se organizan por bounded context siguiendo la estructura de learning-center-platform: `Entreprenly.WebServices.[BoundedContext].[Layer]`. Por ejemplo: `Entreprenly.WebServices.Inventory.Interfaces.REST`, `Entreprenly.WebServices.Inventory.Domain.Model.Aggregates`. Los bounded contexts implementados son `Iam`, `Profiles`, `Subscription`, `Inventory`, `Sales` y `Chatbot`, además de `Shared`.
- La arquitectura interna de cada bounded context sigue el patrón de capas DDD: `Domain` (aggregates, entities, value objects, commands, queries, repository interfaces), `Application` (command/query services e internal handlers), `Infrastructure` (repositories con Entity Framework Core sobre MySQL y adaptadores externos) e `Interfaces` (REST controllers y transform/resources). La comunicación entre capas mediante comandos y queries se apoya en el patrón **Mediator** (Cortex.Mediator), siguiendo el enfoque CQRS de learning-center-platform.
- Los **endpoints** de los controladores REST se nombran en **kebab-case** y en plural para recursos: `/api/v1/inventory-unit-products`, `/api/v1/inventory-lots`, `/api/v1/sales`.
- Los **métodos HTTP** se emplean de acuerdo con su semántica RESTful: `GET` para consultas, `POST` para creación, `PUT` para actualización completa, `PATCH` para actualización parcial y `DELETE` para eliminación.
- Se utilizan los **atributos estándar** de ASP.NET Core: `[ApiController]`, `[Route]`, `[HttpGet]`, `[HttpPost]`, entre otros.
- Se aplica **indentación de 4 espacios** de acuerdo con las C# Coding Conventions.
- Los **comentarios XML de documentación** (`/// <summary>`) se incluyen en las clases públicas y en los métodos cuya lógica no sea autoexplicativa, sirviendo además de base para la documentación OpenAPI/Swagger.

#### Gherkin (Acceptance Criteria)

Para la redacción de los criterios de aceptación de las User Stories y los escenarios de prueba de aceptación de los RESTful Web Services, el equipo adopta las **Gherkin Conventions for Readable Specifications**.

Las convenciones aplicadas son las siguientes:

- Cada escenario se redacta en inglés, en **tiempo presente y tercera persona**.
- La estructura `Given – When – Then` se respeta estrictamente: `Given` define el contexto inicial, `When` describe la acción del usuario o del sistema y `Then` especifica el resultado esperado.
- Se utiliza `And` para añadir condiciones adicionales dentro de un mismo bloque, evitando repetir la palabra clave principal.
- Los nombres de los escenarios son descriptivos y comunican el comportamiento esperado sin referirse a detalles de implementación.
- Se evita la lógica condicional dentro de un mismo escenario; cada escenario cubre un único camino de ejecución (happy path o unhappy path).

**Ejemplo de escenario para un endpoint de la API:**

```gherkin
Scenario: Developer retrieves an existing project successfully
  Given a project with id 1 exists in the system
  When the developer sends a GET request to "/api/v1/projects/1"
  Then the response status code should be 200
  And the response body should contain the project details
```

### 5.1.4. Software Deployment Configuration

En esta sección se especifica la configuración de despliegue definida por el equipo de Kauflink para cada uno de los productos digitales que conforman la solución **Entreprenly**: Landing Page, Frontend Web Application y RESTful Web Services. El objetivo es establecer, desde el inicio del ciclo de vida, los pasos y herramientas necesarias para lograr el despliegue o publicación satisfactoria de cada producto a partir de los repositorios de código fuente.

**Productos desplegados y URLs públicas**

La siguiente tabla resume los tres productos digitales de la solución, con su tecnología y plataforma de despliegue y la URL pública donde se encuentran disponibles.

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th>Producto</th>
      <th>Tecnología / Plataforma de despliegue</th>
      <th>URL pública</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Landing Page</td>
      <td>HTML5 + Tailwind CSS / GitHub Pages</td>
      <td><a href="https://landing.entreprenly.online/">https://landing.entreprenly.online/</a></td>
    </tr>
    <tr>
      <td>Frontend Web Application</td>
      <td>Vue 3 (Vite) / Firebase Hosting</td>
      <td><a href="https://ap.entreprenly.online/">https://ap.entreprenly.online/</a></td>
    </tr>
    <tr>
      <td>RESTful Web Services (API)</td>
      <td>ASP.NET Core (.NET 10) / Google Cloud Run</td>
      <td><a href="https://ap-api.entreprenly.online/swagger">https://ap-api.entreprenly.online/swagger</a></td>
    </tr>
  </tbody>
</table>

#### Landing Page (GitHub Pages)

El Landing Page de Entreprenly está desarrollado con HTML5, JavaScript y **Tailwind CSS**, y se despliega mediante **GitHub Pages** sirviendo directamente desde la rama `main`. En el Sprint 1 la publicación se automatizó con un workflow de GitHub Actions y, posteriormente, el equipo simplificó el flujo dejando la publicación directa desde la rama. El estilo se compila localmente con la CLI de Tailwind y el `styles.css` resultante se versiona en el repositorio, de modo que GitHub Pages publica los archivos estáticos tal cual al integrarse cambios en `main`. El sitio se encuentra disponible en el dominio personalizado **[landing.entreprenly.online](https://landing.entreprenly.online)**.

**Paso 1.** Asegurar que el repositorio del Landing Page (`Kauflink/ap-entreprenly-landing`) esté **público** en GitHub y siga GitFlow (ramas `main` y `develop`).

<p align="center"><img src="images/capitulo5/deploy-landing-01.png" width="700" alt="Repositorio del Landing en GitHub"></p>

**Paso 2.** Generar la hoja de estilos de producción ejecutando `npm run build` (`tailwindcss -i ./src/input.css -o ./styles.css --minify`) y versionar el `styles.css` resultante junto con el resto de archivos estáticos.

<p align="center"><img src="images/capitulo5/deploy-landing-02.png" width="700" alt="Compilación de estilos con Tailwind CSS"></p>

**Paso 3.** En la configuración del repositorio, ingresar a **Settings > Pages** y seleccionar como fuente de publicación (**Source**) la rama `main` y la carpeta raíz (`/`).

<p align="center"><img src="images/capitulo5/deploy-landing-03.png" width="700" alt="Settings > Pages con Source = main"></p>

**Paso 4.** Configurar el dominio personalizado ingresando `landing.entreprenly.online` en el campo **Custom domain** y habilitando **Enforce HTTPS**.

<p align="center"><img src="images/capitulo5/deploy-landing-04.png" width="700" alt="Dominio personalizado en GitHub Pages"></p>

**Paso 5.** En el proveedor de DNS del dominio, crear los registros `A`/`CNAME` que apunten a los servidores de GitHub Pages, de acuerdo con la documentación oficial de GitHub.

<p align="center"><img src="images/capitulo5/deploy-landing-05.png" width="700" alt="Registros DNS del dominio"></p>

**Paso 6.** Verificar que el archivo `CNAME` con el valor `landing.entreprenly.online` esté presente en la raíz del repositorio para que GitHub Pages respete el dominio personalizado entre despliegues.

<p align="center"><img src="images/capitulo5/deploy-landing-06.png" width="700" alt="Archivo CNAME en el repositorio"></p>

**Paso 7.** Validar el despliegue accediendo a `https://landing.entreprenly.online` y confirmando que la versión publicada corresponde con el último commit integrado en `main`.

<p align="center"><img src="images/capitulo5/deploy-landing-07.png" width="700" alt="Landing Page publicado"></p>

#### Frontend Web Application (Firebase Hosting)

El Frontend Web Application de Entreprenly está desarrollado con **Vue 3** (construido con **Vite**) y se despliega mediante **Firebase Hosting**, disponible en el subdominio personalizado **[https://ap.entreprenly.online](https://ap.entreprenly.online)** (y también accesible mediante el dominio por defecto de Firebase **ap-entreprenly.web.app**). Firebase Hosting fue elegido sobre GitHub Pages por tres razones concretas: soporta el enrutamiento del lado del cliente (SPA routing) de Vue Router de forma nativa sin configuraciones adicionales, permite asociar subdominios personalizados sin conflictos con el dominio principal ya utilizado por el Landing Page en GitHub Pages, y se integra de forma directa con GitHub Actions para automatizar el ciclo de build y despliegue.

**Paso 1.** Crear un proyecto en **Firebase Console** ([console.firebase.google.com](https://console.firebase.google.com)) e ingresar a la sección **Hosting**. Activar el servicio y asociarlo al proyecto `ap-entreprenly`.

<p align="center"><img src="images/capitulo5/deploy-frontend-01.png" width="700" alt="Proyecto Firebase con Hosting activado"></p>

**Paso 2.** En el entorno local, instalar Firebase CLI e iniciar sesión:
```bash
npm install -g firebase-tools
firebase login
```

<p align="center"><img src="images/capitulo5/deploy-frontend-02-01.png" width="700" alt="Firebase CLI instalado y login"></p>

<p align="center"><img src="images/capitulo5/deploy-frontend-02-02.png" width="700" alt="Firebase CLI instalado y login"></p>

**Paso 3.** Dentro del repositorio del Frontend (`Kauflink/ap-entreprenly-frontend`), inicializar Firebase Hosting con `firebase init hosting`: seleccionar el proyecto `ap-entreprenly`, indicar `dist` como directorio público (output del build de Vite), responder `Yes` a la reescritura de rutas al `index.html` (SPA) y no sobrescribir el `index.html` existente.
```bash
firebase init hosting
```

<p align="center"><img src="images/capitulo5/deploy-frontend-03.png" width="700" alt="firebase init hosting"></p>

**Paso 4.** Verificar que el archivo `firebase.json` incluya la regla de reescritura para el SPA routing de Vue Router:
```json
{
  "hosting": {
    "public": "dist",
    "ignore": ["firebase.json", "**/.*", "**/node_modules/**"],
    "rewrites": [{ "source": "**", "destination": "/index.html" }]
  }
}
```

<p align="center"><img src="images/capitulo5/deploy-frontend-04.png" width="700" alt="firebase.json con rewrites"></p>

**Paso 5.** En **Firebase Console > Hosting > Add custom domain**, registrar el subdominio `ap.entreprenly.online` y crear en el proveedor de DNS los registros que indica Firebase (tipo `A` o `CNAME`), esperando la emisión automática del certificado TLS.

<p align="center"><img src="images/capitulo5/deploy-frontend-05.png" width="700" alt="Dominio personalizado en Firebase Hosting"></p>

**Paso 6.** En el repositorio, configurar el **GitHub Secret** `FIREBASE_SERVICE_ACCOUNT_AP_ENTREPRENLY` con las credenciales de la cuenta de servicio de Firebase, necesarias para autenticar el despliegue desde GitHub Actions.

<p align="center"><img src="images/capitulo5/deploy-frontend-06.png" width="700" alt="GitHub Secret de Firebase"></p>

**Paso 7.** Crear el workflow `.github/workflows/firebase-hosting.yml`, que ante cada push a `main` ejecuta: checkout, configuración de **Node.js 22**, instalación de dependencias con `npm ci`, build de producción con `npm run build` (Vite) y despliegue con la acción oficial `FirebaseExtended/action-hosting-deploy` (proyecto `ap-entreprenly`, canal `live`).

<p align="center"><img src="images/capitulo5/deploy-frontend-07.png" width="700" alt="Workflow de Firebase Hosting en GitHub Actions"></p>

**Paso 8.** Verificar la ejecución del workflow en **Actions** (estado verde) y validar accediendo a `https://ap.entreprenly.online`, comprobando que la navegación entre vistas de Vue funciona sin errores 404 al refrescar el navegador.

<p align="center"><img src="images/capitulo5/deploy-frontend-08.png" width="700" alt="Frontend desplegado en Firebase Hosting"></p>

#### RESTful Web Services (Google Cloud Run)

El Backend de Entreprenly está desarrollado con **ASP.NET Core** (C#, .NET 10) y se empaqueta con un **`Dockerfile`** multi-etapa. Se despliega en **Google Cloud Run** (servicio `ap-entreprenly-web-services`, región `us-east1`), donde el contenedor se construye a partir del código fuente mediante **Cloud Build** y la imagen queda publicada en **Google Artifact Registry**. La persistencia se realiza sobre **Cloud SQL para MySQL 8.4** (instancia `entreprenly-db`), a la que Cloud Run se conecta mediante el **conector nativo de Cloud SQL** (socket Unix). El servicio se expone en el subdominio personalizado **[ap-api.entreprenly.online](https://ap-api.entreprenly.online)** y el despliegue se realiza tomando como fuente la rama `main` del repositorio `Kauflink/ap-entreprenly-web-services`.

**Paso 1.** En **Google Cloud Console**, seleccionar (o crear) el proyecto y habilitar las APIs necesarias: **Cloud Run Admin**, **Cloud Build**, **Artifact Registry** y **Cloud SQL Admin**.

<p align="center"><img src="images/capitulo5/deploy-backend-01.png" width="700" alt="APIs habilitadas en Google Cloud"></p>

**Paso 2.** Provisionar la instancia de **Cloud SQL para MySQL 8.4** (`entreprenly-db`, región `us-east1`), crear la base de datos `ap-entreprenly` y el usuario `entreprenly`, y anotar su **connection name** (`project-46ae30cc-2d30-4c9e-9f5:us-east1:entreprenly-db`), requerido más adelante por la conexión de Cloud Run.

<p align="center"><img src="images/capitulo5/deploy-backend-02.png" width="700" alt="Instancia Cloud SQL para MySQL"></p>

**Paso 3.** Confirmar que el repositorio `Kauflink/ap-entreprenly-web-services` contiene el **`Dockerfile`** multi-etapa: la etapa `build` usa `mcr.microsoft.com/dotnet/sdk:10.0` para ejecutar `dotnet restore` y `dotnet publish -c Release`, y la etapa `runtime` usa `mcr.microsoft.com/dotnet/aspnet:10.0`. La aplicación escucha en el puerto `8080` (`ASPNETCORE_URLS=http://+:8080`) y el `ENTRYPOINT` ejecuta `dotnet Entreprenly.WebServices.dll`.

<p align="center"><img src="images/capitulo5/deploy-backend-03.png" width="700" alt="Dockerfile del backend"></p>

**Paso 4.** Verificar la cadena de conexión del perfil de producción, que apunta al **socket Unix de Cloud SQL** que Cloud Run monta automáticamente y es consumida por **EF Core 9** con el proveedor **Pomelo MySQL**:
```text
server=/cloudsql/<CLOUD_SQL_CONNECTION_NAME>;database=ap-entreprenly;User Id=entreprenly;AllowPublicKeyRetrieval=True
```
El esquema de la base de datos se gestiona con **migraciones de EF Core**.

<p align="center"><img src="images/capitulo5/deploy-backend-04.png" width="700" alt="Cadena de conexión a Cloud SQL"></p>

**Paso 5.** En **Cloud Run > Deploy container > Service**, elegir la opción de desplegar **desde el código fuente / repositorio** (build con Cloud Build a partir del `Dockerfile`). Conectar el repositorio de GitHub `ap-entreprenly-web-services` y seleccionar la rama `main`.

<p align="center"><img src="images/capitulo5/deploy-backend-05.png" width="700" alt="Origen del despliegue en Cloud Run"></p>

**Paso 6.** Definir la configuración del servicio: nombre `ap-entreprenly-web-services`, región `us-east1`, **Authentication = Allow unauthenticated invocations**, **container port = 8080**, **CPU = 1**, **Memory = 1 GiB**, **Max instances = 3** y **Startup CPU boost** activado.

<p align="center"><img src="images/capitulo5/deploy-backend-06.png" width="700" alt="Configuración del servicio Cloud Run"></p>

**Paso 7.** En la pestaña **Containers > Cloud SQL connections**, agregar la conexión a la instancia `entreprenly-db` creada en el Paso 2 (Cloud Run inyecta el socket en `/cloudsql/<connection_name>`).

<p align="center"><img src="images/capitulo5/deploy-backend-07.png" width="700" alt="Conexión Cloud SQL en Cloud Run"></p>

**Paso 8.** En **Variables & Secrets**, definir las variables de entorno del perfil de producción: `ASPNETCORE_ENVIRONMENT=Production`, `DATABASE_PROJECT`, `DATABASE_REGION`, `DATABASE_INSTANCE`, `DATABASE_NAME`, `DATABASE_USER`, `DATABASE_PASSWORD`, `TokenSettings__Secret` (secreto JWT), `WhatsAppBridge__BridgeUrl` y `WhatsAppBridge__BridgeToken`. *(Recomendado: gestionar los valores sensibles —contraseña de la base de datos, secreto JWT y token del bridge— mediante **Secret Manager** en lugar de texto plano.)*

<p align="center"><img src="images/capitulo5/deploy-backend-08.png" width="700" alt="Variables de entorno en Cloud Run"></p>

**Paso 9.** Presionar **Deploy** y esperar a que Cloud Build construya la imagen (publicada en Artifact Registry) y la nueva revisión reciba el **100 % del tráfico**. Cloud Run asigna una URL `*.run.app`.

<p align="center"><img src="images/capitulo5/deploy-backend-09.png" width="700" alt="Revisión desplegada en Cloud Run"></p>

**Paso 10.** En **Cloud Run > Manage Custom Domains > Add mapping**, mapear `ap-api.entreprenly.online` al servicio, crear en el DNS los registros indicados y esperar la emisión automática del certificado TLS. Registrar la URL base `https://ap-api.entreprenly.online/api/v1` como variable de entorno (`VITE_ENTREPENLY_PLATFORM_API_URL`) en el proyecto del Frontend Web Application para su integración.

<p align="center"><img src="images/capitulo5/deploy-backend-10.png" width="700" alt="Dominio personalizado del backend"></p>

**Paso 11.** Validar el despliegue accediendo a la documentación **Swagger UI** en `https://ap-api.entreprenly.online/swagger` y realizando una petición de prueba desde Swagger o Postman, confirmando la respuesta correcta sobre HTTPS.

<p align="center"><img src="images/capitulo5/deploy-backend-11.png" width="700" alt="Swagger UI del backend desplegado"></p>

## 5.2. Landing Page, Services & Applications Implementation

### 5.2.1. Sprint 1

#### 5.2.1.1. Sprint Planning 1

Para este primer Sprint, el equipo estableció como objetivo principal la implementación y despliegue de la primera versión del Landing Page de Entreprenly. La reunión de planificación se llevó a cabo de manera virtual, donde se definieron las User Stories a abordar, el Sprint Goal y la distribución de responsabilidades entre los miembros del equipo.

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <tbody>
    <tr>
      <td colspan="2"><strong>Sprint 1</strong></td>
    </tr>
    <tr>
      <td colspan="2"><strong>Sprint Planning Background</strong></td>
    </tr>
    <tr>
      <td><strong>Date</strong></td>
      <td>2026-04-18</td>
    </tr>
    <tr>
      <td><strong>Time</strong></td>
      <td>09:00 AM</td>
    </tr>
    <tr>
      <td><strong>Location</strong></td>
      <td>Reunión virtual vía Discord</td>
    </tr>
    <tr>
      <td><strong>Prepared By</strong></td>
      <td>Camargo Briceño, Joseph Julius</td>
    </tr>
    <tr>
      <td><strong>Attendees (to planning meeting)</strong></td>
      <td>Camargo Briceño, Joseph Julius / Chavez Carrasco, Lionel Abraham / Palma De Los Santos, Elynor Mikela / Peirano Brun, José Antonio / Flores Pinchi, José Fernando</td>
    </tr>
    <tr>
      <td><strong>Sprint 1 – 1 Review Summary</strong></td>
      <td>Al ser el primer Sprint del proyecto, no existe un Sprint anterior que revisar. Se parte desde cero con el inicio del ciclo de vida del producto.</td>
    </tr>
    <tr>
      <td><strong>Sprint 1 – 1 Retrospective Summary</strong></td>
      <td>Al ser el primer Sprint del proyecto, no existe retrospectiva previa. El equipo acordó mantener comunicación constante vía Discord y respetar los plazos de entrega de cada tarea.</td>
    </tr>
    <tr>
      <td colspan="2"><strong>Sprint Goal &amp; User Stories</strong></td>
    </tr>
    <tr>
      <td><strong>Sprint 1 Goal</strong></td>
      <td>Nuestro enfoque está en presentar la propuesta de valor de Entreprenly a los usuarios potenciales a través de un Landing Page funcional y desplegado. Creemos que genera una primera impresión clara del producto y motiva a los visitantes de nuestros segmentos objetivo a explorar la plataforma. Esto se confirmará cuando el Landing Page esté públicamente accesible, incluya todas las secciones clave (hero, funcionalidades, planes y llamados a la acción) y redirija correctamente a los visitantes hacia la Web Application.</td>
    </tr>
    <tr>
      <td><strong>Sprint 1 Velocity</strong></td>
      <td>8</td>
    </tr>
    <tr>
      <td><strong>Sum of Story Points</strong></td>
      <td>8</td>
    </tr>
  </tbody>
</table>

---

#### 5.2.1.2. Aspect Leaders and Collaborators

En este primer Sprint, el equipo organizó su trabajo en torno a cuatro aspectos principales: la configuración inicial del repositorio y entorno de despliegue, el desarrollo de la estructura base del Landing Page, la implementación de funcionalidades interactivas (cambio de tema e idioma, animaciones y CTAs), y la revisión y corrección del contenido textual. A continuación, se presenta la matriz de liderazgo y colaboración (LACX):

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th>Team Member (Last Name, First Name)</th>
      <th>GitHub Username</th>
      <th>Configuración del Repositorio y CI/CD<br>Leader (L) / Collaborator (C)</th>
      <th>Estructura Base del Landing Page<br>Leader (L) / Collaborator (C)</th>
      <th>Funcionalidades Interactivas (Tema, Idioma, CTAs)<br>Leader (L) / Collaborator (C)</th>
      <th>Corrección de Contenido<br>Leader (L) / Collaborator (C)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Juyens</td>
      <td>L</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Chavez Carrasco, Lionel Abraham</td>
      <td>LioTG</td>
      <td>C</td>
      <td>L</td>
      <td>L</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Palma De Los Santos, Elynor Mikela</td>
      <td>elynorpalma</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
      <td>L</td>
    </tr>
    <tr>
      <td>Peirano Brun, José Antonio</td>
      <td>DoomerGX</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
      <td>L</td>
    </tr>
    <tr>
      <td>Flores Pinchi, José Fernando</td>
      <td>Ferdinant12-ops</td>
      <td>C</td>
      <td>L</td>
      <td>C</td>
      <td>L</td>
    </tr>
  </tbody>
</table>

---

#### 5.2.1.3. Sprint Backlog 1

El objetivo principal de este Sprint fue implementar y desplegar la primera versión del Landing Page de Entreprenly, cubriendo la User Story US-49 del Product Backlog. A continuación se presenta el tablero del Sprint y el detalle de los Work-items asociados.

![sprint1](./images/capitulo5/sprint1.png "Tablero del Sprint 1 en Trello")

**Board público del Sprint 1 (Trello):** https://trello.com/b/w5cZrD9x/entreprenly-sprint-1

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th colspan="8">Sprint # Sprint 1</th>
    </tr>
    <tr>
      <th colspan="2">User Story</th>
      <th colspan="6">Work-Item / Task</th>
    </tr>
    <tr>
      <th>Id</th>
      <th>Title</th>
      <th>Id</th>
      <th>Title</th>
      <th>Description</th>
      <th>Estimation (Hours)</th>
      <th>Assigned To</th>
      <th>Status</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>US-49</td>
      <td>Conocer propuesta de valor en landing page</td>
      <td>T-01</td>
      <td>Configuración inicial del repositorio</td>
      <td>Crear el repositorio, inicializar el proyecto con HTML/CSS/Tailwind y configurar el <code>.gitignore</code> y <code>package.json</code>.</td>
      <td>4</td>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-49</td>
      <td>Conocer propuesta de valor en landing page</td>
      <td>T-02</td>
      <td>Configurar pipeline de despliegue (GitHub Actions)</td>
      <td>Crear y ajustar el workflow de GitHub Actions para despliegue automático en GitHub Pages con CNAME configurado.</td>
      <td>4</td>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-85</td>
      <td>Visualizar la propuesta de valor</td>
      <td>T-03</td>
      <td>Implementar Hero section y Problem section</td>
      <td>Desarrollar la sección hero con headline "Controla inventario, pedidos y cobros de tu negocio", propuesta de valor y CTAs diferenciados por segmento, y la sección de problema que contextualiza los dolores del comerciante.</td>
      <td>4</td>
      <td>Chavez Carrasco, Lionel Abraham / Flores Pinchi, José Fernando</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-85</td>
      <td>Visualizar la propuesta de valor</td>
      <td>T-04</td>
      <td>Implementar controles de tema e idioma</td>
      <td>Agregar switch de tema claro/oscuro y selector de idioma (Español/Inglés) accesibles desde la barra de navegación, con mejoras en los call-to-action diferenciados por segmento objetivo.</td>
      <td>4</td>
      <td>Chavez Carrasco, Lionel Abraham</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-85</td>
      <td>Visualizar la propuesta de valor</td>
      <td>T-05</td>
      <td>Implementar animaciones y transiciones de la landing</td>
      <td>Agregar transiciones de fade al cambio de tema y animaciones de movimiento en la sección hero para mejorar la experiencia visual del visitante al cargar la página.</td>
      <td>4</td>
      <td>Chavez Carrasco, Lionel Abraham</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-86</td>
      <td>Explorar las funciones principales</td>
      <td>T-06</td>
      <td>Implementar Main Features section y How It Works section</td>
      <td>Desarrollar la sección de funcionalidades principales con los 4 pilares (Inventario, Finanzas, Chatbot, Balanza IoT) y la sección explicativa del flujo de adopción del sistema paso a paso.</td>
      <td>4</td>
      <td>Chavez Carrasco, Lionel Abraham / Flores Pinchi, José Fernando</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-86</td>
      <td>Explorar las funciones principales</td>
      <td>T-07</td>
      <td>Implementar Merchant Benefits section, Client Trust section y Comparativa breve section</td>
      <td>Desarrollar la sección de beneficios operativos para el comerciante, la sección de confianza del cliente final y la sección comparativa que contrasta la gestión manual, sistemas genéricos y Entreprenly.</td>
      <td>4</td>
      <td>Chavez Carrasco, Lionel Abraham / Flores Pinchi, José Fernando</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-87</td>
      <td>Revisar los planes de suscripción</td>
      <td>T-08</td>
      <td>Implementar Planes section</td>
      <td>Desarrollar la sección comercial con las tarjetas del Plan Free y Plan Control, mostrando el costo mensual, la lista de funcionalidades incluidas en cada nivel y los botones de acción hacia el registro.</td>
      <td>4</td>
      <td>Chavez Carrasco, Lionel Abraham / Flores Pinchi, José Fernando</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-88</td>
      <td>Consultar las preguntas frecuentes</td>
      <td>T-09</td>
      <td>Implementar FAQ section y Next Step section</td>
      <td>Desarrollar la sección de preguntas frecuentes con acordeones interactivos que expanden y colapsan respuestas, y la sección de cierre con CTA final que refuerza la conversión hacia el registro.</td>
      <td>4</td>
      <td>Palma De Los Santos, Elynor Mikela / Peirano Brun, José Antonio</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-89</td>
      <td>Iniciar sesión desde la landing page</td>
      <td>T-10</td>
      <td>Implementar navegación del header y enlace "Ingresar"</td>
      <td>Desarrollar el header con la barra de navegación principal (Cómo funciona, Beneficios, Planes, FAQ), el botón "Iniciar sesión" que redirige a <code>./login.html</code> y el menú responsive desplegable para dispositivos móviles.</td>
      <td>4</td>
      <td>Chavez Carrasco, Lionel Abraham</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-90</td>
      <td>Acceder mediante el botón de acción principal</td>
      <td>T-11</td>
      <td>Implementar CTAs "Empezar gratis" y Footer section</td>
      <td>Implementar el botón "Empezar gratis" en el Hero y en la sección Next step que redirige a <code>./register.html</code>, y desarrollar el footer con los grupos Explorar y Siguiente paso, datos de contacto y enlaces de la marca.</td>
      <td>4</td>
      <td>Peirano Brun, José Antonio / Flores Pinchi, José Fernando</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-49</td>
      <td>Conocer propuesta de valor en landing page</td>
      <td>T-12</td>
      <td>Revisión y corrección de contenido textual</td>
      <td>Corregir errores ortográficos, de tildes y redacción en todos los textos del Landing Page para garantizar la calidad del contenido publicado en producción.</td>
      <td>4</td>
      <td>Palma De Los Santos, Elynor Mikela / Peirano Brun, José Antonio / Flores Pinchi, José Fernando</td>
      <td>Done</td>
    </tr>
  </tbody>
</table>

---

#### 5.2.1.4. Development Evidence for Sprint Review

Durante el Sprint 1, el equipo se centró exclusivamente en el repositorio del Landing Page. Se realizaron un total de 20 commits distribuidos entre el 18 y el 20 de abril de 2026, cubriendo desde la configuración inicial del proyecto hasta correcciones de contenido y el despliegue automatizado mediante GitHub Actions. A continuación se presenta el registro de commits:

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th>Repository</th>
      <th>Branch</th>
      <th>Commit Id</th>
      <th>Commit Message</th>
      <th>Commit Message Body</th>
      <th>Committed on (Date)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>main</td>
      <td>d57dee9</td>
      <td>Initial commit</td>
      <td>Creación inicial del repositorio con estructura base del proyecto.</td>
      <td>2026-04-18</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>develop</td>
      <td>86c305f</td>
      <td>chore(config): initialize .gitignore for node and tailwind</td>
      <td>Se agrega <code>.gitignore</code> configurado para excluir dependencias de Node y archivos compilados de Tailwind.</td>
      <td>2026-04-18</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>develop</td>
      <td>568c339</td>
      <td>docs: simplify README with essential information and update license to MIT</td>
      <td>Se simplifica el README con instrucciones esenciales y se actualiza la licencia a MIT.</td>
      <td>2026-04-18</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>main</td>
      <td>5088424</td>
      <td>Merge pull request #1 from Kauflink/develop</td>
      <td>Primera integración de la rama develop a main con la estructura base del proyecto.</td>
      <td>2026-04-18</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>main</td>
      <td>003eb4f</td>
      <td>Create CNAME</td>
      <td>Se crea el archivo CNAME para la configuración del dominio personalizado en GitHub Pages.</td>
      <td>2026-04-18</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>main</td>
      <td>9e82e20</td>
      <td>Refactor GitHub Actions workflow for deployment</td>
      <td>Se refactoriza el workflow de CI/CD para optimizar el proceso de despliegue automático.</td>
      <td>2026-04-18</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>main</td>
      <td>bcc3513</td>
      <td>Update Node.js version and clean install step</td>
      <td>Se actualiza la versión de Node.js y se mejora el paso de instalación limpia en el pipeline.</td>
      <td>2026-04-18</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>main</td>
      <td>ff3e7e6</td>
      <td>Update GitHub Actions workflow for deployment</td>
      <td>Se actualiza la configuración del workflow de despliegue.</td>
      <td>2026-04-18</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>main</td>
      <td>14b3ed7</td>
      <td>Upgrade GitHub Actions to version 4</td>
      <td>Se actualiza GitHub Actions a la versión 4 para compatibilidad y mejoras de rendimiento.</td>
      <td>2026-04-18</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>develop</td>
      <td>54554c9</td>
      <td>feat: agregar controles de tema, idioma y mejorar CTAs de la landing</td>
      <td>Se implementa el selector de idioma (ES/EN), el switch de tema claro/oscuro y se mejoran los call-to-action dirigidos a cada segmento objetivo.</td>
      <td>2026-04-19</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>main</td>
      <td>32ab091</td>
      <td>Merge pull request #2 from Kauflink/develop</td>
      <td>Segunda integración con los controles de tema, idioma y CTAs mejorados.</td>
      <td>2026-04-19</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>develop</td>
      <td>f9a1e00</td>
      <td>feat: add theme fade and hero motion refinements</td>
      <td>Se agregan transiciones de fade al cambio de tema y animaciones de movimiento en la sección hero.</td>
      <td>2026-04-19</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>main</td>
      <td>9136aed</td>
      <td>Merge pull request #3 from Kauflink/develop</td>
      <td>Tercera integración con animaciones y refinamientos del hero.</td>
      <td>2026-04-19</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>develop</td>
      <td>e740b59</td>
      <td>fix: corrección de tildes</td>
      <td>Se corrigen errores de acentuación en el contenido textual del Landing Page.</td>
      <td>2026-04-19</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>develop</td>
      <td>55ee2fb</td>
      <td>fix(landing_page): ortografia arreglada</td>
      <td>Se corrigen errores ortográficos en los textos del Landing Page.</td>
      <td>2026-04-19</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>main</td>
      <td>846f934</td>
      <td>Merge pull request #4 from Kauflink/develop</td>
      <td>Cuarta integración con correcciones ortográficas y de contenido.</td>
      <td>2026-04-19</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>develop</td>
      <td>7e09505</td>
      <td>app:Correccion</td>
      <td>Correcciones generales en el contenido del Landing Page.</td>
      <td>2026-04-19</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>develop</td>
      <td>3cbf2e2</td>
      <td>app:CorreccionPalabras</td>
      <td>Corrección de palabras en el contenido del Landing Page.</td>
      <td>2026-04-19</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>develop</td>
      <td>8c4165b</td>
      <td>app:CorreccionTilde</td>
      <td>Corrección de tildes adicionales en el Landing Page.</td>
      <td>2026-04-19</td>
    </tr>
    <tr>
      <td>Kauflink/ap-entreprenly-landing</td>
      <td>main</td>
      <td>7b8ccfc</td>
      <td>Merge pull request #5 from Kauflink/develop</td>
      <td>Quinta integración con las correcciones finales de contenido.</td>
      <td>2026-04-20</td>
    </tr>
  </tbody>
</table>

---

#### 5.2.1.5. Execution Evidence for Sprint Review

Al término del Sprint 1, el equipo logró implementar y desplegar satisfactoriamente la primera versión del Landing Page de Entreprenly. La página se encuentra disponible públicamente a través de GitHub Pages con dominio personalizado configurado mediante el archivo CNAME. El Landing Page incluye las siguientes secciones:

- **Hero:** Presentación principal del producto con headline, propuesta de valor y llamados a la acción (CTAs) diferenciados por segmento objetivo (comerciantes y clientes finales).
- **Funcionalidades:** Descripción visual de las características principales de Entreprenly: gestión de inventario, chatbot de WhatsApp, balanza IoT y dashboard financiero.
- **Planes:** Sección con los planes disponibles (Plan Free y Plan Control) con sus beneficios y botones de acción.
- **Footer:** Información de contacto, términos y condiciones y enlaces relevantes.
- **Controles de experiencia:** Selector de idioma (Español / Inglés) y switch de tema claro/oscuro, accesibles desde la barra de navegación.

![landing_desplegado](./images/capitulo5/landing_desplegado.png "landing_desplegado")

---

#### 5.2.1.6. Services Documentation Evidence for Sprint Review

Durante el Sprint 1, el alcance de implementación se limitó exclusivamente al Landing Page estático. No se desarrollaron ni desplegaron Web Services (RESTful API) en esta iteración, por lo que no aplica documentación de endpoints para este Sprint. La documentación de servicios web se incorporará a partir del Sprint 3, conforme a lo planificado en el Product Backlog.

---

#### 5.2.1.7. Software Deployment Evidence for Sprint Review

Durante el Sprint 1, el equipo configuró y ejecutó el proceso de despliegue del Landing Page mediante GitHub Pages y un pipeline de integración continua con GitHub Actions. A continuación se describe el proceso realizado:

1. **Creación del repositorio:** Se creó el repositorio público `ap-entreprenly-landing` bajo la organización `Kauflink` en GitHub, aplicando GitFlow con las ramas `main` y `develop`.

![creacion_repos](./images/capitulo5/creacion_repos.png "creacion_repos")

2. **Configuración del dominio personalizado:** Se añadió el archivo `CNAME` al repositorio con el dominio personalizado asignado al Landing Page.

![cname](./images/capitulo5/cname.png "cname")

![entreprenly_cname](./images/capitulo5/entreprenly_cname.png "entreprenly_cname")

3. **Configuración del pipeline de CI/CD:** Se creó un workflow de GitHub Actions (`.github/workflows/`) que automatiza el proceso de build y despliegue. El workflow incluye los pasos de instalación de dependencias (`npm ci`), compilación de estilos con Tailwind CSS (`npm run build`) y despliegue automático a la rama `gh-pages` al fusionar cambios en `main`.

![workflows1](./images/capitulo5/workflows1.png "workflows1")

![workflows2](./images/capitulo5/workflows2.png "workflows2")

4. **Verificación del despliegue:** Se comprobó que el Landing Page quedó correctamente publicado y accesible desde la URL de GitHub Pages con el dominio configurado.

![landing_desplegado](./images/capitulo5/landing_desplegado.png "landing_desplegado")

---

#### 5.2.1.8. Team Collaboration Insights during Sprint

Durante el Sprint 1, todos los miembros del equipo participaron activamente en la implementación del Landing Page, evidenciado a través de los commits registrados en el repositorio `ap-entreprenly-landing`. El trabajo se distribuyó de manera colaborativa: Joseph Julius lideró la configuración del repositorio y el pipeline de despliegue; Lionel Abraham se encargó del desarrollo de funcionalidades interactivas y animaciones; Elynor Mikela, José Antonio y José Fernando contribuyeron con correcciones de contenido y en la estructura base de la página.

El equipo aplicó GitFlow como estrategia de control de versiones, trabajando en la rama `develop` y realizando la integración a `main` mediante Pull Requests revisados y aprobados por otros miembros. Se realizaron un total de 5 Pull Requests durante el Sprint.

![commits1](./images/capitulo5/commits1.png "commits1")

![commits2](./images/capitulo5/commits2.png "commits2")

![commits3](./images/capitulo5/commits3.png "commits3")

**URL del repositorio del Landing Page:** https://github.com/Kauflink/ap-entreprenly-landing

### 5.2.2. Sprint 2

#### 5.2.2.1. Sprint Planning 2

Para este segundo Sprint, el equipo estableció como objetivo principal la implementación de la Frontend Web Application de Entreprenly en Vue, cubriendo todos los Bounded Contexts planificados: Auth, Profile, Subscription, Inventory, Sales y Chatbot. La reunión de planificación se llevó a cabo de manera virtual, donde se definieron las User Stories a abordar, el Sprint Goal y la distribución de responsabilidades por Bounded Context.

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <tbody>
    <tr>
      <td colspan="2"><strong>Sprint 2</strong></td>
    </tr>
    <tr>
      <td colspan="2"><strong>Sprint Planning Background</strong></td>
    </tr>
    <tr>
      <td><strong>Date</strong></td>
      <td>2026-04-21</td>
    </tr>
    <tr>
      <td><strong>Time</strong></td>
      <td>09:00 AM</td>
    </tr>
    <tr>
      <td><strong>Location</strong></td>
      <td>Reunión virtual vía Discord</td>
    </tr>
    <tr>
      <td><strong>Prepared By</strong></td>
      <td>Camargo Briceño, Joseph Julius</td>
    </tr>
    <tr>
      <td><strong>Attendees (to planning meeting)</strong></td>
      <td>Camargo Briceño, Joseph Julius / Chavez Carrasco, Lionel Abraham / Palma De Los Santos, Elynor Mikela / Peirano Brun, José Antonio / Flores Pinchi, José Fernando</td>
    </tr>
    <tr>
      <td><strong>Sprint 1 Review Summary</strong></td>
      <td>En el Sprint 1 se implementó y desplegó exitosamente la primera versión del Landing Page de Entreprenly. La página se encuentra disponible en <a href="https://landing.entreprenly.online">landing.entreprenly.online</a> con dominio personalizado y despliegue continuo mediante GitHub Actions. Se cubrieron todas las secciones planificadas: Hero, Funcionalidades, Planes, FAQ y Footer, con soporte de tema claro/oscuro e idioma Español/Inglés.</td>
    </tr>
    <tr>
      <td><strong>Sprint 1 Retrospective Summary</strong></td>
      <td>El equipo identificó que la coordinación entre ramas mejoró con GitFlow. Para el Sprint 2 se acordó asignar un Bounded Context por miembro del equipo para evitar conflictos de merge, mantener la rama <code>develop</code> como punto de integración central y aumentar la frecuencia de Pull Requests para revisión cruzada.</td>
    </tr>
    <tr>
      <td colspan="2"><strong>Sprint Goal &amp; User Stories</strong></td>
    </tr>
    <tr>
      <td><strong>Sprint 2 Goal</strong></td>
      <td>Nuestro enfoque está en desarrollar el Frontend Web Application completo de Entreprenly en Vue, cubriendo todos los Bounded Contexts principales: Sales (Punto de Venta), Chatbot (Pedidos WhatsApp), Subscription, Inventory y Profile. Creemos que entrega una aplicación web funcional y desplegable con la que los comerciantes peruanos pueden gestionar sus operaciones de venta y sus pedidos de WhatsApp. Esto se confirmará cuando la aplicación Vue esté desplegada exitosamente en Firebase Hosting y todos los flujos clave —registro de ventas en caja, gestión de pedidos por chatbot y configuración del perfil de usuario— sean funcionales y navegables.</td>
    </tr>
    <tr>
      <td><strong>Sprint 2 Velocity</strong></td>
      <td>34</td>
    </tr>
    <tr>
      <td><strong>Sum of Story Points</strong></td>
      <td>34</td>
    </tr>
  </tbody>
</table>

---

#### 5.2.2.2. Aspect Leaders and Collaborators

En el Sprint 2, el equipo organizó el trabajo asignando un Bounded Context principal por miembro para maximizar la autonomía y reducir conflictos de merge. Los aspectos cubiertos fueron: la infraestructura base y el DashboardLayout compartido, el BC de Sales (Punto de Venta), el BC de Chatbot (Pedidos WhatsApp), los BCs de Subscription e Inventory, y el BC de Profile junto con la internacionalización (i18n) y el sistema de temas. A continuación se presenta la matriz de liderazgo y colaboración (LACX):

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th>Team Member (Last Name, First Name)</th>
      <th>GitHub Username</th>
      <th>Infraestructura Base y DashboardLayout<br>Leader (L) / Collaborator (C)</th>
      <th>Sales BC — Punto de Venta<br>Leader (L) / Collaborator (C)</th>
      <th>Chatbot BC — Pedidos WhatsApp<br>Leader (L) / Collaborator (C)</th>
      <th>Subscription & Inventory BC<br>Leader (L) / Collaborator (C)</th>
      <th>Profile BC, i18n y Tema<br>Leader (L) / Collaborator (C)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Juyens</td>
      <td>L</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
      <td>L</td>
    </tr>
    <tr>
      <td>Chavez Carrasco, Lionel Abraham</td>
      <td>LioTG</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
      <td>L</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Palma De Los Santos, Elynor Mikela</td>
      <td>elynorpalma</td>
      <td>C</td>
      <td>C</td>
      <td>L</td>
      <td>C</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Peirano Brun, José Antonio</td>
      <td>DoomerGX</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
      <td>L</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Flores Pinchi, José Fernando</td>
      <td>Ferdinant12-ops</td>
      <td>C</td>
      <td>L</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
    </tr>
  </tbody>
</table>

---

#### 5.2.2.3. Sprint Backlog 2

El objetivo principal de este Sprint fue implementar la Frontend Web Application de Entreprenly en Vue, cubriendo los Bounded Contexts de Auth, Profile, Subscription, Inventory, Sales y Chatbot, junto con las vistas compartidas de Home y Help. A continuación se presenta el tablero del Sprint y el detalle de los Work-items asociados.

![sprint2](./images/capitulo5/sprint2.png "Tablero del Sprint 2 en Trello")

**Board público del Sprint 2 (Trello):** https://trello.com/b/X5XRlVOZ/entreprenly-sprint-2

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th colspan="8">Sprint # Sprint 2</th>
    </tr>
    <tr>
      <th colspan="2">User Story</th>
      <th colspan="6">Work-Item / Task</th>
    </tr>
    <tr>
      <th>Id</th>
      <th>Title</th>
      <th>Id</th>
      <th>Title</th>
      <th>Description</th>
      <th>Estimation (Hours)</th>
      <th>Assigned To</th>
      <th>Status</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>US-01</td>
      <td>Iniciar sesión en la aplicación</td>
      <td>T-01</td>
      <td>Configurar proyecto Vue y estructura base</td>
      <td>Inicializar el proyecto Vue con la arquitectura DDD por Bounded Context, configurar rutas lazy-loading, el shell del DashboardLayout con sidebar naranja y <code>router-view</code>, y conectar las rutas principales.</td>
      <td>4</td>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-01</td>
      <td>Iniciar sesión en la aplicación</td>
      <td>T-02</td>
      <td>Implementar DashboardLayout responsive con sidebar</td>
      <td>Desarrollar el componente <code>DashboardLayoutComponent</code> con sidebar naranja, logotipo, íconos de navegación por BC y botón de logout, con layout responsive para distintas resoluciones de pantalla.</td>
      <td>4</td>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-06</td>
      <td>Configurar perfil de usuario</td>
      <td>T-03</td>
      <td>Implementar Profile BC con 8 tarjetas de configuración</td>
      <td>Desarrollar el Bounded Context de perfil con sus 8 tarjetas de configuración (información personal, seguridad, preferencias, notificaciones, entre otras), siguiendo la arquitectura DDD de 4 capas.</td>
      <td>5</td>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-07</td>
      <td>Personalizar preferencias de idioma y tema</td>
      <td>T-04</td>
      <td>Implementar i18n bilingüe, selector de moneda y persistencia de tema</td>
      <td>Integrar el sistema de internacionalización ES/EN en todos los BCs, agregar el selector de moneda (PEN/USD) en el BC de Profile, y persistir las preferencias de idioma y tema claro/oscuro en <code>localStorage</code> para evitar el flash al recargar.</td>
      <td>4</td>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-24</td>
      <td>Buscar producto en el punto de venta</td>
      <td>T-05</td>
      <td>Implementar Sales BC base y buscador con autocompletado</td>
      <td>Crear la estructura DDD del Sales BC (domain, application, infrastructure, presentation), configurar el <code>db.json</code> con productos peruanos, e implementar el buscador de productos con autocompletado y validación "Producto no encontrado".</td>
      <td>4</td>
      <td>Flores Pinchi, José Fernando</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-25</td>
      <td>Registrar cantidad de producto por unidad</td>
      <td>T-06</td>
      <td>Implementar modal "Registrar Cantidad" con teclado numérico</td>
      <td>Desarrollar el modal de registro de cantidad con teclado numérico y validación de stock disponible para productos vendidos por unidad.</td>
      <td>4</td>
      <td>Flores Pinchi, José Fernando</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-26</td>
      <td>Registrar peso de producto con balanza IoT</td>
      <td>T-07</td>
      <td>Implementar modal "Registrar Peso" con modo IoT y manual</td>
      <td>Desarrollar el modal de peso con dos modos: automático (lee peso de <code>db.json</code> y auto-confirma) cuando la balanza está conectada, y manual con teclado decimal cuando <code>connected: false</code>.</td>
      <td>4</td>
      <td>Flores Pinchi, José Fernando</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-27</td>
      <td>Eliminar producto del ticket de venta</td>
      <td>T-08</td>
      <td>Implementar eliminación de ítems y resumen lateral del ticket</td>
      <td>Agregar el ícono de basurero por ítem del ticket para eliminación individual, y el panel de resumen lateral con subtotal, cantidad de ítems y total en tiempo real usando el sistema de reactividad de Vue (ref y computed).</td>
      <td>4</td>
      <td>Flores Pinchi, José Fernando</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-28</td>
      <td>Seleccionar método de pago</td>
      <td>T-09</td>
      <td>Implementar selección de método de pago y validaciones</td>
      <td>Desarrollar la selección de método de pago (Efectivo / Tarjeta-Yape-Plin agrupados como digital) con validación "Por favor seleccione un método de pago" que se auto-oculta a los 3 segundos.</td>
      <td>4</td>
      <td>Flores Pinchi, José Fernando</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-29</td>
      <td>Finalizar venta y confirmar pago</td>
      <td>T-10</td>
      <td>Implementar finalización de venta y modal "Venta Exitosa"</td>
      <td>Desarrollar el flujo de finalización de venta con validaciones ("No hay productos en el ticket"), modal "Venta Exitosa" con auto-cierre a los 2 segundos, y reset del ticket al completar la venta. Incluir el decremento de stock en el Inventory BC tras cada venta.</td>
      <td>5</td>
      <td>Flores Pinchi, José Fernando</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-30</td>
      <td>Ver resumen del cierre de caja</td>
      <td>T-11</td>
      <td>Implementar Resumen de Caja con persistencia en db.json</td>
      <td>Desarrollar el panel de Resumen de Caja con totales por día (Total Día, Efectivo, Digital), persitirlos en <code>cash-registers</code> del <code>db.json</code> mediante PUT al finalizar cada venta, y recargarlos al volver a la vista de ventas.</td>
      <td>4</td>
      <td>Flores Pinchi, José Fernando</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-32</td>
      <td>Conectar cuenta de WhatsApp al chatbot</td>
      <td>T-12</td>
      <td>Implementar Chatbot BC base y flujo de conexión QR</td>
      <td>Crear la estructura DDD del Chatbot BC e implementar la vista de conexión WhatsApp con generación de QR scannable, countdown de expiración y reinicio automático del código QR.</td>
      <td>4</td>
      <td>Palma De Los Santos, Elynor Mikela</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-33</td>
      <td>Ver conversaciones de WhatsApp entrantes</td>
      <td>T-13</td>
      <td>Implementar vista de conversaciones con session guard</td>
      <td>Desarrollar la lista de conversaciones activas del chatbot con guard que bloquea el acceso si WhatsApp no está conectado, burbuja de escritura del cliente y efecto typewriter del bot en la barra de mensajes.</td>
      <td>4</td>
      <td>Palma De Los Santos, Elynor Mikela</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-34</td>
      <td>Gestionar pedidos recibidos por WhatsApp</td>
      <td>T-14</td>
      <td>Implementar vista de órdenes y validación de pago del chatbot</td>
      <td>Desarrollar la vista de órdenes del chatbot con carga de productos reales del Inventory BC, validación de pago y chips de rechazo traducidos. Implementar soporte i18n bilingüe completo (ES/EN) en todos los componentes del Chatbot BC.</td>
      <td>5</td>
      <td>Palma De Los Santos, Elynor Mikela</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-11</td>
      <td>Ver planes de suscripción disponibles</td>
      <td>T-15</td>
      <td>Implementar Subscription BC con vista de planes</td>
      <td>Desarrollar el Bounded Context de Subscription con la vista de planes disponibles (Plan Free y Plan Control), precios sincronizados con el selector de moneda del Profile BC, y traducciones bilingües completas.</td>
      <td>4</td>
      <td>Chavez Carrasco, Lionel Abraham</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-16</td>
      <td>Ver inventario de productos y lotes</td>
      <td>T-16</td>
      <td>Implementar Inventory BC e integración con Sales y Home</td>
      <td>Desarrollar el Bounded Context de Inventory con la vista de productos y lotes, e integrar sus datos reales con el BC de Sales (para el buscador y el decremento de stock) y con la vista de Home (alertas de lotes próximos a vencer).</td>
      <td>4</td>
      <td>Chavez Carrasco, Lionel Abraham / Peirano Brun, José Antonio</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-41</td>
      <td>Ver panel principal del dashboard</td>
      <td>T-17</td>
      <td>Implementar vistas de Home y Help del dashboard</td>
      <td>Desarrollar la vista de Home con el panel de resumen del negocio (alertas de lotes, accesos rápidos, locale reactivo al idioma) y la vista de Help con el centro de ayuda, artículos bilingües y conteo real por categoría.</td>
      <td>4</td>
      <td>Palma De Los Santos, Elynor Mikela</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-01</td>
      <td>Iniciar sesión en la aplicación</td>
      <td>T-18</td>
      <td>Configurar despliegue en Firebase Hosting</td>
      <td>Configurar Firebase Hosting para el Frontend Web Application, crear el workflow de GitHub Actions para despliegue continuo al integrar cambios en <code>main</code>, y validar el despliegue en <code>https://ap.entreprenly.online</code>.</td>
      <td>4</td>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Done</td>
    </tr>
  </tbody>
</table>

---

#### 5.2.2.4. Development Evidence for Sprint Review

Durante el Sprint 2, el equipo trabajó exclusivamente sobre el repositorio del Frontend Web Application (`ap-entreprenly-frontend`). El repositorio se inicializó el 25 de abril de 2026 y el grueso de la implementación se realizó entre el 14 y el 16 de mayo de 2026, sumando más de 70 commits que cubren desde la configuración inicial del proyecto Vue 3 hasta la integración de todos los Bounded Contexts sobre una API simulada con JSON-Server. A continuación se presenta el registro de los commits más representativos:

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th>Repository</th>
      <th>Branch</th>
      <th>Commit Id</th>
      <th>Commit Message</th>
      <th>Commit Message Body</th>
      <th>Committed on (Date)</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>main</td><td>4bb3de2</td><td>Initial commit</td><td>Creación inicial del repositorio del Frontend Web Application.</td><td>2026-04-25</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>main</td><td>e8abfa9</td><td>chore: set up initial Vue 3 project with Vite and Pinia</td><td>Se configura el proyecto base de Vue 3 con Vite como herramienta de build y Pinia para la gestión de estado.</td><td>2026-05-14</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>develop</td><td>887fb9c</td><td>fix: correct db.json structure</td><td>Se corrige la estructura del <code>db.json</code> utilizado como API simulada con JSON-Server.</td><td>2026-05-14</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>develop</td><td>f8b72c5</td><td>refactor: reorganize project structure - move shared to root src/</td><td>Se reorganiza la estructura del proyecto, moviendo el código compartido (<code>shared</code>) a la raíz de <code>src/</code>.</td><td>2026-05-14</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>feature/chatbot</td><td>07134af</td><td>feat: implementar modulo chatbot-bc</td><td>Se implementa la estructura base del Bounded Context de Chatbot.</td><td>2026-05-14</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>feature/sales</td><td>3393fcc</td><td>feat(sales): implementar módulo de ventas con arquitectura DDD</td><td>Se implementa el Bounded Context de Sales (ventas presenciales) siguiendo la arquitectura DDD.</td><td>2026-05-14</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>main</td><td>2b51099</td><td>Merge pull request #3 from Kauflink/feature/sales</td><td>Integración del Bounded Context de Sales a la rama principal.</td><td>2026-05-14</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>feature/subscription</td><td>31ac9a6</td><td>feat: add subscription module, i18n and routes</td><td>Se agrega el Bounded Context de Subscription con sus traducciones (i18n) y rutas.</td><td>2026-05-15</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>feature/chatbot</td><td>615eecd</td><td>feat(chatbot): add chatbot module with QR session, conversations and payment approval</td><td>Se completa el Chatbot BC con sesión por QR, conversaciones y aprobación de pago.</td><td>2026-05-15</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>develop</td><td>ec046c7</td><td>feat: add help, orders and home views with i18n keys</td><td>Se agregan las vistas de Home, Help y Orders con sus claves de internacionalización.</td><td>2026-05-15</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>feature/chatbot</td><td>0a943eb</td><td>feat(chatbot): add plin and yape receipt components</td><td>Se agregan los componentes de comprobante de Yape y Plin al Chatbot BC.</td><td>2026-05-15</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>feature/chatbot</td><td>be34115</td><td>feat(i18n): add English translations for chatbot module</td><td>Se agregan las traducciones al inglés del módulo de Chatbot.</td><td>2026-05-15</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>feature/inventory</td><td>994a1ef</td><td>feat(inventory): Agregacion de inventory BC</td><td>Se implementa el Bounded Context de Inventory (productos unitarios y por peso, lotes).</td><td>2026-05-15</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>develop</td><td>22807bc</td><td>fix: unify endpoint configuration via environment variables</td><td>Se unifica la configuración de endpoints mediante variables de entorno de Vite (<code>VITE_*</code>).</td><td>2026-05-15</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>feature/profile-configuration</td><td>418ac0b</td><td>feat(profile): add profile bounded context</td><td>Se implementa el Bounded Context de Profile (perfil y configuración del comerciante).</td><td>2026-05-15</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>feature/profile-configuration</td><td>5880670</td><td>feat(profile): connect profile context to app shell</td><td>Se conecta el Bounded Context de Profile al shell de la aplicación.</td><td>2026-05-15</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>develop</td><td>9f0d39f</td><td>fix(router): translate page titles via i18n keys</td><td>Se traducen dinámicamente los títulos de página mediante claves i18n.</td><td>2026-05-15</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>main</td><td>d87e5d0</td><td>fix: responsive zoom layout and chatbot button wrap</td><td>Se corrige el layout responsive ante zoom y el ajuste del botón del Chatbot.</td><td>2026-05-15</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>feature/inventory</td><td>40cfca5</td><td>feat(inventory): close gaps in inventory bounded context</td><td>Se cierran brechas funcionales pendientes del Inventory BC.</td><td>2026-05-16</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>develop</td><td>db3be9d</td><td>feat: add login/register flows, assets and UI updates</td><td>Se agregan los flujos de inicio de sesión y registro (UI), recursos y mejoras visuales.</td><td>2026-05-16</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>develop</td><td>317da6d</td><td>feat: env</td><td>Se agrega la configuración de variables de entorno del proyecto.</td><td>2026-05-16</td></tr>
  </tbody>
</table>

---

#### 5.2.2.5. Execution Evidence for Sprint Review

Al término del Sprint 2, el equipo implementó y desplegó el Frontend Web Application de Entreprenly en Vue. La aplicación se encuentra disponible públicamente en Firebase Hosting en la URL `https://ap.entreprenly.online`. Los Bounded Contexts implementados y sus funcionalidades clave son los siguientes:

- **DashboardLayout:** Sidebar naranja responsive con logo de Entreprenly, íconos de navegación por BC y botón de logout. Funciona como shell de la aplicación con rutas lazy-loading anidadas.

- **Sales BC — Punto de Venta:** Buscador de productos con autocompletado, modales de registro por cantidad (teclado numérico) y por peso (modo balanza IoT automático / modo manual), eliminación de ítems del ticket, selección de método de pago (Efectivo / Tarjeta-Yape-Plin), finalización de venta con modal "Venta Exitosa", y Resumen de Caja con persistencia en `db.json`.

- **Chatbot BC — Pedidos WhatsApp:** Vista de conexión de cuenta WhatsApp mediante QR escaneable con countdown de expiración, guard de sesión, lista de conversaciones activas con burbuja de escritura del cliente, gestión de órdenes con productos reales del inventario, y validación de pago con chips de rechazo.

- **Subscription BC:** Vista de planes disponibles (Plan Free y Plan Control) con precios sincronizados al selector de moneda del usuario.

- **Inventory BC:** Vista de productos y lotes con datos reales consumidos por el Sales BC (decremento de stock) y por el Home BC (alertas de lotes próximos a vencer).

- **Profile BC:** 8 tarjetas de configuración incluyendo selector de moneda (PEN/USD) y preferencias de idioma/tema que persisten en `localStorage`.

- **Home y Help:** Panel resumen del negocio con alertas reactivas al idioma activo, y centro de ayuda con artículos bilingües agrupados por categoría con conteos reales.

- **i18n:** Soporte bilingüe ES/EN en todos los BCs con traducción dinámica del título de la pestaña del navegador.

![home_p](./images/capitulo5/home_p.png "home_p")

![sales_p](./images/capitulo5/sales_p.png "sales_p")

![chatbot_p](./images/capitulo5/chatbot_p.png "chatbot_p")

![profile_p](./images/capitulo5/profile_p.png "profile_p")

![subscription_p](./images/capitulo5/subscription_p.png "subscription_p")

---

#### 5.2.2.6. Services Documentation Evidence for Sprint Review

Durante el Sprint 2, el Backend (RESTful Web Services con ASP.NET Core) aún no ha sido implementado. Por ello, la Frontend Web Application consume una API simulada mediante **JSON-Server**, que sirve el archivo `server/db.json` como una REST API completa. Esta API está disponible localmente en `http://localhost:3000/api/v1` y, adicionalmente, se desplegó una instancia remota en `http://db.entreprenly.online/api/v1` para que los datos también sean accesibles desde la aplicación publicada en Firebase. A continuación se documentan los endpoints utilizados durante este Sprint:

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th>Endpoint</th>
      <th>Verbo HTTP</th>
      <th>Descripción</th>
      <th>Parámetros</th>
      <th>Response ejemplo</th>
    </tr>
  </thead>
  <tbody>

  <!-- Inventario: productos unitarios -->
  <tr>
    <td><code>/api/v1/inventory-unit-products</code></td>
    <td>GET</td>
    <td>Retorna la lista completa de productos vendidos por unidad.</td>
    <td>Ninguno</td>
    <td><code>[{ "id": 1, "name": "Coca Cola 500ml", "price": 2.50, "productType": "unit", "codeQR": "7501055363483", "weightGrams": 500, "brand": "Coca-Cola" }]</code></td>
  </tr>
  <tr>
    <td><code>/api/v1/inventory-unit-products/:id</code></td>
    <td>GET</td>
    <td>Retorna un producto unitario específico por su ID.</td>
    <td><code>id</code>: identificador numérico del producto (path param)</td>
    <td><code>{ "id": 1, "name": "Coca Cola 500ml", "price": 2.50, "productType": "unit", "codeQR": "7501055363483", "weightGrams": 500, "brand": "Coca-Cola" }</code></td>
  </tr>
  <tr>
    <td><code>/api/v1/inventory-unit-products/:id</code></td>
    <td>PATCH</td>
    <td>Actualiza parcialmente un producto unitario (precio, descripción, etc.).</td>
    <td><code>id</code>: path param. Body: campos a actualizar, ej. <code>{ "price": 3.00 }</code></td>
    <td><code>{ "id": 1, "name": "Coca Cola 500ml", "price": 3.00, "productType": "unit", ... }</code></td>
  </tr>

  <!-- Inventario: productos a granel -->
  <tr>
    <td><code>/api/v1/inventory-weight-products</code></td>
    <td>GET</td>
    <td>Retorna la lista completa de productos vendidos por kilogramo.</td>
    <td>Ninguno</td>
    <td><code>[{ "id": 1, "name": "White Rice", "pricePerKg": 1.80, "productType": "weight", "codeQR": "WP-RICE-001" }]</code></td>
  </tr>
  <tr>
    <td><code>/api/v1/inventory-weight-products/:id</code></td>
    <td>PATCH</td>
    <td>Actualiza parcialmente un producto a granel (precio por kg, descripción, etc.).</td>
    <td><code>id</code>: path param. Body: campos a actualizar, ej. <code>{ "pricePerKg": 2.00 }</code></td>
    <td><code>{ "id": 1, "name": "White Rice", "pricePerKg": 2.00, "productType": "weight", ... }</code></td>
  </tr>

  <!-- Inventario: lotes unitarios -->
  <tr>
    <td><code>/api/v1/inventory-unit-lots</code></td>
    <td>GET</td>
    <td>Retorna todos los lotes de productos unitarios con su cantidad y fecha de vencimiento.</td>
    <td>Ninguno</td>
    <td><code>[{ "id": 1, "productId": 1, "codeQR": "LOT-CC-001", "lotType": "unit", "quantity": 80, "expiryDate": "2026-03-15T00:00:00.000Z" }]</code></td>
  </tr>
  <tr>
    <td><code>/api/v1/inventory-unit-lots/:id</code></td>
    <td>PATCH</td>
    <td>Actualiza la cantidad de un lote unitario, usado para decrementar stock tras una venta.</td>
    <td><code>id</code>: path param. Body: <code>{ "quantity": &lt;nuevo valor&gt; }</code></td>
    <td><code>{ "id": 1, "productId": 1, "quantity": 77, "expiryDate": "2026-03-15T00:00:00.000Z" }</code></td>
  </tr>

  <!-- Inventario: lotes a granel -->
  <tr>
    <td><code>/api/v1/inventory-weight-lots</code></td>
    <td>GET</td>
    <td>Retorna todos los lotes de productos a granel con su cantidad en kg.</td>
    <td>Ninguno</td>
    <td><code>[{ "id": 1, "productId": 1, "codeQR": "WLOT-RICE-001", "lotType": "weight", "quantityKg": 120 }]</code></td>
  </tr>
  <tr>
    <td><code>/api/v1/inventory-weight-lots/:id</code></td>
    <td>PATCH</td>
    <td>Actualiza la cantidad en kg de un lote a granel tras una venta o ajuste de inventario.</td>
    <td><code>id</code>: path param. Body: <code>{ "quantityKg": &lt;nuevo valor&gt; }</code></td>
    <td><code>{ "id": 1, "productId": 1, "quantityKg": 118.5, "lotType": "weight" }</code></td>
  </tr>

  <!-- Alertas de stock -->
  <tr>
    <td><code>/api/v1/inventory-stock-alerts</code></td>
    <td>GET</td>
    <td>Retorna las alertas activas de inventario: productos vencidos, por vencer, con bajo stock o agotados.</td>
    <td>Ninguno</td>
    <td><code>[{ "id": 1, "lotId": 1, "productId": 1, "alertType": "expired", "severity": "critical", "message": "Coca Cola 500ml lot #1 expired on 15/3/2026.", "createdAt": "2026-03-16T08:00:00Z" }]</code></td>
  </tr>

  <!-- Ventas -->
  <tr>
    <td><code>/api/v1/sales</code></td>
    <td>GET</td>
    <td>Retorna el historial de ventas registradas en el Punto de Venta.</td>
    <td>Ninguno</td>
    <td><code>[{ "id": 1, "date": "2026-05-12", "total": 25.50, "paymentMethod": "cash", "items": [...] }]</code></td>
  </tr>
  <tr>
    <td><code>/api/v1/sales</code></td>
    <td>POST</td>
    <td>Registra una nueva venta al finalizar el ticket en el Punto de Venta.</td>
    <td>Body: <code>{ "date", "total", "paymentMethod", "items": [{ "productId", "quantity", "subtotal" }] }</code></td>
    <td><code>{ "id": 1, "date": "2026-05-12", "total": 5.00, "paymentMethod": "cash", "items": [...] }</code> — HTTP 201</td>
  </tr>
  <tr>
    <td><code>/api/v1/cash-registers</code></td>
    <td>GET</td>
    <td>Retorna los registros de caja por fecha, con totales de efectivo, digital y conteo de ventas.</td>
    <td>Ninguno</td>
    <td><code>[{ "id": 1, "date": "2026-05-12", "totalCash": 5, "totalDigital": 0, "saleCount": 1 }]</code></td>
  </tr>
  <tr>
    <td><code>/api/v1/cash-registers/:id</code></td>
    <td>PUT</td>
    <td>Actualiza el registro de caja del día con los nuevos totales acumulados tras cada venta.</td>
    <td><code>id</code>: path param. Body: <code>{ "date", "totalCash", "totalDigital", "saleCount" }</code></td>
    <td><code>{ "id": 2, "date": "2026-05-12", "totalCash": 10, "totalDigital": 0, "saleCount": 2 }</code></td>
  </tr>

  <!-- Balanza IoT -->
  <tr>
    <td><code>/api/v1/iot-scale</code></td>
    <td>GET</td>
    <td>Retorna el estado actual de la balanza IoT (conectada o desconectada) y su identificador de dispositivo.</td>
    <td>Ninguno</td>
    <td><code>{ "id": 1, "connected": false, "deviceId": "SCALE-001" }</code></td>
  </tr>
  <tr>
    <td><code>/api/v1/iot-scale/1</code></td>
    <td>PATCH</td>
    <td>Actualiza el estado de conexión de la balanza IoT.</td>
    <td>Body: <code>{ "connected": true }</code></td>
    <td><code>{ "id": 1, "connected": true, "deviceId": "SCALE-001" }</code></td>
  </tr>

  <!-- Chatbot WhatsApp -->
  <tr>
    <td><code>/api/v1/whatsapp-sessions</code></td>
    <td>GET</td>
    <td>Retorna las sesiones de WhatsApp vinculadas al vendedor.</td>
    <td>Ninguno</td>
    <td><code>[{ "id": 1, "sellerId": 1, "phone": "+51 999 888 777", "businessName": "Bodega El Huerto", "status": "connected", "connectedAt": "11/5/2026..." }]</code></td>
  </tr>
  <tr>
    <td><code>/api/v1/conversations</code></td>
    <td>GET</td>
    <td>Retorna las conversaciones de WhatsApp con su estado: ACTIVE, WAITING_PAYMENT, COMPLETED o CLOSED.</td>
    <td>Ninguno</td>
    <td><code>[{ "id": 1, "sellerId": 1, "clientPhone": "+51 987 654 321", "clientName": "Andrea Torres", "status": "WAITING_PAYMENT", "lastMessage": "Comprobante enviado" }]</code></td>
  </tr>
  <tr>
    <td><code>/api/v1/conversations/:id</code></td>
    <td>PATCH</td>
    <td>Actualiza el estado de una conversación (ej: marcar como COMPLETED tras aprobar el pago).</td>
    <td><code>id</code>: path param. Body: <code>{ "status": "COMPLETED" }</code></td>
    <td><code>{ "id": 1, "clientName": "Andrea Torres", "status": "COMPLETED", ... }</code></td>
  </tr>
  <tr>
    <td><code>/api/v1/chat-messages</code></td>
    <td>GET</td>
    <td>Retorna los mensajes de una conversación (remitente: bot, client o system).</td>
    <td>Query param: <code>?conversationId=1</code></td>
    <td><code>[{ "id": 1, "conversationId": 1, "sender": "bot", "type": "text", "content": "Hola Andrea...", "sentAt": "2026-04-15T10:00:00.000Z" }]</code></td>
  </tr>
  <tr>
    <td><code>/api/v1/chat-orders</code></td>
    <td>GET</td>
    <td>Retorna los pedidos generados por WhatsApp con sus items, dirección de entrega y estado de pago.</td>
    <td>Ninguno</td>
    <td><code>[{ "id": 1, "conversationId": 1, "orderNumber": "#0042", "total": 7.50, "status": "WAITING_PAYMENT", "paymentMethod": "YAPE", "deliveryAddress": "Av. Los Alamos 234, Miraflores" }]</code></td>
  </tr>
  <tr>
    <td><code>/api/v1/chat-orders/:id</code></td>
    <td>PATCH</td>
    <td>Actualiza el estado de un pedido de WhatsApp (ej: CONFIRMED, BLOCKED, CANCELLED).</td>
    <td><code>id</code>: path param. Body: <code>{ "status": "CONFIRMED" }</code></td>
    <td><code>{ "id": 3, "orderNumber": "#0044", "status": "CONFIRMED", "total": 7.60, ... }</code></td>
  </tr>

  <!-- Perfil y suscripción -->
  <tr>
    <td><code>/api/v1/profile</code></td>
    <td>GET</td>
    <td>Retorna los datos del usuario, preferencias (idioma, tema, moneda) y configuración de notificaciones.</td>
    <td>Ninguno</td>
    <td><code>{ "user": { "id": 1, "role": "Administrador", "plan": "Plan Control" }, "preferences": { "language": "en", "theme": "light" }, "notification_settings": { "stock_alerts": true } }</code></td>
  </tr>
  <tr>
    <td><code>/api/v1/subscription-dashboard</code></td>
    <td>GET</td>
    <td>Retorna el plan actual, plan recomendado, límites de uso y configuración de facturación y métodos de pago.</td>
    <td>Ninguno</td>
    <td><code>[{ "id": 1, "currentPlan": { "name": "Plan Control", "status": "active", "monthlyPrice": 89 }, "limits": [...], "billingSetup": { "hasPaymentMethod": true, ... } }]</code></td>
  </tr>
  </tbody>
</table>

![json-server](./images/capitulo5/json-server.png "json-server")

![postman](./images/capitulo5/postman.png "postman")

![postman2](./images/capitulo5/postman2.png "postman2")

**URL del repositorio del Frontend Web Application:** https://github.com/Kauflink/ap-entreprenly-frontend

La documentación formal de los endpoints con OpenAPI/Swagger se incorporará a partir del Sprint 3, cuando se implemente el Backend con ASP.NET Core, conforme a lo planificado en el Product Backlog.

---

#### 5.2.2.7. Software Deployment Evidence for Sprint Review

Durante el Sprint 2, el equipo configuró y ejecutó el proceso de despliegue del Frontend Web Application mediante Firebase Hosting y un pipeline de integración continua con GitHub Actions. A continuación se describe el proceso realizado:

1. **Creación del repositorio del Frontend:** Se creó el repositorio público `ap-entreprenly-frontend` bajo la organización `Kauflink` en GitHub, aplicando GitFlow con ramas `main`, `develop` y ramas `feature/` por Bounded Context.

![repo_frontend](./images/capitulo5/repo_frontend.png "repo_frontend")

2. **Configuración de Firebase Hosting:** Se creó un proyecto en Firebase Console, se inicializó Firebase Hosting en el repositorio del frontend con `firebase init hosting`, configurando `dist` como directorio público y habilitando la reescritura de rutas al `index.html` para el SPA routing de Vue Router.

![firebase_p](./images/capitulo5/firebase_p.png "firebase_p")

3. **Verificación del despliegue:** Se validó que la aplicación Vue se encuentra correctamente desplegada y accesible en `https://ap.entreprenly.online`, con navegación entre BCs funcional sin errores 404 al refrescar el navegador.

![app_firebase](./images/capitulo5/app_firebase.png "app_firebase")

---

#### 5.2.2.8. Team Collaboration Insights during Sprint

Durante el Sprint 2, los cinco miembros del equipo participaron activamente en la implementación del Frontend Web Application, evidenciado a través de los commits y Pull Requests registrados en el repositorio `ap-entreprenly-frontend`. El trabajo se distribuyó por Bounded Context: Joseph Julius lideró la infraestructura base, el DashboardLayout, el Profile BC y la configuración del i18n y el sistema de temas; Elynor Mikela lideró el Chatbot BC y las vistas de Home y Help; José Fernando lideró el Sales BC; Lionel Abraham lideró el Subscription BC con soporte en el Inventory BzC; y José Antonio contribuyó con las traducciones del Subscription BC.

El equipo aplicó GitFlow como estrategia de control de versiones, trabajando en ramas `feature/` por Bounded Context (e.g., `feature/sales`, `feature/chatbot`, `feature/profile-configuration`, `feature/subscription`, `feature/inventory`) y realizando la integración a `develop` y `main` mediante Pull Requests. Se realizaron un total de **53 Pull Requests** durante el Sprint. La distribución de commits por miembro del equipo fue la siguiente: Camargo Briceño (87 commits), Palma De Los Santos (58 commits), Flores Pinchi (51 commits), Chavez Carrasco (49 commits) y Peirano Brun (5 commits).

![contributors_p2](./images/capitulo5/contributors_p2.png "contributors_p2")

![pull_p2](./images/capitulo5/pull_p2.png "pull_p2")

![network_g](./images/capitulo5/network_g.png "network_g")

**URL del repositorio del Frontend Web Application:** https://github.com/Kauflink/ap-entreprenly-frontend

---

### 5.2.3. Sprint 3

#### 5.2.3.1. Sprint Planning 3

Para el tercer Sprint, el equipo estableció como objetivo principal la implementación y despliegue de los **RESTful Web Services** de Entreprenly en **ASP.NET Core (C#, .NET 10)**, cubriendo todos los Bounded Contexts del backend (IAM, Profiles, Inventory, Sales, Subscription y Chatbot), y la **integración del Frontend Web Application con la API real**, reemplazando el mock de JSON-Server utilizado en el Sprint 2. La reunión de planificación se realizó de forma virtual.

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <tbody>
    <tr>
      <td colspan="2"><strong>Sprint 3</strong></td>
    </tr>
    <tr>
      <td colspan="2"><strong>Sprint Planning Background</strong></td>
    </tr>
    <tr>
      <td><strong>Date</strong></td>
      <td>2026-06-11</td>
    </tr>
    <tr>
      <td><strong>Time</strong></td>
      <td>09:00 PM</td>
    </tr>
    <tr>
      <td><strong>Location</strong></td>
      <td>Reunión virtual vía Discord</td>
    </tr>
    <tr>
      <td><strong>Prepared By</strong></td>
      <td>Camargo Briceño, Joseph Julius</td>
    </tr>
    <tr>
      <td><strong>Attendees (to planning meeting)</strong></td>
      <td>Camargo Briceño, Joseph Julius / Chavez Carrasco, Lionel Abraham / Palma De Los Santos, Elynor Mikela / Peirano Brun, José Antonio / Flores Pinchi, José Fernando</td>
    </tr>
    <tr>
      <td><strong>Sprint 2 Review Summary</strong></td>
      <td>En el Sprint 2 se implementó y desplegó la Frontend Web Application en Vue 3 + PrimeVue sobre Firebase Hosting (<a href="https://ap.entreprenly.online">ap.entreprenly.online</a>), cubriendo todos los Bounded Contexts con una API simulada mediante JSON-Server. Quedó pendiente la implementación del backend real y la integración de la aplicación con dicho backend.</td>
    </tr>
    <tr>
      <td><strong>Sprint 2 Retrospective Summary</strong></td>
      <td>El equipo confirmó que la asignación de un Bounded Context por miembro funcionó bien para el frontend. Para el Sprint 3 se acordó replicar ese esquema en el backend (un BC por responsable), tomar como referencia la arquitectura de <code>learning-center-platform</code>, y coordinar tempranamente los contratos REST para minimizar el retrabajo durante la integración frontend–backend.</td>
    </tr>
    <tr>
      <td colspan="2"><strong>Sprint Goal &amp; User Stories</strong></td>
    </tr>
    <tr>
      <td><strong>Sprint 3 Goal</strong></td>
      <td>Nuestro enfoque está en implementar y desplegar los RESTful Web Services de Entreprenly en ASP.NET Core, exponiendo los endpoints de IAM, Profiles, Inventory, Sales, Subscription y Chatbot, e integrar la Frontend Web Application con la API real. Creemos que entrega a los comerciantes una solución completamente funcional con datos persistentes, y a los desarrolladores una API documentada y desplegada. Esto se confirmará cuando la API esté desplegada en <code>ap-api.entreprenly.online</code> con su documentación Swagger disponible, y la aplicación web consuma los endpoints reales en todos los flujos clave sin depender del mock de JSON-Server.</td>
    </tr>
    <tr>
      <td><strong>Sprint 3 Velocity</strong></td>
      <td>42</td>
    </tr>
    <tr>
      <td><strong>Sum of Story Points</strong></td>
      <td>42</td>
    </tr>
  </tbody>
</table>

---

#### 5.2.3.2. Aspect Leaders and Collaborators

En el Sprint 3, el equipo replicó el esquema de un Bounded Context por responsable, esta vez sobre el backend. Los aspectos cubiertos fueron: el Shared Kernel, la infraestructura de despliegue (Docker, Cloud Run, Cloud SQL) y los BCs de IAM y Profiles; el BC de Inventory; el BC de Sales; el BC de Subscription; y el BC de Chatbot. A continuación se presenta la matriz de liderazgo y colaboración (LACX):

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th>Team Member (Last Name, First Name)</th>
      <th>GitHub Username</th>
      <th>Shared Kernel, Deploy, IAM & Profiles<br>Leader (L) / Collaborator (C)</th>
      <th>Inventory BC<br>Leader (L) / Collaborator (C)</th>
      <th>Sales BC<br>Leader (L) / Collaborator (C)</th>
      <th>Subscription BC<br>Leader (L) / Collaborator (C)</th>
      <th>Chatbot BC<br>Leader (L) / Collaborator (C)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Juyens</td>
      <td>L</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Peirano Brun, José Antonio</td>
      <td>DoomerGX</td>
      <td>C</td>
      <td>L</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Flores Pinchi, José Fernando</td>
      <td>Ferdinant12-ops</td>
      <td>C</td>
      <td>C</td>
      <td>L</td>
      <td>C</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Chavez Carrasco, Lionel Abraham</td>
      <td>LioTG</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
      <td>L</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Palma De Los Santos, Elynor Mikela</td>
      <td>elynorpalma</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
      <td>L</td>
    </tr>
  </tbody>
</table>

---

#### 5.2.3.3. Sprint Backlog 3

El objetivo principal de este Sprint fue implementar los RESTful Web Services por Bounded Context e integrarlos con el Frontend Web Application. A continuación se presentan los Work-items, organizados por aspecto, con el responsable y su estado al cierre del Sprint.

![sprint3](./images/capitulo5/sprint3.png "Tablero del Sprint 3 en Trello")

**Board público del Sprint 3 (Trello):** https://trello.com/b/kcHoLNFO/entreprenly-sprint-3

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th>Aspecto / Bounded Context</th>
      <th>Work-item / Task</th>
      <th>Estimation (Hours)</th>
      <th>Assigned To</th>
      <th>Status</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Shared Kernel</td>
      <td>Configurar el shared kernel y la configuración base de la Web API (EF Core, MySQL, mediator Cortex, manejo de errores).</td>
      <td>8</td>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>IAM</td>
      <td>Implementar el modelo de dominio de usuarios y roles, servicios de aplicación, persistencia, hashing BCrypt y autenticación JWT; exponer endpoints de authentication, users y roles; agregar cambio de contraseña y de correo.</td>
      <td>14</td>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>Profiles</td>
      <td>Implementar el modelo de dominio y value objects de perfil, auto-aprovisionamiento vía evento de integración de IAM, almacenamiento de avatar y endpoints REST de perfil y preferencias.</td>
      <td>10</td>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>Deploy / CI/CD</td>
      <td>Containerizar el backend (Dockerfile multi-etapa) y desplegarlo en Google Cloud Run construyendo la imagen con Cloud Build, conectándolo a Cloud SQL para MySQL mediante el conector nativo (socket Unix) y parametrizando la configuración con variables de entorno.</td>
      <td>10</td>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>Inventory</td>
      <td>Implementar el Bounded Context de Inventory (productos por unidad y por peso, lotes, alertas de stock) con su migración de base de datos y endpoints REST.</td>
      <td>12</td>
      <td>Peirano Brun, José Antonio</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>Sales</td>
      <td>Implementar el Bounded Context de Sales (capas de dominio, aplicación, persistencia e interfaces REST), el descuento de stock vía Inventory y el filtrado de ventas por día de negocio.</td>
      <td>12</td>
      <td>Flores Pinchi, José Fernando</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>Subscription</td>
      <td>Implementar el Bounded Context de Subscription con su migración, el mapeo de planes y datos de facturación, y los endpoints <code>me/dashboard</code> y <code>me/payment-confirmation</code>.</td>
      <td>12</td>
      <td>Chavez Carrasco, Lionel Abraham</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>Chatbot</td>
      <td>Implementar el Bounded Context de Chatbot (dominio, aplicación, infraestructura e interfaces REST), la máquina de estados de pedidos, la detección de productos contra el inventario real, el QR del bridge de WhatsApp y los endpoints de conversaciones, mensajes y pedidos.</td>
      <td>16</td>
      <td>Palma De Los Santos, Elynor Mikela</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>Integración Frontend–API</td>
      <td>Reemplazar el mock de JSON-Server por la API real: cliente HTTP autenticado con interceptor de token, alineación de modelos y assemblers por BC y parametrización de endpoints vía variables de entorno (<code>VITE_*</code>).</td>
      <td>14</td>
      <td>Equipo completo</td>
      <td>Done</td>
    </tr>
  </tbody>
</table>

---

#### 5.2.3.4. Development Evidence for Sprint Review

Durante el Sprint 3, el equipo trabajó principalmente sobre el repositorio de Web Services (`ap-entreprenly-web-services`) y, de forma complementaria, sobre el repositorio del Frontend (`ap-entreprenly-frontend`) para la integración con la API real. El trabajo se realizó entre el 12 y el 26 de junio de 2026, aplicando GitFlow con ramas `feature/` por Bounded Context. A continuación se presenta el registro de los commits más representativos:

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th>Repository</th>
      <th>Branch</th>
      <th>Commit Id</th>
      <th>Commit Message</th>
      <th>Commit Message Body</th>
      <th>Committed on (Date)</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>feature/shared-kernel</td><td>71c25cb</td><td>feat: add shared kernel and web api configuration</td><td>Se establece la base transversal compartida por todos los bounded contexts: tipo Result, primitivas de dominio, contexto EF Core MySQL y manejo global de excepciones.</td><td>2026-06-12</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>feature/iam-context</td><td>64aad46</td><td>feat(iam): expose authentication, users and roles rest endpoints</td><td>Se exponen los endpoints REST de autenticación (sign-in/sign-up), usuarios y roles del BC de IAM, con autorización por token.</td><td>2026-06-12</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>feature/profiles-context</td><td>0408620</td><td>feat(profiles): expose profile rest endpoints</td><td>Se exponen los endpoints REST del BC de Profiles: lectura, creación y actualización de perfil, preferencias y ajustes de notificación.</td><td>2026-06-12</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>feature/app-bootstrap</td><td>8f8d85a</td><td>feat(persistence): add initial database migration</td><td>Se agrega la migración inicial que crea las tablas de usuarios, roles, perfiles y user-roles con sus índices y relaciones.</td><td>2026-06-12</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>feature/deployment</td><td>2976a19</td><td>feat(deploy): containerize the backend</td><td>Se containeriza el backend con un Dockerfile multi-etapa sobre .NET 10, preparado para ejecutarse detrás de un proxy con terminación TLS.</td><td>2026-06-12</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>develop</td><td>6629653</td><td>refactor: use Cloud SQL socket connection string driven by environment variables</td><td>Se adopta la cadena de conexión por socket de Cloud SQL, parametrizada mediante variables de entorno.</td><td>2026-06-26</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>develop</td><td>cdb9937</td><td>fix: switch MySQL provider to Pomelo/MySqlConnector for Cloud SQL Unix socket support</td><td>Se cambia el proveedor de MySQL a Pomelo/MySqlConnector para soportar la conexión por socket Unix de Cloud SQL.</td><td>2026-06-26</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>develop</td><td>c639c2f</td><td>chore: remove obsolete VM deploy artifacts and add project README</td><td>Se eliminan los artefactos obsoletos del despliegue en VM y se agrega el README del proyecto.</td><td>2026-06-26</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>feature/chatbot</td><td>6211f75</td><td>feat(chatbot): add chatbot bounded context — domain, application, infrastructure and REST interfaces</td><td>Se implementa el BC de Chatbot completo (dominio, aplicación, infraestructura e interfaces REST) siguiendo la arquitectura del BC de IAM.</td><td>2026-06-13</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>feature/sales</td><td>1e278ef</td><td>feat(sales): add sales persistence and REST interfaces</td><td>Se agregan la persistencia EF Core y las interfaces REST del BC de Sales, expuestas en /api/v1/sales y /api/v1/cash-registers y documentadas en Swagger.</td><td>2026-06-15</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>feature/inventory</td><td>1cd6fa6</td><td>feat(inventory): add inventory bounded context</td><td>Se introduce el BC de Inventory con cuatro agregados (productos y lotes por unidad y por peso), alertas de stock derivadas y sus endpoints REST.</td><td>2026-06-15</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>feature/subscription</td><td>ffac4aa</td><td>feat: add Subscription bounded context and migration</td><td>Se introduce el BC de Subscription (dominio, servicios, repositorio EF Core y controlador REST) con su migración y mensajes de error localizados (EN/ES).</td><td>2026-06-15</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>feature/chatbot</td><td>a52153a</td><td>feat(chatbot): implement conversation flow with product detection and order state machine</td><td>Se implementa el flujo de conversación del chatbot con detección de productos y la máquina de estados de pedidos.</td><td>2026-06-17</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>feature/chatbot</td><td>c181a2b</td><td>feat(chatbot): wire catalog product repository to real inventory</td><td>Se conecta el repositorio de productos del chatbot al inventario real, permitiendo detectar y cotizar productos por nombre con el stock calculado del vendedor.</td><td>2026-06-18</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>develop</td><td>763b6d3</td><td>feat(subscription): add me/dashboard and me/payment-confirmation endpoints</td><td>Se agregan los endpoints me/dashboard y me/payment-confirmation del BC de Subscription.</td><td>2026-06-18</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>feature/change-credentials</td><td>26106e1</td><td>feat(iam): add change password and change email endpoints</td><td>Se exponen los endpoints autenticados de cambio de contraseña y de correo, validando la contraseña actual y rechazando correos sin cambios o ya en uso.</td><td>2026-06-19</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>feature/connect-backend</td><td>46ccfa0</td><td>feat(auth): add IAM session store, API client and token interceptor</td><td>Se agrega la autenticación real: cliente de API de auth, store Pinia que persiste el JWT y un interceptor axios que adjunta el token Bearer a cada petición.</td><td>2026-06-12</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>develop</td><td>e5e0ef1</td><td>feat(sales): align sales domain models and assemblers with backend contract</td><td>Se alinean los modelos y assemblers de ventas del frontend con el contrato de la API de Sales en C#/.NET (métodos de pago, estados e ítems con cantidad/peso).</td><td>2026-06-15</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>develop</td><td>b8f2e57</td><td>feat(chatbot): connect store and API to real backend endpoints</td><td>Se conecta el store y la API del chatbot del frontend a los endpoints reales del backend.</td><td>2026-06-15</td></tr>
    <tr><td>Kauflink/ap-entreprenly-frontend</td><td>develop</td><td>5f76582</td><td>fix(dashboard): route home API calls through authenticated client</td><td>Se enrutan las llamadas del dashboard por el cliente autenticado (SalesApi/InventoryApi) para adjuntar el token JWT y evitar los errores 401.</td><td>2026-06-18</td></tr>
  </tbody>
</table>

---

#### 5.2.3.5. Execution Evidence for Sprint Review

Al término del Sprint 3, la Frontend Web Application consume la API real desplegada en `https://ap-api.entreprenly.online/api/v1`, con persistencia en MySQL y autenticación JWT. Los flujos clave —registro e inicio de sesión, gestión de inventario y lotes, registro de ventas en el punto de venta, gestión de la suscripción y atención de pedidos por el chatbot de WhatsApp— operan sobre datos persistentes reales. A continuación se incluyen las capturas de las principales vistas funcionando contra el backend.

<img src="images/capitulo5/exec_s3_login.png" width="600">

<img src="images/capitulo5/exec_s3_inventory.png" width="600">

<img src="images/capitulo5/exec_s3_sales.png" width="600">

<img src="images/capitulo5/exec_s3_subscription.png" width="600">

<img src="images/capitulo5/exec_s3_chatbot.png" width="600">

---

#### 5.2.3.6. Services Documentation Evidence for Sprint Review

A diferencia del Sprint 2, en el que la Frontend Web Application consumía una Fake RESTful API servida con **JSON-Server**, en el Sprint 3 se implementó el Backend real con **ASP.NET Core** y se documentó formalmente mediante **OpenAPI/Swagger** (Swashbuckle). La especificación OpenAPI está disponible en `https://ap-api.entreprenly.online/swagger/v1/swagger.json` y la interfaz interactiva de exploración y prueba (Swagger UI) en `https://ap-api.entreprenly.online/swagger`.

La API expone **72 operaciones** distribuidas en **19 controladores REST** a través de 6 Bounded Contexts. Todos los endpoints de negocio están protegidos con **JWT** (esquema `Bearer`); únicamente el `sign-in` y el `sign-up` quedan fuera de esa protección. Los endpoints del webhook/bridge de WhatsApp se documentan en la sección del Sprint 4 (5.2.4.6). A continuación se documentan los endpoints implementados por Bounded Context:

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th>Bounded Context</th>
      <th>Endpoint</th>
      <th>Verbo(s) HTTP</th>
      <th>Descripción</th>
      <th>Autenticación</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>IAM / Authentication</td><td><code>/api/v1/authentication/sign-in</code></td><td>POST</td><td>Autentica al usuario por email y contraseña y retorna un token JWT.</td><td>No (anónimo)</td></tr>
    <tr><td>IAM / Authentication</td><td><code>/api/v1/authentication/sign-up</code></td><td>POST</td><td>Registra una nueva cuenta y aprovisiona su perfil y suscripción por defecto.</td><td>No (anónimo)</td></tr>
    <tr><td>IAM</td><td><code>/api/v1/users</code> · <code>/api/v1/users/{id}</code></td><td>GET</td><td>Lista los usuarios y obtiene uno por su identificador.</td><td>JWT</td></tr>
    <tr><td>IAM</td><td><code>/api/v1/users/me/password</code></td><td>PUT</td><td>Cambia la contraseña del usuario autenticado (valida la actual).</td><td>JWT</td></tr>
    <tr><td>IAM</td><td><code>/api/v1/users/me/email</code></td><td>PUT</td><td>Cambia el correo del usuario autenticado.</td><td>JWT</td></tr>
    <tr><td>IAM</td><td><code>/api/v1/roles</code></td><td>GET</td><td>Lista los roles disponibles en el sistema.</td><td>JWT</td></tr>
    <tr><td>Profiles</td><td><code>/api/v1/profiles</code></td><td>GET / POST</td><td>Lista y crea perfiles de comerciante.</td><td>JWT</td></tr>
    <tr><td>Profiles</td><td><code>/api/v1/profiles/{profileId}</code></td><td>GET / PUT</td><td>Consulta y actualiza el perfil del comerciante.</td><td>JWT</td></tr>
    <tr><td>Profiles</td><td><code>/api/v1/profiles/by-user/{userId}</code></td><td>GET</td><td>Obtiene el perfil asociado a un usuario.</td><td>JWT</td></tr>
    <tr><td>Profiles</td><td><code>/api/v1/profiles/{profileId}/preferences</code></td><td>PUT</td><td>Actualiza idioma, tema y moneda del comerciante.</td><td>JWT</td></tr>
    <tr><td>Profiles</td><td><code>/api/v1/profiles/{profileId}/notification-settings</code></td><td>PUT</td><td>Actualiza las preferencias de notificación.</td><td>JWT</td></tr>
    <tr><td>Inventory</td><td><code>/api/v1/inventory-unit-products</code></td><td>GET / POST / PUT / DELETE</td><td>Gestiona los productos vendidos por unidad (CRUD).</td><td>JWT</td></tr>
    <tr><td>Inventory</td><td><code>/api/v1/inventory-weight-products</code></td><td>GET / POST / PUT / DELETE</td><td>Gestiona los productos vendidos por kilogramo (CRUD).</td><td>JWT</td></tr>
    <tr><td>Inventory</td><td><code>/api/v1/inventory-unit-lots</code></td><td>GET / POST / PUT / DELETE</td><td>Gestiona los lotes de productos unitarios (CRUD).</td><td>JWT</td></tr>
    <tr><td>Inventory</td><td><code>/api/v1/inventory-weight-lots</code></td><td>GET / POST / PUT / DELETE</td><td>Gestiona los lotes de productos a granel (CRUD).</td><td>JWT</td></tr>
    <tr><td>Inventory</td><td><code>/api/v1/inventory-lots</code></td><td>GET</td><td>Retorna la vista combinada de lotes; <code>/{lotId}</code> para el detalle.</td><td>JWT</td></tr>
    <tr><td>Inventory</td><td><code>/api/v1/inventory-stock-alerts</code></td><td>GET</td><td>Retorna las alertas de stock derivadas (vencido, por vencer, bajo, agotado).</td><td>JWT</td></tr>
    <tr><td>Sales</td><td><code>/api/v1/sales</code></td><td>POST / GET</td><td>Registra una venta (descontando stock) y lista las ventas; filtro opcional <code>?date</code>.</td><td>JWT</td></tr>
    <tr><td>Sales</td><td><code>/api/v1/sales/{saleId}</code></td><td>GET</td><td>Obtiene el detalle de una venta.</td><td>JWT</td></tr>
    <tr><td>Sales</td><td><code>/api/v1/sales-products</code></td><td>GET</td><td>Catálogo de productos disponibles para registrar en una venta.</td><td>JWT</td></tr>
    <tr><td>Subscription</td><td><code>/api/v1/subscriptions/me/dashboard</code></td><td>GET / PUT</td><td>Consulta y actualiza el dashboard de suscripción del usuario autenticado.</td><td>JWT</td></tr>
    <tr><td>Subscription</td><td><code>/api/v1/subscriptions/me/payment-confirmation</code></td><td>GET</td><td>Obtiene el estado de confirmación de pago del usuario autenticado.</td><td>JWT</td></tr>
    <tr><td>Subscription</td><td><code>/api/v1/subscriptions/active</code></td><td>GET</td><td>Retorna la suscripción activa.</td><td>JWT</td></tr>
    <tr><td>Subscription</td><td><code>/api/v1/subscriptions/by-user/{userId}/billing-setup</code></td><td>PUT</td><td>Registra los datos de facturación y el método de pago.</td><td>JWT</td></tr>
    <tr><td>Subscription</td><td><code>/api/v1/subscriptions/by-user/{userId}/activate-control</code></td><td>POST</td><td>Activa el plan Control para el usuario.</td><td>JWT</td></tr>
    <tr><td>Subscription</td><td><code>/api/v1/subscriptions/by-user/{userId}/schedule-cancellation</code> · <code>/keep-control</code></td><td>POST</td><td>Programa la cancelación al fin del período o revierte dicha cancelación.</td><td>JWT</td></tr>
    <tr><td>Chatbot</td><td><code>/api/v1/conversations</code></td><td>GET / POST</td><td>Lista, crea y consulta (<code>/{id}</code>) las conversaciones.</td><td>JWT</td></tr>
    <tr><td>Chatbot</td><td><code>/api/v1/chat-messages</code></td><td>GET / POST</td><td>Registra y lista mensajes; <code>/by-conversation/{conversationId}</code> filtra por conversación.</td><td>JWT</td></tr>
    <tr><td>Chatbot</td><td><code>/api/v1/chat-orders</code></td><td>GET / POST</td><td>Gestiona los pedidos generados por el chatbot; <code>/{id}</code> para el detalle.</td><td>JWT</td></tr>
    <tr><td>Chatbot</td><td><code>/api/v1/chat-orders/{id}/confirm</code> · <code>/reject</code></td><td>POST</td><td>Aprueba (tras validar el comprobante) o rechaza un pedido.</td><td>JWT</td></tr>
    <tr><td>Chatbot</td><td><code>/api/v1/whatsapp-sessions</code></td><td>GET / POST</td><td>Gestiona las sesiones de WhatsApp del comerciante.</td><td>JWT</td></tr>
  </tbody>
</table>

**Sintaxis, parámetros y ejemplos de response.** Los identificadores de recurso se pasan como *path parameters* (por ejemplo `{userId}`, `{profileId}`, `{saleId}`) y algunos listados aceptan *query parameters* (por ejemplo `GET /api/v1/sales?date=2026-06-18`). A continuación se muestran dos interacciones representativas con datos de muestra.

*Ejemplo 1 — Autenticación (`POST /api/v1/authentication/sign-in`).* Recibe email y contraseña; retorna el usuario y el token JWT.

```http
POST /api/v1/authentication/sign-in
Content-Type: application/json

{ "email": "comerciante@entreprenly.com", "password": "MiClaveSegura123" }
```
```json
// 200 OK
{
  "id": 12,
  "email": "comerciante@entreprenly.com",
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9..."
}
```
El `token` retornado debe enviarse como `Authorization: Bearer <token>` en las peticiones a endpoints protegidos. Credenciales inválidas retornan `401 Unauthorized`.

*Ejemplo 2 — Registro de venta (`POST /api/v1/sales`).* Cada ítem se indica por `quantity` (productos por unidad) o por `weightKg` (productos por peso). El backend resuelve el `unitPrice`, calcula `subtotal` y `total`, y descuenta el stock del inventario del vendedor.

```http
POST /api/v1/sales
Authorization: Bearer <token>
Content-Type: application/json

{
  "sellerId": 12,
  "items": [
    { "productId": 3, "quantity": 2 },
    { "productId": 7, "weightKg": 1.5 }
  ],
  "paymentMethod": "YAPE"
}
```
```json
// 201 Created
{
  "id": 45,
  "sellerId": 12,
  "items": [
    { "productId": 3, "productName": "Arroz 1kg",   "quantity": 2,    "weightKg": null, "unitPrice": 4.50, "subtotal": 9.00 },
    { "productId": 7, "productName": "Azúcar rubia", "quantity": null, "weightKg": 1.5,  "unitPrice": 5.20, "subtotal": 7.80 }
  ],
  "total": 16.80,
  "paymentMethod": "YAPE",
  "paymentReceipt": null,
  "status": "COMPLETED"
}
```
Una petición con parámetros faltantes o con ítems sin stock suficiente retorna `400 Bad Request` con un cuerpo *problem-details* que describe el error.

A continuación se muestra la interfaz Swagger UI con la relación de endpoints y una ejecución de prueba (*Try it out*) con datos de muestra:

<img src="./images/capitulo5/swagger_s3.png" width="600">

<img src="./images/capitulo5/swagger_s3_prueba.png" width="600">

**URL del repositorio de Web Services:** https://github.com/Kauflink/ap-entreprenly-web-services

**Commits relacionados con la documentación (Sprint 3):** las anotaciones OpenAPI (`SwaggerSchema`, descripciones de operaciones y *problem-details*) se incorporaron dentro de los commits de cada Bounded Context; la configuración del esquema de seguridad `Bearer` para Swagger UI se realizó en el commit `cd2d1ff` (`fix(swagger): match bearer security scheme name so authorize sends token`, 2026-06-19).

---

#### 5.2.3.7. Software Deployment Evidence for Sprint Review

Durante el Sprint 3 se configuró y ejecutó el despliegue del RESTful Web Services. El proceso (detallado en la sección 5.1.4) consistió en: construir la imagen Docker multi-etapa del backend (`mcr.microsoft.com/dotnet/sdk:10.0` → `aspnet:10.0`) mediante **Cloud Build**, publicarla en **Google Artifact Registry** y desplegarla en **Google Cloud Run** (servicio `ap-entreprenly-web-services`, región `us-east1`, con *allow unauthenticated*, 1 vCPU, 1 GiB y *startup CPU boost*). La persistencia se realiza sobre **Cloud SQL para MySQL 8.4** (instancia `entreprenly-db`), a la que Cloud Run se conecta mediante el **conector nativo de Cloud SQL** (socket Unix), consumido por **EF Core** con el proveedor **Pomelo/MySqlConnector**. El API quedó disponible en `https://ap-api.entreprenly.online`, con su documentación Swagger en `https://ap-api.entreprenly.online/swagger`.

<img src="./images/capitulo5/deploy-backend-09.png" width="600">

<img src="./images/capitulo5/deploy-backend-11.png" width="600">

---

#### 5.2.3.8. Team Collaboration Insights during Sprint

Durante el Sprint 3, los cinco miembros del equipo participaron en la implementación del backend y su integración con el frontend. El trabajo se distribuyó por Bounded Context en el repositorio `ap-entreprenly-web-services`: Joseph Julius lideró el Shared Kernel, la infraestructura de despliegue (Docker, Cloud Run, Cloud SQL) y los BCs de IAM y Profiles; José Antonio lideró el BC de Inventory; José Fernando lideró el BC de Sales; Lionel Abraham lideró el BC de Subscription; y Elynor Mikela lideró el BC de Chatbot. La integración del frontend con la API real se realizó de forma colaborativa, cada miembro sobre su BC.

El equipo aplicó GitFlow con ramas `feature/` por Bounded Context (`feature/iam-context`, `feature/profiles-context`, `feature/inventory`, `feature/sales`, `feature/subscription`, `feature/chatbot`, `feature/deployment`) integradas a `develop` y `main` mediante Pull Requests (más de 20 PRs en el repositorio de Web Services). La distribución aproximada de commits en el backend fue: Camargo Briceño (37), Palma De Los Santos (25), Chavez Carrasco (12), Flores Pinchi (6) y Peirano Brun (3).

<img src="./images/capitulo5/collab_s3_1.png" width="600">

<img src="./images/capitulo5/collab_s3_2.png" width="600">

---

### 5.2.4. Sprint 4

#### 5.2.4.1. Sprint Planning 4

Para este cuarto y último Sprint, el equipo estableció como objetivo principal la integración del **canal real de WhatsApp** para el chatbot de Entreprenly mediante un **WhatsApp bridge multi-tenant**, conectando la lógica de pedidos ya implementada en el Backend con conversaciones reales de clientes, y desplegando la versión final de los tres productos digitales. La reunión de planificación se llevó a cabo de manera virtual, donde se definieron las User Stories a abordar, el Sprint Goal y la distribución de responsabilidades.

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <tbody>
    <tr><td colspan="2"><strong>Sprint 4</strong></td></tr>
    <tr><td colspan="2"><strong>Sprint Planning Background</strong></td></tr>
    <tr><td><strong>Date</strong></td><td>2026-06-04</td></tr>
    <tr><td><strong>Time</strong></td><td>09:00 AM</td></tr>
    <tr><td><strong>Location</strong></td><td>Reunión virtual vía Discord</td></tr>
    <tr><td><strong>Prepared By</strong></td><td>Camargo Briceño, Joseph Julius</td></tr>
    <tr><td><strong>Attendees (to planning meeting)</strong></td><td>Camargo Briceño, Joseph Julius / Chavez Carrasco, Lionel Abraham / Palma De Los Santos, Elynor Mikela / Peirano Brun, José Antonio / Flores Pinchi, José Fernando</td></tr>
    <tr><td><strong>Sprint 3 Review Summary</strong></td><td>En el Sprint 3 se implementó y desplegó el Backend real con ASP.NET Core sobre Google Cloud Run, con base de datos en Cloud SQL para MySQL, autenticación JWT, persistencia con Entity Framework Core por bounded context y la lógica del flujo de pedidos del chatbot (US-41 a US-52). El Frontend se integró con la API real reemplazando la Fake API del Sprint 2.</td></tr>
    <tr><td><strong>Sprint 3 Retrospective Summary</strong></td><td>El equipo identificó que, si bien la lógica del chatbot residía en el Backend, faltaba la integración con WhatsApp real: las conversaciones seguían siendo simuladas. Para el Sprint 4 se acordó implementar un WhatsApp bridge multi-tenant con <code>whatsapp-web.js</code>, conectar el canal real (vinculación por QR, recepción de mensajes y de comprobantes por imagen, y envío de respuestas al cliente) y desplegar la versión final de los tres productos.</td></tr>
    <tr><td colspan="2"><strong>Sprint Goal &amp; User Stories</strong></td></tr>
    <tr><td><strong>Sprint 4 Goal</strong></td><td>Nuestro enfoque está en habilitar la atención real de clientes por WhatsApp, conectando el chatbot de Entreprenly a cuentas reales mediante un bridge multi-tenant. Creemos que entrega valor inmediato al comerciante al automatizar consultas de productos, pedidos y validación de pagos digitales directamente sobre WhatsApp. Esto se confirmará cuando un cliente pueda vincular su WhatsApp por código QR, conversar con el bot, enviar su comprobante de pago como imagen y recibir la confirmación de su pedido de extremo a extremo. User Stories: US-37, US-38, US-44, US-45 y US-47.</td></tr>
    <tr><td><strong>Sprint 4 Velocity</strong></td><td>14</td></tr>
    <tr><td><strong>Sum of Story Points</strong></td><td>14</td></tr>
  </tbody>
</table>

---

#### 5.2.4.2. Aspect Leaders and Collaborators

En el Sprint 4, el equipo organizó el trabajo en torno a cuatro aspectos: el **WhatsApp Bridge multi-tenant**, la **integración del Chatbot en el Backend**, la **integración del Chatbot en el Frontend** y el **despliegue final con enrutamiento multi-backend** (página `/switch`). A continuación se presenta la matriz de liderazgo y colaboración (LACX):

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th>Team Member (Last Name, First Name)</th>
      <th>GitHub Username</th>
      <th>WhatsApp Bridge<br>Leader (L) / Collaborator (C)</th>
      <th>Chatbot Backend<br>Leader (L) / Collaborator (C)</th>
      <th>Chatbot Frontend<br>Leader (L) / Collaborator (C)</th>
      <th>Despliegue final y Switch<br>Leader (L) / Collaborator (C)</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Camargo Briceño, Joseph Julius</td><td>Juyens</td><td>C</td><td>L</td><td>C</td><td>L</td></tr>
    <tr><td>Chavez Carrasco, Lionel Abraham</td><td>LioTG</td><td>C</td><td>C</td><td>C</td><td>C</td></tr>
    <tr><td>Palma De Los Santos, Elynor Mikela</td><td>elynorpalma</td><td>L</td><td>C</td><td>L</td><td>C</td></tr>
    <tr><td>Peirano Brun, José Antonio</td><td>DoomerGX</td><td>C</td><td>C</td><td>C</td><td>C</td></tr>
    <tr><td>Flores Pinchi, José Fernando</td><td>Ferdinant12-ops</td><td>C</td><td>C</td><td>C</td><td>C</td></tr>
  </tbody>
</table>

---

#### 5.2.4.3. Sprint Backlog 4

El objetivo principal de este Sprint fue integrar el canal real de WhatsApp para el chatbot, cubriendo las User Stories **US-37, US-38, US-44, US-45 y US-47**, que se realizaron de forma efectiva mediante el WhatsApp bridge (en Sprints previos US-37, US-38 y US-45 se abordaron de forma simulada o solo en el Backend). Cada historia se descompuso en Engineering Tasks con una estimación individual de entre 4 y 8 horas, gestionadas en el tablero Kanban del Sprint con las columnas **To Do, In Process, To Review y Done**.

![sprint4](./images/capitulo5/sprint4.png "Tablero del Sprint 4 en Trello")

**Board público del Sprint 4 (Trello):** https://trello.com/b/msBZdIfS/entreprenly-sprint-4

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th colspan="8">Sprint # Sprint 4</th>
    </tr>
    <tr>
      <th colspan="2">User Story</th>
      <th colspan="6">Work-Item / Task</th>
    </tr>
    <tr>
      <th>Id</th><th>Title</th><th>Id</th><th>Title</th><th>Description</th><th>Estimation (Hours)</th><th>Assigned To</th><th>Status</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>US-37</td>
      <td>Vincular cuenta de WhatsApp Business mediante código QR</td>
      <td>T-01</td>
      <td>Implementar el WhatsApp bridge con whatsapp-web.js</td>
      <td>Construir el servicio bridge en Node.js con <code>whatsapp-web.js</code> que genera el código QR y mantiene la sesión de WhatsApp Web.</td>
      <td>8</td>
      <td>Palma De Los Santos, Elynor Mikela</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-37</td>
      <td>Vincular cuenta de WhatsApp Business mediante código QR</td>
      <td>T-02</td>
      <td>Reconciliar el estado de vinculación desde el QR</td>
      <td>Relevar el QR real hacia el Backend y reconciliar el estado de vinculación a partir de la respuesta del sondeo (poll) del bridge.</td>
      <td>5</td>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-37</td>
      <td>Vincular cuenta de WhatsApp Business mediante código QR</td>
      <td>T-03</td>
      <td>Habilitar sesión de WhatsApp por vendedor (multi-tenant)</td>
      <td>Mantener una sesión de WhatsApp independiente por email de vendedor, para que cada comerciante vincule su propia cuenta.</td>
      <td>6</td>
      <td>Palma De Los Santos, Elynor Mikela</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-38</td>
      <td>Consultar estado de vinculación del chatbot</td>
      <td>T-04</td>
      <td>Exponer y consultar el estado de conexión del bridge</td>
      <td>Reportar el estado de conexión del bridge al Backend y agregar el endpoint de desconexión que limpia el estado y notifica el logout.</td>
      <td>5</td>
      <td>Palma De Los Santos, Elynor Mikela</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-44</td>
      <td>Recibir instrucciones de pago por WhatsApp</td>
      <td>T-05</td>
      <td>Enviar mensajes salientes al cliente (POST /send)</td>
      <td>Agregar el endpoint <code>POST /send</code> del bridge para que el Backend empuje mensajes salientes (incluidas las instrucciones de pago) al cliente por WhatsApp.</td>
      <td>5</td>
      <td>Palma De Los Santos, Elynor Mikela</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-45</td>
      <td>Reportar comprobante de pago digital</td>
      <td>T-06</td>
      <td>Reenviar imágenes de WhatsApp como comprobantes</td>
      <td>Detectar los mensajes de imagen entrantes y reenviarlos al Backend como comprobantes de pago, usando un centinela para no saturar los eventos SSE con el base64.</td>
      <td>6</td>
      <td>Palma De Los Santos, Elynor Mikela</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-47</td>
      <td>Notificar resultado de validación al cliente</td>
      <td>T-07</td>
      <td>Notificar el resultado de la validación por WhatsApp</td>
      <td>Enviar al cliente, a través del bridge, la confirmación o el rechazo del pago tras la validación del comprobante desde el dashboard.</td>
      <td>4</td>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-47</td>
      <td>Notificar resultado de validación al cliente</td>
      <td>T-08</td>
      <td>Enrutar el canal a uno de dos backends (switch)</td>
      <td>Implementar el enrutamiento del canal de WhatsApp hacia uno de dos backends con un turno conmutable y una página <code>/switch</code>, re-sincronizando el estado de la sesión.</td>
      <td>6</td>
      <td>Camargo Briceño, Joseph Julius</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-37</td>
      <td>Vincular cuenta de WhatsApp Business mediante código QR</td>
      <td>T-09</td>
      <td>Containerizar y desplegar el bridge</td>
      <td>Crear el <code>Dockerfile</code> del bridge y automatizar su despliegue en una instancia de Compute Engine (VM) ante cada push a <code>main</code>.</td>
      <td>5</td>
      <td>Palma De Los Santos, Elynor Mikela</td>
      <td>Done</td>
    </tr>
  </tbody>
</table>

---

#### 5.2.4.4. Development Evidence for Sprint Review

Durante el Sprint 4, el equipo trabajó principalmente sobre el repositorio del **WhatsApp bridge** (`daop-entreprenly-whatsapp-bridge`) y realizó ajustes de integración en el **Backend** (`ap-entreprenly-web-services`) y el **Frontend** (`ap-entreprenly-frontend`). El bridge acumuló **13 commits** (sin contar merges) entre el 5 y el 26 de junio de 2026. A continuación se presenta el registro de los commits más representativos:

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th>Repository</th>
      <th>Branch</th>
      <th>Commit Id</th>
      <th>Commit Message</th>
      <th>Commit Message Body</th>
      <th>Committed on (Date)</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Kauflink/daop-entreprenly-whatsapp-bridge</td><td>main</td><td>a78855b</td><td>feat: WhatsApp bridge (whatsapp-web.js) for the Entreprenly chatbot</td><td>Se crea el servicio bridge en Node.js con whatsapp-web.js como base del canal de WhatsApp.</td><td>2026-06-05</td></tr>
    <tr><td>Kauflink/daop-entreprenly-whatsapp-bridge</td><td>main</td><td>f1d9226</td><td>feat(bridge): multi-tenant — one WhatsApp session per seller email</td><td>Se habilita una sesión de WhatsApp independiente por email de vendedor.</td><td>2026-06-09</td></tr>
    <tr><td>Kauflink/daop-entreprenly-whatsapp-bridge</td><td>main</td><td>26202b2</td><td>feat(bridge): add POST /send endpoint to push outbound messages from backend to clients</td><td>Se agrega el endpoint POST /send para enviar mensajes salientes al cliente por WhatsApp.</td><td>2026-06-09</td></tr>
    <tr><td>Kauflink/daop-entreprenly-whatsapp-bridge</td><td>main</td><td>c9cbff6</td><td>feat: forward WhatsApp image messages as payment receipts</td><td>Se reenvían las imágenes entrantes de WhatsApp al Backend como comprobantes de pago.</td><td>2026-06-09</td></tr>
    <tr><td>Kauflink/daop-entreprenly-whatsapp-bridge</td><td>main</td><td>8f788e7</td><td>feat(docker): add Dockerfile and dockerignore for VM deployment</td><td>Se containeriza el bridge para su despliegue en una VM.</td><td>2026-06-09</td></tr>
    <tr><td>Kauflink/daop-entreprenly-whatsapp-bridge</td><td>main</td><td>0eaae2e</td><td>ci: auto-deploy bridge to Compute Engine VM on push to main</td><td>Se automatiza el despliegue del bridge en Compute Engine ante cada push a main.</td><td>2026-06-10</td></tr>
    <tr><td>Kauflink/daop-entreprenly-whatsapp-bridge</td><td>main</td><td>83df0e6</td><td>feat: route WhatsApp to one of two backends with a switchable turn and /switch page</td><td>Se enruta el canal a uno de dos backends con turno conmutable y una página /switch.</td><td>2026-06-26</td></tr>
    <tr><td>Kauflink/daop-entreprenly-whatsapp-bridge</td><td>main</td><td>f802a49</td><td>fix: clean stale Chromium singleton locks on container startup</td><td>Se limpian los locks obsoletos de Chromium al iniciar el contenedor para estabilizar el arranque.</td><td>2026-06-26</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>develop</td><td>3d5d18f</td><td>feat(chatbot): reconcile bridge link state from QR poll response</td><td>Se reconcilia el estado de vinculación del bridge a partir del sondeo del QR.</td><td>2026-06-16</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>develop</td><td>1ceb0a8</td><td>feat(chatbot): expand rule-based responder with more intents</td><td>Se amplía el responder basado en reglas con más intenciones para las consultas de clientes.</td><td>2026-06-16</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>develop</td><td>7a992ea</td><td>fix(chatbot): suggest catalog alternatives when requested product not found</td><td>Se sugieren alternativas del catálogo cuando el producto solicitado no está disponible.</td><td>2026-06-16</td></tr>
    <tr><td>Kauflink/ap-entreprenly-web-services</td><td>develop</td><td>fff996b</td><td>fix(chatbot): add disconnect endpoint to clear bridge state and notify bridge logout</td><td>Se agrega el endpoint de desconexión que limpia el estado del bridge y notifica el logout.</td><td>2026-06-17</td></tr>
  </tbody>
</table>

**URL del repositorio del WhatsApp Bridge:** https://github.com/Kauflink/daop-entreprenly-whatsapp-bridge

<img src="images/capitulo5/bridge_evi.png" width="800">

---

#### 5.2.4.5. Execution Evidence for Sprint Review

Al término del Sprint 4, el chatbot de Entreprenly quedó operativo sobre **WhatsApp real** mediante el bridge multi-tenant. El flujo funcional de extremo a extremo es el siguiente:

- **Vinculación por QR (US-37):** el comerciante escanea el código QR desde el dashboard para vincular su cuenta de WhatsApp; cada vendedor mantiene su propia sesión (multi-tenant).

![sprint4_chatbot_qr](./images/capitulo5/sprint4_chatbot_qr.png "sprint4_chatbot_qr")

- **Estado de vinculación (US-38):** el dashboard consulta y refleja el estado de conexión del bridge, con opción de desconexión.

![sprint4_chatbot_state](./images/capitulo5/sprint4_chatbot_state.png "sprint4_chatbot_state")

- **Atención automatizada:** el bot responde consultas de productos con datos reales del inventario y sugiere alternativas cuando un producto no está disponible.

![sprint4_chatbot_demo](./images/capitulo5/sprint4_chatbot_demo.png "Conversación real del chatbot por WhatsApp")

- **Instrucciones de pago (US-44):** el Backend envía al cliente, vía `POST /send` del bridge, las instrucciones de pago para completar su pedido.

![sprint4_chatbot_pedido](./images/capitulo5/sprint4_chatbot_pedido.png "sprint4_chatbot_pedido")

- **Comprobante por imagen (US-45):** el cliente envía la foto de su comprobante por WhatsApp y el bridge la reenvía al Backend como comprobante de pago.

![sprint4_chatbot_comprobante](./images/capitulo5/sprint4_chatbot_comprobante.png "sprint4_chatbot_comprobante")

- **Notificación de validación (US-47):** tras aprobar o rechazar el comprobante desde el dashboard, el resultado se notifica al cliente por WhatsApp.

![sprint4_chatbot_aprobado](./images/capitulo5/sprint4_chatbot_aprobado.png "sprint4_chatbot_aprobado")

---

#### 5.2.4.6. Services Documentation Evidence for Sprint Review

La comunicación entre el Backend y el canal de WhatsApp se realiza a través del **WhatsApp bridge**, cuyos endpoints se documentan a continuación. Los endpoints del bridge se autentican con un **token de bridge dedicado**, y los endpoints del Backend asociados (webhook y relay) ya forman parte de la especificación OpenAPI/Swagger documentada en el Sprint 3.

<table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th>Componente</th>
      <th>Endpoint</th>
      <th>Verbo HTTP</th>
      <th>Descripción</th>
      <th>Autenticación</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Backend ← Bridge</td><td><code>/api/v1/chatbot/whatsapp/bridge/qr</code></td><td>POST</td><td>El bridge releva el último QR de emparejamiento al Backend.</td><td>Token de bridge</td></tr>
    <tr><td>Backend ← Bridge</td><td><code>/api/v1/chatbot/whatsapp/bridge/status</code></td><td>POST</td><td>El bridge reporta el estado de conexión de la sesión.</td><td>Token de bridge</td></tr>
    <tr><td>Frontend → Backend</td><td><code>/api/v1/chatbot/whatsapp/qr?ownerEmail={email}</code></td><td>GET</td><td>El dashboard obtiene el QR actual y el estado de vinculación de la sesión del vendedor.</td><td>No (anónimo)</td></tr>
    <tr><td>Backend ← Bridge</td><td><code>/api/v1/chatbot/whatsapp/webhook</code></td><td>POST</td><td>Recibe un mensaje entrante de WhatsApp (texto o imagen).</td><td>Token de bridge</td></tr>
    <tr><td>Backend ← Bridge</td><td><code>/api/v1/chatbot/whatsapp/webhook/receipt</code></td><td>POST</td><td>Recibe un comprobante de pago (imagen) enviado por el cliente.</td><td>Token de bridge</td></tr>
    <tr><td>Backend → Bridge</td><td><code>/send</code></td><td>POST</td><td>El Backend empuja un mensaje saliente hacia el cliente por WhatsApp.</td><td>Token de bridge</td></tr>
  </tbody>
</table>

**URL del repositorio de Web Services:** https://github.com/Kauflink/ap-entreprenly-web-services

**Commit relacionado con la documentación (Sprint 4):** `bba48f8` (`docs(chatbot): add descriptions to all endpoint operations`, 2026-07-09), que completa las descripciones OpenAPI de las operaciones del Chatbot.

---

#### 5.2.4.7. Software Deployment Evidence for Sprint Review

Durante el Sprint 4, el equipo desplegó el **WhatsApp bridge** de forma containerizada con Docker sobre una instancia de **Google Compute Engine (VM)**, con despliegue automatizado ante cada push a `main`. El bridge se comunica con el Backend desplegado en Google Cloud Run y expone la página `/switch` para el enrutamiento entre backends. Con esto quedó desplegada la **versión final** de los tres productos digitales (Landing Page, Frontend y Web Services) más el canal de WhatsApp. El proceso realizado fue el siguiente:

1. **Containerización del bridge:** Se creó un `Dockerfile` para el servicio Node.js con `whatsapp-web.js` y las dependencias de Chromium necesarias para WhatsApp Web.

![sprint4_bridge_docker](./images/capitulo5/sprint4_bridge_docker.png "sprint4_bridge_docker")

2. **Despliegue automatizado en la VM:** Se configuró el despliegue automático del bridge en una instancia de Compute Engine ante cada push a `main`.

![sprint4_bridge_vm](./images/capitulo5/sprint4_bridge_vm.png "sprint4_bridge_vm")

![sprint4_bridge_deploy](./images/capitulo5/sprint4_bridge_deploy.png "Despliegue del WhatsApp bridge")

---

#### 5.2.4.8. Team Collaboration Insights during Sprint

Durante el Sprint 4, la implementación del canal de WhatsApp se concentró en el repositorio `daop-entreprenly-whatsapp-bridge`, con ajustes de integración en el Backend y el Frontend. El equipo mantuvo GitFlow con ramas `feature/` integradas a `develop` y `main` mediante Pull Requests. La distribución de commits del bridge (sin contar merges) por miembro fue la siguiente: **Palma De Los Santos (8 commits)** y **Camargo Briceño (5 commits)**, con la colaboración del resto del equipo en las tareas de integración del Backend y el Frontend.

![contributors_p4](./images/capitulo5/contributors_p4.png "Contribuidores del Sprint 4")

![pull_p4](./images/capitulo5/pull_p4.png "Pull Requests del Sprint 4")

**URL del repositorio del WhatsApp Bridge:** https://github.com/Kauflink/daop-entreprenly-whatsapp-bridge

---

## 5.3. Validation Interviews

En esta sección el equipo registra y explica las actividades de entrevistas de validación realizadas durante el proyecto. A diferencia de las entrevistas de elicitación presentadas en la sección 2.2 —cuyo objetivo fue descubrir los problemas y necesidades de los usuarios—, las entrevistas de validación tienen como propósito confirmar si la solución construida (Landing Page y aplicaciones) resuelve efectivamente esos problemas y resulta usable para los segmentos objetivo.

Para ello se realizaron sesiones en las que usuarios reales de cada segmento interactuaron directamente con el Landing Page y con las aplicaciones de Entreprenly, ejecutando tareas concretas basadas en los User Flows definidos en la sección 4.4.4. Durante cada sesión se observó el desempeño del usuario al completar las tareas y, al finalizar, se aplicó un cuestionario de validación orientado a contrastar los dolores identificados en el needfinding con la experiencia real de uso del producto. Adicionalmente, se registraron observaciones de usabilidad siguiendo principios de evaluación heurística. Cada entrevista fue grabada en video como evidencia y se encuentra disponible en Microsoft Stream.

### 5.3.1. Diseño de Entrevistas

Antes de iniciar cada sesión de validación se brinda un saludo cordial y una breve presentación del entrevistador, explicando que el propósito de la sesión es evaluar la facilidad de uso y la utilidad del producto Entreprenly, y no evaluar al participante. Se aclara que la información será utilizada únicamente con fines académicos y se mantendrá en estricta confidencialidad. Como primer paso se solicita al participante su nombre completo, edad y distrito de residencia para fines de registro. Luego se le invita a interactuar libremente con el Landing Page y las aplicaciones, ejecutando las tareas propuestas y expresando en voz alta sus impresiones (técnica de _thinking aloud_), destacando que no existen respuestas correctas o incorrectas.

El proceso de validación para cada segmento se compone de tres momentos: (1) la exploración del Landing Page, (2) la ejecución de tareas guiadas sobre las aplicaciones siguiendo los User Flows correspondientes, y (3) un cuestionario de validación de diez preguntas. A continuación se detallan los elementos a incluir en la sesión de validación para cada segmento objetivo.

**Preguntas introductorias (ambos segmentos)**

- ¿Cuál es su nombre y apellidos?
- ¿Cuántos años tiene?
- ¿En qué distrito vive?

---

**Segmento objetivo 1: Comerciantes (Dueños de Minimarkets/Mercados)**

_Elementos a validar:_ Landing Page y Aplicación Web (Dashboard de gestión).

_User Flows a validar (sección 4.4.4):_

- User Flow 1 – Gestión de inventario (agregar, editar y buscar productos).
- User Flow 2 – Creación de lotes y gestión de alertas de vencimiento.
- User Flow 3 – Registro de venta presencial (POS con pesaje).
- User Flow 4 – Validación de pago de pedido del chatbot.
- User Flow 5 – Suscripción al Plan Control.

_Tareas asignadas:_

1. Explorar el Landing Page e identificar qué ofrece Entreprenly y los planes disponibles.
2. Registrar un producto nuevo, editarlo y luego buscarlo en el inventario.
3. Crear un lote con fecha de vencimiento y revisar las alertas del dashboard de lotes.
4. Registrar una venta presencial seleccionando un producto por peso y uno por unidad, y finalizar el cobro.
5. Revisar un pedido del chatbot pendiente y aprobar (o rechazar) su pago.
6. Iniciar el proceso de suscripción al Plan Control.

_Preguntas de validación:_

1. Después de explorar el Landing Page, ¿quedó claro qué hace Entreprenly y cómo resolvería los problemas de su negocio?
2. Al registrar, editar y buscar productos en el módulo de inventario, ¿le resultó más sencillo y ordenado que su método actual (cuaderno, Excel o memoria)?
3. Cuando creó un lote y visualizó las alertas de stock y vencimiento, ¿siente que esto le ayudaría a evitar pérdidas por productos vencidos o desabastecimiento no detectado?
4. Al registrar una venta presencial con el POS, incluido el pesaje, ¿le pareció un proceso rápido y confiable para el día a día en el local?
5. ¿La separación automática de los ingresos por efectivo y por medios digitales (Yape, Plin, POS) le daría mayor control al momento de cuadrar la caja?
6. Al validar el pago de un pedido del chatbot desde el dashboard, ¿le resultó claro el proceso de aprobar o rechazar el pago y confirmar el pedido?
7. ¿Considera que atender los pedidos por WhatsApp mediante el chatbot le quitaría la carga de estar pendiente del celular mientras atiende a los clientes en el local?
8. Durante el uso de la aplicación, ¿encontró alguna pantalla, botón o paso que le resultara confuso o difícil de entender?
9. En una escala del 1 al 5, ¿qué tan probable es que utilice Entreprenly en su negocio? ¿Por qué?
10. ¿Qué funcionalidad agregaría, quitaría o mejoraría para que la aplicación se ajuste mejor a su forma de trabajar?

---

**Segmento objetivo 2: Clientes Finales**

_Elementos a validar:_ Landing Page y Chatbot de WhatsApp (experiencia de compra).

_User Flows a validar:_

- Flujo de pedido por el chatbot: consulta de producto disponible, confirmación del pedido, recepción de las instrucciones de pago, reporte del comprobante de pago digital y recepción de la confirmación/comprobante.

_Tareas asignadas:_

1. Explorar el Landing Page e identificar qué ofrece la tienda y por qué convendría comprar por este medio.
2. Iniciar una conversación con el chatbot y consultar la disponibilidad de un producto.
3. Confirmar un pedido a través del chatbot.
4. Recibir las instrucciones de pago y reportar el comprobante de pago digital.
5. Recibir la confirmación del pedido y su comprobante.

_Preguntas de validación:_

1. Después de ver el Landing Page, ¿entendió qué ofrece la tienda y por qué le convendría comprar por este medio?
2. Al realizar un pedido por el chatbot de WhatsApp, ¿le resultó fácil y rápido encontrar el producto y completar la compra?
3. ¿La confirmación de stock en tiempo real le dio mayor confianza de que el producto que pidió sí está disponible?
4. Al recibir las instrucciones de pago y reportar su comprobante por el chat, ¿le pareció un proceso claro y seguro?
5. ¿Recibir una confirmación o comprobante automático del pedido le dio mayor tranquilidad al pagar por adelantado?
6. ¿Le resultó cómodo el medio de pago ofrecido (efectivo, Yape o Plin)?
7. ¿Prefiere esta experiencia de compra mediante el chatbot frente a esperar que una persona le responda manualmente?
8. Durante el pedido, ¿hubo algún mensaje o paso del chatbot que le resultara confuso o poco claro?
9. En una escala del 1 al 5, ¿qué tan probable es que vuelva a comprar en una tienda que use este sistema? ¿Por qué?
10. ¿Qué mejoraría de la experiencia de compra a través del chatbot?

### 5.3.2. Registro de Entrevistas

A continuación se registran las entrevistas de validación realizadas por segmento. Para cada entrevista se consigna el nombre y apellidos del participante, su edad, su distrito de residencia, un screenshot de un cuadro del video, el enlace al video alojado en Microsoft Stream —indicando el timing donde inicia la entrevista y su duración— y un resumen descriptivo de las principales apreciaciones del entrevistado respecto a las tareas asignadas. De acuerdo con lo planificado por el equipo, se realizaron dos entrevistas para el Segmento 1 (Comerciantes) y una entrevista para el Segmento 2 (Clientes Finales).

**Segmento 1: Comerciantes (Dueños de Minimarkets/Mercados)**

- Primera entrevista:

<div align="center">
<div style="font-family: 'Segoe UI', sans-serif; max-width: 680px; margin: 24px auto; border: 1.5px solid #b0bec5; border-radius: 4px; overflow: hidden; box-shadow: 0 2px 8px rgba(0,0,0,0.12);">

  <!-- Encabezado -->
  <div style="background-color: #1a6b6b; color: white; padding: 10px 16px; font-weight: 700; font-size: 1.1em; letter-spacing: 0.05em;">
  Entrevista de Validación
  </div>

  <!-- Imagen de la captura de pantalla -->
  <div style="background-color: #1a6b6b; padding: 12px 16px 16px;">
    <img src="images/capitulo5/val_comerciante_1.png" alt="Screenshot de la entrevista de validación" style="width: 100%; border-radius: 3px; display: block;">
  </div>

  <!-- Datos en dos columnas -->
  <table style="width: 100%; border-collapse: collapse; font-size: 0.88em;">
    <tr>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc; width: 50%;">
        <strong>Entrevistado(a):</strong> María Encarnación Velasquez
      </td>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc; width: 50%;">
        <strong>Edad:</strong> 62
      </td>
    </tr>
    <tr>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Entrevistador(a):</strong> Lionel Chavez Carrasco
      </td>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Distrito:</strong> San Miguel, Lima
      </td>
    </tr>
    <tr>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Inicio de la entrevista:</strong> 03:20
      </td>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Duración:</strong> 16:34
      </td>
    </tr>
  </table>

  <!-- Link -->
  <table style="width: 100%; border-collapse: collapse; font-size: 0.88em;">
    <tr>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Link de la entrevista (Microsoft Stream):</strong>
        <a href="https://upcedupe-my.sharepoint.com/:v:/g/personal/u202416151_upc_edu_pe/IQDLOgZZQciGT4vb_yjShsLTAS0Hr5RXYveIiQsCDk62_3g?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=Ykle0r">https://upcedupe-my.sharepoint.com/:v:/g/personal/u202416151_upc_edu_pe/IQDLOgZZQciGT4vb_yjShsLTAS0Hr5RXYveIiQsCDk62_3g?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=Ykle0r</a>
      </td>
    </tr>
  </table>

  <!-- Descripción -->
  <table style="width: 100%; border-collapse: collapse; font-size: 0.88em;">
    <tr>
      <td style="padding: 10px 14px; border: 1px solid #cfd8dc; line-height: 1.6;">
        Durante la entrevista, María Encarnación Velázquez manifestó que el Landing Page de Entreprenly le pareció claro y fácil de comprender, ya que explica de manera sencilla los beneficios de la aplicación y cómo puede ayudar a los pequeños comerciantes en la gestión de sus negocios. Respecto a los User Flows ejecutados, consideró que las funciones de inventario y gestión de lotes son intuitivas y facilitan el registro, búsqueda y control de productos. Asimismo, indicó que el proceso de venta presencial es rápido y permite llevar un mejor control de los ingresos diarios. La validación de pagos mediante el chatbot de WhatsApp le pareció una alternativa práctica para automatizar pedidos y cobros, mientras que el flujo de suscripción resultó sencillo y comprensible. La entrevistada señaló que la solución contribuye significativamente a resolver problemas operativos relacionados con el control de inventario, seguimiento de ventas y organización de productos, reduciendo la necesidad de registros manuales y disminuyendo el riesgo de errores o pérdidas. No se identificaron dificultades importantes durante la interacción con la aplicación; sin embargo, sugirió incorporar funcionalidades adicionales como la generación de facturas y guías de remisión para complementar la gestión comercial. Finalmente, manifestó una alta probabilidad de utilizar la aplicación en su negocio debido a los beneficios que ofrece en términos de organización, ahorro de tiempo y reducción del estrés asociado a las tareas administrativas.
      </td>
    </tr>
  </table>

</div>

</div>

---

- Segunda entrevista:

<div align="center">
<div style="font-family: 'Segoe UI', sans-serif; max-width: 680px; margin: 24px auto; border: 1.5px solid #b0bec5; border-radius: 4px; overflow: hidden; box-shadow: 0 2px 8px rgba(0,0,0,0.12);">

  <!-- Encabezado -->
  <div style="background-color: #1a6b6b; color: white; padding: 10px 16px; font-weight: 700; font-size: 1.1em; letter-spacing: 0.05em;">
  Entrevista de Validación
  </div>

  <!-- Imagen de la captura de pantalla -->
  <div style="background-color: #1a6b6b; padding: 12px 16px 16px;">
    <img src="images/capitulo5/val_comerciante_2.png" alt="Screenshot de la entrevista de validación" style="width: 100%; border-radius: 3px; display: block;">
  </div>

  <!-- Datos en dos columnas -->
  <table style="width: 100%; border-collapse: collapse; font-size: 0.88em;">
    <tr>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc; width: 50%;">
        <strong>Entrevistado(a):</strong> Hercilio Carrasco Herrera
      </td>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc; width: 50%;">
        <strong>Edad:</strong> 59
      </td>
    </tr>
    <tr>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Entrevistador(a):</strong> Lionel Chavez Carrasco
      </td>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Distrito:</strong> San Miguel, Lima
      </td>
    </tr>
    <tr>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Inicio de la entrevista:</strong> 03:35
      </td>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Duración:</strong> 17:07
      </td>
    </tr>
  </table>

  <!-- Link -->
  <table style="width: 100%; border-collapse: collapse; font-size: 0.88em;">
    <tr>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Link de la entrevista (Microsoft Stream):</strong>
        <a href="https://upcedupe-my.sharepoint.com/:v:/g/personal/u202416151_upc_edu_pe/IQDfZ1lUJuh6QIJJfAiZtDGhAfoa0SvaRV9JKz7SKHOnDxQ?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=1rjqKF">https://upcedupe-my.sharepoint.com/:v:/g/personal/u202416151_upc_edu_pe/IQDfZ1lUJuh6QIJJfAiZtDGhAfoa0SvaRV9JKz7SKHOnDxQ?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=1rjqKF</a>
      </td>
    </tr>
  </table>

  <!-- Descripción -->
  <table style="width: 100%; border-collapse: collapse; font-size: 0.88em;">
    <tr>
      <td style="padding: 10px 14px; border: 1px solid #cfd8dc; line-height: 1.6;">
        Durante la entrevista, Hercilio Carrasco Herrera indicó que el Landing Page de Entreprenly presenta de manera clara las funcionalidades y beneficios de la aplicación, permitiéndole comprender rápidamente cómo la herramienta puede apoyar la gestión de su negocio. En cuanto a los User Flows ejecutados, consideró que los procesos de inventario y gestión de lotes son fáciles de utilizar y útiles para mantener un mejor control de los productos, especialmente aquellos con fecha de vencimiento. Asimismo, valoró positivamente el flujo de venta presencial, destacando la facilidad para registrar ventas y diferenciar ingresos por efectivo y pagos electrónicos. La validación de pagos mediante el chatbot de WhatsApp le pareció una funcionalidad innovadora que simplifica la atención de pedidos, mientras que el proceso de suscripción fue percibido como sencillo y accesible. El entrevistado señaló que la solución responde adecuadamente a varios de sus problemas operativos, principalmente en el control de inventario, la gestión de productos perecibles y la organización de ventas. También destacó que las alertas de vencimiento y el control de stock en tiempo real pueden contribuir a reducir pérdidas económicas y mejorar la eficiencia del negocio. No reportó dificultades significativas durante la ejecución de las tareas; sin embargo, identificó una oportunidad de mejora relacionada con la incorporación de recordatorios automáticos para clientes con pagos pendientes, lo que facilitaría la gestión de cobranzas y reduciría el riesgo de impagos. Finalmente, manifestó una alta disposición a utilizar la aplicación en su actividad comercial, ya que considera que las funcionalidades propuestas aportan valor y contribuyen a modernizar la administración de pequeños negocios.
      </td>
    </tr>
  </table>

</div>

</div>

---

**Segmento 2: Clientes Finales**

- Primera entrevista:

<div align="center">
<div style="font-family: 'Segoe UI', sans-serif; max-width: 680px; margin: 24px auto; border: 1.5px solid #b0bec5; border-radius: 4px; overflow: hidden; box-shadow: 0 2px 8px rgba(0,0,0,0.12);">

  <!-- Encabezado -->
  <div style="background-color: #1a6b6b; color: white; padding: 10px 16px; font-weight: 700; font-size: 1.1em; letter-spacing: 0.05em;">
  Entrevista de Validación
  </div>

  <!-- Imagen de la captura de pantalla -->
  <div style="background-color: #1a6b6b; padding: 12px 16px 16px;">
    <img src="images/capitulo5/val_cliente_1.png" alt="Screenshot de la entrevista de validación" style="width: 100%; border-radius: 3px; display: block;">
  </div>

  <!-- Datos en dos columnas -->
  <table style="width: 100%; border-collapse: collapse; font-size: 0.88em;">
    <tr>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc; width: 50%;">
        <strong>Entrevistado(a):</strong> Sebastián Curay
      </td>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc; width: 50%;">
        <strong>Edad:</strong> 19
      </td>
    </tr>
    <tr>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Entrevistador(a):</strong> Fernando Flores
      </td>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Distrito:</strong> San Martín de Porres, Lima
      </td>
    </tr>
    <tr>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Inicio de la entrevista:</strong> 00:00
      </td>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Duración:</strong> 09:50
      </td>
    </tr>
  </table>

  <!-- Link -->
  <table style="width: 100%; border-collapse: collapse; font-size: 0.88em;">
    <tr>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Link de la entrevista (Microsoft Stream):</strong>
        <a href="https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241a290_upc_edu_pe/IQBA8Q70W8bCRoDGM1oUhrJdATc8nAY1ysMnwvptFJXACZk?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=wdusaa">https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241a290_upc_edu_pe/IQBA8Q70W8bCRoDGM1oUhrJdATc8nAY1ysMnwvptFJXACZk?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=wdusaa</a>
      </td>
    </tr>
  </table>

  <!-- Descripción -->
  <table style="width: 100%; border-collapse: collapse; font-size: 0.88em;">
    <tr>
      <td style="padding: 10px 14px; border: 1px solid #cfd8dc; line-height: 1.6;">
        Sebastián, cliente final de 19 años habituado a los pagos digitales (Yape y Plin), validó el Landing Page y el flujo de compra por el chatbot de WhatsApp realizando un pedido real durante la sesión (dos Coca-Colas, con entrega en Girón Apurímac y pago reportado mediante una captura de Yape). Sobre el Landing Page, indicó que comprendió la propuesta de valor y la encontró interesante, destacando que representa una forma más rápida de comprar y que poder ver el stock disponible le resulta útil. Respecto al pedido por el chatbot, lo percibió rápido y directo, con mensajes claros y bien enfocados. Valoró especialmente la confirmación de stock en tiempo real: comentó que en otros emprendimientos suele ocurrir que paga y luego le indican que el producto está agotado, le retrasan o le cancelan el pedido, por lo que ver la cantidad disponible al momento de consultar le da confianza para comprar.
        Sobre el pago, calificó el proceso de recibir las instrucciones y reportar el comprobante como claro, seguro, dinámico y sencillo, y señaló que recibir la confirmación automática del pedido le da tranquilidad al pagar por adelantado, pues le permite verificar que el pago fue confirmado y que no fue estafado ni perdió el tiempo. Indicó que el medio de pago ofrecido (Yape/Plin) le resulta cómodo por ser de uso generalizado. Manifestó preferir la atención por chatbot frente a la respuesta manual de una persona, por considerarla rápida y eficiente al estar todo automatizado. No identificó pasos confusos durante el flujo. Calificó con 5 sobre 5 la probabilidad de volver a comprar en una tienda que utilice este sistema, por considerarlo rápido, eficiente e intuitivo y fácil de usar para cualquier persona. Como mejora, sugirió que el mensaje de bienvenida del chatbot muestre un pequeño catálogo de los productos más solicitados o más vendidos y que, en caso de no estar disponibles, el cliente pueda escribir el producto para verificar su disponibilidad.
      </td>
    </tr>
  </table>

</div>

</div>

### 5.3.3. Evaluaciones según heurísticas

Esta sección presenta la evaluación heurística aplicada a **Entreprenly** durante la etapa de validación. La evaluación se organiza en tres grupos: heurísticas de usabilidad, arquitectura de información e inclusive design. Cada criterio incluye un puntaje del 1 al 5, la evidencia observada (referenciada por figura) y las oportunidades de mejora identificadas.

#### Catálogo de figuras

| Fig.    | Pantalla                                                        | Archivo                                                |
| ------- | --------------------------------------------------------------- | ------------------------------------------------------ |
| Fig. 1  | Panel de Inicio (Dashboard)                                     | `Fig-01-panel-de-inicio.png`                           |
| Fig. 2  | Catálogo de Productos                                           | `Fig-02-catalogo-de-productos.png`                     |
| Fig. 3  | Modal "Editar Producto"                                         | `Fig-03-modal-editar-producto.png`                     |
| Fig. 4  | Modal "Agregar Nuevo Producto"                                  | `Fig-04-modal-agregar-producto.png`                    |
| Fig. 5  | Lotes de Inventario (vista general)                             | `Fig-05-lotes-de-inventario.png`                       |
| Fig. 6  | Panel de Alertas de Lotes                                       | `Fig-06-panel-alertas-de-lotes.png`                    |
| Fig. 7  | Modal "Agregar Nuevo Lote"                                      | `Fig-07-modal-agregar-lote.png`                        |
| Fig. 8  | Detalle de Lote (lote vencido)                                  | `Fig-08-detalle-de-lote-vencido.png`                   |
| Fig. 9  | Ventas – "Producto no encontrado"                               | `Fig-09-ventas-producto-no-encontrado.png`             |
| Fig. 10 | Suscripción – Planes Free y Control                             | `Fig-10-suscripcion-planes.png`                        |
| Fig. 11 | Suscripción – Límites, facturación e historial                  | `Fig-11-suscripcion-limites-facturacion-historial.png` |
| Fig. 12 | Modal "Agregar método de pago"                                  | `Fig-12-modal-agregar-metodo-de-pago.png`              |
| Fig. 13 | Modal "Completar datos de facturación"                          | `Fig-13-modal-datos-de-facturacion.png`                |
| Fig. 14 | Modal "Historial de suscripción"                                | `Fig-14-modal-historial-de-suscripcion.png`            |
| Fig. 15 | Ventas – Registrar cantidad (teclado numérico)                  | `Fig-15-ventas-registrar-cantidad.png`                 |
| Fig. 16 | Centro de Ayuda                                                 | `Fig-16-centro-de-ayuda.png`                           |
| Fig. 17 | Formulario "Reportar un problema"                               | `Fig-17-reportar-un-problema.png`                      |
| Fig. 18 | Artículo de ayuda "¿Cómo aprobar o rechazar un pedido del bot?" | `Fig-18-articulo-aprobar-pedido.png`                   |
| Fig. 19 | Perfil y configuración de cuenta                                | `Fig-19-perfil-configuracion.png`                      |

#### 5.3.3.1. Heurísticas de usabilidad

En esta subsección se evalúa la experiencia de uso de Entreprenly tomando como referencia las heurísticas de Nielsen.

##### Visibilidad del estado del sistema — Puntaje: 5/5

Entreprenly comunica oportunamente el estado del sistema. El Panel de Inicio muestra en tiempo real el resumen del día (ventas, ingresos, pedidos y alertas), el estado del chatbot ("Activo") y el estado del inventario con etiquetas como "Vencido" y "Stock bajo". El panel de alertas de lotes notifica vencimientos y faltantes, y la vista de Suscripción refleja el plan activo y el consumo de límites mediante barras de progreso.

<img src="images/capitulo5/Fig-01-panel-de-inicio.png" width="600">

<img src="images/capitulo5/Fig-06-panel-alertas-de-lotes.png" width="600">

**Evidencia observada:** Fig. 1 (resumen y alertas del dashboard), Fig. 6 (notificaciones de lotes), Fig. 11 (uso del plan y estado de facturación).

**Mejora sugerida:** Añadir un _toast_ de confirmación visible tras guardar producto/lote, ya que el modal se cierra sin un mensaje persistente de éxito.

---

##### Relación entre el sistema y el mundo real — Puntaje: 5/5

El lenguaje es cercano al comerciante peruano: "Lotes", "Stock", "Caja diaria", "Boleta", "Yape/Plin", "RUC" y "Razón social". En las vistas de Lotes y de Datos de facturación se emplean términos fiscales y de inventario propios del rubro.

<img src="images/capitulo5/Fig-05-lotes-de-inventario.png" width="600">

<img src="images/capitulo5/Fig-13-modal-datos-de-facturacion.png" width="600">

**Evidencia observada:** Fig. 5 (lotes/unidades), Fig. 8 (fecha de vencimiento), Fig. 13 (RUC, razón social, dirección fiscal), Fig. 9 ("Tarjeta – Yape/Plin").

**Mejora sugerida:** Incluir ayuda contextual (tooltip) en "Peso (g)" para productos a granel, diferenciándolo de "Unidad".

---

##### Libertad y control por parte del usuario — Puntaje: 5/5

Todos los modales tienen botón de cierre (×) y opción Cancelar; el detalle de lote ofrece "Volver"; el Perfil permite editar datos, cambiar contraseña, idioma, tema y notificaciones sin quedar atrapado. En Ventas existe "Cancelar Venta".

<img src="images/capitulo5/Fig-03-modal-editar-producto.png" width="600">

<img src="images/capitulo5/Fig-19-perfil-configuracion.png" width="600">

**Evidencia observada:** Fig. 3 y Fig. 4 (× y Cancelar en modales), Fig. 8 (botón Volver), Fig. 13 (Cancelar), Fig. 19 (edición libre de perfil).

**Mejora sugerida:** Agregar confirmación "¿Descartar cambios?" al cerrar un modal con campos ya editados, para evitar pérdidas accidentales.

---

##### Consistencia y estándares — Puntaje: 5/5

Se mantiene un patrón visual uniforme: sidebar naranja fija, tipografía estable, botones primarios naranjas, y tarjetas y tablas con el mismo estilo en Productos, Lotes, Ventas, Suscripción y Ayuda. La nomenclatura de navegación es consistente en todas las pantallas.

<img src="images/capitulo5/Fig-02-catalogo-de-productos.png" width="600">

<img src="images/capitulo5/Fig-10-suscripcion-planes.png" width="600">

**Evidencia observada:** Fig. 1, Fig. 2, Fig. 5, Fig. 10 y Fig. 16 comparten layout, colores y jerarquía de botones.

**Mejora sugerida:** Unificar el estilo del botón "Volver" (Fig. 8, negro) con el resto de botones secundarios (blancos con borde).

---

##### Prevención de errores — Puntaje: 4/5

Los formularios usan campos guía y valores por defecto. En Agregar Producto el botón Guardar permanece atenuado hasta completar lo necesario; en Agregar Lote se solicitan fecha de ingreso y vencimiento; en Datos de facturación y Método de pago se marcan formatos esperados (tarjeta, CVV, RUC).

<img src="images/capitulo5/Fig-04-modal-agregar-producto.png" width="600">

<img src="images/capitulo5/Fig-07-modal-agregar-lote.png" width="600">

**Evidencia observada:** Fig. 4 (Guardar atenuado), Fig. 7 (fechas obligatorias), Fig. 12 y Fig. 13 (formatos guía).

**Mejora sugerida:** Validar en línea que la _Fecha de Vencimiento_ sea posterior a la _Fecha de Ingreso_ y advertir antes de registrar un lote ya vencido.

---

##### Reconocer antes que recordar — Puntaje: 5/5

El dashboard ofrece "Accesos rápidos" con íconos y una sidebar siempre visible con etiquetas de texto. El usuario reconoce los módulos sin memorizar rutas; las tarjetas resumen muestran lo relevante de un vistazo.

<img src="images/capitulo5/Fig-01-panel-de-inicio.png" width="600">

**Evidencia observada:** Fig. 1 (accesos rápidos e íconos), sidebar persistente en todas las figuras, Fig. 16 (categorías con íconos).

**Mejora sugerida:** Resaltar de forma más marcada el ítem activo del menú para reforzar la ubicación del usuario.

---

##### Flexibilidad y eficiencia en el uso — Puntaje: 4/5

Existen atajos (accesos rápidos del dashboard), buscador de lotes, descarga de historial, teclado numérico para registrar cantidad en ventas y generación automática de código QR, lo que agiliza tanto al usuario nuevo como al recurrente.

<img src="images/capitulo5/Fig-15-ventas-registrar-cantidad.png" width="600">

<img src="images/capitulo5/Fig-14-modal-historial-de-suscripcion.png" width="600">

**Evidencia observada:** Fig. 1 (accesos rápidos), Fig. 14 (Descargar historial), Fig. 15 (teclado numérico), Fig. 2 (QR por producto).

**Mejora sugerida:** Incorporar búsqueda/filtros en el catálogo de Productos y atajos de teclado en el módulo de Ventas para usuarios avanzados.

---

##### Diseño estético y minimalista — Puntaje: 5/5

La interfaz mantiene jerarquía clara y bajo ruido visual: uso consistente del naranja como color de acción, espacios en blanco amplios y tarjetas bien delimitadas en Suscripción y en el dashboard.

<img src="images/capitulo5/Fig-10-suscripcion-planes.png" width="600">

**Evidencia observada:** Fig. 1, Fig. 10 (cards de planes), Fig. 16 (centro de ayuda ordenado).

**Mejora sugerida:** En el dashboard, equilibrar la densidad de la zona inferior (estado de inventario) para evitar acumulación de tarjetas pequeñas.

---

##### Ayuda a los usuarios a reconocer, diagnosticar y recuperarse de los errores — Puntaje: 4/5

El sistema señala errores con color y texto: en Ventas muestra "⊘ Producto no encontrado"; en Lotes marca el lote "Vencido" en rojo con la fecha. Los estados de error son reconocibles.

<img src="images/capitulo5/Fig-09-ventas-producto-no-encontrado.png" width="600">

<img src="images/capitulo5/Fig-08-detalle-de-lote-vencido.png" width="600">

**Evidencia observada:** Fig. 9 (producto no encontrado), Fig. 8 (lote vencido), Fig. 11 (estados "pendiente de completar").

**Mejora sugerida:** Que el mensaje "Producto no encontrado" sugiera la acción siguiente (p. ej. "Verifica el nombre o créalo en Productos"), explicando cómo recuperarse y no solo qué ocurrió.

---

##### Ayuda y documentación — Puntaje: 5/5

Cuenta con un Centro de Ayuda con artículos frecuentes, categorías, buscador y datos de soporte (correo, WhatsApp, horario); artículos paso a paso; y un formulario para reportar problemas con tiempos de respuesta.

<img src="images/capitulo5/Fig-16-centro-de-ayuda.png" width="600">

<img src="images/capitulo5/Fig-17-reportar-un-problema.png" width="600">

<img src="images/capitulo5/Fig-18-articulo-aprobar-pedido.png" width="600">

**Evidencia observada:** Fig. 16 (artículos y soporte), Fig. 17 (reporte de problema), Fig. 18 (guía "¿Cómo aprobar o rechazar un pedido del bot?").

**Mejora sugerida:** Enlazar ayuda contextual ("?") desde cada módulo directamente al artículo correspondiente del centro de ayuda.

---

#### 5.3.3.2. Arquitectura de información

En esta subsección se evalúa si la organización de la información permite encontrar, comprender y utilizar el contenido de forma clara.

##### Is it findable? — Puntaje: 5/5

Las funciones principales se ubican en la sidebar fija y en los accesos rápidos del dashboard; el Centro de Ayuda agrupa soporte y FAQ por categorías.

<img src="images/capitulo5/Fig-01-panel-de-inicio.png" width="600">

**Evidencia observada:** Fig. 1, Fig. 16, navegación lateral presente en todas las figuras.

**Mejora sugerida:** Añadir un buscador global en el header del dashboard.

---

##### Is it accessible? — Puntaje: 4/5

Buen contraste (texto oscuro sobre blanco, acción naranja), etiquetas visibles y opción de tema Claro/Oscuro e idioma/zona horaria configurables.

<img src="images/capitulo5/Fig-19-perfil-configuracion.png" width="600">

**Evidencia observada:** Fig. 19 (preferencias de tema/idioma), formularios con labels (Fig. 4, Fig. 13).

**Mejora sugerida:** Validar el contraste del texto blanco sobre naranja (banner del dashboard) y confirmar el comportamiento responsivo en móvil/tablet.

---

##### Is it clear? — Puntaje: 5/5

Títulos y subtítulos describen cada sección ("Catálogo de productos disponibles", "Registra y procesa las ventas del día"); los modales incluyen título y descripción.

<img src="images/capitulo5/Fig-05-lotes-de-inventario.png" width="600">

**Evidencia observada:** Fig. 2, Fig. 5, Fig. 8 (encabezados descriptivos).

**Mejora sugerida:** Acompañar las barras de "Límites disponibles" con una leyenda del significado al alcanzar el tope.

---

##### Is it communicative? — Puntaje: 5/5

La interfaz informa en el momento adecuado: estado del plan, stock, alertas de lotes y actividad de suscripción.

<img src="images/capitulo5/Fig-11-suscripcion-limites-facturacion-historial.png" width="600">

**Evidencia observada:** Fig. 1 (resumen), Fig. 6 (alertas), Fig. 11 (historial/estado de facturación).

**Mejora sugerida:** Mostrar contadores de notificaciones también en la sidebar (módulos Lotes/Pedidos).

---

##### Is it usable? — Puntaje: 4/5

Las tareas principales se completan sin asistencia: alta de productos y lotes, registro de ventas, gestión de suscripción, método de pago, datos fiscales y descarga de historial.

<img src="images/capitulo5/Fig-12-modal-agregar-metodo-de-pago.png" width="600">

**Evidencia observada:** Fig. 4, Fig. 7, Fig. 12, Fig. 13, Fig. 14, Fig. 15.

**Mejora sugerida:** Guiar el primer registro con un mini-onboarding; los módulos vacíos ya muestran estados como "Aún no hay pedidos".

---

##### Is it credible? — Puntaje: 5/5

Transmite confianza con precios transparentes, identidad visual coherente, datos de soporte reales y una propuesta de valor clara.

<img src="images/capitulo5/Fig-10-suscripcion-planes.png" width="600">

**Evidencia observada:** Fig. 10 (planes y precios), Fig. 16 (soporte con correo/WhatsApp/horario).

**Mejora sugerida:** Incluir un sello/nota de seguridad de pago en el modal de tarjeta (Fig. 12).

---

##### Is it controllable? — Puntaje: 5/5

El usuario cambia de sección, cancela acciones, mantiene su plan, edita su perfil y vuelve a estados previos (botón Volver, ×, Cancelar).

<img src="images/capitulo5/Fig-08-detalle-de-lote-vencido.png" width="600">

**Evidencia observada:** Fig. 8 (Volver), Fig. 13 (Cancelar), Fig. 19 (control total del perfil).

**Mejora sugerida:** Confirmar antes de cerrar modales con cambios sin guardar.

---

##### Is it valuable? — Puntaje: 5/5

Aporta valor real: control de stock y vencimientos, conciliación de caja por método de pago, pedidos por WhatsApp vía chatbot y gestión de suscripción.

<img src="images/capitulo5/Fig-01-panel-de-inicio.png" width="600">

**Evidencia observada:** Fig. 1 (caja por método de pago), Fig. 6 (vencimientos), Fig. 10 (valor del plan Control).

**Mejora sugerida:** Resaltar en el dashboard el beneficio acumulado (p. ej. mermas evitadas por alertas de vencimiento).

---

##### Is it learnable? — Puntaje: 5/5

Patrones repetidos, labels claros y guías paso a paso facilitan el aprendizaje.

<img src="images/capitulo5/Fig-18-articulo-aprobar-pedido.png" width="600">

**Evidencia observada:** Fig. 4 (formulario autoexplicativo), Fig. 18 (artículo paso a paso).

**Mejora sugerida:** Tour interactivo opcional en el primer ingreso.

---

##### Is it delightful? — Puntaje: 4/5

La experiencia es fluida, limpia y profesional, con estados claros y sensación de control.

<img src="images/capitulo5/Fig-10-suscripcion-planes.png" width="600">

**Evidencia observada:** Fig. 1, Fig. 10 (estética cuidada).

**Mejora sugerida:** Sumar microinteracciones (animación al guardar, checkmark al finalizar una venta) para reforzar la satisfacción.

---

#### 5.3.3.3. Inclusive design

En esta subsección se evalúa si Entreprenly considera distintos contextos de uso, niveles de experiencia digital y necesidades de accesibilidad.

##### Principio 1: Proporciona experiencias comparables — Puntaje: 5/5

Los puntos de contacto (dashboard, módulos, soporte y chatbot) ofrecen una experiencia equivalente y coherente; el chatbot habilita la compra por WhatsApp como canal alterno.

<img src="images/capitulo5/Fig-01-panel-de-inicio.png" width="600">

**Evidencia observada:** Fig. 1 (chatbot activo), Fig. 16 (soporte), navegación uniforme en todas las figuras.

**Mejora sugerida:** Garantizar paridad de la experiencia en la versión móvil del dashboard.

---

##### Principio 2: Considera la situación del usuario — Puntaje: 5/5

Responde a contextos reales de tienda: registro ágil de ventas con teclado numérico, cierre de caja por método de pago, revisión rápida de stock y alertas, y pedidos por WhatsApp en horas de demanda.

<img src="images/capitulo5/Fig-15-ventas-registrar-cantidad.png" width="600">

**Evidencia observada:** Fig. 15 (registro rápido), Fig. 1 (resumen de caja), Fig. 6 (alertas operativas).

**Mejora sugerida:** Modo de venta rápida a pantalla completa para horas pico.

---

##### Principio 3: Sé consistente — Puntaje: 5/5

Botones, formularios, mensajes y navegación se mantienen consistentes en todos los módulos.

<img src="images/capitulo5/Fig-02-catalogo-de-productos.png" width="600">

**Evidencia observada:** Fig. 2, Fig. 5, Fig. 10, Fig. 16 (mismo sistema visual).

**Mejora sugerida:** Homogeneizar el estilo del botón "Volver" (Fig. 8).

---

##### Principio 4: Deja al usuario mandar — Puntaje: 5/5

El usuario conserva autonomía: editar perfil, mantener su plan, cancelar, corregir y cerrar popups.

<img src="images/capitulo5/Fig-19-perfil-configuracion.png" width="600">

**Evidencia observada:** Fig. 19 (perfil), Fig. 3 (editar), Fig. 13 (Cancelar), Fig. 14 (descargar/cerrar).

**Mejora sugerida:** Permitir deshacer la última acción en Ventas (quitar un producto agregado por error).

---

##### Principio 5: Ofrece opciones — Puntaje: 5/5

Brinda alternativas de navegación y acción: botones primarios y secundarios, sidebar, accesos rápidos, FAQ, reporte de problema y métodos de pago Efectivo / Tarjeta-Yape/Plin.

<img src="images/capitulo5/Fig-09-ventas-producto-no-encontrado.png" width="600">

<img src="images/capitulo5/Fig-16-centro-de-ayuda.png" width="600">

**Evidencia observada:** Fig. 9 (métodos de pago), Fig. 16 (FAQ + reporte), Fig. 1 (accesos rápidos).

**Mejora sugerida:** Hacer más visible la comparación de ahorro entre el plan Mensual y Anual (el toggle ya existe en Fig. 10).

---

##### Principio 6: Prioriza el contenido — Puntaje: 5/5

El contenido más importante aparece primero: resumen del día y alertas en el tope del dashboard; plan recomendado destacado en Suscripción.

<img src="images/capitulo5/Fig-10-suscripcion-planes.png" width="600">

**Evidencia observada:** Fig. 1 (jerarquía del resumen), Fig. 10 (Plan Control "Recomendado" resaltado).

**Mejora sugerida:** Priorizar visualmente las alertas críticas (vencidos) sobre las informativas.

---

##### Principio 7: Agrega valor — Puntaje: 5/5

Genera beneficios concretos: ahorro de tiempo, menos errores, confianza en el stock, control de caja, automatización por chatbot y claridad de suscripción.

<img src="images/capitulo5/Fig-06-panel-alertas-de-lotes.png" width="600">

**Evidencia observada:** Fig. 6 (evita mermas), Fig. 1 (control de caja), Fig. 10 (valor del plan), Fig. 18 (autoservicio de soporte).

**Mejora sugerida:** Agregar reportes/indicadores de tendencia (ventas semanales, productos más vendidos) para reforzar el valor analítico.

---

#### Resumen de puntajes

| Grupo                                       | Promedio    |
| ------------------------------------------- | ----------- |
| 5.3.3.1 Heurísticas de usabilidad (Nielsen) | **4.7 / 5** |
| 5.3.3.2 Arquitectura de información         | **4.8 / 5** |
| 5.3.3.3 Inclusive design                    | **5.0 / 5** |

---

## 5.4. Video About-the-Product

En esta sección se presenta el video **About-the-Product** de Entreprenly, una pieza de orientación promocional que resume el modelo de negocio, las características y los beneficios del producto. El video, de una duración de entre uno y tres minutos, parte de los dolores cotidianos de un negocio de barrio —el inventario llevado en cuaderno, los productos que se vencen y los pedidos de WhatsApp que no paran— para presentar a **Entreprenly como la plataforma que digitaliza el negocio de retail integrando inventario, ventas y atención por WhatsApp en un solo lugar**. A lo largo de la narración se muestran sus capacidades centrales: el control del stock en tiempo real con alertas anticipadas de vencimiento y desabastecimiento, el registro de ventas en segundos con cuadre de caja que separa automáticamente el efectivo de los medios digitales, y un chatbot que atiende los pedidos por WhatsApp de forma automática —confirmando stock y registrando la venta— de modo que el comerciante solo aprueba el pago.

El video incluye escenas de interacción real con el producto (navegación por el dashboard de inventario, registro de ventas y el flujo de pedido por el chatbot) y recoge **al menos una opinión por cada segmento objetivo**. Por el **Segmento 1 (Comerciantes)** participa Stephanie, dueña de negocio, quien destaca que la plataforma reúne inventario, ventas y caja en un solo lugar de forma ordenada, frente a su método anterior basado en cuaderno y celular; resalta el ahorro de tiempo, la prevención de pérdidas gracias a las alertas de vencimiento y la rapidez al cuadrar la caja, y califica con 5/5 la probabilidad de volver a comprar en una tienda que use el sistema por considerarlo rápido, eficiente e intuitivo. Por el **Segmento 2 (Clientes Finales)** se incorpora la apreciación de Sebastián (registrada en la sección 5.3.2), quien valora la confirmación de stock en tiempo real y la atención automatizada por el chatbot de WhatsApp como un proceso claro, seguro y rápido.

El video fue subido a **Microsoft Stream** y a **YouTube**. A continuación se incluye un screenshot del video con su respectivo enlace.

<div align="center">
<div style="font-family: 'Segoe UI', sans-serif; max-width: 680px; margin: 24px auto; border: 1.5px solid #b0bec5; border-radius: 4px; overflow: hidden; box-shadow: 0 2px 8px rgba(0,0,0,0.12);">

  <!-- Encabezado -->
  <div style="background-color: #1a6b6b; color: white; padding: 10px 16px; font-weight: 700; font-size: 1.1em; letter-spacing: 0.05em;">
  Video About-the-Product — Entreprenly
  </div>

  <!-- Imagen de la captura de pantalla -->
  <div style="background-color: #1a6b6b; padding: 12px 16px 16px;">
    <img src="images/capitulo5/about-the-product-video.png" alt="Screenshot del video About-the-Product de Entreprenly" style="width: 100%; border-radius: 3px; display: block;">
  </div>

  <!-- Links -->
  <table style="width: 100%; border-collapse: collapse; font-size: 0.88em;">
    <tr>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Link del video (Microsoft Stream):</strong>
        <a href="https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241a290_upc_edu_pe/IQD7F8snmaJaQoAKXPJo6MHJARZWmd7lIrkanbWw0uIJt9Y?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=i9I4BZ">https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241a290_upc_edu_pe/IQD7F8snmaJaQoAKXPJo6MHJARZWmd7lIrkanbWw0uIJt9Y?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=i9I4BZ</a>
      </td>
    </tr>
    <tr>
      <td style="padding: 7px 14px; border: 1px solid #cfd8dc;">
        <strong>Link del video (YouTube):</strong>
        <a href="https://youtu.be/JFLwl_6-Alg">https://youtu.be/JFLwl_6-Alg</a>
      </td>
    </tr>
  </table>

</div>
</div>
