# Matchy Star - Game Design Document

Steam Page: https://matchystar.com  
Developer: [Silverware Games, Inc.](https://silverwaregames.com)  
Primary Contact: michael@silverwaregames.com / @michaelplzno  
Uncut Play Video: https://www.youtube.com/watch?v=rDVWQaZiYxs

## 1. What Matchy Star Is

Matchy Star is a skill-driven matching adventure about helping goofy little ships cross strange cosmic routes by matching Stars, managing resources, and making increasingly clever decisions.

The game should feel colorful, funny, readable, optimistic, and fair. It should be easy to start, but deep enough that experienced players can chase better routes, better builds, better scores, and better runs.

The core player promise:

> Move Stars. Fuel ships. Read the route. Make smart choices. Survive the trip. Discover the Matchyverse.

Matchy Star is not trying to be a casino-style mobile puzzle game. It avoids gacha pressure, energy timers, pay-to-win systems, and psychological manipulation. It is a real game first.

## 2. Design North Star

When evaluating any design, UI, system, item, level, or piece of writing, ask:

**Does this increase clarity, mastery, personality, or meaningful choice?**

If not, reconsider it.

The current priority is **player understanding**. Matchy Star already has interesting systems, but players must be able to see what those systems do, why they matter, and how their own choices affect the result.

## 3. The First-Time Player Experience

The first ten minutes matter more than any late-game system.

A new player should quickly understand:

- What they are trying to do.
- How matching Stars helps ships.
- Why ships win or lose a route.
- What makes one move better than another.
- Why they should care about the next planet, item, or run.

The player should never feel like they won or lost for mysterious reasons. Discovery is good when it reveals depth. It is bad when it hides basic rules.

### 3.1 First Tutorial Arc

The tutorial should teach one concept at a time, then let the player prove they understand it.

**Beat 1: Make a Match**
- Teach moving a Star.
- Teach making a match.
- Celebrate the first successful match.

**Beat 2: Feed the Ship**
- Show that matched Stars become fuel or movement help for the ship.
- Use clear animation, sound, and text to connect the match to the ship.
- The player should understand: "I matched Stars, so the ship advanced or survived."

**Beat 3: Read the Route**
- Show where the ship is trying to go.
- Make path arrows readable early enough for planning.
- Teach that the player is guiding ships across a route, not just clearing a board.

**Beat 4: Understand Win and Loss**
- Explain the level objective before play begins.
- Explain victory after the route is cleared.
- Explain failure in a useful, friendly way.

**Beat 5: Progression and Items**
- Introduce Zoot, items, upgrades, and the Matchydex only after the player understands the basic route.
- When something changes, show what changed and why it matters.

## 4. Core Gameplay Loop

1. Choose a route, planet, or run.
2. Read the current mission goal.
3. Match Stars to fuel ships, shape the board, and support the route.
4. Watch ships move, collect Stars, trigger items, and face hazards.
5. Clear the level or learn why the route failed.
6. Earn Zoot, discover entries, adjust items, and continue through the Matchyverse.
7. Build mastery across repeated runs.

The loop works only if cause and effect are visible. The player should be able to answer: "What did I just do, what changed, and what should I try next?"

## 5. Minimum Viable Narrative

Matchy Star does not need expensive animated cutscenes to have story. It does need enough context to make progress feel like a journey.

The minimum narrative goal is to answer:

- Who am I helping?
- Why are these ships traveling?
- What is this planet or system about?
- Why does reaching the next destination matter?

Working frame:

> Matchy is a cosmic guide helping a fleet of silly ships travel through the Matchyverse. Every planet has a weird rule, hazard, reward, or personality. The player clears routes, earns Zoot, discovers Stars and items, and fills out the Matchydex as a record of the journey.

Narrative can be delivered cheaply through:

- Short mission briefings.
- Character quips.
- Planet intro text.
- Ship reactions.
- Results screen comments.
- Matchydex flavor text.
- Small VO barks where useful.

Example tone:

> Matchy: "Welcome to Starter Sprinkles. The routes are short, the Stars are friendly, and Zippy only panics a little."
>
> Zippy: "I heard that!"

The goal is emotional glue, not lore bloat.

## 6. Strategic Depth

The game should explicitly teach players what makes a good move.

A good move might:

- Fuel a ship before it runs out.
- Set up a larger future match.
- Preserve useful Stars for later.
- Support the current ship, item, or Cluster build.
- Reduce risk before the next ship movement.
- Sacrifice points for survival.
- Accept danger for a bigger score or Zoot payoff.

Players should gradually learn to plan rather than only grabbing the most obvious match. The game should support this through tutorials, route readability, tips, item feedback, and results screens that explain what mattered.

## 7. Core Systems

### 7.1 Ships, Routes, and Fuel

Ships are the emotional and mechanical center of a level.

Player-facing rule:

> Match Stars to help ships survive the route.

Ships should clearly show:

- Where they are going.
- How much danger they are in.
- What resource they need.
- Why they advanced, stalled, succeeded, or failed.

If a ship runs out of fuel, the game should explain what happened and what the player can try differently.

### 7.2 Ballast / Movement Budget

Ballast is the pacing and pressure system.

Player-facing rule:

> Ballast tells you how much control you have before ships advance.

Design meaning:

- More control gives players time to plan.
- Less control creates pressure and risk.
- High-score or high-power builds may accept more danger.
- Ballast can replace a hard split between turn-based and real-time modes with a continuous spectrum.

Working thresholds:

- **0-5:** planning-focused, effectively turn-based.
- **6+:** ships begin to feel more autonomous and pressured.
- **Around 10:** upper pressure range for skilled play.

The term "Ballast" can stay because it has flavor, but the UI must explain its practical meaning before relying on the term.

### 7.3 Cluster

The Cluster is the player's active pool of Stars. It is the deck-like system behind board randomness.

The Cluster can include:

- Standard Stars.
- Asteroids and wild Stars.
- Shiny, glowing, or buffed Stars.
- Optional size variants.
- Stars modified by items, characters, or run events.

Design goal:

> Reduce pure randomness, reward foresight, and support deck-building style mastery.

The Cluster View should help players understand what is in their pool, what changed, and how their build affects future levels.

### 7.4 Characters and Ships as Rule Sets

Characters and ships are not cosmetic. They should change how the player thinks.

Working concepts:

- **Matchy:** planning-focused, low-pressure introduction.
- **Speedy Sputnik:** speed and execution.
- **Guru Moon:** prediction and queued moves.
- **Dr. UFO:** healing, survival, and recovery.
- **Loony Lander:** environmental manipulation.
- **Pirate Planet:** economy-focused high-risk Zoot runs.
- **King Zazz:** rule-bending mastery play.

Each character or ship should have:

- A short intro.
- A readable gameplay identity.
- A personality hook.
- Clear item or rule synergies.

### 7.5 Inventory, Items, Shop, and Zoot

The inventory is a curated loadout, not storage.

Design goals:

- Few active item slots.
- Items involve commitment and tradeoffs.
- Swapping items is costly or constrained.
- Items visibly activate when they matter.
- Hoarding and mindless item churn are discouraged.

Zoot is the economy. Even 1 Zoot can matter.

Items should be functionally unique and readable. Each item should clearly explain:

- What it does.
- When it triggers.
- Which ship or system it affects.
- What tradeoff it creates.

Power should usually come with risk, commitment, Ballast pressure, Cluster instability, opportunity cost, or other readable tradeoffs.

## 8. Progression

Progression must be felt, not just recorded.

When the player reaches a new planet, unlocks an item, buys an upgrade, discovers a new Star, or clears a route, the game should show what changed.

Progression tools:

- Planet intro cards.
- Route summaries.
- Upgrade demonstrations.
- New mechanic callouts.
- Matchydex entries.
- Character quips.
- Results screens.
- Milestone celebrations.

A player should feel: "I am somewhere new, I learned something, and my choices matter."

## 9. Celestials and World Structure

The Matchyverse is intentionally playful, colorful, and memorable. Names should communicate tone, mechanics, and escalation, not realism.

Example Celestials:

- Tube-Top Galaxy.
- Starter Sprinkles.
- Snack Station.
- Moon Spittoon.
- Cherry Bombast.
- Rubble Rumble.
- The Snack Hole.
- Double Bubble Zone.
- Matchsplosion.
- Tangle Spangle.
- Blurple Soup.
- Xanadu.

There are 11 total Celestials in the complete game.

Each Celestial should ideally have:

- A visual theme.
- A short narrative premise.
- A mechanical identity.
- A reason the player cares about reaching or clearing it.

## 10. Five-System Run

The Five-System Run is the repeatable high-skill mode.

Working structure:

- Five Star Systems placed procedurally.
- Systems connected by a generated path.
- Each system contains a small set of levels or planets.
- Mix of hand-authored and procedural content.
- Cosmic modifiers create variety.

Possible modifiers:

- Aligned planets.
- Extra planets.
- Ascending or descending planets.
- Fuel pressure changes.
- Ballast changes.
- Score or Zoot risk/reward changes.

Poor item or Cluster decisions can make a run fail. That is acceptable only when the player can understand the risk, see the consequence, and learn from the loss.

The run must support mid-run save and continue. A player should never lose a run by accidentally returning to the menu.

## 11. Matchydex

The Matchydex is the discovery, glossary, stats, and mastery hub.

It should include entries for:

- Stars.
- Star states.
- Items.
- Characters.
- Ships.
- Celestials.
- Key mechanics.
- Run modifiers.

Entry states:

- Locked.
- Undiscovered.
- Known.

Stats may include:

- Stars matched by color.
- Runs won and lost.
- Total Zoot collected.
- Items discovered.
- Characters unlocked.
- Best runs, scores, and seeds.

The Matchydex should also help teach the game. It is not only a completionist screen. It is a player-facing guide to the Matchyverse.

## 12. Results Screens and Cause-and-Effect Feedback

Every level ending should teach the player something.

Victory screens should explain:

- Why the player succeeded.
- Which ships completed the route.
- What reward was earned.
- What changed in progression.
- What the next decision is.

Failure screens should explain:

- What caused the failure.
- Which resource or route condition broke down.
- One useful retry suggestion.

Examples:

> Cleared! Zippy reached the gate with 2 fuel left. Your big purple match gave the final boost.

> Route Failed. Skippy ran out of fuel before the last bend. Try setting up a larger match before the ship reaches the danger zone.

Avoid harsh language that makes players feel punished. The tone should encourage another try.

## 13. Accessibility and Clarity

Matchy Star should be approachable without flattening its depth.

Important clarity and accessibility goals:

- Tutorial is replayable.
- Path arrows are readable.
- Drag and click controls are supported.
- Items have tooltips.
- Important terms have plain-language explanations.
- Camera and view options support readability.
- Settings labels say exactly what they do.
- Leaving a run never silently destroys progress.
- Victory and failure screens explain cause and effect.
- Audio, speech, and visual feedback have adjustable settings.

## 14. Localization and Internationalization

Localization is a strong future opportunity, but core English clarity comes first.

Before translation, player-facing text should be:

- Short.
- Consistent.
- Plain-language first.
- Flavorful only after meaning is clear.
- Organized so translators understand context.

Potential future language priorities include Spanish, French, and Galician, with community translations possible later.

## 15. Positioning and Marketing Promise

The game should be easy to explain in one sentence.

Working hook:

> Matchy Star is a skill-based space matching adventure where every match fuels goofy ships through dangerous cosmic routes, and every item can change the run.

Marketing should emphasize what players actually do and feel:

- Guide ships through space routes.
- Match Stars with skill and planning.
- Build weird item synergies.
- Discover goofy planets and characters.
- Play a fair, non-predatory puzzle game.

Avoid relying only on broad terms like "strategic," "tactical," or "puzzle adventure" unless the page immediately shows what those words mean in Matchy Star.

## 16. Current Production Priority

The current priority is not more complexity. It is making the existing depth visible.

Near-term focus:

1. Redesign onboarding around one concept at a time.
2. Improve cause-and-effect feedback.
3. Make wins and losses educational.
4. Add cheap narrative context between levels and planets.
5. Make progression and upgrades feel tangible.
6. Show item effects and ship identities during play.
7. Make strategic play easier to recognize.
8. Preserve runs safely with save and continue support.

## 17. Design Constraints

Matchy Star avoids:

- Energy timers.
- Gacha mechanics.
- Pay-to-win systems.
- Psychological manipulation.
- Casino-style monetization pressure.

If a feature relies on frustration, coercion, or fear of missing out, it does not belong.

## 18. Feedback and Contributions

Feedback is welcome and encouraged.

- Submit ideas or bugs via GitHub Issues:  
  https://github.com/Silverware-Games/matchy-star-gdd/issues
- Email: michael@silverwaregames.com
- Discord: https://discord.silverwaregames.com

### Contribution Rules

- GitHub Community Guidelines apply.
- This repository is for Matchy Star only.
- Final creative decisions belong to Silverware Games.
- No guaranteed compensation for ideas.
- Report vulnerabilities privately.
