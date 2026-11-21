# ❄️ Arctic Flight 2

> **🎮 Play:** **[Arctic_Flight 2](https://ajil07.github.io/arctic-flight-2/)**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Canvas API](https://img.shields.io/badge/Canvas_2D-16--Bit_Procedural-38BDF8?style=for-the-badge)
![JavaScript](https://img.shields.io/badge/Vanilla_JS-Zero_Dependencies-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Web Audio](https://img.shields.io/badge/Web_Audio-Retro_Synth-58B4A8?style=for-the-badge)
![License: MIT](https://img.shields.io/badge/License-MIT-69B882?style=for-the-badge)

**Arctic Flight 2** expands the 16-bit retro atmospheric arcade game built in a **single, zero-dependency HTML5 file** (`index.html`). Guide a nimble **Shima Enaga** (Hokkaido's native "snow fairy" bird) across towering winter pine forests, through extended glacial caverns with falling icicle hazards, and into an **Old Hokkaido Pagoda Village**—complete with biome-specific rare beetle power-ups, dynamic day/night Aurora Borealis cycles, and 100% procedural HTML5 Canvas & Web Audio.

---

## 📸 Gameplay Preview

<!-- Uncomment once you upload a gameplay GIF or screenshot to assets/gameplay.gif -->
<!-- ![Arctic Flight 2 Gameplay](assets/gameplay.gif) -->

*Play directly in any desktop or mobile browser at **[https://ajil07.github.io/arctic-flight/](https://ajil07.github.io/arctic-flight/)**—no installation or downloads required.*

---

## ✨ What's New in Arctic Flight 2

### ⛩️ New Biome: Old Hokkaido Village (`VILLAGE`)
Paying homage to the Shima Enaga's native home in Hokkaido, Japan, exiting the glacial cave now leads into a richly detailed historic winter village before passing beneath a snow-laden **Torii Gate** back into the forest:
* **Multi-Tiered Pagoda Pillars:** Tall, ground-anchored Japanese pagodas (`4` to `6` stories, up to `356px` tall) featuring sweeping upturned snow-dusted eaves, wooden railings, warm amber shoji windows at night, corner wind-bells (*futaku*), and bronze/gold *sorin* spire finials.
* **Layered Hokkaido Scenery:** Backed by snow-capped **Mount Yotei** (*Ezo Fuji*), historic Hokkaido Shrine roofs with crossed *chigi* finials, the **Akarenga** red-brick hall with its verdigris dome, timber *machiya* & stone *kura* storehouses, flickering stone lanterns (*ishidoro*) at night, and scattered snow-laden pines.
* **2.5D Snow-Laden Torii Gate Transition:** Fly directly through a non-collidable foreground vermilion Torii gate to transition smoothly from the village back into the snowy forest.

### 🪲 Biome-Exclusive Rare Beetle Power-Ups (30+ Points)
Once your score climbs past **30 points**, rare metallic beetles begin appearing **10 to 25 points apart** in specific high-reward locations:
* **Golden Beetle (Hokkaido Village Only):** Perched atop the spire peaks of tall pagodas. Collecting one **doubles your horizontal speed (`2.0x`) for the next 5 turns** (5 obstacles cleared) and surrounds the bird in a golden aura.

<img width="256" height="256" alt="Code_Generated_Image (1)" src="https://github.com/user-attachments/assets/00a48cca-78e4-44d0-ae5a-f254a3d9664a" />


* **Royal Purple-Blue Beetle (Glacial Cave Only):** Suspended directly in the narrow gap between upper stalactites and lower stalagmites. Collecting one **permanently increases your run speed by `1.5x`** with an iridescent violet-blue aura.

<img width="256" height="256" alt="Code_Generated_Image" src="https://github.com/user-attachments/assets/7e2881ba-dde3-4334-815b-e5161446e94d" />


* **Game Over Specimen Log:** Tracks and displays your collected `GOLD ×N` and `ROYAL ×N` beetle counts with pixel-rendered icons on the Game Over card.

### 🧊 Extended Glacial Cave & Falling Icicles Hazard (`CAVE`)
* **Longer Cavern Runs:** Cave expeditions now span **15 to 18 obstacles** (up from 8–11), making underground navigation a true endurance test.
* **Falling Icicles Event:** Exclusive to the cave biome, ceiling tremors trigger a `FALLING ICICLES!` alert and drop **2 to 3 lethal smaller icicles** after a brief quiver telegraph—preventing players from safely camping at the top of the screen.

### 🌲 Towering Winter Forest & 2.5D Transitions
* **Taller Pine Clusters:** Chrome Dino-style clusters of **2–4 snow-covered pine trees** now reach heights of `178–358px` (up to `366px` for peak trees) across `4–6` sharp polygonal tiers, planted onto rolling terrain (`getGroundY`) in front of a **4-layer parallax pine forest** and faceted mountains.
* **2.5D Cave Archway:** Seamless obstacle-free portal transitions framed by a foreground jagged ice-and-rock archway that scrolls in front of the Shima Enaga.

### 🌌 Smooth Day / Night Cycle, Bioluminescence & Blizzards
* **76-Second Atmospheric Loop:** Gradually interpolates desaturated gradients, building windows, and lighting from crisp Arctic daylight to deep twilight.
* **Nighttime Glow:** Reveals twinkling stars, a pale moon, and emerald-to-cyan **Aurora Borealis** ribbons outdoors; warm glowing shoji windows and stone lanterns in the village; and **multi-depth glowing crystals** plus hanging **bioluminescent ceiling glowworms** inside the cave.
* **Outdoor Snowstorm Event (20+ Points):** Random blizzards roll across the forest with fast diagonal snow streaks, whiteout mist, and subtle wind-gust physics.

### ⚡ Progressive Horizontal Speed Scaling
* Smoothly ramps up base horizontal speed alongside active beetle power-ups (capped at `2.85x` total speed multiplier):

| Score Range | Base Multiplier | Pacing & Unlocks |
| :--- | :---: | :--- |
| `0 – 19` | `1.0x` | Classic Arctic Cruise |
| `20 – 29` | `1.1x – 1.18x` | Outdoor Blizzard Threshold (`20+` pts) |
| `30+` | `+0.08x` / 5 pts (`1.65x` base cap) | Rare Golden & Royal Beetles Unlocked (`31+` pts) |
| **Golden Beetle** | `× 2.0` (5 Turns) | Temporary Turbo Burst from Pagoda Peaks |
| **Royal Beetle** | `× 1.5` (Permanent) | Permanent Run Speed Boost from Cave Gaps |

### 🕹️ 16-Bit Retro Arcade UI & Procedural Web Audio
* Classic SNES/arcade cabinet bezel with an integrated top HUD (`SCORE`, live biome/hazard indicator, `BEST`, and 4 milestone stars unlocked at `5`, `15`, `30`, and `50` points).
* Synthesized Web Audio retro-synth flap chirps, 4-note square-wave power-up fanfare, and collision crunch (with repetitive per-point chimes omitted for a cleaner atmosphere).

---

## 🎮 Controls

| Input | Action |
| :--- | :--- |
| `Space` / `↑` / `W` | Flap / Start / Quick Restart |
| `Left Click` / `Tap` | Flap / Start (Desktop & Mobile) |
| `P` / `Esc` | Pause / Resume |
| `M` | Toggle Retro Synth SFX |
| `R` | Instant Reset |

---

## 🛠️ Development Process & Evolution

Arctic Flight evolved iteratively from a single-file arcade prototype into a multi-biome 16-bit experience:

1. **Stage 1 — Core Arcade Engine:**
   Built a delta-time normalized (`60 FPS` baseline) HTML5 Canvas loop, HiDPI (`devicePixelRatio`) scaling, velocity-based pitch rotation, Web Audio synthesis, and persistent `localStorage` high scores.
2. **Stage 2 — Arctic World-Building:**
   Created the nimble **Shima Enaga** protagonist, continuous Day/Night cycle with **Aurora Borealis**, indoor glacial cavern with glowing crystals and glowworms, and the 20+ point random snowstorm event.
3. **Stage 3 — 16-Bit Retro Overhaul & Layered Depth:**
   Upgraded to a sharp-bordered 16-bit arcade cabinet frame, angular multi-polygon art direction, 4-layer parallax forests, undulating terrain (`getGroundY`), Chrome Dino-style pine clusters, and a 2.5D foreground cave archway transition.
4. **Stage 4 — Arctic Flight 2 Expansion:**
   * Added the **Old Hokkaido Village** biome (`VILLAGE`) with Mount Yotei, Hokkaido Shrine & Akarenga brick landmarks, snow-covered Torii gate transitions, and towering multi-tiered Pagoda pillars.
   * Extended cave durations (`15–18` obstacles) and introduced the lethal **Falling Icicles** event (`2–3` telegraphed ceiling icicles) to eliminate ceiling camping.
   * Raised tree and pagoda obstacle heights (`178–366px`) and introduced biome-exclusive **Golden Beetles** (atop pagodas) and **Royal Purple-Blue Beetles** (inside cave icicle gaps) with Game Over loot tracking.

---

## 🧩 Technical Architecture

Everything lives inside a single self-contained `index.html` file with zero external images, fonts, or audio assets:

* **Deterministic Procedural Graphics:** Uses 1D hash functions (`hash1D`) and multi-stop linear/radial gradients to render mountain facets, pine tiers, pagoda eaves, mineral cave speckles, and iridescent beetle carapaces consistently every frame.
* **Exact Geometric Hitboxes:** Implements circle-vs-triangle (`circleIntersectsTriangle`) and circle-vs-rectangle collision checks inset slightly from sharp pine, pagoda spire, and icicle tips for fair near-misses.
* **Continuous Terrain Function:** A dual-sine elevation function (`getGroundY(worldX)`) synchronizes ground rendering, ground collision, pine cluster planting, pagoda foundations, and stalagmite anchoring.
* **Zero-Asset Web Audio API:** Synthesizes triangle-wave flap chirps, square-wave power-up arpeggios, and collision effects on the fly, unlocking automatically on the player's first gesture.

---

## 💻 How to Run Locally

Because **Arctic Flight 2** has zero dependencies or build steps, running it locally takes seconds:

```bash
# 1. Clone the repository
git clone [https://github.com/ajil07/arctic-flight.git](https://github.com/ajil07/arctic-flight-2.git)

# 2. Navigate into the project folder
cd arctic-flight-2

# 3. Open index.html directly in any modern browser
