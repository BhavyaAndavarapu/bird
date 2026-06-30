# 🐦 Flappy Bird

A browser-based recreation of the classic **Flappy Bird** game, built using vanilla HTML, CSS, and JavaScript. Tap or press a key to keep the bird airborne while dodging pipes and racking up your high score.

## Features

- **Classic Gameplay** – Press the spacebar to flap and navigate the bird through pipe gaps
- **Physics-Based Movement** – Gravity and lift mechanics simulate realistic falling and flapping motion
- **Animated Pipes** – Randomly generated pipe heights with smooth scrolling animation
- **Collision Detection** – Game ends on collision with pipes, the ground, or screen boundaries
- **Score Tracking** – Live score counter that updates as you pass through pipes
- **Sound Effects** – Audio feedback for flapping, scoring points, and collisions
- **Game States** – Welcome screen, active gameplay, and game-over screen with restart support

## Project Structure

```
flappy-bird/
├── gallery/
│   ├── sprites/        # Game images (bird, pipes, background, base, messages)
│   └── audio/           # Sound effects (wing, point, hit)
├── index.html             # Main HTML file
├── style.css               # Styling and animations
└── script.js                 # Game logic and mechanics
```

## Tech Stack

- **HTML5** – Game container structure
- **CSS3** – Sprite-based styling, animations, and layout
- **JavaScript (Vanilla)** – Game loop, physics, collision detection, and state management

## Getting Started

### Prerequisites

No build tools or dependencies are required — this is a static, client-side game.

### Installation

1. Clone or download this repository:
   ```bash
   git clone https://github.com/BhavyaAndavarapu/bird
   ```
2. Navigate into the project folder:
   ```bash
   cd flappy-bird
   ```
3. Open `index.html` in your browser:
   - Double-click the file, **or**
   - Use a local development server (recommended), e.g.:
     ```bash
     npx serve .
     ```

## How to Play

1. Open the game in your browser.
2. Press the **Spacebar** to make the bird flap and start the game.
3. Keep pressing Spacebar to avoid hitting the pipes, ground, or ceiling.
4. Try to fly through as many pipes as possible to increase your score.
5. On game over, press any key to return to the welcome screen and play again.

## Game Mechanics

- **Gravity**: Continuously pulls the bird downward each frame.
- **Lift**: Pressing Spacebar applies an upward velocity to counter gravity.
- **Pipes**: Spawn from the right edge of the screen with randomized gap heights, scrolling left in a continuous loop.
- **Collision**: Detected using bounding box comparisons between the bird and pipes/boundaries.

## Customization

- **Difficulty**: Adjust `gravity` and `lift` values in `script.js` to make the game easier or harder.
- **Pipe Speed**: Modify the `pipe` animation duration in `style.css` (`animation: pipe 3s linear infinite;`).
- **Sprites**: Replace images in `gallery/sprites/` to reskin the game (keep filenames consistent, or update references in `style.css`/`index.html`).
- **Sounds**: Replace audio files in `gallery/audio/` to change sound effects.

## Browser Support

Works on all modern browsers, including Chrome, Firefox, Safari, and Edge.


## Acknowledgments

Built as a front-end practice project recreating the classic Flappy Bird game mechanics using pure JavaScript, CSS animations, and DOM manipulation.
