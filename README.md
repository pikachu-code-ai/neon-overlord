# neon-overlord# 👑 NEON OVERLORD — Cyberpunk Bullet-Heaven Arena

An over-the-top, single-file cyberpunk bullet-heaven arena roguelite built with HTML5 Canvas, Vanilla JavaScript, Tailwind CSS, and procedural Web Audio synthesis. Pilot your Overlord starfighter across a glowing neon grid, vacuum up magnetic XP gems, draft broken weapon and passive synergies, unleash **God-Mode Overdrive**, and annihilate colossal **Neon Leviathan** Mega Bosses!

---

## ✨ Key Features

* **60 FPS Dual-Pass Vector Neon Engine:** Additive outer neon glows (`lighter` blend mode) paired with razor-sharp inner vector cores, pooled particle sparks, floating damage numbers, screen shake, and capped `devicePixelRatio` (`<= 2`) for smooth performance on desktop and mobile.
* **3-Card Level-Up Evolution Draft:** Collect magnetic XP gems dropped by defeated enemies to level up and choose 1 of 3 randomized weapon ranks or passive upgrades.
* **God-Mode Overdrive:** Build up your Overdrive meter through kills and trigger an **8-second rainbow-neon invulnerability rampage** featuring **2.5x fire rate**, **+35% area & speed**, **full-arena XP vacuum**, contact ramming damage, and continuous shockwave pulses.
* **Aegis Shield & Anti-Pinning Defense:** Recharging Aegis Shield absorbs incoming hits before Hull damage, while hard circle-circle separation and a **165px Defensive Repulsion Shockwave** (with `0.85s` invulnerability flicker) prevent enemies or bosses from pinning your ship.
* **Procedural Web Audio Synth:** Synthesized laser fire, chain lightning, homing missiles, rail-beams, explosions, level-up fanfares, and boss alarms with zero external audio files.
* **Adaptive Desktop & Touch Controls:** Seamless keyboard/mouse play on desktop and an automatic virtual joystick + Overdrive button on mobile and tablet devices.

---

## 🔫 6 Stackable Weapons (Up to Rank 8)

All weapons auto-target nearby threats and can be stacked together simultaneously:

| Badge | Weapon | Max Rank | Capabilities & Evolution |
| :--- | :--- | :--- | :--- |
| **⚡** | **Plasma Repeater** | `Rank 8` | Rapid auto-aiming plasma streams; evolves at Rank 8 into a **7-way piercing hyper-spread storm**. |
| **⚙** | **Orbital Sawblades** | `Rank 8` | Up to **7 spinning neon sawblades** orbit your ship, shredding enemies and deflecting incoming plasma bolts. |
| **🌩** | **Tesla Arc Lightning** | `Rank 8` | High-voltage arc jumps across up to **10 chained targets** and applies a micro-stun. |
| **💫** | **Nova Shockwave** | `Rank 8` | Periodically emits a wide expanding plasma ring that damages and knocks back surrounding swarms. |
| **🚀** | **Swarm Seeker Missiles** | `Rank 8` | Launches salvos of up to **8 homing micro-missiles** with glowing trails and explosive splash radius. |
| **🔥** | **Omega Rail-Beam** | `Rank 8` | Fires a screen-slicing piercing hyper-beam (upgrades to **bi-directional dual beams** at Rank 7+). |

---

## 🧬 6 Passive Synergies

* **⏩ Overclocked Cores (Max Lvl 6):** `+35%` Fire Rate across all active weapons per level.
* **💠 Quantum Splitter (Max Lvl 4):** `+1` Extra Projectile, Sawblade, or Chain Lightning target per level.
* **🌀 Flux Amplifier (Max Lvl 5):** `+40%` Blast Radius, Rail-Beam Width, and Sawblade Orbit Size per level.
* **💨 Ion Thrusters (Max Lvl 5):** `+30%` Movement Speed and agility per level.
* **🧲 Singularity Magnet (Max Lvl 5):** `+60%` XP Gem and Power-Up Capsule vacuum radius per level.
* **💚 Nanite Hull Matrix (Max Lvl 5):** `+5 HP/s` Hull regeneration, `+25` Max Hull, and `+15` Max Aegis Shield per level.

---

## ⚡ 4 Battlefield Power-Up Drops

* **`NUKE` (Omega Nuke):** Detonates an arena-wide shockwave that vaporizes regular enemies, clears enemy projectiles, and deals massive damage to Mega Bosses.
* **`MAG` (Hyper Magnet):** Instantly pulls every XP gem across the entire map straight to your ship.
* **`OD+` (Overdrive +50%):** Immediately charges **50%** of your God-Mode Overdrive gauge.
* **`HP+` (Nano Repair + Aegis):** Restores **45% Max Hull** and fully recharges your **Aegis Shield**.

---

## 👾 Enemy Archetypes & Mega Bosses

* **Neon Swarmers (Crimson):** Fast, relentless interceptors that attack in dense waves.
* **Cyber Hexagons (Purple):** Heavy armored polygons with high hull integrity.
* **Splitter Diamonds (Lime):** Geometric crystals that split into **2 fast Mini-Drones** when destroyed.
* **Sniper Prisms (Amber):** Ranged units that maintain distance and lock onto you with a telegraphed red laser sightline before firing.
* **Neon Leviathan Mega Bosses (Every 45s):** Colossal rotating octagons with a dedicated Boss Health Bar, spiral bullet-hell patterns, standoff orbit AI, telegraphed pass-through Cyber Charges, and **3 guaranteed power-up capsule drops** upon defeat.

---

## 🎮 Controls

### Desktop
| Action | Keys |
| :--- | :--- |
| **Move Fighter** | `W` `A` `S` `D` or `Arrow Keys` |
| **Aim Weapons** | Automatic nearest-enemy lock (or Mouse Cursor when idle) |
| **Activate God-Mode Overdrive** | `Space`, `E`, or click the HUD Overdrive Gauge |
| **Pause / Resume** | `P` or `Esc` |
| **Mute / Unmute Audio** | `M` |

### Mobile & Touch Devices
* **Left Virtual Joystick:** Drag anywhere inside the bottom-left control ring to steer smoothly in 360 degrees.
* **Right `GOD MODE` Button:** Tap when Overdrive reaches `100%` to unleash God-Mode Overdrive.

---


## 🛠️ Tech Stack

* **HTML5 Canvas (2D Context):** Dual-pass additive vector rendering, camera tracking, toroidal/arena clamping, and pooled particle systems.
* **Vanilla JavaScript (ES6+):** Real-time delta-time combat simulation, hard circle-circle anti-pinning collision resolution, roguelite draft engine, and `localStorage` high-score persistence.
* **Web Audio API:** Procedural oscillators with rate-limited polyphony for crisp retro synth sound effects.
* **Tailwind CSS (CDN) & Orbitron Typography:** High-contrast cyberpunk HUD bars, Boss Health Bar, and responsive modal overlays.
