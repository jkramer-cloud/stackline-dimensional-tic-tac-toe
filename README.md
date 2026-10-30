# Stackline: Dimensional Tic Tac Toe — v2.2 Retro Arcade Background

A visual-only enhancement of the supplied GitHub `index.html`.

## What's new
- Animated 1990s retro arcade environment: sunset sun, scrolling perspective grid, mountain silhouette, star sparkles, floating Memphis-style geometric shapes, and vivid violet/cyan/magenta lighting.
- A darkened central area to keep the transparent 3D board and game pieces legible.
- Retro FX on/pause button with its own browser-saved preference.
- Honors the operating system's reduced-motion accessibility setting and pauses animation while the tab is hidden.
- No external libraries, assets, or service dependencies.

## What remains unchanged
All original gameplay code from the provided Stackline source: 2D/3D/4D boards, 2–5 players, computer opponents, colors, controls, rotation, reasoning puzzles, scoring, and local match saves. The background uses a completely separate canvas positioned below the game board; it does not intercept mouse, keyboard, or touch events.

## Publish
Extract the ZIP and upload `index.html` to your existing `stackline-dimensional-tic-tac-toe` GitHub repository, replacing the old root `index.html`. Commit the change. GitHub Pages will continue serving the game at your existing address; the Naches Learning Hub needs no update.

## Test checklist
- Select Classic (2D), Stacked (3D), and Hyper (4D); ensure each renders normally.
- Make a move with the 3D board and the sidebar grid. Drag to rotate and use the zoom buttons.
- Start and exit Reasoning Lab; select a computer opponent.
- Toggle Retro FX Off and On; check the background pauses and resumes.
- Reload the page and confirm game progress and motion preference persist.
