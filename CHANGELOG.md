# Changelog

All notable changes to **Pixel Quest Deluxe** are documented here.

The format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [Unreleased]

- Bonus challenge levels: Glitch Dimension, Neon Speedway, Infernal Escape, Spike Maze, Crystal Tower

---

## [v1.11.0] — 2026-05-19

### Added
- Expanded campaign with **Level 9: The Ascension** (Void theme, 80% darkness)
- **Level 10: The Wizard's Throne** — final boss stage featuring a full boss fight against The Dark Wizard
- Boss HUD with HP bar and boss name display
- Boss fight systems: shockwave attacks, phase transitions, and defeat sequence
- Victory screen and full game ending after defeating the boss

---

## [v1.10.0] — 2026-05-18

### Added
- **Windwalker** character (Scout role): speed 230, jump force -380, dash speed 450, 0.2s dash duration, 0.7s cooldown
- Windwalker's unique ability: **hold Jump to Glide**, slowing descent mid-air
- Animated character select portraits for all four characters
- Character stat display (ATK / SPD / MAG) on the selection screen

### Changed
- Character select screen redesigned with a wider layout to accommodate the fourth slot

---

## [v1.9.0] — 2026-05-18

### Added
- Pause menu with resume and quit options
- **Personal best time tracking** — best time per level stored in `localStorage`
- Level timer display on HUD during gameplay

### Fixed
- Timer no longer increments during dialogue sequences or the pause menu

---

## [v1.8.0] — 2026-05-18

### Added
- **Speedrun timer** — per-level elapsed time shown on the HUD
- Level transition animation with area title card (`AREA X` + level name)
- Ambient particle effects on the menu background
- Cinematic animated menu background (camera panning across level map)

### Changed
- Tuned particle sizes and amplitudes to match the 640×360 internal resolution

---

## [v1.7.0] — 2026-05-15

### Added
- **Control remapping** — players can rebind all keys from the Controls screen in the main menu
- Touch D-Pad sliding support: a single touch can slide between left and right buttons
- Safe-area padding for mobile notch/home-bar devices

### Changed
- Increased player acceleration and air acceleration for snappier feel
- Extended coyote time and jump buffer window for more forgiving platforming
- Added extra friction on stop for crisper halts

---

## [v1.6.0] — 2026-05-15

### Added
- **Fullscreen toggle** button on the start screen
- Native Fullscreen API support with webkit fallbacks
- CSS fullscreen fallback mode (`.css-fullscreen-mode`) for browsers that block native fullscreen

### Fixed
- Resize event dispatched after fullscreen toggle to correctly reflow canvas and UI layouts

---

## [v1.5.0] — 2026-05-15

### Added
- **Character selection screen** with three playable characters
  - **Paladin** (Vanguard): speed 220, balanced stats, single jump
  - **Assassin** (Shadow): speed 250, double jump, fast dash cooldown
  - **Sorcerer** (Spellcaster): speed 185, extra-long dash, slowest movement
- `applyCharacterStats()` — applies selected character's stats and colors to the player at game start
- Character-specific pixel-art sprites with unique body, eye, and particle colors

---

## [v1.4.0] — 2026-05-15

### Added
- **Custom-built procedural soundtrack** using the Web Audio API (no audio files required)
  - Forest Drone (Level 1), Cave Drone (Level 2), Volcano Synth (Level 3)
  - Ice Chimes (Level 4), Void Bass (Level 5), Sky Bells (Level 6)
  - Swamp Tones (Level 7), Core Synth (Level 8)
- Retro logo rendered on the start screen using a canvas-drawn pixel banner

### Removed
- Scanlines post-processing filter (performance improvement)

### Fixed
- Audio context unlock on first user interaction to comply with browser autoplay policies

---

## [v1.3.0] — 2026-05-15

### Added
- **Dialogue / story system** with typewriter-style text reveal
- Animated portrait with "talking" bounce effect during dialogue
- Story sequences triggered between levels using a `level_clear` dialogue map
- Tap-to-advance dialogue on both keyboard and touch

---

## [v1.2.0] — 2026-05-15

### Added
- **Wall sliding** — player slows descent when pressing into a wall mid-air
- **Wall jumping** — jump away from a wall while sliding
- **Air dash** — single mid-air dash, resets on grounding or wall contact
- **Dynamic lighting system** — per-level darkness value with a radial light radius around the player
- Dedicated offscreen light canvas for darkness rendering
- Level-specific darkness settings (0% – 90%)

### Changed
- Rescaled internal resolution from a higher value to **640×360** with **32px tiles**
- Rebalanced all physics values (gravity, jump force, dash) for the new resolution
- Improved hitbox accuracy for crystals, spikes, lava, and springs

---

## [v1.1.0] — 2026-05-15

### Added
- **8 handcrafted levels**: The Green Valley, Echoing Caves, The Infernal Keep, Crystal Caverns, The Void, Sky Ruins, Swamp Depths, The True Core
- Per-level themes: `forest`, `cave`, `volcano`, `ice`, `void`, `sky`, `swamp`, `core`
- Level-specific hazards: spikes, lava tiles, spring pads
- Particle effects: dust on landing, dash trail, crystal sparkle, ambient floating particles
- Spring pad bounce mechanic
- HUD: crystal counter, level name, and area banner on level start
- Mobile on-screen D-Pad with left, right, jump, and dash buttons

### Changed
- Improved level collision detection and tile rendering
- Spring bounce force and hitbox tuned

---

## [v1.0.0] — 2026-05-15

### Added
- Initial release of **Pixel Quest Deluxe**
- Single-file HTML build (`index.html`) — no server or build tools needed
- HTML5 Canvas renderer at 640×360 with pixel scaling
- Core platformer physics: gravity, acceleration, variable jump height
- **Coyote time** — allows jumping shortly after walking off a ledge
- **Jump buffering** — queues a jump input slightly before landing
- Player pixel-art sprite with eye, headband, and scarf trail
- Crystal collectibles and goal tile
- Game Over and Victory screens
- Start screen with animated background
- Keyboard input handling (`ArrowKeys`, `WASD`, `Space`, `Shift`)
- Touch input handling for mobile browsers
- Tailwind CSS via CDN + custom CSS for UI styling
- Press Start 2P font via Google Fonts

---

[Unreleased]: https://github.com/ThVariableYT/Pixel-Quest-Deluxe/compare/v1.11.0...HEAD
[v1.11.0]: https://github.com/ThVariableYT/Pixel-Quest-Deluxe/compare/v1.10.0...v1.11.0
[v1.10.0]: https://github.com/ThVariableYT/Pixel-Quest-Deluxe/compare/v1.9.0...v1.10.0
[v1.9.0]: https://github.com/ThVariableYT/Pixel-Quest-Deluxe/compare/v1.8.0...v1.9.0
[v1.8.0]: https://github.com/ThVariableYT/Pixel-Quest-Deluxe/compare/v1.7.0...v1.8.0
[v1.7.0]: https://github.com/ThVariableYT/Pixel-Quest-Deluxe/compare/v1.6.0...v1.7.0
[v1.6.0]: https://github.com/ThVariableYT/Pixel-Quest-Deluxe/compare/v1.5.0...v1.6.0
[v1.5.0]: https://github.com/ThVariableYT/Pixel-Quest-Deluxe/compare/v1.4.0...v1.5.0
[v1.4.0]: https://github.com/ThVariableYT/Pixel-Quest-Deluxe/compare/v1.3.0...v1.4.0
[v1.3.0]: https://github.com/ThVariableYT/Pixel-Quest-Deluxe/compare/v1.2.0...v1.3.0
[v1.2.0]: https://github.com/ThVariableYT/Pixel-Quest-Deluxe/compare/v1.1.0...v1.2.0
[v1.1.0]: https://github.com/ThVariableYT/Pixel-Quest-Deluxe/compare/v1.0.0...v1.1.0
[v1.0.0]: https://github.com/ThVariableYT/Pixel-Quest-Deluxe/releases/tag/v1.0.0
