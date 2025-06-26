GridSketch - Landing Page y Explorador de Política de Privacidad
Este proyecto es una página web de una sola página (SPA - Single Page Application) totalmente responsiva, creada para servir como la landing page oficial de la aplicación móvil GridSketch. La página está diseñada no solo para presentar la aplicación a los usuarios potenciales, sino también para alojar una política de privacida interactiva y bilingüe.

✨ Características Principales
Diseño Moderno y Responsivo: Construido con Tailwind CSS, el diseño es limpio, profesional y se adapta perfectamente a cualquier tamaño de pantalla, desde dispositivos móviles hasta monitores de escritorio.

Experiencia de Página Única (SPA): La navegación entre la landing page y el explorador de la política de privacidad se realiza de forma dinámica con JavaScript, sin necesidad de recargar la página, ofreciendo una experiencia de usuario fluida.

Navegación Intuitiva:

Landing Page: Menú de navegación con enlaces que se desplazan suavemente (scroll-smooth) a las diferentes secciones de la página.

Política de Privacidad: Un menú lateral permite al usuario saltar directamente a la sección que le interesa.

Componente Interactivo: El explorador de la política de privacidad permite cambiar entre español e inglés de forma instantánea.

Cero Dependencias Externas (excepto CDNs): Todo el código está contenido en un único archivo index.html, utilizando CDNs para Tailwind CSS y Google Fonts, lo que lo hace extremadamente portátil y fácil de desplegar.

🛠️ Tecnologías Utilizadas
HTML5: Para la estructura semántica del contenido.

Tailwind CSS v3: Para todo el diseño y la estilización, cargado a través de CDN.

JavaScript (Vanilla): Para toda la lógica de interactividad, incluyendo:

El menú de navegación móvil.

El cambio dinámico de vistas entre la landing page y la política de privacidad.

La renderización y el cambio de idioma del explorador de la política de privacidad.

Google Fonts: Para la tipografía (Manrope).

🚀 Cómo Utilizar
Simplemente abre el archivo index.html en cualquier navegador web moderno. No se requiere un servidor local ni pasos de compilación.

📂 Estructura del Proyecto
El proyecto consiste en un único archivo index.html que está estructurado de la siguiente manera:

<head>:

Configuración del meta viewport para el diseño responsivo.

Enlaces a los CDNs de Tailwind CSS y Google Fonts.

Un bloque <style> para estilos personalizados y animaciones sutiles.

<body>:

div#landing-page: Contenedor principal para la landing page.

<header>: Barra de navegación fija y menú móvil.

<main>: Contiene las diferentes secciones (<section>) de la página:

Hero: Sección de bienvenida con el título principal y una maqueta de la app.

Features: Rejilla con las funcionalidades clave.

About: Sección "Sobre Nosotros".

News: Sección de "Novedades".

Download: Llamada a la acción final.

<footer>: Pie de página.

div#privacy-explorer: Contenedor vacío que se rellena dinámicamente con el explorador de la política de privacidad cuando el usuario hace clic en el enlace correspondiente.

<script>: Todo el código JavaScript que controla la interactividad de la página.

🤖 Lógica de JavaScript
El script principal se encarga de varias tareas:

Control del Menú Móvil: Muestra y oculta el menú de navegación en pantallas pequeñas.

Cambio de Vistas: Gestiona la visibilidad de div#landing-page y div#privacy-explorer para simular la navegación entre páginas.

Inicialización del Explorador de Política:

Cuando se muestra la vista de privacidad, una función initializePrivacyPolicyExplorer() inyecta el HTML del explorador.

Define un objeto content que contiene todos los textos en español e inglés.

Una función renderPolicy() se encarga de actualizar dinámicamente el contenido (títulos, menús, textos) según el idioma y la sección activa seleccionada por el usuario.

Añade los event listeners a los botones de idioma y navegación de la política.