# Matchy Star – Game Design Document (Concise)

Steam Page: https://matchystar.com  
Developer: Silverware Games, Inc.  
Primary Contact: michael@silverwaregames.com / @michaelplzno  
Uncut Play Video: https://www.youtube.com/watch?v=rDVWQaZiYxs

## 1. What Matchy Star Is

Matchy Star is a **skill-driven, replayable matching game** set in a sci-fi universe, focused on *clarity, mastery, and long-term fun* rather than monetization pressure or casino-style manipulation.

The current alpha proves the core loop is solid. The goal of this design document is to define **what systems, content, and structure are required to turn it into a complete, exceptional game** with depth, progression, and hundreds of hours of meaningful play.

This document summarizes the **actual planned features and milestones**, as tracked in the Matchy Star GDD issues repository.

## 2. Core Gameplay Loop (Current + Planned)

### Current Loop (Alpha)
1. Select level.
2. Make matches to supply ship with fuel.
3. Once 3 ships reach the end you win the level.
4. Run ends → results shown → repeat

This loop works, but lacks:
- Long-term structure
- Player agency before runs
- Meaningful progression systems
- Clear world context

The planned systems below extend and deepen this loop.

## 3. Core Gameplay Systems

### 3.1 Ballast System (Planned Core System)

The **Ballast System** introduces weight, balance, and risk management into gameplay.

- Ships have a ballast value affected by player actions
- Ballast influences gameplay outcomes (difficulty, stability, or scoring)
- A **Ballast Counter UI** gives constant feedback to the player

Purpose:
- Adds decision-making beyond simple matching
- Creates tension and mastery opportunities
- Makes runs feel distinct and skill-based

This is a **pillar system**, not optional content.

### 3.2 Arc Chart UI (Planned Core UI)

The **Arc Chart** is a visual gameplay aid showing:
- Progression arcs
- Risk thresholds
- Outcome trends

Purpose:
- Improve player understanding of cause → effect
- Reduce confusion during advanced play
- Support higher skill ceilings without tutorials

This UI is meant to **teach through visualization**, not text.

## 4. Player Agency & Progression

### 4.1 Character Selection (Pre-Run)

Players will select a character (or ship / loadout equivalent) **before starting a run**.

Each character may affect:
- Starting conditions
- Ballast behavior
- Rules or modifiers

Purpose:
- Give players intentional choices
- Encourage experimentation
- Support replayability

### 4.2 Unlockables & Game Modes

Players unlock:
- Characters
- Gameplay modes
- Rule variants (e.g. “Breaks On” vs “Breaks Off”)

Unlocks are **earned through play**, not monetization.

Purpose:
- Extend long-term engagement
- Allow players to tailor difficulty and style
- Prevent stagnation of the core loop

## 5. World & Level Structure

Matchy Star uses a **celestial progression model**, with themed regions that introduce new challenges and visual identity.

### Planned Regions:
1. **Celestial 1 – Alpha System**  
   - Introductory region  
   - Teaches baseline mechanics  

2. **Celestial 2 – Starbase**  
   - Increased system interaction  
   - Greater emphasis on planning and control  

3. **Celestial 3 – Moon Spittoon**  
   - Advanced mechanics  
   - Higher risk / reward  
   - Designed for experienced players

4. ** There will be 11 total celestials **

Each region is intended to:
- Reinforce mastery
- Introduce variation without overwhelming
- Provide a sense of journey and place

## 6. Game Flow & UX Improvements

### 6.1 Lobby Flow

The current lobby is under review.

Planned actions:
- Either remove it entirely or redesign it
- Reduce friction between runs
- Prevent UI obstruction or confusion (e.g., ships blocking visibility)

Goal:
- Faster time from “launch game” → “playing”
- Cleaner mental model for players

### 6.2 Level Naming & Clarity

Some levels currently suffer from unclear naming or intent.

Planned improvements:
- Rename levels where necessary
- Align names with mechanics and expectations

Goal:
- Reduce confusion
- Make progression feel intentional and readable

## 7. Visual & Technical Cleanup

### Planned Technical Work:
- Migrate item handling to a **Sprite-based system**
- Fix known visual bugs (e.g., incorrect runway lights)
- Improve ship visibility and UI layering

Purpose:
- Reduce bugs
- Improve maintainability
- Increase visual clarity during play

## 8. Milestone Overview

### Phase 1 – Core Systems
- Ballast system implemented
- Ballast UI integrated
- Sprite system migration

### Phase 2 – Player Choice
- Character select screen
- Unlockable characters
- Alternate gameplay modes

### Phase 3 – World Completion
- Alpha System finalized
- Starbase region implemented
- Moon Spittoon region implemented

### Phase 4 – Polish & Flow
- Lobby redesign or removal
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

### Contribution Rules:
- GitHub Community Guidelines apply
- This repo is for Matchy Star only
- Final creative decisions belong to Silverware Games
- No guaranteed compensation for ideas (free copy if used)
- Report vulnerabilities privately

## 11. Design North Star

When making decisions, ask:

**Does this increase clarity, mastery, or long-term fun?**

If not, it should be reconsidered.
