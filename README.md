# Parasomnia - Map System (Unreal Engine 5)

---

## Overview
Developed a fully functional in game map system during an internship project for Parasomnia.

The system was rebuilt from scratch due to incomplete documentation and unstable prior implementation. The goal was to design a scalable and maintainable solution while supporting UI integration, player tracking and multi-floor navigation.

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
- Optimised performance by updating map data only when the map is opened

### Navigation & Controls
- WASD-based map movement (inspired by Resident Evil 2)
- Zoom in/out functionality
- Floor switching (Next / Previous system)

### Room Reveal System
- Implemented trigger-based discovery system
- Reveals rooms dynamically as the player explores

### Texture & Pipeline Workflow
- Captured high-resolution map images using Render Targets
- Exported textures for artist overdraw
- Resolved resolution mismatches using external tools (Photoshop)

### Prototype Feature
- Basic objective tracking system (limited due to production constraints)

---

## Challenges & Solutions

- Problem:
Map alignment broke when SceneCapture and player were offset from origin

- Solution:
Reworked UV mapping logic using relative positioning and normalization instead of absolute coordinates

---

- Problem:
Real-time updates caused unnecessary performance overhead

- Solution:
Switched to on-demand updates triggered when opening the map

---

## Technical Highlights
- Coordinate transformation (World → UI space)
- UV mapping and alignment correction
- SceneCapture2D configuration for minimap rendering
- Blueprint-based modular system design
- Performance optimisation through event-based updates

---

## Tools & Technologies
- Unreal Engine 5
- Blueprint System
- SceneCapture2D & Render Targets
- UMG (UI System)
- Photoshop (Texture adjustments)

---

## Media
- WASD-based map movement






