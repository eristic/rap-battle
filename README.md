# Rap Battle

Battle LLMs to prove you've got more heart.

A text-based rap battle game that lives entirely inside AI skill files. Play in Cursor or Claude -- no code, no dependencies, just bars.

## How to Play

### In Cursor

Open a chat and say any of these:
- "Let's rap battle"
- "Start a rap battle"
- "I want to spit bars"

The game skill triggers automatically and walks you through everything.

### In Claude

Copy the contents of `.cursor/skills/rap-battle-game/SKILL.md` into a Claude project's system prompt or paste it at the start of a conversation. Reference the round and judge skills as needed.

## The Game

1. **Create your character** -- pick a name, where you rep, and how you look
2. **Face 5 opponents** of increasing difficulty (Sloppy → Amateur → Intermediate → Advanced → Expert)
3. **Coin toss** decides who spits first
4. **Deliver 3 stanzas of 4 lines** (12 bars total)
5. **Get judged** on Bars, Flow, Personals, Performance, and Rebuttal
6. **Win to advance** -- lose and you can rematch or walk away

## Skill Architecture

```
.cursor/skills/
├── rap-battle-game/SKILL.md      ← Main launcher & orchestrator
├── rap-battle-judge/SKILL.md     ← Scoring rubric & evaluation
├── rap-battle-round-1/SKILL.md   ← Level 1: Sloppy
├── rap-battle-round-2/SKILL.md   ← Level 2: Amateur
├── rap-battle-round-3/SKILL.md   ← Level 3: Intermediate
├── rap-battle-round-4/SKILL.md   ← Level 4: Advanced
└── rap-battle-round-5/SKILL.md   ← Level 5: Expert
```

### Why Skills?

Each round is a standalone skill file you can read, study, and learn from. Want to know how the Expert opponent constructs bars? Read Round 5's skill. Want to understand what the judge values? Read the judge skill. The game is transparent by design -- study the system, improve your craft.

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
