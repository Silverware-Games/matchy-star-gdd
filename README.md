# Matchy Star – Game Design Document

Steam Page: https://matchystar.com  
Developer: [Silverware Games, Inc.](https://silverwaregames.com)  
Primary Contact: michael@silverwaregames.com / @michaelplzno  
Uncut Play Video: https://www.youtube.com/watch?v=rDVWQaZiYxs

## 1. What Matchy Star Is

Matchy Star is a **skill-driven, system-focused matching game** set in a colorful, wacky sci-fi universe (“the Matchyverse”).  
It prioritizes **clarity, mastery, and long-term replayability**, and intentionally avoids monetization pressure, casino mechanics, or psychological manipulation.

The current alpha proves the core gameplay is already fun.  
This document defines the systems and structure that turn Matchy Star into a **deep, replayable, high-skill game** that remains accessible.

This is a design plan, not a pitch.

## 2. Core Gameplay Loop

### Current Loop (Alpha)
1. Select a level.
2. Match Stars to fuel ships.
3. If ships run out of fuel it's game over.
4. When three ships reach the destination, the level is cleared.
5. Results → next level.

This loop works, but is extended by the systems below to support mastery, progression, and long-term play.

## 3. Core Systems

### 3.1 Ballast/Speed System (Pacing & Difficulty Core)

**Ballast** is the single system governing pacing, difficulty, and risk.

- Ballast is an integer value
- It determines how much the player can manipulate the board before ships advance

**Thresholds (tunable):**
- **Speed 0–5:** Effectively turn-based (high control)
- **Speed 6+:** Ships move autonomously
- **Speed ~10:** Upper bound for skilled play

**Movement Budget:**
- Each ship has a Ballast value (≥1)
- The player may move gems **one grid space per point of Ballast** before ships advance
  - Ballast 20 → 20 grid spaces
  - Ballast 1 → 1 grid space

As Celestials progress, baseline Ballast decreases, increasing pressure.

**Tradeoffs:**
- Powerful items and score multipliers often **increase Ballast**
- Control-oriented play reduces Ballast but limits scoring
- High scores require accepting risk

Ballast replaces “turn-based vs speed modes” with a **single continuous spectrum**.

### 3.2 Cluster System (Persistent Star Pool)

The **Cluster** is the player’s active pool of Stars, treated as a **managed set**, not pure randomness.

- Finite Star pool (e.g., 70–140 total, tunable)
- Stars are drawn from this pool during play
- Items, characters, and modes modify the Cluster over time

**Star Variants include:**
- Standard Stars
- Asteroids (match anything in a 3-match, bonus points)
- Shiny / Glowing / Special Stars with buffs
- Optional size variants (small / medium / large)

A **Cluster View** screen shows the current pool and modifications.

**Goal:**  
Reduce randomness, reward foresight, and support deck-building style mastery.

### 3.3 Characters as Rule Sets

Characters are **not cosmetic**.  
Each character represents a **distinct way of playing the game**, unlocking modes and rule variations.

Examples (working concepts):

- **Matchy** – Low Ballast, planning-focused
- **Speedy Sputnik** – High Ballast, execution-focused
- **Guru Moon** – Prediction and move queuing
- **Dr. UFO** – Healing, survival, recovery
- **Loony Lander** – Environmental manipulation
- **Pirate Planet** – Economy-focused, high-risk Zoot runs
- **King Zazz** – Rule-bending, mastery-only play

Some items are **character-locked or character-enhanced**, creating unique synergies.

### 3.4 Inventory Overhaul (Meaningful Choice)

The inventory is redesigned as a **curated loadout**, not storage.

- Few active item slots
- Items involve commitment and tradeoffs
- Swapping items is costly or constrained
- Items may increase Ballast, distort the Cluster, or lock future choices

The goal is to eliminate “best item forever” behavior and force **intentional decisions**. Also hoarding/churning through items is not allowed.

### 3.5 Items, Shop, & Zoot Economy

Zoot and items are **high-impact systems**.

- Even 1 Zoot can matter (Think Balatro Money System)
- There is no inflation phase
- Buying the wrong item can doom a run

**Items:**
- ~150 functionally unique items
- No filler or minor stat bumps
- Each item meaningfully changes playstyle

**Synergies:**
- Rare combinations can “break” scoring systems
- High-upside runs are possible but not guaranteed
- Inspired by Balatro-style discovery and risk

Power always comes with tradeoffs (Ballast, commitment, instability).

## 4. World Structure & Tone

### 4.1 Celestials & Naming

The Matchyverse is intentionally playful and memorable (Bikini Bottom–style tone).

Example Celestials:
- Tube-Top Galaxy
- Starter Sprinkles
- Snack Station
- Moon Spittoon
- Cherry Bombast
- Rubble Rumble
- The Snack Hole
- Double Bubble Zone
- Matchsplosion
- Tangle Spangle
- Blurple Soup
- Xanadu (final system)

There are **11 total Celestials** in the complete game.

Names communicate **tone, mechanics, and escalation**, not realism.

## 5. Five-System Run (Procedural Galaxy Mode)

A repeatable, high-skill mode.

- Five Star Systems placed procedurally
- Connected via a generated path
- Each system contains five regenerating levels
- Mix of hand-authored and procedural content

**Cosmic Modifiers:**
- Aligned planets
- Extra planets
- Ascending / descending planets (affect Ballast & scoring)

Poor item or Cluster decisions can make a run unwinnable.  
This is intentional.

## 6. Meta Systems

### 6.1 Matchydex (Discovery & Stats)

An in-game encyclopedia and stat hub.

- Entries for all Stars, items, states, characters, and systems
- Entry states: Locked → Undiscovered → Known
- Tracks stats like:
  - Stars matched (by color)
  - Runs won / lost
  - Total Zoot collected

Designed to reward curiosity and mastery.

## 7. Design Constraints

Matchy Star avoids:
- Energy timers
- Gacha mechanics
- Pay-to-win systems
- Psychological manipulation

If a feature relies on frustration or coercion, it does not belong.

## 8. Design North Star

When evaluating any decision, ask:

**Does this increase clarity, mastery, or meaningful choice?**

If not, reconsider.

## 9. Feedback & Contributions

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
