# Matchy Star – Game Design Document

Steam Page: https://matchystar.com  
Developer: Silverware Games, Inc.  
Primary Contact: michael@silverwaregames.com / @michaelplzno  
Uncut Play Video: https://www.youtube.com/watch?v=rDVWQaZiYxs

## 1. What Matchy Star Is

Matchy Star is a **skill-driven, replayable matching game** set in a sci-fi universe. It prioritizes **clarity, mastery, and long-term fun**, deliberately avoiding monetization pressure, casino mechanics, or psychological manipulation.

The current alpha build demonstrates that the core loop is already fun and functional. The purpose of this document is not to justify the game’s existence, but to define **the systems, structure, and content required to elevate it into a complete, exceptional experience** with strong progression and long-term replay value.

This document reflects the **actual planned design direction and milestones**, as tracked in the Matchy Star GDD issues repository.

## 2. Core Gameplay Loop (Current + Planned)

### Current Loop (Alpha)
1. Select a level  
2. Make matches to supply ships with fuel  
3. Once three ships reach the destination, the level is cleared  
4. Results are shown → next level

This loop is solid, readable, and fun, but currently lacks:
- Long-term progression context
- Pre-run player agency
- Systems that reward mastery over time
- A strong sense of world and journey

The systems below extend this loop without replacing it.

## 3. Core Gameplay Systems

### 3.1 Ballast System (Core Pillar)

The **Ballast System** introduces weight, balance, and risk management into matching decisions.

- Ships accumulate ballast based on player actions
- Ballast meaningfully affects outcomes (difficulty, stability, scoring, or efficiency)
- A dedicated **Ballast Counter UI** provides continuous feedback

**Purpose:**
- Elevates matching from pattern recognition to decision-making
- Creates tension and meaningful trade-offs
- Allows mastery to emerge over repeated play

This is a **foundational system**, not optional content.

### 3.2 Arc Chart UI (Core UI System)

The **Arc Chart** visually communicates:
- Progression arcs
- Risk thresholds
- Likely outcomes based on current state

**Purpose:**
- Makes cause → effect legible at a glance
- Reduces confusion as systems stack
- Supports higher skill ceilings without relying on text tutorials

This UI teaches through **visualization and feedback**, not instruction.

## 4. Player Agency & Progression

### 4.1 Character Selection (Pre-Run)

Players select a character (or equivalent ship/loadout) before starting a run.

Characters influence:
- Starting conditions
- Ballast behavior
- Rules, modifiers, or strategic emphasis

**Purpose:**
- Give players ownership over how they play
- Encourage experimentation
- Increase replayability without content bloat

### 4.2 Unlockables & Game Modes

Players unlock:
- Characters
- Gameplay modes
- Rule variants (e.g., “Breaks On” vs “Breaks Off”)

All unlocks are **earned through play**, not monetization.

**Purpose:**
- Sustain long-term engagement
- Let players tailor difficulty and playstyle
- Keep the core loop fresh without relying on RNG or grind

## 5. World & Level Structure

Matchy Star uses a **celestial progression model**, where themed regions introduce new mechanics, constraints, and visual identity.

### Planned Regions (Examples):
1. **Celestial 1 – Alpha System**  
   - Introductory region  
   - Establishes baseline mechanics  

2. **Celestial 2 – Starbase**  
   - Increased system interaction  
   - Greater emphasis on planning and control  

3. **Celestial 3 – Moon Spittoon**  
   - Advanced mechanics  
   - Higher risk / reward  
   - Designed for experienced players  

There will be **11 total Celestials** in the complete game.

Each region is designed to:
- Reinforce mastery
- Introduce variation without overwhelming the player
- Provide a clear sense of progression, place, and journey

## 6. Game Flow & UX Improvements

### 6.1 Lobby Flow

The current lobby flow will be refined.

Planned actions:
- Simplify or remove unnecessary transitions
- Reduce friction between levels
- Prevent UI obstruction or visual confusion

**Goal:**
- Minimize time from “launch game” → “playing”
- Maintain a clean, intuitive mental model

### 6.2 Level Naming & Clarity

Some levels require clearer naming or framing.

Planned improvements:
- Rename levels where intent is unclear
- Align names with mechanics and expectations

**Goal:**
- Reduce player confusion
- Make progression feel deliberate and readable

## 7. Visual & Technical Cleanup

### Planned Technical Work:
- Migrate item handling to a centralized **Sprite-based system**
- Resolve known visual bugs (e.g., runway lighting inconsistencies)
- Improve ship visibility and UI layering

**Purpose:**
- Increase stability and maintainability
- Improve visual clarity during play
- Support future expansion cleanly

## 8. Milestone Overview

### Phase 1 – Core Systems
- Ballast system implementation
- Ballast UI integration
- Sprite system migration

### Phase 2 – Player Choice
- Character select screen
- Unlockable characters
- Alternate gameplay modes

### Phase 3 – World Completion
- Alpha System finalized
- Starbase region implemented
- Moon Spittoon region implemented
- Additional Celestials in production

### Phase 4 – Polish & Flow
- Lobby flow refinement
- Arc Chart UI finalized
- Bug fixes and UX clarity pass

## 9. Design Constraints

Matchy Star intentionally avoids:
- Energy timers
- Gacha mechanics
- Pay-to-win systems
- Psychological manipulation

If a feature relies on frustration, confusion, or coercion to increase engagement, it does not belong in this game.

## 10. Feedback & Contributions

Feedback is welcome and encouraged.

- Submit ideas or bugs via GitHub Issues:  
  https://github.com/Silverware-Games/matchy-star-gdd/issues
- Email: michael@silverwaregames.com
- Discord: https://discord.silverwaregames.com

### Contribution Rules
- GitHub Community Guidelines apply
- This repository is for Matchy Star only
- Final creative decisions belong to Silverware Games
- No guaranteed compensation for ideas (free copy if used)
- Report vulnerabilities privately

## 11. Design North Star

When evaluating any decision, ask:

**Does this increase clarity, mastery, or long-term fun?**

If not, it should be reconsidered.
