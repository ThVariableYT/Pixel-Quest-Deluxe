# 🎮 Pixel Quest Deluxe

<img width="2816" height="1536" alt="logo" src="https://github.com/user-attachments/assets/8e963db4-f6f5-426e-a4c8-5c8ea61e32ca" />

A pixel-art style RPG platformer that runs entirely in the browser. [page:1]

## Overview

**Pixel Quest Deluxe** is a browser-based 2D platformer with a retro pixel-art aesthetic. Players explore a shattered realm, collect crystals, avoid hazards, and restore the Realm Core across multiple themed levels. [page:1]

The project runs from a single `index.html` file and uses HTML5 Canvas, vanilla JavaScript, Web Audio API, Tailwind CSS, and Google Fonts. [page:1]

## Live Demo

Play here: [Pixel Quest Deluxe](https://thvariableyt.github.io/Pixel-Quest-Deluxe/) [page:1]

## Features

| Feature | Description |
|---|---|
| Pixel-art rendering | Canvas rendered at 640×360 and scaled for a crisp retro look. [page:1] |
| Multiple themed levels | Each level has its own atmosphere, hazards, and music style. [page:1] |
| Playable characters | Includes Knight, Ninja, and Mage in the character section of the current README. [page:1] |
| Retro synth audio | Procedural audio built with the Web Audio API, with no audio files required. [page:1] |
| Dynamic lighting | Darkness system with radial lighting effects around the player. [page:1] |
| Story sequences | Dialogue scenes with a typewriter-style presentation. [page:1] |
| Mobile support | On-screen controls for touch devices. [page:1] |
| Remappable controls | Keyboard controls can be changed in-game. [page:1] |
| Fullscreen support | Uses the Fullscreen API with fallback behavior. [page:1] |
| Particle effects | Includes dust, dash trails, sparkles, and ambient effects. [page:1] |
| Advanced movement | Supports coyote time, jump buffering, wall sliding, wall jumping, and air dashing. [page:1] |
| Pause and timing systems | Includes pause controls and personal best time tracking. [page:1] |

## Gameplay

### Objective

Collect all crystals in each level and reach the goal tile to finish the stage. Spikes and lava are instant-kill hazards. [page:1]

### Core Loop

1. Start the game from the main menu. [page:1]
2. Select a character. [page:1]
3. Traverse the level using movement mechanics like jumping, dashing, and wall-jumping. [page:1]
4. Collect all crystals in the level. [page:1]
5. Reach the goal to unlock the next stage. [page:1]
6. Progress through story scenes between levels. [page:1]

### Tips

- Use wall slide and wall jump to navigate tight vertical sections. [page:1]
- Save your mid-air dash for gaps or hazard recovery. [page:1]
- Coyote time and jump buffering make movement more forgiving. [page:1]
- In darker levels, staying near lit areas improves visibility. [page:1]

## Controls

### Keyboard Controls

| Action | Keys |
|---|---|
| Move Left | `ArrowLeft` / `A` [page:1] |
| Move Right | `ArrowRight` / `D` [page:1] |
| Jump | `Space` / `ArrowUp` / `W` [page:1] |
| Dash | `Shift` / `Z` / `X` [page:1] |
| Advance Dialogue | `Space` / jump key [page:1] |

### Touch Controls

On touch-enabled devices, the game displays on-screen controls for movement, jump, and dash. [page:1]

### Remapping

You can remap controls from the **Controls** screen in the main menu. [page:1]

## Characters

### ⚔️ Knight

A balanced default character recommended for beginners. [page:1]

| Stat | Value |
|---|---|
| Speed | 220 [page:1] |
| Jump Force | -400 [page:1] |
| Dash Speed | 500 [page:1] |
| Dash Duration | 0.25s [page:1] |
| Dash Cooldown | 0.8s [page:1] |

### 🥷 Ninja

A fast character with a higher jump and a shorter dash cooldown. [page:1]

| Stat | Value |
|---|---|
| Speed | 250 [page:1] |
| Jump Force | -450 [page:1] |
| Dash Speed | 400 [page:1] |
| Dash Duration | 0.2s [page:1] |
| Dash Cooldown | 0.6s [page:1] |

### 🧙 Mage

A slower character with a stronger, longer dash. [page:1]

| Stat | Value |
|---|---|
| Speed | 185 [page:1] |
| Jump Force | -365 [page:1] |
| Dash Speed | 565 [page:1] |
| Dash Duration | 0.35s [page:1] |
| Dash Cooldown | 0.5s [page:1] |

## Levels

The current README describes 8 handcrafted levels with different hazards, themes, and music. [page:1]

| # | Level Name | Theme | Darkness | Hazards | Music |
|---|---|---|---|---|---|
| 1 | The Green Valley | Forest | None | Spikes | Forest Drone [page:1] |
| 2 | Echoing Caves | Cave | High (85%) | Spikes | Cave Drone [page:1] |
| 3 | The Infernal Keep | Volcano | Low (30%) | Spikes, Lava, Springs | Volcano Synth [page:1] |
| 4 | Crystal Caverns | Ice | Medium (60%) | Spikes, Lava, Springs | Ice Chimes [page:1] |
| 5 | The Void | Void | Very High (90%) | Spikes, Lava, Springs | Void Bass [page:1] |
| 6 | Sky Ruins | Sky | None | Spikes, Springs | Sky Bells [page:1] |
| 7 | Swamp Depths | Swamp | High (70%) | Spikes, Lava, Springs | Swamp Tones [page:1] |
| 8 | The True Core | Core | Medium (50%) | Spikes, Lava, Springs | Core Synth [page:1] |

### Tile Legend

| Symbol | Meaning |
|---|---|
| `P` | Player start position [page:1] |
| `#` | Solid platform tile [page:1] |
| `C` | Crystal / collectible [page:1] |
| `G` | Goal / exit [page:1] |
| `^` | Spring pad [page:1] |
| `S` | Spike [page:1] |
| `~` | Lava [page:1] |
| `.` | Empty space [page:1] |

## Story

The Dark Wizard has shattered the Realm Core and scattered its fragments across dangerous lands. The player journeys through forests, caves, volcanic ruins, icy caverns, the void, sky ruins, swamps, and the core itself while story dialogue unfolds between stages. [page:1]

## Technical Details

- Engine: Vanilla JavaScript with HTML5 Canvas. [page:1]
- Internal resolution: 640×360. [page:1]
- Audio: Procedural Web Audio API synthesis. [page:1]
- Rendering: Offscreen canvas and dedicated light canvas. [page:1]
- Physics: Custom gravity, acceleration, coyote time, jump buffering, wall sliding, and wall jumping. [page:1]
- Styling: Tailwind CSS via CDN plus custom CSS. [page:1]
- Fonts: Press Start 2P via Google Fonts. [page:1]

## Running Locally

```bash
git clone https://github.com/ThVariableYT/Pixel-Quest-Deluxe.git
cd Pixel-Quest-Deluxe
```

Then open `index.html` in any modern browser. [page:1]

## Update History

The current README includes version history from `v1.0.0` through `v1.11.0`, covering the initial release, core engine work, character selection, fullscreen support, control remapping, speedrun timing, pause features, and an endgame expansion. [page:1]

You can keep the full changelog here, or move detailed version notes into a separate `CHANGELOG.md` for a shorter README. [page:1]

## Contributing

Contributions, issues, and feature requests are welcome. [page:1]

1. Fork the repository. [page:1]
2. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your feature"
   ```
4. Push to your branch:
   ```bash
   git push origin feature/your-feature
   ```
5. Open a pull request. [page:1]

## License

This project is intended to be licensed under the MIT License, but the current README links to an incorrect Google Docs URL rather than a standard license file. Replace that link with a local `LICENSE` file once added. [page:1]

Example:

```md
This project is licensed under the [MIT License](LICENSE).
```

---

Made with ❤️ by [ThVariableYT](https://github.com/ThVariableYT)
