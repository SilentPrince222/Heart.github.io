# Heart Landing Page

A simple HTML/CSS/JavaScript implementation of a heart animation effect inspired by TikTok trends.

## Description

This project creates an interactive "Heart Landing Page" effect where:
1. Initially displays a dark screen with a centered "DECRYPT MESSAGE" button
2. When clicked, the button disappears and hundreds of small "love" text particles animate
3. Particles first fly chaotically across the screen
4. Then smoothly converge to form a filled heart shape in the center
5. Each particle is rendered as the text "love" with pink/red colors and glow effect

## Features

- Dark background (#0a0a0a)
- Interactive "DECRYPT MESSAGE" button to start animation
- HTML5 Canvas for particle rendering
- Particles as text "love" with varying sizes (6-14px)
- Pink/red color scheme with glow effect (shadowBlur)
- Heart shape formed using parametric equations
- Responsive design works on both desktop and mobile
- Particle rotation for added visual detail
- Pure HTML/CSS/JS - no external dependencies

## How to Use

1. Simply open `index.html` in any modern web browser
2. Click the "DECRYPT MESSAGE" button to start the animation
3. Enjoy the heart filling effect!

## Files

- `index.html` - Contains all HTML, CSS, and JavaScript in a single file

## Implementation Details

- Uses HTML5 Canvas for particle animation
- Heart shape generated using parametric equations:
  - x = 16 * sin³(t)
  - y = 13*cos(t) - 5*cos(2t) - 2*cos(3t) - cos(4t)
- Particles distributed using radial scaling for uniform area coverage
- Animation sequence: idle → chaos (random movement) → form (heart shape)
- Each particle rotates independently for dynamic visual effect

## Customization

Adjust these constants in the JavaScript section of index.html to modify behavior:
- `CONFIG.particleCount`: Number of particles (default: 600)
- `CONFIG.particleFontSizeMin/Max`: Text size range
- `CONFIG.chaosDuration/FormDelay`: Animation timing
- `CONFIG.particleJitter`: Position randomness
- Color scheme in `draw()` method

## License

MIT License - feel free to use and modify as desired.