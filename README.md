# Delta's Enigma Systems

This project is a game set on a mysterious planet where players must survive in extreme conditions. They will explore the world, interact with objects, and battle dangerous creatures. The focus is on high-quality graphics, sound effects, and intuitive controls to create an immersive and engaging gameplay experience.

[Delta's Enigma Systems RU](https://github.com/4eryemyha/Delta-s_Enigma_Systems/blob/main/READMEru.md) — a link to file in Russian.

### Project Link
[Delta's Enigma](https://github.com/4eryemyha/Delta-s_Enigma) — a project file link **(not finished)**.

---

# Table of Contents

1. [Character](#1-character)  
   &nbsp;&nbsp;&nbsp;1.1 [Movement](#11-movement)  
   &nbsp;&nbsp;&nbsp;1.2 [Input System: KeyMapping for Key Customization](#12-input-system-keymapping-for-key-customization)  
   &nbsp;&nbsp;&nbsp;1.3 [Character Interface](#13-character-interface)   

2. [Animations and AI](#2-animations-and-ai)  
   &nbsp;&nbsp;&nbsp;2.1 [Flying Dragons](#21-flying-dragons)  
   &nbsp;&nbsp;&nbsp;2.2 [Spiders](#22-spiders)

3. [World Interaction](#3-world-interaction)  
   &nbsp;&nbsp;&nbsp;3.1 [Character Interaction with the World via Interfaces](#31-character-interaction-with-the-world-via-interfaces)  
   &nbsp;&nbsp;&nbsp;3.2 [Object System with Physics and Interaction](#32-object-system-with-physics-and-interaction)  

4. [Base](#4-base)  
   &nbsp;&nbsp;&nbsp;4.1 [Core Systems](#41-core-systems)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.1 [Door System](#411-door-system)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.2 [Rooms](#412-rooms)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.3 [Lighting](#413-lighting)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.4 [Oxygen System](#414-oxygen-system)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.5 [Elevators](#415-elevators)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.6 [Crafting System](#416-crafting-system)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.7 [Research System](#417-research-system)  

5. [Transport and Resource Extraction](#5-transport-and-resource-extraction)  
   &nbsp;&nbsp;&nbsp;5.1 [Vehicles](#51-vehicles)  
   &nbsp;&nbsp;&nbsp;5.2 [Drilling Site Search System](#52-drilling-site-search-system)  
   &nbsp;&nbsp;&nbsp;5.3 [Mineral Extraction System](#53-mineral-extraction-system)

6. [Graphics and Materials](#6-graphics-and-materials)  
   &nbsp;&nbsp;&nbsp;6.1 [Materials](#61-materials)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.1 [Landscape (Large Landscape)](#611-landscape-large-landscape)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.2 [Procedural CellShader](#612-procedural-cellshader)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.3 [Metallic Material for CellShader](#613-metallic-material-for-cellshader)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.4 [Material for Foliage with Wind](#614-material-for-foliage-with-wind)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.5 [Material for Rocks with Moss](#615-material-for-rocks-with-moss)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.6 [Holographic Material](#616-holographic-material)  
   &nbsp;&nbsp;&nbsp;6.2 [Niagara System](#62-niagara-system)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.2.1 [Dissolve Effect](#621-dissolve-effect)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.2.2 [Cartoon Explosion](#622-cartoon-explosion)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.2.3 [Cartoon Smoke](#623-cartoon-smoke)  
   &nbsp;&nbsp;&nbsp;6.3 [Landscape and Environment](#63-landscape-and-environment)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.3.1 [Different Types of Foliage and Grass](#631-different-types-of-foliage-and-grass)

7. [User Interface (UI)](#7-user-interface-ui)  
   &nbsp;&nbsp;&nbsp;7.1 [Main Menu](#71-main-menu)  
   &nbsp;&nbsp;&nbsp;7.2 [Settings](#72-settings)  
   &nbsp;&nbsp;&nbsp;7.3 [Pause](#73-pause)  
   &nbsp;&nbsp;&nbsp;7.4 [Inventory](#74-inventory)  
   &nbsp;&nbsp;&nbsp;7.5 [Research](#75-research)  

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

## 1. Character

### 1.1 &nbsp;Movement

Description of player movement, running, jumping, and camera control mechanics, including movement speed control, jumping behavior, and camera interaction.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/CharacterMovement.gif" width="830" height="470">

**Implementation Details:**  
- Smooth interaction with physics and objects during movement.

---

### 1.2 &nbsp;Input System: KeyMapping for Key Customization

Input system allowing players to re-map keys for character control to suit their preferences.

<img src="https://github.com/4eryemyha/Media/blob/main/PHOTOs/KeyMapping.png" width="830" height="470">

**Implementation Details:**
- KeyMapping system setup and structure (Optimized code).

---

### 1.3 &nbsp;Character Interface

Character interface displaying health, energy, and other important metrics.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Character%20Interface.gif" width="830" height="470">

**Implementation Details:**
- Custom design of health, energy, and other parameter indicators.
- Interface reacts to external factors dynamically.

---

## 2. Animations and AI

### 2.1 &nbsp;Flying Dragons

Flying dragons animation, their movements in the air, and AI behavior.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Dragons.gif" width="830" height="470">

**Implementation Details:**
- Procedural animation for dynamic dragon movement in the air.
- Procedurally adjustable size and shape of the dragon.

---

### 2.2 &nbsp;Spiders

Animation for spiders, their movement across different surfaces, and AI behavior.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Spiders.gif" width="830" height="470">

**Implementation Details:**
- Procedural animation with IK and skeleton for multi-legged creatures.
- Adaptation to any spider size for climbing on vertical surfaces.
- Expanded area for AI movement interaction.

---

## 3. World Interaction

### 3.1 &nbsp;Character Interaction with the World via Interfaces

Ways the character interacts with the game world through various interfaces, including interacting with objects, using items, and activating mechanisms.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Character%20Interaction%20with%20the%20World.gif" width="830" height="470">

**Implementation Details:**
- Quick creation of any object and addition of interaction system.

---

### 3.2 &nbsp;&nbsp;Object System with Physics and Interaction

Object system with physics and interaction capabilities. How objects respond to physical forces and interact with characters and other objects.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Object%20System%20with%20Physics%20and%20Interaction.gif" width="830" height="470">

**Implementation Details:**
- Quick addition of any object with full functionality and physics.
- Highly optimized code for object interaction with characters and the environment.

---

## 4. Base

### 4.1 &nbsp;Core Systems
---
### 4.1.1 &nbsp;&nbsp;Door System

Door system, including opening, closing, and interaction with the player and the environment.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Door%20System.gif" width="830" height="470">

**Implementation Details:**
- Procedural sound for door opening and closing mechanisms.

---

### 4.1.2 &nbsp;&nbsp;Rooms

Room system based on the base and its organization.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Rooms.gif" width="830" height="470">

**Implementation Details:**
- Base building system, allowing the assembly of a base from rooms.

---

### 4.1.3 &nbsp;&nbsp;Lighting

Lighting system for controlling brightness and switching lights on and off in different areas.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Light.gif" width="830" height="470">

**Implementation Details:**
- Modular lighting system with quick implementation.

---

### 4.1.4 &nbsp;&nbsp;Oxygen System

Oxygen system for sustaining life on the base, regulating oxygen levels and distribution processes.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Oxygen%20System.gif" width="830" height="470">

**Implementation Details:**
- Oxygen storage on the base with visual representation.
- Mineral processing system to generate oxygen on the base.

---

### 4.1.5 &nbsp;&nbsp;Elevators

Elevator system for managing movement between different levels of the base.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Elevators.gif" width="830" height="470">

**Implementation Details:**
- Use of the door system for elevator operation.

---

### 4.1.6 &nbsp;&nbsp;Crafting System

Crafting system for creating new objects using resources at a special station.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Crafting%20System.gif" width="830" height="470">

**Implementation Details:**
- Visual representation with materials and particles.
- Complex crafting tree system linked to the research system.

---

### 4.1.7 &nbsp;&nbsp;Research System

Research system that allows players to unlock new technologies and craft items.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/ResearchBase.gif" width="830" height="470">

**Implementation Details:**
- None.

---

## 5. Transport and Resource Extraction

### 5.1 &nbsp;Vehicles

Vehicle system used for character movement across the game world.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Vehicles.gif" width="830" height="470">

**Implementation Details:**
- Levitation-based vehicle system.
- Multiple types of vehicles.

---

### 5.2 &nbsp;&nbsp;Drilling Site Search System

Drilling site search system.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Drilling%20Site%20Search%20System.gif" width="830" height="470">

**Implementation Details:**
- Search using a specific item.

---

### 5.3 &nbsp;&nbsp;Mineral Extraction System

Mineral extraction system, where a drill arrives and extracts minerals for collection, processing, and further use.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Mineral%20Extraction%20System.gif" width="830" height="470">

**Implementation Details:**
- Procedural animation for the entire drill.

---

## 6. Graphics and Materials

### 6.1 &nbsp;Materials
---
### 6.1.1 &nbsp;&nbsp;Landscape (Large Landscape)

Material system for creating large landscapes, including layers, textures, and their adaptation across vast areas.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/LandscapeMaterial.gif" width="830" height="470">

**Implementation Details:**
- Use of virtual texture system for landscape creation.
- Grass system for large areas.
- Fine-tuning for performance optimization.

---

### 6.1.2 &nbsp;&nbsp;Procedural CellShader

Procedural shader for creating a cartoon-like visual style through texture and lighting processing.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/CellShader.gif" width="830" height="470">

**Implementation Details:**
- Fine-tuning of all layers.
- All issues related to external effects resolved.

---

### 6.1.3 &nbsp;&nbsp;Metallic Material for CellShader

Metallic material used in shaders to create shine and reflection effects. Only one material is used.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Metallic%20Materials%20for%20CellShader.gif" width="830" height="470">

**Implementation Details:**
- Development of metallic materials for cellshader.

---

### 6.1.4 &nbsp;&nbsp;Material for Foliage with Wind

Vegetation materials reacting to wind, creating foliage and grass movement effects.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Materials%20for%20Foliage%20with%20Wind.gif" width="830" height="470">

**Implementation Details:**
- Implementation of vegetation materials with adjustable wind strength and direction.

---

### 6.1.5 &nbsp;&nbsp;Material for Rocks with Moss

Materials for procedural moss on rocks, including texture details and visual effects.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Materials%20for%20Rocks%20with%20Moss.gif" width="830" height="470">

**Implementation Details:**
- Fine-tuning of various material parameters.

---

### 6.1.6 &nbsp;&nbsp;Holographic Material

Holographic material for unique objects and effects in the game.  

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Holographic%20Material.gif" width="830" height="470">

**Implementation Details:**
- Fine-tuning of holographic material.

---

### 6.2 &nbsp;Niagara System
---
### 6.2.1 &nbsp;&nbsp;Dissolve Effect

Dissolve effect for objects that can disappear or dissolve based on interaction.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Dissolve%20Effect.gif" width="830" height="470">

**Implementation Details:**
- Fine-tuning of dissolution effects.

---

### 6.2.2 &nbsp;&nbsp;Cartoon Explosion

Creation of cartoon-style explosions using the Niagara system.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Cartoon%20Explosion.gif" width="830" height="470">

**Implementation Details:**
- Custom VFX effect with fine-tuning for cartoon-style explosions.

---

### 6.2.3 &nbsp;&nbsp;Cartoon Smoke

Creation of cartoon-style smoke using the Niagara system, used in various situations like explosions or fire.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Cartoon%20Smoke.gif" width="830" height="470">

**Implementation Details:**
- Simplicity and optimization for cartoon-style smoke.

---

### 6.3 &nbsp;Landscape and Environment
---
### 6.3.1 &nbsp;&nbsp;Different Types of Foliage and Grass

Various types of vegetation, such as trees, shrubs, and grass, and the materials used for their creation and animation.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Different%20Types%20of%20Foliage%20and%20Grass.gif" width="830" height="470">

**Implementation Details:**
- Interaction capabilities with certain types of vegetation.

---

## 7. User Interface (UI)

### 7.1 &nbsp;Main Menu

The main menu screen of the game, serving as the central hub for navigating various game features.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Main%20Menu.gif" width="830" height="470">

**Implementation Details:**
- Custom animations created specifically for this project.
- Custom design created specifically for this project.

---

### 7.2 &nbsp;Settings

Settings menu allowing players to adjust game parameters such as graphics, sound, and controls.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Settings.gif" width="830" height="470">

**Implementation Details:**
- Modular system for creating settings.
- Custom visuals and animations for the settings menu.
- Full saving of player settings.

---

### 7.3 &nbsp;Pause

Pause screen allowing the player to stop the game and access various options.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Pause.gif" width="830" height="470">

**Implementation Details:**
- None.

---

### 7.4 &nbsp;Inventory

Inventory system allowing players to collect and manage items within the game.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Inventory.gif" width="830" height="470">

**Implementation Details:**
- Custom visuals and animations for the inventory system.
- All test cases and errors resolved and accounted for.

---

### 7.5 &nbsp;Research

Research system allowing players to develop new technologies and capabilities within the game.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/ResearchUI.gif" width="830" height="470">

**Implementation Details:**
- Custom visuals and animations for the research system.
- Modular system for creating research trees.
