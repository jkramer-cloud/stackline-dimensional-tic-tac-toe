# Stackline changelog

## v2.1 — Scene selectors, tower-following camera, and dimensional badges (October 29, 2026)

- Added clickable L# level selectors directly beside the 3D board layers in Stacked and Hyper modes.
- Added T# selectors above every tower in the Hyper world overview.
- Corrected the Hyper focus bug: towers retain separate X coordinates, so selecting T1–T5 moves the camera to the actual target tower.
- Added a smooth camera transition, focus/overview toggle, and dimmed neighboring towers when focused.
- Kept all existing sidebar selectors and keyboard controls.
- Updated the three mode tabs with stylized embossed 2D, 3D, and 4D lettering.
- Prevented scene selector clicks from making accidental moves and simplified small-screen Hyper overview labels.
- Retained computer opponents, Spatial Reasoning Lab, saved matches, gameplay rules, and custom player pieces.

## v2.0 — Computer opponents and Spatial Reasoning Lab (October 28, 2026)

- Added Explorer, Strategist, and Master computer opponents for student-versus-computer matches.
- Preserved the existing local multiplayer modes, custom player pieces and colors, camera rotation, undo, and saved matches.
- Added adjustable Explorer, Standard, and Expert puzzle complexity and four procedural reasoning puzzle types: finish the line, block the line, straight versus bent, and count changing coordinate axes.
- Added puzzle hints, answer feedback, first-try tracking and format-specific progress storage.
- Puzzles operate on the same exact 2D, 3D, and 4-coordinate winning-line geometry as multiplayer.
- Lab preserves the currently open match and restores it when exited.
- No external game framework, AI API, analytics, or account required.

## v1.0 — Initial Stackline

- Classic 3×3, Stacked 4×4×4, and Hyper 5×5×5×5 games with transparent boards, custom pieces and multi-axis win checking.
