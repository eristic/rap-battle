# Rap Battle

Battle LLMs to prove you've got more heart.

A text-based rap battle game that lives entirely inside AI skill files. Play in Cursor or Claude -- no code, no dependencies, just bars.

## How to Play

### In Cursor

Add the `rap-battle/` directory to your project, then open a chat and say any of these:
- "Let's rap battle"
- "Start a rap battle"
- "I want to spit bars"

Cursor picks up `rap-battle/SKILL.md` as a skill and triggers the game automatically.

### In Claude

1. Create a Claude project.
2. Paste the contents of `rap-battle/SKILL.md` into the project's system prompt (or at the start of a conversation).
3. Also paste (or attach) the round skills (`rap-battle/round-1/SKILL.md` through `rap-battle/round-5/SKILL.md`) and the judge (`rap-battle/judge/SKILL.md`) so the model can reference them when running a round or scoring.

## The Game

1. **Create your character** -- pick a name, where you rep, and how you look
2. **Face 5 opponents** of increasing difficulty (Sloppy → Amateur → Intermediate → Advanced → Expert)
3. **Coin toss** decides who spits first
4. **Deliver 3 stanzas of 4 lines** (12 bars total)
5. **Get judged** on Bars, Flow, Personals, Performance, and Rebuttal
6. **Win to advance** -- lose and you can rematch or walk away

## Structure

```
rap-battle/
├── SKILL.md          ← Orchestrator (game launcher & flow control)
├── judge/SKILL.md    ← Scoring rubric & evaluation
├── round-1/SKILL.md  ← Level 1: Sloppy
├── round-2/SKILL.md  ← Level 2: Amateur
├── round-3/SKILL.md  ← Level 3: Intermediate
├── round-4/SKILL.md  ← Level 4: Advanced
└── round-5/SKILL.md  ← Level 5: Expert
```

### Why Markdown Files?

Each round is a standalone instruction file you can read, study, and learn from. Want to know how the Expert opponent constructs bars? Read `round-5/SKILL.md`. Want to understand what the judge values? Read `judge/SKILL.md`. The game is transparent by design -- study the system, improve your craft.

## Judging Criteria

| Category | Weight | What It Measures |
|----------|--------|------------------|
| Bars | 30% | Punchlines, wordplay, multisyllabics, creativity |
| Flow | 20% | Rhythm, cadence, internal rhymes |
| Personals | 20% | Opponent-specific disses, relevance |
| Performance | 15% | Confidence, swagger, delivery |
| Rebuttal | 15% | Flipping opponent's lines, counter-punches |

## Tips

- Read the round skills to understand what you're up against
- Personals matter -- use your opponent's name, look, and location against them
- Save your hardest bar for last (the judge notices closers)
- If you go second, flip something specific from their verse
- Multisyllabic rhymes score higher than single-syllable ones
