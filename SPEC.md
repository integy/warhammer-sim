# Warhammer 40K WTC Simulator

## Project Overview
- **Type:** Single-page web application (HTML/CSS/JS)
- **Purpose:** Web-based Warhammer 40K tabletop simulator following WTC rules
- **Target:** 10th Edition Warhammer 40K players

## WTC Rules Features

### Game Structure
- 5 rounds, 3 hours total
- 5 Battle Rounds
- Primary Objectives: WTC 2025/2026 missions
- Secondary Objectives: WTC fixed set

### Scoring (WTC)
- Battle Points (BP): 20 max per round
- Win: 20BP, Draw: 15BP each, Loss: 12BP
- Margin of Victory bonus

### Phase System
1. **Command Phase** - CP re-rolls, battle-shock
2. **Movement Phase** - Move, Advance, Fall Back
3. **Shooting Phase** - Select unit, select weapon, roll attacks
4. **Charge Phase** - Charge moves, Heroic Interventions
5. **Fight Phase** - Fight with units
6. **Morale Phase** - Morale tests

## Core Features

### 1. Army Builder
- Select Faction (all 10th ed factions)
- Add Units with wargear
- Point calculation (2000pts standard)
- Load/Save army lists (localStorage)

### 2. Dice Roller
- Hit Roll (BS/WS)
- Wound Roll (S vs T)
- Save Roll (AP modified)
- Invulnerable saves
- Rerolls (1s, failed, +1/+2 modifiers)
- Damage allocation

### 3. Unit Cards
- Model count
- Wounds, Toughness, Save, Leadership
- Weapon profiles (Range, S, AP, D, abilities)
- Unit abilities

### 4. Game Board
- Visual battlefield (HTML5 Canvas)
- Movement templates (3", 6", 9", 12")
- Deployment zones
- Objective markers

### 5. Phase Tracker
- Current phase display
- Turn number
- Round number
- Command Points

### 6. WTC Scoring
- Primary objective tracker
- Secondary objective selection
- Battle Points calculator
- Match score display

## UI Design

### Layout
- Dark theme (Warhammer aesthetic)
- Left sidebar: Unit list, Army builder
- Center: Game board / Dice roller
- Right sidebar: Phase tracker, Score

### Colors
- Background: #1a1a1a
- Accent: Gold #c9a227
- Text: #e0e0e0
- Buttons: #2d2d2d with gold borders

## Technical Implementation
- Pure HTML/CSS/JavaScript (no frameworks)
- localStorage for army persistence
- Canvas for game board
- Responsive design

## File Structure
```
warhammer-sim/
├── index.html      # Main game
├── SPEC.md         # This file
└── README.md       # Instructions
```

## Evolution
- Hourly improvements via OpenClaw cron job
- New features, bug fixes, UI enhancements
