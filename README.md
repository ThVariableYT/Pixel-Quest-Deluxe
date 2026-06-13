# 🎮 Pixel Quest Deluxe

<img width="2816" height="1536" alt="logo" src="https://github.com/user-attachments/assets/c5f5781b-df60-4a2f-b5e5-29132552fe82" />

A pixel-art style RPG platformer that runs entirely in the browser.

## Overview

**Pixel Quest Deluxe** is a browser-based 2D platformer with a retro pixel-art aesthetic. Players explore a shattered realm, collect crystals, avoid hazards, and restore the Realm Core across multiple themed levels.

The project runs from a single `index.html` file and uses HTML5 Canvas, vanilla JavaScript, Web Audio API, Tailwind CSS, and Google Fonts — no build tools or dependencies required.

## Live Demo

▶️ **[Play Now](https://thvariableyt.github.io/Pixel-Quest-Deluxe/)**

## Features

| Feature | Description |
|---|---|
| Pixel-art rendering | Canvas rendered at 640×360 and scaled for a crisp retro look |
| Multiple themed levels | Each level has its own atmosphere, hazards, and music style |
| 4 playable characters | Paladin, Assassin, Sorcerer, and Windwalker with unique stats and abilities |
| Retro synth audio | Procedural audio built with the Web Audio API — no audio files required |
| Dynamic lighting | Darkness system with radial lighting effects around the player |
| Story sequences | Dialogue scenes with a typewriter-style presentation |
| Mobile support | On-screen controls for touch devices |
| Remappable controls | Keyboard controls can be changed in-game |
| Fullscreen support | Uses the Fullscreen API with CSS fallback |
| Particle effects | Includes dust, dash trails, sparkles, and ambient effects |
| Advanced movement | Coyote time, jump buffering, wall sliding, wall jumping, and air dashing |
| Pause & timing | Pause controls and personal best time tracking |

## Gameplay

### Objective

Collect all crystals in each level and reach the goal tile to finish the stage. Spikes and lava are instant-kill hazards.

### Core Loop

1. Start the game from the main menu
2. Select a character
3. Traverse the level using jumping, dashing, and wall-jumping
4. Collect all crystals
5. Reach the goal to unlock the next stage
6. Progress through story scenes between levels

### Tips

- Use wall slide and wall jump to navigate tight vertical sections
- Save your mid-air dash for gaps or hazard recovery
- Coyote time and jump buffering make movement more forgiving
- In darker levels, staying near lit areas improves visibility

## Controls

### Keyboard

| Action | Keys |
|---|---|
| Move Left | `ArrowLeft` / `A` |
| Move Right | `ArrowRight` / `D` |
| Jump | `Space` / `ArrowUp` / `W` |
| Dash | `Shift` / `Z` / `X` |
| Advance Dialogue | `Space` / jump key |

### Touch

On touch-enabled devices, on-screen controls appear for movement, jump, and dash.

### Remapping

Controls can be remapped from the **Controls** screen in the main menu.

## Characters

| Character | Role | Speed | Jump Force | Dash Speed | Dash Duration | Dash Cooldown | Special |
|---|---|---|---|---|---|---|---|
| ⚔️ Paladin | Vanguard | 220 | -400 | 500 | 0.25s | 0.8s | Balanced all-rounder |
| 🥷 Assassin | Shadow | 250 | -450 | 400 | 0.2s | 0.6s | Double jump |
| 🧙 Sorcerer | Spellcaster | 185 | -365 | 565 | 0.35s | 0.5s | Long powerful dash |
| 🍃 Windwalker | Scout | 230 | -380 | 450 | 0.2s | 0.7s | Hold jump to glide |

## Levels

| # | Level Name | Theme | Darkness | Hazards |
|---|---|---|---|---|
| 1 | The Green Valley | Forest | None | Spikes |
| 2 | Echoing Caves | Cave | 85% | Spikes |
| 3 | The Infernal Keep | Volcano | 30% | Spikes, Lava, Springs |
| 4 | Crystal Caverns | Ice | 60% | Spikes, Lava, Springs |
| 5 | The Void | Void | 90% | Spikes, Lava, Springs |
| 6 | Sky Ruins | Sky | None | Spikes, Springs |
| 7 | Swamp Depths | Swamp | 70% | Spikes, Lava, Springs |
| 8 | The True Core | Core | 50% | Spikes, Lava, Springs |
| 9 | The Ascension | Void | 80% | Spikes, Lava, Springs |
| 10 | The Wizard's Throne | Core | None | Boss Fight |

### Tile Legend

| Symbol | Meaning |
|---|---|
| `P` | Player start position |
| `#` | Solid platform tile |
| `C` | Crystal / collectible |
| `G` | Goal / exit |
| `^` | Spring pad |
| `S` | Spike |
| `~` | Lava |
| `.` | Empty space |

## Story

The Dark Wizard has shattered the Realm Core and scattered its fragments across dangerous lands. The player journeys through forests, caves, volcanic ruins, icy caverns, the void, sky ruins, swamps, and the core itself — ultimately confronting the wizard in his throne. Story dialogue unfolds between each stage.

## Technical Details

- **Engine:** Vanilla JavaScript with HTML5 Canvas
- **Internal Resolution:** 640×360 (32px tiles)
- **Audio:** Procedural Web Audio API synthesis — no audio files needed
- **Rendering:** Offscreen canvas + dedicated light canvas for darkness effects
- **Physics:** Custom gravity, acceleration, coyote time, jump buffering, wall sliding, and wall jumping
- **Styling:** Tailwind CSS via CDN + custom CSS
- **Fonts:** Press Start 2P via Google Fonts

## Running Locally

```bash
git clone https://github.com/ThVariableYT/Pixel-Quest-Deluxe.git
cd Pixel-Quest-Deluxe
```

Then open `index.html` in any modern browser. No server or build step required.

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for the full version history.

## Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the repository
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
5. Open a pull request

## License

This project is licensed under the [MIT License](LICENSE).

---

Made with ❤️ by [ThVariableYT](https://github.com/ThVariableYT)
