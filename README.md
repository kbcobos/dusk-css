# dusk-css

Ilustración de paisaje día/noche hecha 100% con CSS puro.

## Features

- Escena en capas (cielo, astro, estrellas, nubes, montañas, árbol, suelo) armada solo con `div`s y CSS
- Toggle día/noche funcional, sin una sola línea de JavaScript (checkbox hack)
- Transiciones suaves entre paletas de color
- Animaciones sutiles: parpadeo de estrellas, deriva de nubes, pulso de luz
- Totalmente responsive: se reacomoda de forma fluida en cualquier tamaño de pantalla
- Respeta `prefers-reduced-motion` para accesibilidad

## Stack

HTML5 + CSS3 puro. Sin dependencias, ni build tools, tampoco paquetes que instalar.

## Técnicas destacadas

- **`clip-path: polygon()`** para las siluetas de montaña
- **Checkbox hack** para el toggle día/noche sin JavaScript
- **Custom properties (`--var`)** como sistema de temas: todas las capas leen su color de una variable, así el toggle solo redefine variables en vez de tocar cada elemento
- **`box-shadow` múltiple** para dibujar el campo de estrellas con un solo elemento
- **Unidades relativas (`%`, `vw`, `clamp()`, `aspect-ratio`)** en vez de píxeles fijos, para que toda la escena escale de forma fluida

## Licencia

Este proyecto está bajo la licencia [MIT](LICENSE).
