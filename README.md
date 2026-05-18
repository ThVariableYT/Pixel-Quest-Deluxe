# **🎮 Pixel Quest Deluxe**

**A pixel-art style RPG platformer, playable entirely in your browser.**

## **📖 Table of Contents**

- [About the Game](#-about-the-game)
- [Features](#-features)
- [How to Play](#-how-to-play)
- [Controls](#-controls)
- [Characters](#-characters)
- [Levels](#-levels)
- [Story](#-story)
- [Technical Details](#-technical-details)
- [Update History](#-update-history)
- [Contributing](#-contributing)
- [License](#-license)

## **🕹️ About the Game**

**Pixel Quest Deluxe** is a browser-based 2D platformer with a retro pixel-art aesthetic. Set in a shattered realm, you take on the role of a hero tasked with recovering fragments of the **Realm Core** scattered across 8 treacherous lands — from enchanted forests to volcanic keeps, icy caverns, and the void itself.

The game runs entirely in the browser using a single HTML file with no external dependencies beyond a font and Tailwind CSS. It features a procedurally rendered tile system, a dynamic lighting engine, a retro synth audio engine, and full mobile touch support.

## **✨ Features**

|

| **Feature** | **Description** |

| 🖼️ Pixel Art Rendering | Canvas rendered at 640×360 and scaled with image-rendering: pixelated for a crisp retro look |

| 🌍 8 Unique Levels | Each level has its own theme, atmosphere, music, and darkness level |

| 🎭 3 Playable Characters | Knight, Ninja, and Mage — each with distinct speed, jump, and dash stats |

| 🎵 Retro Synth Audio | Fully procedural Web Audio API engine — no audio files needed |

| 💡 Dynamic Lighting | Per-level darkness system with radial light effects around the player |

| 📖 Story & Dialogue | Typewriter-style dialogue system with character portraits |

| 📱 Mobile Support | Full on-screen D-pad and action buttons for touch devices |

| 🎮 Remappable Controls | All keyboard controls can be remapped in-game |

| ⛶ Fullscreen Mode | Native Fullscreen API with CSS fallback |

| 🌊 Particle Effects | Jump dust, dash trails, crystal sparkles, and ambient particles |

| 🏃 Advanced Movement | Coyote time, jump buffering, wall sliding, wall jumping, and air dashing |

| ⏸️ Pause Menu | Press Esc or P to pause/resume; mobile pause button included with Resume and Quit-to-Menu options |

| 🏆 Best Time Tracking | Speedrun timer per level; personal bests saved to localStorage and shown on level select |

| ✨ Visual Effects | Damage flash on death, shockwave on crystal collect, and enhanced crystal/vortex animations |

## **🎮 How to Play**

### **Objective**

Collect **all crystals** hidden in each level and reach the **Goal (G)** tile to clear the stage. Avoid spikes (S) and lava (\~) — touching them kills you instantly.

### **Game Loop**

1. **Start the game** from the main menu.  
2. **Select your hero** from the character selection screen.  
3. **Navigate each level** using platforming skills — jump, dash, and wall-jump your way through hazards.  
4. **Collect all crystals** scattered around the level.  
5. **Reach the glowing Goal** to complete the level and unlock the next.  
6. **Watch the story unfold** between levels via dialogue cutscenes.  
7. **Beat all 8 levels** to restore the Realm Core and see the ending.

### **Tips & Tricks**

* **Wall Slide \+ Wall Jump**: Press into a wall mid-air to slow your fall, then jump again to leap off.  
* **Dash mid-air**: You get one dash per jump — use it to clear gaps or dodge hazards.  
* **Coyote Time**: You have a short window to jump even after walking off a platform edge.  
* **Jump Buffering**: Pressing jump just before landing will register the jump automatically.  
* **Spring Pads (^)**: Land on them to launch up to great heights.  
* **Darkness Levels**: In dark levels, stay close to lit areas — the further you go, the darker it gets.

## **⌨️ Controls**

### **Default Keyboard Controls**

| **Action** | **Keys** |

| Move Left | Arrow Left / A |

| Move Right | Arrow Right / D |

| Jump | Space / Arrow Up / W |

| Dash | Shift / Z / X |

| Advance Dialogue | Space / Jump Key |

### **Mobile / Touch Controls**

On touch-enabled devices, an on-screen control pad is automatically shown:

* **Left / Right arrows** — D-pad for movement  
* **⚡ (Dash button)** — Activates the dash ability  
* **▲ (Jump button)** — Makes the character jump

### **Remapping Controls**

You can remap any control from the **Controls** screen in the main menu:

1. Go to **Controls** from the main menu.  
2. Click **REMAP CONTROLS**.  
3. Click the button for the action you want to remap (e.g., LEFT, RIGHT, JUMP, DASH).  
4. Press any key on your keyboard to assign it.

## **🧙 Characters**

Choose your hero before starting the game. Each character has unique movement stats that change the feel of gameplay.

### **⚔️ Knight**

*"Balanced Stats"*

| **Stat** | **Value** |

| Speed | 220 |

| Jump Force | \-400 |

| Dash Speed | 500 |

| Dash Duration | 0.25s |

| Dash Cooldown | 0.8s |

The default hero. Well-rounded and recommended for beginners.

### **🥷 Ninja**

*"Fast & High Jump"*

| **Stat** | **Value** |

| Speed | 250 |

| Jump Force | \-450 |

| Dash Speed | 400 |

| Dash Duration | 0.2s |

| Dash Cooldown | 0.6s |

The fastest character with the highest jump. Shorter dash but quicker cooldown. Great for expert players who want agility.

### **🧙 Mage**

*"Long Dash, Slower"*

| **Stat** | **Value** |

| Speed | 185 |

| Jump Force | \-365 |

| Dash Speed | 565 |

| Dash Duration | 0.35s |

| Dash Cooldown | 0.5s |

Slower movement and lower jump, but possesses the most powerful and longest dash in the game with the fastest cooldown.

## **🗺️ Levels**

The game features **8 handcrafted levels**, each with a distinct environment, ambient music theme, and hazard configuration.

| **\#** | **Level Name** | **Theme** | **Darkness** | **Hazards** | **Music** |

| 1 | The Green Valley | 🌿 Forest | None | Spikes | Forest Drone |

| 2 | Echoing Caves | 🪨 Cave | High (85%) | Spikes | Cave Drone |

| 3 | The Infernal Keep | 🌋 Volcano | Low (30%) | Spikes, Lava, Springs | Volcano Synth |

| 4 | Crystal Caverns | 🧊 Ice | Medium (60%) | Spikes, Lava, Springs | Ice Chimes |

| 5 | The Void | 🌌 Void | Very High (90%) | Spikes, Lava, Springs | Void Bass |

| 6 | Sky Ruins | ☁️ Sky | None | Spikes, Springs | Sky Bells |

| 7 | Swamp Depths | 🌿 Swamp | High (70%) | Spikes, Lava, Springs | Swamp Tones |

| 8 | The True Core | 🔥 Core | Medium (50%) | Spikes, Lava, Springs | Core Synth |

### **Tile Legend**

| **Symbol** | **Meaning** |

| P | Player Start Position |

| \# | Solid Platform Tile |

| C | Crystal (Collectible) |

| G | Goal (Level Exit) |

| ^ | Spring Pad (Launches player upward) |

| S | Spike (Instant Kill) |

| \~ | Lava (Instant Kill) |

| . | Empty Space |

## **📜 Story**

The realm has been shattered. The **Dark Wizard** has destroyed the **Realm Core**, scattering its fragments across eight dangerous lands. The sage **Eldor** reaches out to the last hero standing:

*"Hero\! The Dark Wizard has shattered the Realm Core. Its fragments are scattered across treacherous lands."*

Your mission takes you through dense forests, ancient caves, volcanic fortresses, crystalline ice caverns, the emptiness of the Void, ruined sky temples, toxic swamp depths, and finally the blazing True Core — recovering fragments one level at a time. Each cleared area is narrated through a short dialogue between Eldor and your chosen hero.

## **🛠️ Technical Details**

* **Engine**: Vanilla JavaScript with HTML5 Canvas API  
* **Resolution**: Internal render at 640×360, scaled via CSS for pixel-perfect display  
* **Audio**: Web Audio API — fully procedural synth, no audio files  
* **Rendering**: Offscreen canvas for map pre-rendering \+ a dedicated light canvas for the darkness overlay  
* **Physics**: Custom physics loop with gravity (1000 units/s²), acceleration, coyote time (0.15s), jump buffering (0.2s), wall sliding, and wall jumping  
* **Particles**: Dynamic particle system for jump dust, dash trails, crystal collection sparks, and ambient environment particles  
* **Fonts**: [Press Start 2P](https://fonts.google.com/specimen/Press+Start+2P) via Google Fonts  
* **Styling**: Tailwind CSS (CDN) \+ custom CSS  
* **No build step required** — open index.html directly in any modern browser

### **Running Locally**

git clone \[https://github.com/ThVariableYT/Pixel-Quest-Deluxe.git\](https://github.com/ThVariableYT/Pixel-Quest-Deluxe.git)  
cd Pixel-Quest-Deluxe  
\# Open index.html in your browser  
open index.html

## **📋 Update History**

### **v1.0.0 — Initial Release *(May 15, 2026\)***

* **Commit:** Initial  
* Project scaffolding and repository setup.

### **v1.1.0 — Core Game Engine *(May 16, 2026\)***

* **Commit:** a8749b3  
* Added the full **Epic Pixel Quest Deluxe** HTML game file.  
* Implemented 8-level campaign with a tile-based map system.  
* Built custom physics engine with gravity, acceleration, and collision detection.  
* Added procedural pixel-art tile texture rendering per theme.  
* Integrated story and dialogue system with typewriter effect.  
* Created retro synth audio engine using Web Audio API.  
* Implemented dynamic darkness/lighting overlay system and particle system.  
* Added HUD display and menu screens.

### **v1.2.0 — Character Selection & Player Tuning *(May 16, 2026\)***

* **Commit:** ce333b9  
* Added **character selection screen** with 3 playable heroes: Knight, Ninja, and Mage.  
* Configured unique speed, jump force, dash stats, and color palettes for each character.  
* Implemented dynamic player stat updates on selection.

### **v1.3.0 — Gameplay Physics & UI Polish *(May 16, 2026\)***

* **Commit:** bac3007  
* Tuned gameplay physics for air control and player acceleration.  
* Polished overall UI elements and mobile touch responsiveness.

### **v1.4.0 — Fullscreen Support *(May 16, 2026\)***

* **Commit:** c7054d3  
* Added **fullscreen toggle button** leveraging the native Fullscreen API.  
* Implemented CSS position: fixed fallback for unsupported browsers.  
* Ensured fullscreen button is visible at top-right corner during gameplay and menus.

### **v1.5.0 — Control Remapping & Touch D-Pad *(May 16, 2026\)***

* **Commit:** 0be5d66  
* Added **in-game control remapping** allowing players to remap Left, Right, Jump, and Dash.  
* Improved touch D-pad with multi-touch slide support for smoother mobile movement.  
* Designed and integrated Remap UI into the Controls screen in the main menu.

### **v1.6.0 — General index.html Update *(May 16, 2026\)***

* **Commit:** b69282e  
* Performed general code updates to index.html.  
* Improved overall stability and optimized internal logic.

### **v1.7.0 — Refinements and Bug Fixes *(May 16, 2026\)***

* **Commit:** 69c5944  
* Applied further gameplay and UI refinements.  
* Fixed miscellaneous bugs affecting rendering and state transitions.

### **v1.8.0 — Final Polish Update *(May 16, 2026\)***

* **Commit:** 4a49d37  
* Final polish update to smooth out animations and UI quirks.  
* Ensured consistent visual fidelity across varying display sizes.

### **v1.9.0 — Speedrun Timer & Visual Polish *(May 16, 2026\)***

* **Commit:** c040db0  
* Added **speedrun timer** tracking level completion time (displayed in HUD).  
* Implemented level transition effects between stages.  
* Enhanced canvas particle effects including crystal sparkles and ambient particles.

### **v1.10.0 — Pause System & Best Time Tracking *(May 16, 2026\)***

* **Commit:** 1a22dd2  
* Added **pause menu** accessed via Esc or P, and a mobile pause button.  
* Included Resume and Quit to Menu options in the pause screen.  
* Implemented speedrun best times saved locally and displayed on level select.  
* Added **damage flash** and **shockwave** visual effects for death and crystal collection.  
* Improved crystal inner pulse animation and vortex/goal rendering.

### **v1.11.0 — The Deluxe Endgame Expansion *(May 16, 2026\)***

* **Commit:** d7a10e9  
* **Boss Battle Added:** Epic final scripted encounter against The Dark Wizard (Level 10\) featuring predictive projectiles and a custom boss HP HUD.  
* **Level Expansion:** Expanded the standard campaign, adding Level 9 (The Ascension) and Level 10 (The Wizard's Throne).  
* **New Hero (Scout):** Added a 4th playable character (Windwalker) possessing a unique Glide ability.  
* **The Void Archives:** Introduced a secret developer menu containing 5 extreme-difficulty bonus levels (Glitch Dimension, Neon Speedway, Infernal Escape, Spike Maze, Crystal Tower).  
* **Cinematic Post-Game Polish:** Implemented rich visual feedback upon beating the game, including God Rays, a Majestic Gold Pulse background, and a Platinum Crown logo transformation.

## **🤝 Contributing**

Contributions, issues, and feature requests are welcome\!

1. Fork the repository.  
2. Create your feature branch: git checkout \-b feature/your-feature  
3. Commit your changes: git commit \-m 'Add your feature'  
4. Push to the branch: git push origin feature/your-feature  
5. Open a Pull Request.

## **📄 License**

This project is open source and available under the [MIT License](http://docs.google.com/LICENSE).

Made with ❤️ by [ThVariableYT](https://github.com/ThVariableYT)