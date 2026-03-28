# Map System (Unreal Engine 5)

---

## Overview
Developed an in game-map system during my internship.

The system was rebuilt to improve stability and make it easier to maintain and expand. The goal was to design a scalable and maintainable solution while supporting UI integration, player tracking and multi-floor navigation.

--- 

## Key Features 

### Map System Architecture
- Converted player world position into map space using UV normalisation logic
- Implemented orthographic map capture using SceneCapture2D
- Defined map boundaries through adjustable Ortho Width and camera positioning

### UI Integration
- Integrated map widget system with level-specific maps
- Implemented dynamic map swapping for different floors
- Displayed contextual information such as room names and floor labels

### Player Tracking
- Developed player icon system with support for different characters and game modes
- Optimised performance by updating map data only (When the map is opened)

### Navigation & Controls
- WASD-based map movement
- Zoom in/out functionality
- Floor switching (Next / Previous system)

### Room Reveal System
- Implemented trigger-based discovery system
- Reveals rooms dynamically as the player explores

### Map Texture Pipeline
- Captured high-resolution map images using Render Targets
- Exported textures for artist overdraw
- Resolved resolution mismatches using external tools (Photoshop)

### Prototype Feature
- Basic point-of-interest display (implemented as a simplified system near the end of internship)

---

## Challenges & Solutions

- **Problem:** Map alignment broke when SceneCapture and player were offset from origin
- **Solution:** Reworked UV mapping logic using relative positioning and normalization instead of absolute coordinates

---

- **Problem:** Opening the map was slow due to repeated casting of objects in nested loops.
- **Solution:** Stored object references in variables and updated the map only when it was opened to make it faster and smoother

---

## Technical Highlights
- Coordinate transformation (World → UI space)
- UV mapping and alignment correction
- SceneCapture2D configuration for minimap rendering
- Blueprint-based modular system design
- Performance optimisation through event-based updates

---

## Tools & Technologies
- Unreal Engine 5 (Blueprint)
- SceneCapture2D & Render Targets
- UMG (UI System)
- Photoshop (Texture adjustments)

---

## Media
- WASD-based Map Navigation
Singleplayer:
![Map Movement](image/MapSystem_Features_01.gif)

--- 

- Zoom In/Out
![Zoom](image/MapSystem_Features_02.gif)

---

- Floor switching (Next / Previous system)

- Singleplayer:
![Floor Switch](image/MapSystem_Features_03.gif)

- Multiplayer:
![Floor Switch](image/MapSystem_Features_04.gif)

---

- Update Map
Multiplayer: 
![Alt text](image/MapSystem_Features_05.gif)



