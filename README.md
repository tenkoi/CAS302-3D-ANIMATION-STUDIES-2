# Blender Quest — CAS302 Learning Guide Website

A retro pixel-arcade learning guide for **CAS302 – 3D Animation Studies 2**, Asia e University (AeU).
Semester 6, Year 2 • Lecturer: Mohd Faiz Alias

**File:** `CAS302_Blender_Quest_Learning_Guide.html`

## What It Is

A single-file website that guides students through 6 weeks of course topics, styled as an 8-bit arcade game. Each week is a "level" containing learning objectives, 4 curated YouTube tutorials (Blender 4.5+ focus), a real-world case study, and a practice task ("Boss Quest") that builds toward the course assessments.

## How to Use

1. Double-click the HTML file — it opens in any modern browser (Chrome, Edge, Firefox, Safari).
2. No installation or server required. The AeU logo is embedded inside the file.
3. Internet connection is needed for the YouTube videos, Google Fonts, and jQuery CDN.
4. Click a **level button** to switch weeks. Click a **cartridge card** to open that tutorial on YouTube in a new tab.

## The 6 Levels

| Level | Week Topic | CLO |
|---|---|---|
| 1 | Introduction to Blender (interface, navigation, first keyframes) | CLO1 |
| 2 | Camera Animation (framing, follow path, camera switching) | CLO1 |
| 3 | Object Animation & Physics (graph editor, rigid body) | CLO2 |
| 4 | 3D Motion Graphics & Typography (text animation, title design) | CLO4 |
| 5 | 3D Visual Effects (particles, smoke, simulations) | CLO3 |
| 6 | Rendering & Basic Compositing (Eevee/Cycles, color grading) | CLO5 |

Each level contains:
- **Objectives** — skill chips plus the mapped CLO
- **4 video cartridges** — title, channel, year and Blender version badges; opens in a new tab
- **Case File** — a real-world case study with discussion questions (e.g., Blender Open Movies, OK Go's chain reaction, Ian Hubert's *Dynamo Dream*)
- **Boss Quest** — a hands-on practice task; Weeks 3–6 quests feed directly into Assignment 1 Part B and the Final Project

## Game Features

- **Score & HUD** — each video clicked earns +100 PTS and marks the cartridge "CLEARED"
- **Progress bars** — per-level power bar fills as videos are watched; finishing all 4 flags the level "CLEAR!"
- **Mission Briefing** — course info panel (code, credits, lecturer, assessment weightings) and a CLO "skill tree"
- **Keyboard support** — left/right arrow keys switch levels when a tab is focused
- Progress is **per-session only** — it resets when the page is refreshed (no data is stored)

## Built With

- HTML + CSS + JavaScript + jQuery 3.7 (cdnjs)
- Fonts: Press Start 2P and VT323 (Google Fonts)
- No frameworks, no build step — everything in one file

## Editing the Content

Open the HTML file in any text editor:
- **Videos** — each tutorial is an `<a class="cartridge" href="...">` block; change the YouTube URL, title, channel, and badges
- **Weekly topics** — edit the text inside each `<section class="panel" data-week="...">`
- **Colors** — change the CSS variables at the top of the `<style>` block (`--coin`, `--cyan`, `--magenta`, etc.)
- **Case studies / Boss Quests** — edit the `.case-file` and `.boss` blocks in each panel

## Notes

- Tutorial links were verified at time of creation; YouTube videos can be removed or region-blocked over time, so spot-check before each semester.
- Where strong Blender 4.5 videos weren't available for a topic, well-regarded evergreen tutorials are included and honestly labelled with their year.
