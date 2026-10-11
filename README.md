# Portfolio Website

Personal developer portfolio and interactive resume featuring a single-file architecture, glassmorphic design, custom 3D dot-matrix canvas background, and GSAP animations.

**Live Site:** [fa-iizii.github.io](https://fa-iizii.github.io/) / [fa3z.com](https://fa3z.com/)

## Key Features

- **Single-File Architecture:** Vanilla HTML5, CSS3, and JavaScript bundled in a single file (`index.html`) for performance.
- **Glassmorphic Aesthetic:** Frosted glass UI cards utilizing `backdrop-filter: blur()` over an interactive background.
- **Interactive Background:** Custom canvas dot-matrix grid reacting to cursor proximity, pointer movement, and click ripples.
- **Animations & Scrolling:** Velocity-reactive marquee tickers and character-splitting title animations powered by GSAP, ScrollTrigger, and Lenis.
- **Multilingual Boot Intro:** Boot screen featuring multilingual greetings assembled from dot-matrix particles.
- **Interactive Easter Eggs:** Built-in playable Snake arcade game and hacker-style string scramble sequence.

## Technical Stack

- **Markup & Styling:** HTML5, CSS3, CSS Custom Properties, Flexbox/Grid
- **Scripting:** Vanilla JavaScript (ES6+), Canvas API, Intersection Observer
- **Libraries:** 
  - GSAP & ScrollTrigger (Animations)
  - Lenis (Smooth scrolling)
- **Hosting:** GitHub Pages

## Project Structure

```text
/
├── index.html        # Core application (HTML, CSS, and JS)
├── README.md         # Documentation
└── /images           # Optimized project assets
    ├── campus.png
    ├── python.png
    ├── ml-data.jpg
    ├── smartguard.jpg
    ├── rc-car.jpg
    └── python-projects.jpg
```

## Local Development

No complex build tools or package managers are required.

1. Clone or download the repository.
2. Ensure the `images` folder contains all required project asset files with matching lowercase names.
3. Open `index.html` in any modern web browser.

---
*Designed & Developed by [Faiz Muhammed](https://uk.linkedin.com/in/faiz-muhammed/)*
