# Portafolio Interactivo - CaféCode

CaféCode es una página web de ejemplo para una cafetería que también ofrece espacios de coworking. La hice utilizando HTML, CSS y Bootstrap 5, aplicando diferentes efectos visuales, transformaciones y animaciones. El diseño se adapta a distintos tamaños de pantalla.

## Estructura del proyecto

- `index.html`: contiene la estructura y los elementos de la página.
- `styles.css`: contiene los estilos, las transformaciones y las animaciones.

## Bootstrap 5

Para organizar el contenido y facilitar el diseño responsivo, utilicé Bootstrap 5 mediante CDN. Entre sus componentes se encuentran:

- Una barra de navegación con el logo y las opciones Inicio, Proyectos y Contacto. En pantallas pequeñas, el menú se convierte en un botón de hamburguesa.
- Un sistema de columnas para distribuir el contenido según el tamaño de la pantalla.
- Un formulario de contacto con campos para nombre, correo electrónico y mensaje.
- Botones para enviar y limpiar el formulario.

## Transformaciones 2D

Agregué efectos al pasar el cursor sobre las tarjetas de proyectos para darles más movimiento.

| Elemento | Efecto aplicado |
|---|---|
| Menú Digital | Gira 8 grados. |
| App de Reservas | Aumenta su tamaño al 110 %. |
| Tienda Online | Se desplaza hacia arriba y se inclina. |

Estos efectos utilizan `transition: transform 0.5s ease` para que los cambios se vean de forma gradual.

## Transformaciones 3D

También incluí algunos elementos con perspectiva para practicar las transformaciones en tres dimensiones.

- La clase `.escena` establece la perspectiva del elemento.
- La tarjeta `.tarjeta-3d` gira sobre el eje Y y muestra su reverso.
- El elemento `.cubo-perspectiva` tiene una inclinación inicial que cambia cuando se pasa el cursor sobre él.

Para conseguir estos efectos utilicé propiedades como `perspective`, `transform-style`, `rotateY()` y `backface-visibility`.

## Animaciones CSS

La página cuenta con varias animaciones creadas mediante `@keyframes`:

- `girar`: se utiliza en el indicador de carga y en el botón Enviar.
- `deslizarIzquierda`: hace que el título y el subtítulo aparezcan desplazándose desde la izquierda.
- `colorTamano`: cambia continuamente el color y el tamaño de un círculo.
- `pulso`: agrega un efecto de brillo al botón Ver proyectos.

## Cómo ejecutar el proyecto

1. Descargar o clonar el proyecto.
2. Abrir el archivo `index.html` en un navegador.
3. Probar los efectos pasando el cursor sobre las tarjetas y los botones.

No es necesario instalar dependencias para visualizar la página, ya que Bootstrap 5 se carga mediante CDN.
