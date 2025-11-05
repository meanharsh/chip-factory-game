# AI Assistant Instructions for Chip Factory Game

This document guides AI coding assistants on the key aspects and conventions of this project.

## Project Overview

Chip Factory Game is an educational web game that simulates semiconductor manufacturing through puzzle mechanics. The project:
- Uses vanilla JavaScript with HTML5 Canvas for rendering
- Has no external dependencies or build tools
- Focuses on educational value while maintaining engaging gameplay
- Is designed to be lightweight and performant

## Core Architecture

The game is structured in a single-page application pattern:
- `src/index.html` contains all game code (HTML, CSS, JavaScript)
- Uses embedded styles and scripts for simplicity
- Canvas-based rendering in a responsive container
- Game state management through vanilla JavaScript

### Key Components:
1. Game initialization and loop (around line 300)
2. Canvas rendering functions (around line 500)
3. Input handling and controls (around line 800)
4. Chip pattern definitions (around line 1000)

## Development Workflow

### Local Development
```bash
# Serve the project (either method works):
python -m http.server 8000
# OR
npx http-server

# Access the game at:
http://localhost:8000/src/
```

### Deployment
The game is hosted on GitHub Pages from the `gh-pages` branch. The `src` directory is the root of the deployed site.

## Project Conventions

1. **Code Organization:**
   - All game logic is in `index.html` for simplicity
   - CSS uses modern features like flexbox and CSS Grid
   - JavaScript follows functional programming patterns

2. **Canvas Usage:**
   - Canvas size is responsive to viewport
   - Double buffering used for smooth rendering
   - Custom drawing utilities for common shapes

3. **Game State:**
   - State managed through vanilla JS objects
   - No global variables except for core game instance
   - Event-based communication between components

## Integration Points

1. **User Input:**
   - Arrow keys for movement
   - Space bar for instant drop
   - P key for pause
   - Touch/click controls for mobile support

2. **Game Loop:**
   - Fixed timestep for physics
   - Render loop synchronized with browser
   - State updates decoupled from rendering

## Common Tasks

1. **Adding New Chip Types:**
   - Define pattern in chip patterns section
   - Add corresponding score values
   - Create preview graphics
   - Update selection UI

2. **Modifying Game Rules:**
   - Speed settings in game configuration
   - Scoring system in score calculation logic
   - Level progression in game loop

## Copyright Notice

All modifications must maintain the copyright header and credits to the original author (Harsh Meena). See README.md for full license terms.