# Portafolio Interactivo - CaféCode

Landing page de un negocio ficticio (CaféCode, cafetería y coworking) hecha con **Bootstrap 5**, **Transformaciones CSS** y **Animaciones CSS**. Totalmente responsiva.

## Estructura
- `index.html`: estructura de la página con Bootstrap 5 (CDN).
- `styles.css`: estilos, transformaciones y animaciones.

## Bootstrap 5
- **Navbar** `bg-dark` con logo y menú (Inicio, Proyectos, Contacto) que colapsa en hamburguesa en móviles.
- **Grid**: `container`, `row`, `col-sm-12`, `col-md-6`, `col-lg-4`.
- **Formulario** con `form-label`, `form-control`, `mb-3` (Nombre, Email, Mensaje).
- **Botones** "Enviar" (`btn btn-primary`) y "Limpiar" (`btn btn-secondary`) dentro de `d-grid gap-2`.

## Transformaciones 2D (con `transition`)
| Caja | Efecto en `:hover` |
|------|--------------------|
| Menú Digital | `rotate(8deg)` |
| App de Reservas | `scale(1.1)` |
| Tienda Online | `translateY(-20px) skew(-6deg)` |

Todas usan `transition: transform 0.5s ease` para un cambio suave.

## Transformaciones 3D
- Contenedor `.escena` con `perspective: 1000px`.
- `.tarjeta-3d` con `transform-style: preserve-3d` que gira con `rotateY(180deg) rotateX(10deg)` y muestra su reverso (`backface-visibility: hidden`).
- `.cubo-perspectiva` inclinado con `rotateX(20deg) rotateY(-25deg)` que cambia de ángulo al hacer hover.

## Animaciones (`@keyframes`)
- **`girar`**: loader (spinner) al inicio de la página y dentro del botón "Enviar". `animation-duration: 1s`, `animation-iteration-count: infinite`, `animation-timing-function: linear`.
- **`deslizarIzquierda`**: el título y subtítulo aparecen deslizándose desde la izquierda (`ease-out`, 1 iteración).
- **`colorTamano`**: círculo que cambia de color y tamaño constantemente (`infinite`, `ease-in-out`, `alternate`).
- **`pulso`**: brillo pulsante del botón "Ver proyectos".

## Cómo verlo
Abrir `index.html` en el navegador.
