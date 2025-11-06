# Chip Factory Game

[![GitHub Pages](https://img.shields.io/badge/Play-Online-blueviolet.svg)](https://meanharsh.github.io/chip-factory-game/src/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Built With](https://img.shields.io/badge/built%20with-HTML5%20%7C%20CSS%20%7C%20JS-ffc107.svg)](#tech-stack)

> Learn how modern semiconductor devices are assembled by stacking layers in a retro arcade puzzle.

---

## Table of Contents
1. [Overview](#overview)
2. [Live Demo](#live-demo)
3. [Gameplay Highlights](#gameplay-highlights)
4. [Chip Curriculum](#chip-curriculum)
5. [Controls](#controls)
6. [Tech Stack](#tech-stack)
7. [Getting Started](#getting-started)
8. [Development Scripts](#development-scripts)
9. [Deployment](#deployment)
10. [Learning Resources](#learning-resources)
11. [Roadmap](#roadmap)
12. [Contributing](#contributing)
13. [License](#license)
14. [Acknowledgements](#acknowledgements)
15. [Contact](#contact)

---

## Overview
Chip Factory is an educational puzzler that translates the multi-layer semiconductor fabrication process into intuitive Tetris-like gameplay. Every layer you place mirrors a real manufacturing step—perfect for students, hobbyists, or anyone curious about how chips power everything from smartphones to avionics.

### Why You'll Love It
- 🧠 **Authentic learning** – Accurate fabrication steps grounded in semiconductor packaging research.
- 🕹️ **Retro-inspired UI** – Neon grids, responsive typography, and smooth canvas rendering.
- 🧩 **Layer-by-layer mastery** – Six to seven distinct layers per chip device.
- 📈 **Skill feedback** – Scores, perfect placement streaks, and real-world facts after each build.

---

## Live Demo
👉 **Play now:** https://meanharsh.github.io/chip-factory-game/src/

For the best experience, use the latest version of Chrome, Edge, or Safari.

---

## Gameplay Highlights
- **Growing Complexity:** Each device now stacks 6–7 fabrication layers to mirror real production flows.
- **Forced Orientation:** Pieces drop misaligned, encouraging spatial reasoning before locking them in place.
- **Blueprint Visuals:** A holo-style blueprint updates in real time so you never lose sight of the target stack.
- **Short Circuit Protection:** Misplaced cells trigger an electrical fault with actionable diagnostics.

---

## Chip Curriculum

| Device | Layers (bottom → top) | Real-World Focus |
| ------ | --------------------- | ---------------- |
| **Logic Switch (Transistor)** | Silicon wafer • Shallow trench isolation • Well implants • Gate oxide • Gate stack • Spacers & silicide • Metal contacts | Front-end-of-line CMOS fabrication |
| **Memory Stack (DRAM)** | Silicon substrate • Isolation grid • Deep capacitor trenches • Storage dielectric • Access transistor • Bit-line metal • Bond pads | 1T1C DRAM cell packaging |
| **Power Manager (PMIC)** | Power substrate • Epitaxial drift region • Copper spreaders • Driver FET array • Interconnect mesh • Solder bumps | High-current power management IC |

Each successful build ties your work to a real application—think iPhone RAM buffers, jet engine controllers, or electric vehicle power stages.

---

## Controls

| Input | Action |
| ----- | ------ |
| ← / → | Move piece horizontally |
| ↑ / Z | Rotate 90° |
| ↓ | Soft drop |
| Space | Hard drop |
| P | Pause/unpause |

---

## Tech Stack
- **HTML5 Canvas** for rendering and ghost-layer previews.
- **Vanilla JavaScript** state machine for game logic, scoring, and collision checks.
- **Retro UI theme** handcrafted in modern CSS (neon grid, outlines, and glass panels).
- **GitHub Actions** deployment pipeline for GitHub Pages.

---

## Getting Started

### Requirements
- A modern browser (Chrome, Edge, Firefox, or Safari).
- Optional: Python 3 or Node.js to run a local static server.

### Local Setup
```bash
git clone https://github.com/meanharsh/chip-factory-game.git
cd chip-factory-game

# Option 1: Python
python -m http.server 8000

# Option 2: Node (http-server)
npx http-server
```

Then open http://localhost:8000/src/ in your browser.

---

## Development Scripts
| Task | Command |
| ---- | ------- |
| Launch local server | `python -m http.server 8000` |
| Run Node static server | `npx http-server` |
| Format HTML/CSS/JS (manual) | Use your editor's formatter of choice |

---

## Deployment
- The project deploys from the `gh-pages` branch using the GitHub Pages workflow located at `.github/workflows/deploy.yml`.
- Whenever you push to `gh-pages`, the workflow builds the static site and publishes it to the `github-pages` environment.
- Main branch commits won’t deploy automatically—create or update `gh-pages` when you are ready to ship.

---

## Learning Resources
- [How Semiconductors Work](https://science.howstuffworks.com/semiconductor.htm)
- [Intel’s Semiconductor Manufacturing Process](https://www.intel.com/content/www/us/en/silicon-innovations/semiconductor-manufacturing-process.html)
- [SparkFun: Introduction to Transistors](https://learn.sparkfun.com/tutorials/transistors)

---

## Roadmap
- [ ] Add additional device families (RF front-end, image sensors).
- [ ] Introduce timed challenge and combo scoring.
- [ ] Support touch controls for mobile devices.
- [ ] Add multilingual facts and tooltips.

Have an idea? [Open an issue](https://github.com/meanharsh/chip-factory-game/issues/new) and let’s discuss.

---

## Contributing
Contributions are welcome! To get started:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/amazing-idea`).
3. Commit your updates with clear messages.
4. Submit a pull request describing the rationale and testing.

Please review the [Contributing Guidelines](CONTRIBUTING.md) before opening a PR.

---

## License
This project is available under the MIT License with additional attribution requirements. See [LICENSE](LICENSE) for the full text.

---

## Acknowledgements
- UI inspiration from [Retro UI](https://retroui.io/components).
- Educational direction informed by industry primers from Intel, TSMC whitepapers, and IEEE tutorials.
- Original concept and art direction by **Harsh Meena**.

---

## Contact
- **Author:** Harsh Meena — harshmiitk@gmail.com  
- **Project Page:** https://github.com/meanharsh/chip-factory-game

If you build something awesome with Chip Factory, share it—learning devices deserve a spotlight! ✨
