# falla_el_juego
# 🎼 El Viaje Musical de Falla

![Licencia](https://img.shields.io/badge/Licencia-MIT-blue.svg)
![Estado](https://img.shields.io/badge/Estado-Completado-brightgreen.svg)
![Tecnologías](https://img.shields.io/badge/Tecnologías-HTML5%20%7C%20Canvas%20%7C%20Tone.js%20%7C%20Tailwind-orange)

Un videojuego interactivo de plataformas y aventura en **un único archivo HTML** creado como homenaje al ilustre compositor español Manuel de Falla. 

Con un encantador estilo visual inspirado en el tebeo clásico español (tipo Bruguera/Ibáñez), el juego lleva a los jugadores (especialmente diseñado para público infantil) a través de un viaje mágico que conecta su obra musical desde la soleada Andalucía, pasando por la misteriosa Atlántida sumergida, hasta llegar a las cumbres nevadas de Argentina.

## ✨ Características Principales

*   **Renderizado Procedimental:** Gráficos, fondos y personajes dibujados enteramente mediante código en HTML5 `<canvas>`, sin dependencias de imágenes externas.
*   **Audio Generativo a prueba de fallos:** Música y efectos de sonido creados en tiempo real utilizando [Tone.js](https://tonejs.github.io/). Implementa sintetizadores polifónicos (`PolySynth`) y el reloj interno de la API para garantizar un rendimiento óptimo sin cuelgues (*scheduling collisions*).
*   **Diseño 100% Responsivo:** Interfaz adaptativa construida con **Tailwind CSS**. El lienzo del juego se ajusta dinámicamente a cualquier resolución de pantalla (PC, tablet o móvil).
*   **Controles Híbridos:** Soporte nativo para teclado en escritorio y controles táctiles translúcidos en pantalla para dispositivos móviles.
*   **Físicas y Colisiones AABB:** Sistema de gravedad, flotabilidad (en fases acuáticas) y colisiones sólido y fluido.

## 🗺️ Los Niveles (El Recorrido)

El juego cuenta con tres fases generadas de forma procedimental, cada una con sus propios fondos *parallax*, gravedades y mecánicas:

1.  🇪🇸 **Nivel 1: Andalucía.** Plataformas terrestres bajo el Sol y la silueta de Cádiz. Inspirado en *Noches en los jardines de España*.
2.  🌊 **Nivel 2: La Atlántida.** Falla pilotea su icónico **Submarino Blue-Bot**. Mecánica de nado (flotabilidad), esquivando medusas entre las ruinas sumergidas de los palacios de cristal. Inspirado en *El amor brujo*.
3.  🇦🇷 **Nivel 3: Argentina (Alta Gracia).** Escalada de plataformas montañosas bajo los gélidos picos de la Cordillera de los Andes. Inspirado en la cantata monumental *La Atlántida*.

## 🎮 Controles

### Ordenador (PC / Mac)
*   **Moverse:** `Flecha Izquierda` / `Flecha Derecha` (o `A` / `D`)
*   **Saltar / Nadar:** `Flecha Arriba`, `W` o `Barra Espaciadora`

### Dispositivos Móviles (Tablets / Smartphones)
*   El juego detecta pantallas táctiles y muestra automáticamente botones virtuales en la parte inferior de la pantalla para el movimiento lateral y el salto.

## 🚀 Cómo Jugar / Instalación

Al estar empaquetado en una arquitectura de **archivo único**, no necesitas instalar Node.js, Webpack, ni servidores complejos:

1. Clona o descarga este repositorio.
2. Haz doble clic en el archivo `falla_aventura.html` para abrirlo en cualquier navegador web moderno (Chrome, Firefox, Safari, Edge).
3. ¡Haz clic en "Comenzar Aventura" y disfruta!

*Nota: Para el correcto funcionamiento del audio, es necesario que el dispositivo tenga conexión a internet la primera vez que se abre para cargar la librería Tone.js desde su CDN.*

## 🛠️ Tecnologías Utilizadas

*   **HTML5 & Canvas API:** Motor gráfico 2D, renderizado de formas y sistema de cámara *side-scrolling*.
*   **JavaScript (Vanilla ES6+):** Lógica del juego, físicas, generación procedimental y gestión de estados (Bucle `requestAnimationFrame`).
*   **Tailwind CSS (v3 via CDN):** Estilizado de la Interfaz de Usuario (UI), tipografías, modales emergentes y *game over* screens.
*   **Tone.js (v14):** Motor de síntesis de audio para la música de fondo y los efectos (salto, moneda, daño).

## 👨‍💻 Arquitectura del Código

El archivo HTML está dividido en tres secciones claramente comentadas para facilitar su estudio y modificación:
1.  **`<head>` y `<style>`:** Importación de librerías, tipografías y CSS personalizado para elementos inyectados.
2.  **Estructura HTML (UI Layer):** Pantallas superpuestas, HUD de vidas/puntuación y botones usando clases utilitarias de Tailwind.
3.  **`<script>` (Lógica Core):**
    *   Configuración y Audio (Contexto Tone.js).
    *   Entidades (`player`, `platforms`, `items`, `enemies`).
    *   Motor de Físicas y Colisiones.
    *   Renderizado de Entorno y Fondos Parallax.
    *   Bucle Principal (`update` & `draw`).
    *   Control de Estados y Eventos de Teclado/Táctiles.

## 🤝 Contribución

Este proyecto es de código abierto y tiene un fuerte enfoque educativo. ¡Las contribuciones, informes de errores (issues) y pull requests son más que bienvenidos! Si tienes ideas para nuevos niveles, enemigos, o melodías de Falla generadas con Tone.js, no dudes en participar.

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - mira el archivo [LICENSE.md](LICENSE) para más detalles.
