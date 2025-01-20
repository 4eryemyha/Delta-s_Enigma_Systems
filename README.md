# Delta's Enigma

This project is a game set on a mysterious planet where players must survive in extreme conditions. They will explore the world, interact with objects, and battle dangerous creatures. The focus is on high-quality graphics, sound effects, and intuitive controls to create an immersive and engaging gameplay experience.

### Project Link (if it's large)
[Project Link](#) — a link to an archive or another resource if the project has a large size.

---

# Table of Contents

[Heading Link](#section-i-want)



1. [Character2](#сharacter)  
   &nbsp;&nbsp;&nbsp;1.1 [Walking, Running, Jumping, General Control](#walking-running-jumping-general-control)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.1.1 [Input System: KeyMapping for Key Customization](#input-system-keymapping-for-key-customization)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.1.2 [Character Interface: Displaying Health, Energy, and Other Parameters](#character-interface-displaying-health-energy-and-other-parameters)  

2. [Animations and AI](#animations-and-ai)  
   &nbsp;&nbsp;&nbsp;2.1 [Procedural Animations](#procedural-animations)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.1.1 [Flying Dragons](#flying-dragons)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.1.2 [Spiders](#spiders)  

3. [World Interaction](#world-interaction)  
   &nbsp;&nbsp;&nbsp;3.1 [Character Interaction with the World via Interfaces](#character-interaction-with-the-world-via-interfaces)  
   &nbsp;&nbsp;&nbsp;3.2 [Object System with Physics and Interaction](#object-system-with-physics-and-interaction)  
   &nbsp;&nbsp;&nbsp;3.3 [Drilling Site Location Search System](#drilling-site-location-search-system)  

4. [Base](#base)  
   &nbsp;&nbsp;&nbsp;4.1 [Core Systems](#core-systems)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.1 [Door System](#door-system)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.2 [Rooms](#rooms)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.3 [Lighting](#lighting)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.4 [Oxygen System](#oxygen-system)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.5 [Elevators](#elevators)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.6 [Crafting System](#crafting-system)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.7 [Research System](#research-system)  

   &nbsp;&nbsp;&nbsp;4.2 [Additional Elements](#additional-elements)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.2.1 [Object Capture System (Bringing Object to a Connection/Installation Spot)](#object-capture-system)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.2.2 [Base Defense: Logic for Interaction with Invaders (if planned)](#base-defense-logic-for-interaction-with-invaders)  

5. [Transport and Resource Extraction](#transport-and-resource-extraction)  
   &nbsp;&nbsp;&nbsp;5.1 [Vehicles (Transport System, Current Implementation is Broken)](#vehicles-transport-system)  
   &nbsp;&nbsp;&nbsp;5.2 [Mineral Extraction System](#mineral-extraction-system)  
   &nbsp;&nbsp;&nbsp;5.3 [Drilling Site Search System](#drilling-site-search-system)  

6. [Graphics and Materials](#graphics-and-materials)  
   &nbsp;&nbsp;&nbsp;6.1 [Materials](#materials)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.1 [Landscape (Large Landscape)](#landscape-large-landscape)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.2 [Procedural CellShader](#procedural-cellshader)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.3 [Metallic Materials for CellShader](#metallic-materials-for-cellshader)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.4 [Materials for Foliage with Wind](#materials-for-foliage-with-wind)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.5 [Materials for Rocks with Moss](#materials-for-rocks-with-moss)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.6 [Holographic Material](#holographic-material)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.7 [Particle Materials (Various)](#particle-materials-various)  

   &nbsp;&nbsp;&nbsp;6.2 [Niagara System](#niagara-system)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.2.1 [Dissolve Effect for Objects](#dissolve-effect-for-objects)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.2.2 [Cartoon Explosion](#cartoon-explosion)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.2.3 [Cartoon Smoke](#cartoon-smoke)  

   &nbsp;&nbsp;&nbsp;6.3 [Landscape and Environment](#landscape-and-environment)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.3.1 [Different Types of Foliage and Grass](#different-types-of-foliage-and-grass)  

7. [User Interface (UI)](#user-interface-ui)  
   &nbsp;&nbsp;&nbsp;7.1 [Main Menu](#main-menu)  
   &nbsp;&nbsp;&nbsp;7.2 [Settings](#settings)  
   &nbsp;&nbsp;&nbsp;7.3 [Pause](#pause)  
   &nbsp;&nbsp;&nbsp;7.4 [Inventory](#inventory)  
   &nbsp;&nbsp;&nbsp;7.5 [Research](#research)  
   &nbsp;&nbsp;&nbsp;7.6 [Character Interface](#character-interface)

---

# Project Description

Delta's Enigma is an exciting adventure game set on a mysterious planet where players must navigate extreme conditions to survive. With its vibrant, cartoon-style graphics, the game immerses players in a world filled with diverse landscapes, from lush jungles to perilous wastelands, where both hidden opportunities and deadly threats await.

Players will gather resources and craft various items through an in-depth inventory and crafting system. They can create weapons, tools, and devices by combining materials, giving them the freedom to adapt and survive in the harsh environment.

A key feature of the game is its exploration system. Players can study the planet’s unique flora and fauna, unlocking new survival options and improving their skills. This helps them develop more effective strategies to handle different challenges.

The planet is also home to many enemies, each with its own behaviors and difficulty levels. Players will need to figure out how to best approach each enemy, whether by confronting them or avoiding danger.

To make traveling across the vast planet easier, Delta's Enigma offers various forms of transport. This allows players to quickly explore the world and adapt to new challenges, giving them more strategic options along the way.

Every element of the game, from the inventory system to the dynamic enemies, is designed to create a deeply engaging and thrilling adventure where every decision counts.

---

# Implemented Systems

## Section I Want

## 1. Character

### 1.1 Walking, Running, Jumping, General Control

A detailed description of how the player moves, runs, jumps, and interacts with the world. This includes the mechanics of how walking and running speeds are controlled, how jumping works, and any general movement functionality.

![Character Movement](path_to_image)

**Implementation Details:**
- Character control system with defined key mappings
- Response to user inputs and environmental factors
- System for speed adjustment and transition between movement states

---

### 1.1.1 Input System: KeyMapping for Key Customization

Explains the input system that allows players to re-map keys for character control to suit their preferences.

![Keymapping System](path_to_image)

**Implementation Details:**
- KeyMapping system setup and structure
- Configuration files and user interface for key customization
- Challenges encountered during implementation

---

### 1.1.2 Character Interface: Displaying Health, Energy, and Other Parameters

This section describes the character interface that displays health, energy, and other important metrics.

![Character Interface](path_to_image)

**Implementation Details:**
- Design of health, energy, and other parameter indicators
- How these parameters update dynamically during gameplay
- Technical considerations in keeping the interface responsive and readable

---

## AI and Animation

### Procedural Animation for Flying Dragons

A brief description of how flying dragons move and behave procedurally.

![Dragon Animation](path_to_image)

**Implementation Details:**
- Use of procedural animation techniques
- AI decision-making processes
- Challenges faced and optimizations

### Procedural Animation for Spiders

A description of spider movement and AI logic.

![Spider Animation](path_to_image)

**Implementation Details:**
- Bone-based procedural animation
- AI pathfinding and behavior scripting
- Performance improvements and debugging

---

## Interaction Systems

### Character Interaction with Environment

A description of how the player interacts with objects and interfaces in the game.

![Interaction System](path_to_image)

**Implementation Details:**
- Implementation of interaction prompts and logic
- Technologies used for physics-based interaction
- Difficulties and solutions

### Object Physics and Interaction

A description of how objects with physics respond to player actions.

![Physics Interaction](path_to_image)

**Implementation Details:**
- Physics engine implementation details
- Interaction mechanics
- Edge cases and fixes

---

## Base Systems

### Core Base Features

A breakdown of the base systems such as oxygen management, doors, and lighting.

![Base Systems](path_to_image)

**Implementation Details:**
- Oxygen system tracking and UI integration
- Door opening logic and interactions
- Handling of light sources

### Crafting and Research

A description of the crafting and research systems.

![Crafting System](path_to_image)

**Implementation Details:**
- Crafting recipes and material management
- Research progression system
- Balancing challenges

---

## Transport and Resource Extraction

### Vehicles and Exploration

A description of the transport systems available in the game.

![Vehicles](path_to_image)

**Implementation Details:**
- Vehicle physics and handling
- Interaction with terrain
- Bug fixes and optimizations

### Mining System

A description of how resources are extracted from the environment.

![Mining System](path_to_image)

**Implementation Details:**
- Automated drill mechanics
- Resource spawn and collection
- Optimizing mining effects

---

## Graphics and Materials

### Environment Materials

A breakdown of landscape and environmental materials.

![Landscape Materials](path_to_image)

**Implementation Details:**
- Procedural terrain materials
- Foliage and wind interaction
- Optimization strategies

### Niagara FX and Visual Effects

A description of the visual effects created using Niagara.

![Niagara Effects](path_to_image)

**Implementation Details:**
- Dissolve effects for objects
- Cartoon explosion and smoke effects
- Performance optimization

---

## User Interface (UI)

### Main Menu and Settings

A breakdown of the game's user interface, including menus and in-game HUD.

![Main Menu](path_to_image)

**Implementation Details:**
- Menu layout and navigation
- Settings and key remapping
- UX considerations

### Inventory System

A description of the player's inventory and item management system.

![Inventory System](path_to_image)

**Implementation Details:**
- Inventory UI and item categorization
- Storage and retrieval logic
- Challenges with performance

---

