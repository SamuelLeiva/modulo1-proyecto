# Landing Page – Estructura Semántica, Accesibilidad y Diseño Responsive

## Descripción

Landing Page de una panadería. Esta página está desarrollada con HTML5 semántico y un diseño adaptable a cualquier dispositivo.

---

## Estructura Semántica

- **`<header>`**  
  Contiene la barra de navegación principal, que permite acceder rápidamente a las secciones clave de la página.
  Se utiliza flexbox para la disposición del logo y del nav y para los elementos dentrodel mismo nav.

- **`<main>`**  
  Agrupa el contenido principal de la página, dividido en secciones:

  - **`<section id="hero">`**  
    Presenta el producto con una imagen destacada, un título y una frase de valor.
    Se utilizó display flex para el texto dentro de esta sección.

  - **`<section id="features">`**  
    Muestra una grilla de tarjetas de características, usando display: grid, cada una con una imagen y una descripción.  
    Se utiliza Flexbox para la disposición de la descripción.

  - **`<section id="testimonials">`**  
    Sección de testimonios, donde cada opinión se presenta con display flex.

  - **`<section id="gallery">`**  
    Galería de imágenes, cada una con un título y una pequeña descripción.  
    Las imágenes y sus descripciones se distribuyen usando grid y el contenido de la descripción usa flexbox.

- **`<footer>`**  
  Proporciona información de contacto, un pequeño nav, íconos de redes sociales y el copyright.

---

## Decisiones técnicas clave

- **Paleta de colores y tipografía**
  - La selección de colores (marrón, beige, blanco) y fuentes (Pacifico y Montserrat) es fundamental para establecer la identidad de la marca.
  - Pacifico se utiliza para títulos y logos, evocando un estilo artesanal y amigable, mientras que Montserrat ofrece una tipografía limpia y legible para el cuerpo del texto.

- **Unidades de medidas responsivas**
  - El uso de rem y em en lugar de px. Esto asegura que el diseño no se rompa en diferentes dispositivos y que la página sea accesible para personas que necesitan cambiar el tamaño de la fuente en su navegador. Esta flexibilidad es un pilar del diseño web moderno.

- **Disposición de las secciones features y gallery**
  - El uso de CSS Grid (display: grid) para la sección de características y la galería simplifica el diseño de la página y su adaptación a diferentes tamaños de pantalla. La propiedad display: contents; se utiliza para que los elementos hijos se comporten como si estuvieran directamente dentro de la cuadrícula, permitiendo un control más preciso del diseño.

- **Uso de propiedades específicas clave**
  - El uso de backdrop-filter: blur(8px) le da un efecto de transparencia al área detrás del header.
  - El uso de la propiedad background-blend-mode: multiply hace que el color del fondo y la imagen se multipliquen, lo que le da un efecto oscurecido.
  - El uso de overflow: hidden y object-fit: cover en las secciones features, testimonials y gallery hace que las imágenes no se desborden del contenedor y se ajusten al tamaño de este.
