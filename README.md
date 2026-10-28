# Stackline — Dimensional Tic Tac Toe

A rotatable 3D-style tic-tac-toe strategy game for the Naches Learning Hub. Students can learn spatial reasoning, multi-axis diagonals, coordinate systems, and strategic planning through three board formats. The application is self-contained: **no accounts, libraries, CDN files, or API keys**.

## Game formats

| Mode | Grid | Boards displayed | Target | Coordinate axes | Players | Winning lines |
| --- | --- | --- | --- | --- | --- | --- |
| Classic | 3 × 3 | One flat board | 3 in a row | 2 | 2–3 | 8 |
| Stacked | 4 × 4 × 4 | Four transparent 4 × 4 boards stacked vertically | 4 in a row | 3 | 2–4 | 76 |
| Hyper | 5 × 5 × 5 × 5 | Five side-by-side towers; each has five transparent 5 × 5 boards (25 total) | 5 in a row | 4 | 2–5 | 888 |

### How the four-axis mode is represented

We cannot draw four independent spatial axes directly in three-dimensional space. Hyper mode therefore represents the **fourth coordinate as a separate tower**. A move has four coordinates: column (X), row (Z), height (Y), and tower (W). A five-piece line is valid whenever the pieces form a straight line in that four-coordinate grid. For example, `(0,0,0,0) → (1,1,1,1) → ... → (4,4,4,4)` is a winning four-axis diagonal.

This is a game with *five in a row* across a four-axis grid; the row length and the number of mathematical dimensions are different quantities. The underlying game accepts all horizontal, vertical, within-board diagonal, cross-level diagonal, cross-tower diagonal, and all-axis diagonal wins. Lines that bend or skip squares are not wins.

## Controls

- **Click/tap a highlighted tile** in the rotatable 3D view to place a piece.
- **Click/tap a square in the 2D Active Board grid** for precise placement when towers overlap visually.
- **Drag** on the large game board to orbit the scene. **Mouse wheel** or the **Zoom** buttons zoom in and out.
- **View, Top, Side** select useful camera angles.
- **Height / Level tabs** choose which of the stacked boards is active.
- **Tower tabs** choose a fourth-axis coordinate in Hyper mode.
- **Focus Tower** isolates one Hyper tower for easier inspection; toggle again to see all five.
- **Threat Lens** highlights immediately winning empty positions for the current player on the selected board.
- **Undo** reverses the most recent move.
- **Up / Down arrows** change active height; **[ / ]** change the tower in Hyper mode.
- **New match** resets the board. Changing game modes or the player count starts a fresh board after confirmation.

## Player customization

Each local player chooses a name, **any six-digit RGB color** using the browser's color picker, and a piece shape: orb, cube, diamond, pyramid, ring, or star. Shapes are distinguishable without relying solely on color. The game supports two to five local players depending on the board type. It is a turn-taking, same-device game and does not require sign-in or networked multiplayer.

## Progress and privacy

- Current board, player names, player colors, shapes, and last selected view are saved automatically in the **local browser storage** (when storage is available).
- Disable **Save match in this browser** to clear the stored game and turn off future saving.
- No student identity, analytics, or game data is transmitted to a server.
- Original short synthesized sound effects can be turned off with **Sound on/off**.

## Educational opportunities

- **Visual-spatial reasoning:** Mentally rotate stacked boards and track pieces at different heights.
- **Coordinate systems:** Locate a move by 2, 3, or 4 coordinates.
- **Patterns and generalization:** Explain what makes a line straight across an extra axis.
- **Counting and combinatorics:** Compare 8, 76, and 888 possible winning lines and explain why the count grows.
- **Strategy and collaboration:** Predict, defend, and explain moves while taking turns.

Suggested discussion prompts: “What is different about a diagonal going *through* the boards?”; “How do you describe the same move in four coordinates?”; “Why does an additional axis create more winning paths?”

## GitHub Pages installation

1. Create a public GitHub repository such as `stackline-dimensional-tic-tac-toe`.
2. Upload `index.html` and `README.md` to the repository root.
3. Go to **Settings → Pages**, choose **Deploy from a branch**, then select `main` and `/ (root)`.
4. Your URL will be `https://YOUR-USERNAME.github.io/stackline-dimensional-tic-tac-toe/`. Use that as the launch link in the Learning Hub.

Alternatively, open `index.html` in a modern browser to play locally. No separate image or JavaScript files are required.

## Technical notes

The scene uses a custom interactive Canvas renderer with rotatable 3D-like orthographic projection and transparent layered grids, not a GPU 3D engine. This makes the game lightweight on school Chromebooks. Win detection enumerates all mathematically valid straight directions over 2, 3, or 4 coordinates and checks the exact positions placed. The 5×5×5×5 mode contains **625 playable positions**, organized as **25 physical boards**.

**Version:** 1.0 · Designed for the Naches Learning Hub.
