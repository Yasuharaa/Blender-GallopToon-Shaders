# Blender Umamusume Shader

A toon shader for Blender that reproduces the in-game look of **Umamusume: Pretty Derby** characters, built for datamined game assets.

This project is a derivative of [festivities/Blender-miHoYo-Shaders](https://github.com/festivities/Blender-miHoYo-Shaders). The original node architecture was used as a starting point, but the shading logic, material parameters, and texture handling have been reworked to follow Umamusume's own rendering model rather than Genshin Impact's.

---


---

## Background

The festivities shader set is one of the most widely used references for anime-style game rendering in Blender. It was designed specifically around Genshin Impact's texture layout and material properties.

Umamusume uses a different shading pipeline. Its toon shadow, MatCap, and texture channel conventions do not map one-to-one onto the Genshin setup, so applying the original shader to Umamusume assets produces visibly incorrect results. Instead of starting from scratch, this project keeps the parts of the original node structure that are game-agnostic and replaces the game-specific logic with an implementation based on Umamusume's own material data.

## What I used from Original Festivities shader

-Light Vector to control lighting direction
-GenshinImpact Outlines
-Lighting Panel and Custom Lighting for Ambient, Lit Shadow Color, Unlit Shadow Color, Rim Color, and Fresnel Lighting.

## Features

- Toon diffuse shading with Umamusume-style shadow stepping
- MatCap reflections
- Depth-Based Rim lighting (Festivity)
- Face shading (Chips)
- Outlines (Festivity & BonnyAnimations)
- Material inputs aligned with Umamusume material data

## Requirements

- Blender Goo Engine 4.0+ or newer
- Character models, textures, and materials data extracted from the game (not provided in this repository)

## Installation

<!-- Uma-Studio -->

## Usage

<!-- Uma-Studio -->

## Known Limitations

- The shader is an approximation of the in-game look and is not guaranteed to be 100% accurate in every lighting condition.
- It is designed for datamined game assets.

## Credits

**Original project**

- [festivities](https://github.com/festivities) — author of [Blender-miHoYo-Shaders](https://github.com/festivities/Blender-miHoYo-Shaders), which this project is based on. Please refer to the upstream repository for its full list of acknowledgements.
- [BonnyAnimations - HoYOTOON](https://github.com/Hoyotoon/HoyoToon-Blender) - Lighting Panel and Outlines
- [Chips](https://github.com/Elysia-simp) - author of [Honse-Shader - Face shading](https://github.com/Elysia-simp/Honse-Shader)

**This project**

- Nirune Studio — Umamusume shader port, logic modifications, and maintenance

**Game**

- Cygames, Inc. — developer of Umamusume: Pretty Derby

If you use this shader in a render or animation, a credit and link back to this repository is needed.

## License

This project is a derivative work of [festivities/Blender-miHoYo-Shaders](https://github.com/festivities/Blender-miHoYo-Shaders) 
If you redistribute this shader or a modified version of it, you must do so under GPL-3.0 and include a link to both this repository and the original upstream repository.

## Disclaimer

This is a fan-made project and is not affiliated with, endorsed by, or sponsored by Cygames, Inc. or HoYoverse. Umamusume: Pretty Derby and all related characters, names, and assets are the property of Cygames, Inc.
No game assets are distributed in this repository. Users are responsible for complying with the terms of service of the game and with the applicable laws in their jurisdiction.
