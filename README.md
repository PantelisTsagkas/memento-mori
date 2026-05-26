# Life in Weeks

> *"The days are long but the decades are short."*

A single-page web app that renders your entire lifespan as a grid of squares — one square per week, 52 columns wide, one row per year. Inspired by Tim Urban's [Your Life in Weeks](https://waitbutwhy.com/2014/05/life-weeks.html) and the stoic practice of *memento mori*.

![Life in Weeks — dark mode](https://img.shields.io/badge/theme-dark%20%2F%20light-1a1a1f?style=flat-square) ![Vanilla JS](https://img.shields.io/badge/built%20with-vanilla%20JS-f5c542?style=flat-square) ![No dependencies](https://img.shields.io/badge/dependencies-none-4ade9a?style=flat-square)

---

## Features

- **Week-resolution grid** — 52 columns × configurable life expectancy rows; each cell is one week of your life
- **Life stage colours** — five distinct colour bands (Childhood, Teenage, Young Adult, Adulthood, Senior) using CSS custom properties
- **Current week indicator** — the week you're in right now pulses with a white glow so you always know exactly where you stand
- **Interactive tooltips** — hover any square to see the exact calendar date range, your age, and life stage
- **Live stats** — years lived, weeks elapsed, weeks remaining, and percentage of life elapsed
- **Progress bar** — a linear sweep across your full lifespan
- **Dark / light mode** — toggle persisted to `localStorage` with a smooth transition; light is the default
- **Configurable inputs** — enter any date of birth and life expectancy; grid re-renders instantly
- **Responsive** — adapts square size and gap at ≤600px for comfortable mobile viewing
- **Zero dependencies** — pure HTML, CSS, and vanilla JavaScript; no build step, no frameworks

---

## Life Stages

| Stage | Age Range | Colour |
|---|---|---|
| Childhood | 0 – 12 | 🟢 Green |
| Teenage | 13 – 19 | 🔵 Sky blue |
| Young Adult | 20 – 35 | 🟣 Purple |
| Adulthood | 36 – 64 | 🟠 Orange |
| Senior | 65 + | 🩷 Pink |
| Future (unfilled) | — | ⬜ Outline only |

---

## Getting Started

No installation or build step required.

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/life-in-weeks.git

# Open directly in your browser
open index.html
```

Or just drag `index.html` into any browser tab.

### Usage

1. Enter your **Date of Birth** in the input field
2. Optionally adjust the **Life Expectancy** (default: 90 years)
3. Click **Update** — the grid, stats, and progress bar all re-render
4. Toggle between dark and light mode with the ☀ / 🌙 button (top-right)
5. Hover any square to see its exact date range and life stage

---

## Project Structure

```
life-in-weeks/
└── index.html     # Everything — HTML, CSS, and JS in one self-contained file
```

---

## Design

- **Typography** — [Playfair Display](https://fonts.google.com/specimen/Playfair+Display) (headings) + [DM Mono](https://fonts.google.com/specimen/DM+Mono) (UI)
- **Theming** — CSS custom properties (`--bg`, `--surface`, `--border`, stage colours) make both themes a single class override on `<body>`
- **Texture** — inline SVG `feTurbulence` noise overlay for depth without external assets
- **Animations** — CSS `@keyframes` pulse on the current week; staggered `fadeIn` on load

---

## Browser Support

Works in all modern browsers (Chrome, Firefox, Safari, Edge). Requires JavaScript enabled.

---

## Acknowledgements

Concept inspired by [Wait But Why — Your Life in Weeks](https://waitbutwhy.com/2014/05/life-weeks.html) by Tim Urban.

---

## License

MIT — do whatever you like with it.
