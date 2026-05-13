# Tracing Dendur

An interactive browser experience that lets you explore an ancient carving using your hands or mouse. A flashlight effect illuminates the carving as you trace over it.

## How It Works

The app uses your webcam and [MediaPipe Hands](https://google.github.io/mediapipe/solutions/hands) to track hand gestures in real time. The carving image is displayed in low light — you reveal it by moving your finger like a flashlight.

### Controls

| Input | Action |
|-------|--------|
| **Right index finger** | Move to trace / reveal the carving with a glowing flashlight |
| **Left index finger** | Move left/right to scroll the carving |
| **Mouse hover** | Flashlight (fallback when no hand detected) |
| **Mouse drag** | Scroll |
| **Arrow keys** | Scroll left / right |

Mouse mode activates automatically if no hand is detected for more than 1 second.

## Running It

This is a static site — no build step needed.

**Locally:** open `index.html` directly in a browser (camera requires a server or browser permission).

**Live:** hosted on GitHub Pages at  
`https://feliciatiffany.github.io/prototype_dendur_mediapipe/`

## Stack

- Vanilla HTML / CSS / JS
- [MediaPipe Hands](https://cdn.jsdelivr.net/npm/@mediapipe/hands) via CDN
- Canvas 2D API for rendering and glow effects
