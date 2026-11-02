# falla_el_juego
# 🎼 El Viaje Musical de Falla

![Licencia](https://img.shields.io/badge/Licencia-MIT-blue.svg)
![Estado](https://img.shields.io/badge/Estado-Completado-brightgreen.svg)
![Tecnologías](https://img.shields.io/badge/Tecnologías-HTML5%20%7C%20Canvas%20%7C%20Tone.js%20%7C%20Tailwind-orange)

Juego de plataformas y aventura inspirado en la vida y la obra de Manuel de Falla, desarrollado en un único archivo HTML. La historia transcurre desde Andalucía hasta Argentina, con una fase submarina en la Atlántida y un recorrido final montañoso.

El proyecto combina arte procedimental, música generativa y una interfaz con pantalla de inicio, hitos por nivel, HUD de puntos y vidas, y controles táctiles y de teclado.

## ✨ Características actuales

- Renderizado 2D completo con HTML5 Canvas, sin imágenes externas.
- Música y efectos de sonido generados con Tone.js.
- Tres niveles con progresión distinta:
  - Andalucía: plataformas terrestres y recorrido soleado.
  - Atlántida: movimiento submarino con flotabilidad y ritmo más pausado.
  - Argentina: escalada con plataformas elevadas y paisaje montañoso.
- Sistema de puntuación, vidas, enemigos y recompensas musicales.
- Pantalla de inicio, pantalla de hito por nivel y pantalla final de victoria.
- Controles híbridos: teclado en escritorio y botones táctiles en pantalla.
- Diseño responsive para distintas resoluciones y dispositivos móviles.
- Audio controlado por un botón de mute y sincronizado con el progreso del juego.

## 🗺️ Niveles del juego

1. Andalucía
   - Inspirado en la luz y la poesía de Noches en los jardines de España.
   - El jugador avanza saltando entre plataformas y recoge notas musicales.

2. Atlántida
   - El personaje pasa a tener un estilo de movimiento más submarino, con impulsos suaves y gravedad reducida.
   - La música y el ambiente se vuelven más misteriosos.

3. Argentina
   - Recorrido final con plataformas escalonadas y una sensación más épica.
   - Se llega a la conclusión del viaje con la referencia a La Atlántida.

## 🎮 Controles

### Teclado
- Izquierda: Flecha izquierda o A
- Derecha: Flecha derecha o D
- Saltar / nadar: Flecha arriba, W o Barra espaciadora

### Pantalla táctil
- Botones laterales para izquierda, derecha y salto.
- Botón de inicio para volver a la pantalla de instrucciones.
- La interfaz se adapta para ratón, lápiz o pantalla táctil.

## 🚀 Cómo ejecutar el juego

Este proyecto no requiere compilación ni dependencias locales. Basta con abrir el archivo en un navegador moderno:

1. Clona o descarga el repositorio.
2. Abre el archivo `index.html` en tu navegador.
3. Haz clic en “¡COMENZAR AVENTURA!” para iniciar.

Nota: para que el audio funcione correctamente, el navegador debe permitir la inicialización del contexto de audio tras la interacción del usuario. Si se carga desde un entorno con bloqueo de contenido, el sonido puede requerir un primer clic en la pantalla.

## 🛠️ Tecnologías utilizadas

- HTML5 y Canvas API
- JavaScript vanilla (ES6+)
- Tailwind CSS cargado desde CDN
- Tone.js para la música y los efectos sonoros

## 📁 Estructura del proyecto

- `index.html`: archivo principal del juego, con la interfaz, el estilo y la lógica del videojuego.
- `LICENSE`: licencia del proyecto.
- `README.md`: documentación del proyecto.

## 🤝 Estado del proyecto

Es una versión completa de un juego browser-based con recorrido, audio procedural, controles táctiles y tres etapas jugables. La documentación se ha actualizado para reflejar la versión actual del proyecto y eliminar información antigua o desalineada con la implementación real.

## 📄 Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.
