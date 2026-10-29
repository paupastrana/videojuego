# Whack-a-Mole AR 🔨

Juego de realidad aumentada: el tablero se coloca sobre una mesa o el piso y hay que tocar los topos antes de que se escondan. ¡Cuidado con las bombas!

## Archivos

- `whack-a-mole-ar.html`: todo el juego (HTML, CSS y JavaScript con three.js).


## Reglas

- Topo: **+100 puntos**.
- Bomba: **−150 puntos** y **−3 segundos**.
- Tienes **30 segundos**.
- Cada 400 puntos subes de nivel (hasta el 4): salen más rápido y se abre un hoyo nuevo.
- Si tocas y no le das a nada, apunta con el círculo del centro de la pantalla.

## Probar sin AR

Si abres el archivo en un navegador sin WebXR (por ejemplo Safari o el computador), el juego corre en una vista 3D normal. Toca los topos con el dedo o el mouse.

## Ajustes rápidos

- Tamaño del tablero: cambia `BOARD_SCALE` en el código (`0.5` = mitad del tamaño real).
- El texto verde de arriba es información de depuración. Para ocultarlo, agrega `display: none;` a `#dbg` en el CSS.

## Si algo falla

- **No aparece el tablero:** busca buena luz y una superficie con textura, y mueve el teléfono más despacio.
- **El tablero desaparece o los toques no cuentan:** revisa el texto verde de arriba (`err:`, `anchor:`, `dist:`) o la consola del navegador.
- **Sale “WebXR no está disponible”:** en iPhone, ábrelo con el enlace de Needle Go.

## Tecnologías

- [three.js](https://threejs.org/) r128
- WebXR (hit-test y anchors)
- [Needle Go](https://appclip.needle.tools/) para AR en iPhone
