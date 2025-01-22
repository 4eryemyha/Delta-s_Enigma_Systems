# Delta's Enigma

This project is a game set on a mysterious planet where players must survive in extreme conditions. They will explore the world, interact with objects, and battle dangerous creatures. The focus is on high-quality graphics, sound effects, and intuitive controls to create an immersive and engaging gameplay experience.

### Project Link
[Delta's Enigma](#) — a link to an archive or another resource if the project has a large size.

---

# Table of Contents

1. [Character](#1-character)  
   &nbsp;&nbsp;&nbsp;1.1 [Walking, Running, Jumping, General Control](#11-walking-running-jumping-general-control)  
   &nbsp;&nbsp;&nbsp;1.2 [Input System: KeyMapping for Key Customization](#12-input-system-keymapping-for-key-customization)  
   &nbsp;&nbsp;&nbsp;1.3 [Character Interface: Displaying Health, Energy, and Other Parameters](#13-character-interface-displaying-health-energy-and-other-parameters)  

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
   &nbsp;&nbsp;&nbsp;5.1 [Vehicles (Transport System, Current Implementation is Broken)](#51-vehicles-transport-system)  
   &nbsp;&nbsp;&nbsp;5.2 [Mineral Extraction System](#52-mineral-extraction-system)  
   &nbsp;&nbsp;&nbsp;5.3 [Drilling Site Search System](#53-drilling-site-search-system) 

6. [Graphics and Materials](#6-graphics-and-materials)  
   &nbsp;&nbsp;&nbsp;6.1 [Materials](#61-materials)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.1 [Landscape (Large Landscape)](#611-landscape-large-landscape)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.2 [Procedural CellShader](#612-procedural-cellshader)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.3 [Metallic Materials for CellShader](#613-metallic-materials-for-cellshader)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.4 [Materials for Foliage with Wind](#614-materials-for-foliage-with-wind)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.5 [Materials for Rocks with Moss](#615-materials-for-rocks-with-moss)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.6 [Holographic Material](#616-holographic-material)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1.7 [Particle Materials (Various)](#617-particle-materials-various)  
   &nbsp;&nbsp;&nbsp;6.2 [Niagara System](#62-niagara-system)  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.2.1 [Dissolve Effect for Objects](#621-dissolve-effect-for-objects)  
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
   &nbsp;&nbsp;&nbsp;7.6 [Character Interface](#76-character-interface)

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

### 1.1 &nbsp;Walking, Running, Jumping, General Control

A detailed description of how the player moves, runs, jumps, and interacts with the world. This includes the mechanics of how walking and running speeds are controlled, how jumping works, and any general movement functionality.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/CharacterMovement.gif" width="830" height="470">

**Implementation Details:**
- Character control system with defined key mappings
- Response to user inputs and environmental factors
- System for speed adjustment and transition between movement states

---

### 1.2 &nbsp;Input System: KeyMapping for Key Customization

Explains the input system that allows players to re-map keys for character control to suit their preferences.

<img src="https://github.com/4eryemyha/Media/blob/main/PHOTOs/KeyMapping.png" width="830" height="470">

**Implementation Details:**
- KeyMapping system setup and structure
- Configuration files and user interface for key customization
- Challenges encountered during implementation

---

### 1.3 &nbsp;Character Interface: Displaying Health, Energy, and Other Parameters

This section describes the character interface that displays health, energy, and other important metrics.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Character%20Interface.gif" width="830" height="470">

**Implementation Details:**
- Design of health, energy, and other parameter indicators
- How these parameters update dynamically during gameplay
- Technical considerations in keeping the interface responsive and readable

---

## 2. Animations and AI

### 2.1 &nbsp;Flying Dragons

Этот раздел фокусируется на анимации летающих драконов, их движениях в воздухе и взаимодействиях с другими объектами.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Dragons.gif" width="830" height="470">

**Implementation Details:**
- Динамическое управление движением драконов в воздухе
- Применение физики для реалистичных полетов
- Взаимодействие с окружающим миром

---

### 2.2 &nbsp;Spiders

Здесь рассматривается анимация для пауков, их движения по различным поверхностям и реакции на поведение игрока.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Spiders.gif" width="830" height="470">

**Implementation Details:**
- Специфика анимаций для многоногих существ
- Реализация лазания по вертикальным поверхностям
- Интерактивность с игроком и миром

---

## 3. World Interaction

### 3.1 &nbsp;Character Interaction with the World via Interfaces

В этом разделе рассматриваются способы, которыми персонаж взаимодействует с миром игры через различные интерфейсы, включая взаимодействие с объектами, использование предметов и активацию механизмов.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Character%20Interaction%20with%20the%20World.gif" width="830" height="470">

**Implementation Details:**
- Способы взаимодействия персонажа с миром
- Реализация интерфейсов для различных типов объектов
- Технические аспекты обработки пользовательского ввода и обратной связи

---

### 3.2 &nbsp;&nbsp;Object System with Physics and Interaction

Здесь описывается система объектов в игре с физикой и возможностью взаимодействия с ними. Как объекты реагируют на физические силы и как они взаимодействуют с персонажами и другими объектами.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Object%20System%20with%20Physics%20and%20Interaction.gif" width="830" height="470">

**Implementation Details:**
- Реализация системы физики для объектов
- Детали взаимодействия объектов с персонажами и окружающей средой
- Проблемы при учете взаимодействия с разными типами объектов

---

## 4. Base

### 4.1 &nbsp;Core Systems
---
### 4.1.1 &nbsp;&nbsp;Door System

Здесь рассматривается система дверей, включая их открытие, закрытие и взаимодействие с игроком и окружающей средой.

<img src="https://github.com/4eryemyha/Media/blob/main/GIFs/Door%20System.gif" width="830" height="470">

**Implementation Details:**
- Реализация механизмов открытия и закрытия дверей
- Интерактивность дверей с персонажем
- Взаимодействие с другими системами

---

### 4.1.2 &nbsp;&nbsp;Rooms

Этот раздел описывает систему комнат на базе, их организацию и взаимодействие с другими объектами и системами.

![Rooms](path_to_image)

**Implementation Details:**
- Конфигурация комнат и объектов внутри них
- Принципы динамического изменения комнат
- Система обеспечения функциональности каждой комнаты

---

### 4.1.3 &nbsp;&nbsp;Lighting

Здесь описывается система освещения на базе, которая управляет уровнем яркости, состоянием и режимами освещения в разных областях базы.

![Lighting](path_to_image)

**Implementation Details:**
- Управление освещением в различных частях базы
- Реализация динамических эффектов освещения
- Оптимизация для производительности

---

### 4.1.4 &nbsp;&nbsp;Oxygen System

Этот раздел фокусируется на системе кислорода, необходимой для поддержания жизни на базе. Объясняются процессы, регулирующие уровень кислорода и его распределение.

![Oxygen System](path_to_image)

**Implementation Details:**
- Управление уровнем кислорода
- Система мониторинга и контроля
- Взаимодействие с другими жизненно важными системами

---

### 4.1.5 &nbsp;&nbsp;Elevators

Здесь описывается система лифтов, которая управляет перемещением между различными уровнями базы.

![Elevators](path_to_image)

**Implementation Details:**
- Принципы работы лифтов и управления ими
- Взаимодействие с другими системами
- Особенности анимации и механизма лифтов

---

### 4.1.6 &nbsp;&nbsp;Crafting System

Этот раздел посвящен системе крафта, где игроки могут создавать новые объекты, улучшать предметы и собирать ресурсы.

![Crafting System](path_to_image)

**Implementation Details:**
- Механизмы создания и улучшения объектов
- Система ресурсов и их использование
- Балансировка и настройки интерфейса крафта

---

### 4.1.7 &nbsp;&nbsp;Research System

Здесь рассматривается система исследований, которая позволяет игрокам открывать новые технологии и улучшать базу.

![Research System](path_to_image)

**Implementation Details:**
- Алгоритмы и интерфейс для исследований
- Как исследования влияют на развитие базы
- Интеграция с другими системами

---

## 5. Transport and Resource Extraction

### 5.1 &nbsp;Vehicles (Transport System, Current Implementation is Broken)

Этот раздел описывает систему транспортных средств, которая используется для перемещения ресурсов и персонажей по игровому миру. Также рассматриваются проблемы, возникшие в текущей реализации этой системы.

![Vehicles](path_to_image)

**Implementation Details:**
- Механизмы управления транспортными средствами
- Текущие проблемы в реализации транспортной системы
- Планы по улучшению и исправлению багов

---

### 5.2 &nbsp;&nbsp;Mineral Extraction System

Здесь описывается система добычи минералов, включая способы сбора ресурсов, их переработку и использование в дальнейшем.

![Mineral Extraction](path_to_image)

**Implementation Details:**
- Алгоритмы добычи минералов
- Взаимодействие с инструментами и объектами для добычи
- Система переработки и использования добытых материалов

---

### 5.3 &nbsp;&nbsp;Drilling Site Search System

Этот раздел посвящен системе поиска месторождений для бурения. Описание алгоритмов и интерфейсов для поиска и выбора лучших мест для бурения.

![Drilling Site Search](path_to_image)

**Implementation Details:**
- Алгоритмы поиска мест для бурения
- Взаимодействие с картой мира и географическими данными
- Оптимизация для повышения производительности

---

## 6. Graphics and Materials

### 6.1 &nbsp;Materials

Этот раздел описывает материалы, используемые в игре, включая различные текстуры и шейдеры для различных объектов в мире игры.

![Materials](path_to_image)

**Implementation Details:**
- Разнообразие материалов для различных объектов
- Спецификации текстур и шейдеров
- Принципы применения материалов на различных объектах

---

### 6.1.1 &nbsp;&nbsp;Landscape (Large Landscape)

Здесь обсуждается использование материалов для создания больших ландшафтов в игре, включая текстуры и особенности их наложения на большие участки.

![Landscape](path_to_image)

**Implementation Details:**
- Технологии создания ландшафтов
- Использование текстур и материалов на больших пространствах
- Оптимизация для производительности

---

### 6.1.2 &nbsp;&nbsp;Procedural CellShader

Этот раздел посвящен процедурному шейдеру, который используется для создания визуального стиля, похожего на мультфильмы, путем обработки текстур и освещения.

![Procedural CellShader](path_to_image)

**Implementation Details:**
- Разработка и применение процедурного шейдера
- Влияние на внешний вид объектов
- Оптимизация и производительность

---

### 6.1.3 &nbsp;&nbsp;Metallic Materials for CellShader

Здесь рассматриваются металлические материалы, которые применяются в шейдерах для создания эффекта блеска и отражений.

![Metallic Materials](path_to_image)

**Implementation Details:**
- Разработка металлических материалов для шейдера
- Взаимодействие с освещением и отражениями
- Применение в различных объектах

---

### 6.1.4 &nbsp;&nbsp;Materials for Foliage with Wind

Этот раздел описывает материалы для растительности, которые реагируют на ветер, создавая эффект движения листвы и травы.

![Materials for Foliage with Wind](path_to_image)

**Implementation Details:**
- Реализация материалов для растительности с учетом ветра
- Использование шейдеров для имитации движения
- Технические аспекты и производительность

---

### 6.1.5 &nbsp;&nbsp;Materials for Rocks with Moss

Здесь обсуждается создание материалов для камней с мхом, включая особенности текстур и визуальные эффекты.

![Materials for Rocks with Moss](path_to_image)

**Implementation Details:**
- Создание и применение материалов для камней
- Взаимодействие с окружающей средой и растительностью
- Текстуры и эффекты для реалистичного вида

---

### 6.1.6 &nbsp;&nbsp;Holographic Material

Этот раздел объясняет, как создаются голографические материалы, которые могут быть использованы для создания уникальных объектов и эффектов в игре.

![Holographic Material](path_to_image)

**Implementation Details:**
- Применение голографических эффектов
- Реализация шейдеров и текстур
- Взаимодействие с другими объектами в игре

---

### 6.1.7 &nbsp;&nbsp;Particle Materials (Various)

Здесь описываются различные материалы для частиц, используемые в эффектах, таких как дым, огонь и другие визуальные эффекты.

![Particle Materials](path_to_image)

**Implementation Details:**
- Разнообразие материалов для частиц
- Технологии создания эффектов частиц
- Применение материалов в разных частях игры

---

### 6.2 &nbsp;Niagara System

В этом разделе рассматривается система Niagara, которая используется для создания визуальных эффектов, таких как дым, огонь, взрывы и другие динамичные элементы.

![Niagara System](path_to_image)

**Implementation Details:**
- Принципы работы системы Niagara
- Разработка и настройка визуальных эффектов
- Применение Niagara для создания эффектов частиц

---

### 6.2.1 &nbsp;&nbsp;Dissolve Effect for Objects

Здесь объясняется, как создаются эффекты растворения для объектов, которые могут исчезать или растворяться по мере взаимодействия с ними.

![Dissolve Effect](path_to_image)

**Implementation Details:**
- Технологии и шейдеры для эффекта растворения
- Реализация с учетом освещения и физики
- Применение в различных частях игры

---

### 6.2.2 &nbsp;&nbsp;Cartoon Explosion

Этот раздел описывает создание мультяшных взрывов с использованием системы Niagara и других визуальных эффектов.

![Cartoon Explosion](path_to_image)

**Implementation Details:**
- Разработка мультяшных взрывов и их анимация
- Применение системы Niagara для создания эффектов
- Влияние на игровой процесс и визуальные эффекты

---

### 6.2.3 &nbsp;&nbsp;Cartoon Smoke

Здесь рассматривается создание мультяшного дыма с помощью Niagara, который используется в различных ситуациях, таких как взрывы или огонь.

![Cartoon Smoke](path_to_image)

**Implementation Details:**
- Принципы создания мультяшного дыма
- Реализация с учетом взаимодействия с другими эффектами
- Применение в различных частях игры

---

### 6.3 &nbsp;Landscape and Environment

Этот раздел описывает создание ландшафта и окружающей среды, включая текстуры, модели и материалы, которые используются для имитации различных природных элементов.

![Landscape and Environment](path_to_image)

**Implementation Details:**
- Разработка и создание ландшафта
- Применение материалов и текстур для различных природных объектов
- Оптимизация окружения для производительности

---

### 6.3.1 &nbsp;&nbsp;Different Types of Foliage and Grass

Здесь обсуждаются различные виды растительности, такие как деревья, кустарники и трава, и материалы, которые используются для их создания и анимации.

![Different Types of Foliage and Grass](path_to_image)

**Implementation Details:**
- Разнообразие растительности и типов травы
- Применение шейдеров для растительности
- Взаимодействие с окружающим миром

---

## 7. User Interface (UI)

### 7.1 &nbsp;Main Menu

Этот раздел описывает главный экран меню игры, который служит центральным пунктом для навигации по различным функциям игры.

![Main Menu](path_to_image)

**Implementation Details:**
- Структура и элементы главного меню
- Взаимодействие с различными разделами игры
- Анимация и переходы

---

### 7.2 &nbsp;Settings

Здесь описывается меню настроек, которое позволяет игрокам настроить параметры игры, такие как графика, звук и управление.

![Settings](path_to_image)

**Implementation Details:**
- Опции настройки графики, звука и управления
- Использование конфигурационных файлов
- Влияние изменений на игровой процесс

---

### 7.3 &nbsp;Pause

Этот раздел посвящен экрану паузы, который позволяет игроку остановить игру и получить доступ к различным опциям.

![Pause](path_to_image)

**Implementation Details:**
- Взаимодействие с игровой логикой во время паузы
- Доступные опции в меню паузы
- Влияние на производительность игры

---

### 7.4 &nbsp;Inventory

Здесь рассматривается система инвентаря, которая позволяет игрокам собирать и управлять предметами внутри игры.

![Inventory](path_to_image)

**Implementation Details:**
- Структура и интерфейс инвентаря
- Система хранения и сортировки предметов
- Взаимодействие с другими системами игры

---

### 7.5 &nbsp;Research

Этот раздел описывает систему исследования, которая позволяет игрокам развивать новые технологии и возможности в игре.

![Research](path_to_image)

**Implementation Details:**
- Механизм исследования и разработки технологий
- Влияние на прогресс в игре
- Структура и интерфейс системы исследования

---

### 7.6 &nbsp;Character Interface

Здесь обсуждается интерфейс персонажа, который отображает здоровье, энергию и другие параметры, важные для игрового процесса.

![Character Interface](path_to_image)

**Implementation Details:**
- Отображение статуса персонажа
- Обновление и отображение параметров в реальном времени
- Технические детали интерфейса
