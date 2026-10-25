# Tidepool 🪼

A small arcade game that runs in your browser. Steer a glowing jellyfish, collect plankton, and dodge the sea urchins for as long as you can.

It is a single HTML file with no build step, no dependencies and no framework. Everything is plain HTML, CSS and JavaScript drawn on a `<canvas>`.

## How to play

- Swim to the glowing plankton to score points.
- Collecting plankton in a row builds a combo. Every 5 in a row raises the multiplier, up to ×5.
- Avoid the sea urchins. A hit costs one of your 3 lives and resets your combo.
- Grab a bubble to get a 6 second shield. While it is active, touching an urchin scores points instead of costing a life.
- The longer you survive, the faster and more frequent the urchins become.
- Your best score is saved in your browser.

## Controls

| Action | Desktop | Mobile |
| --- | --- | --- |
| Swim | Move the mouse, or use the arrow keys / WASD | Drag a finger |
| Pause or resume | `P`, `Esc` or `Space` | Tap Resume |
| Start | `Enter`, `Space` or the Start button | Tap Start |

The game also pauses automatically when you switch tabs.

## Tech notes

- Rendering: HTML5 Canvas, 480×640 logical size, scaled to fit any screen.
- Input: Pointer Events (mouse and touch) plus keyboard.
- Audio: short sound effects generated with the Web Audio API, with a mute button.
- Storage: best score is kept in `localStorage`.
- Font: Bricolage Grotesque from Google Fonts, with a system font fallback if it cannot load.
- Theme: the page follows your system light or dark mode. Screen shake is turned off if you prefer reduced motion.

## Credits

Made By Aarav.

## License

This project is under MIT License
