# Moka Pot

A Codex skill for dialing in moka pot coffee through measured baselines, taste feedback, and experiments that change one variable at a time.

Find a recipe that suits your pot, beans, grinder, and taste. Keep the settings that improve your cup, confirm them with another brew, and revisit them when your coffee or equipment changes.

## What it does

- Asks about your pot, roast, grinder, stove, water, current recipe, and preferred serving style.
- Uses your existing recipe as a baseline, or helps establish a starting recipe if you do not have one.
- Proposes one change per experiment, such as grind, starting water temperature, heat schedule, or stopping point.
- Uses taste and flow observations to explain the next adjustment, distinguishing bitterness, sourness, astringency, and strength.
- Keeps track of preferred settings, unsuccessful trials, and results that need confirmation.
- Offers local brew journals or chat-only tracking at the start of each session.

The intake covers 1-, 2-, 3-, 4-, 6-, 9-, and 12-cup pots, plus other or unknown sizes. Recommendations account for material and heat source. Brikka, electric, and other special models require their own manufacturer instructions; the skill does not assume that conventional stovetop techniques apply unchanged.

## What you need

- Codex with access to the skill files.
- A moka pot, coffee, water, and a compatible heat source.
- A scale, timer, and thermometer for controlled experiments. A phone timer is fine.
- Your grinder model and current setting, if you grind your own beans. Preground coffee also works; the skill will focus on variables you can adjust.

You can still ask general brewing questions without measurement tools. Controlled comparisons require all three tools so the results can be recorded consistently.

## Installation

### Use this repository

1. Clone or download this repository.
2. Open the repository folder as a project in Codex.
3. Start a chat and invoke `$moka-pot`.

### Use it in another project

Copy the entire `.agents/skills/moka-pot/` folder into the same location in your target project. Keep its `agents/` and `references/` subfolders alongside `SKILL.md`.

Codex discovers repository skills under `.agents/skills/`. If the skill does not appear after copying it, restart Codex. See the [official OpenAI skills documentation](https://learn.chatgpt.com/docs/build-skills) for skill discovery and installation details.

## Getting started

```text
$moka-pot Help me establish my baseline.
```

Or include the equipment details you already know:

```text
$moka-pot I have a 3-cup aluminum Bialetti Moka Express, a gas stove,
a medium-roast coffee, and a Comandante C40 grinder. I have a scale,
timer, and thermometer. Help me record my current recipe and improve it.
```

The skill will ask for missing details, including grinder calibration, before suggesting numerical settings. It treats starting settings as provisional rather than claiming to know an optimal grind before you taste the coffee.

## How an experiment works

1. Record your baseline: water mass and starting temperature, coffee dose, grind, preparation, filter, heat schedule, stopping rule, beverage yield, and timing.
2. Brew and describe the taste, flow, and overall enjoyment.
3. Change one controllable input while keeping the others consistent.
4. Compare the result with your preferred recipe. Keep a promising change as a candidate, reject a worse one, or repeat an inconclusive trial.
5. Confirm improvements with another brew before moving to a different variable.

Brew time and beverage yield are measured outcomes. For example, changing grind may change both; the skill will record those effects rather than also changing heat or water to force the previous timing.

There is no fixed number of experiments. Stop when you enjoy the result.

## Brew journals and memory

At the start of each brewing session, choose:

- **Local journal:** Save equipment profiles, coffee runs, recipes, trials, and next steps under `brew-journal/moka-pot/` in the active project. Confirm the current setup and beans when resuming.
- **Chat only:** Track results in the conversation and request a portable summary to paste into a future chat. No journal files are written in this mode.

Local journals are created only after you choose that mode. They live outside the reusable skill folder. To keep personal brew records out of Git commits, add `/brew-journal/` to your project's `.gitignore`.

## Sources

The brewing guidance draws on user-supplied transcripts of:

- James Hoffmann: [The Ultimate Moka Pot Technique (Episode #3)](https://www.youtube.com/watch?v=BfDLoIvb0w4).
- Lance Hedrick: [The Moka Pot, But Actually Good](https://www.youtube.com/watch?v=wmvEInIdD8U).

Both emphasize repeatable preparation and controlled flow. They differ on starting water temperature and grind. The skill preserves those differences as alternatives to test rather than presenting either method as universally best.

See the [source analysis](.agents/skills/moka-pot/references/source-analysis.md) for the comparison and its limits. Follow your pot manufacturer's instructions for filling, assembly, heat compatibility, and handling.

## Skill files

- [SKILL.md](.agents/skills/moka-pot/SKILL.md): Coaching workflow and skill entry point.
- [openai.yaml](.agents/skills/moka-pot/agents/openai.yaml): Display information and invocation policy.
- [Source analysis](.agents/skills/moka-pot/references/source-analysis.md): Shared principles and differences between the two transcripts.
- [Experiments and journals](.agents/skills/moka-pot/references/experiments-and-journal.md): Measurement definitions, taste diagnosis, trial decisions, and memory handling.
