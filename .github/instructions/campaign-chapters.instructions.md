---
name: Campaign Chapter Guidelines
description: Guidelines for authoring campaign chapter files.
applyTo: '**/Campaign/**.md'
---

# Campaign Authoring Guide

A campaign chapter file is a playable, scene-by-scene document that a Dungeon Master reads and adapts at the table. It should read like a story while also giving the Dungeon Master clear prompts for narration, roleplay, and encounters. Write it to be scannable, warm, and consistent with the rest of the campaign.

## Key Guidelines

- [Campaign Overview]: Always cross-check names, places, items, ships, and mechanics against the campaign overview. It contains the authoritative information about the campaign's world and characters. It also serves as the single source of truth for all campaign-related details, namely any unique rules or mechanics. If a name or detail is not in campaign overview, do not invent one.
- Continuity: You may reference earlier chapters for consistency (things already established and settled). Do not rely on later chapters for details or information because chapters are developed in order, so later chapters are likely unfinished. If a later development is needed, leave a clear note rather than asserting a fact.

## Prologue

The prologue is a special chapter that introduces the campaign and sets the stage for the story. The prologue is optional, but recommended.

* The prologue should contain the campaign title followed by `(Prologue)`
* The prologue should be short and concise, providing just enough information to set the stage for the campaign. It should not contain any major plot points or spoilers for later chapters.
* The prologue should limit the usage of exploration hubs, branching choices, and battles. Those mechanics are better suited for the first chapter of the campaign, which is where the players should be introduced to these concepts.
* Battle sections found in a prologue should be narrative-driven and not an actual encounter with consequences.

## Structure & Hierarchy

The chapter file is a structured document with a clear hierarchy of headings. Use headings to indicate the structural role of each section. The hierarchy is important for both readability and for any future tooling that may parse the chapter files.

1. Title (H1): Provides the chapter title.
  - A chapter uses a numbered form, which can be either a simple number or a decimal number for chapters that are broken apart into smaller parts.
  - The Prologue is special and is referenced as 0.0, but should not be included in the chapter title; The prologue should contain the campaign title followed by `(Prologue)`.

2. Main sections (H2): Each main section of a chapter acts as a different scene and may contain sub sections. These are the only sections that get separated by horizontal rules.
  - Place a horizontal rule (`---` on its own line) between each pair of consecutive main sections.
  - Do not put a horizontal rule after the title, and do not place one between other sub sections (H3+) because those sub sections are part of a main section.

3. Sub sections (H3+): Each subsection belongs to a main section or another sub section. Use subsections to organize the main section: exploration options, roleplay prompts, branching choices, and battle scenarios.

```md
# Chapter {Chapter Number}: {Chapter Title}

## {Main Section (Scene 1)}

{Main Section Content: Narration, Roleplay, Dungeon Master Notes, Combat, etc.}

### {Sub Section}

{Sub Section Content: Narration, Roleplay, Dungeon Master Notes, Combat, etc.}

#### {Sub Section}

{Sub Section Content: Narration, Roleplay, Dungeon Master Notes, Combat, etc.}

---

## {Main Section (Scene 2)}

{Main Section Content: Narration, Roleplay, Dungeon Master Notes, Combat, etc.}

...
```

## Section Types

Use the proper heading level for each section type. Each section type has a specific purpose and should be used consistently throughout the chapter. Use the proper emojis to indicate the type of section. Reference the [Emojis] section for a complete list of emojis and their meanings.

### General Sections

A general section is a main section that is not a part of a scene, but simply provides general information about the chapter. The typical body content of a general section is Dungeon Master notes, but it is not required. This is an optional section that can be used to provide context or background information for the chapter, and if it is used, it should be the first main section of the chapter.

### Story Section

A story section has a meaningful name in its heading. The body content of a story section should contain narrative content that is relevant to the story and should be written in a way that is easy for the Dungeon Master to read and understand.

### Battle Section

A battle section contains the name of the battle and any additional information in its heading. The body content contains information about the battle, including monster (or group), environmental hazards, win conditions, etc. The battle section name does not have to match up to the monster name in the body content.

### Exploration Hub Section

An exploration hub section contains a meaningful name in its heading and provides the Dungeon Master with guidance on how to handle player exploration and interaction with the environment. The body content of an exploration section contains a list of locations that the party can explore, as well as any relevant information about the environment, such as hazards, traps, or hidden items. The different areas within the exploration location should each be presented as a subsection with a consistent naming pattern. The body content of each area should be concise to avoid confusion, but may contain narrative consequences, battles, unique dialogues, etc.

### Branching Choice Section

A branching choice section is a set of unique subsections which present the Dungeon Master with guidance on how to handle player choices that affect the campaign. Each branching choice should be presented as a subsection with a consistent naming pattern. The outcome of each choice should be clearly stated, including any narrative consequences, battles, or other effects. Try to avoid having too many nested choices, as this can make the chapter difficult to read and follow. Instead, consider breaking the chapter into multiple parts if there are too many branching choices.

* `### ❓ Branching Choice 1: {Choice Description}`
* `### ❓ Branching Choice 2: {Choice Description}`

The body content of each branching choice should be concise to avoid confusion, but may contain narrative consequences, battles, unique dialogues, etc.

### Battle Content

The battle content is part of the body content of a battle section. It should contain the monster (or group of monsters). If it is a group of monsters with more than one instance of an monster, use letter markers to distinguish them apart. Each monster should be a reference link to an entry in the [Monsters Guide] for that chapter.

Random battles can contain multiple variations of battle content to select from. The variations should be in a list. Additional information (Dungeon Master Notes, Environmental Hazards, Win Conditions, etc.) should specify which variation they are applicable towards.

Utilize the proper [Emojis] to distinguish a monster from a legendary monster.

Example:
```md
🐉 [Minion 1] (A), 🐉 [Minion 1] (B), 🐉 [Minion 1] (C), 👹 [Mini-Boss]

> 📜 The party is only required to defeat the **Mini-Boss** and not any of the **Minion** enemies.
>
> 🌴 There is a poisonous cloud surrounding the **Mini-Boss** in a 10 foot radius. Entering this area inflicts you with **1d6 Poison Damage**.
```

### Narrative Voice Content

The narrative voice content is part of the body content of a section. It should follow a second person, present tense perspective, and should be written in a way that is easy for the Dungeon Master to read and understand. The narrative voice should also be consistent with the tone and style of the campaign.

Example:
```md
You step into the darkened chamber, the air thick with the scent of decay. The flickering torchlight casts eerie shadows on the walls, and you can hear the distant sound of dripping water echoing through the cavern.
```

### Character Speech Content

The character speech content is part of the body content of a section. The dialogue should match the tone and style of the character. It is formatted in a manner that distinguishes it from narrative text using italics and quotation marks.

Example:
```md
The old man looked at you with a twinkle in his eye and a mischievous grin. *"I wasn't sure that would work!"* he exclaimed, shaking his head in disbelief.
```

### Exploration Hubs/Locations Content

The exploration hubs (locations) content is part of the body content of a section. It should provide the Dungeon Master with clear guidance on how to handle player exploration and interaction with the environment. The exploration location should be structured in a way that allows the Dungeon Master to easily reference and navigate the different areas within the location. The exploration location should also include any relevant information about the environment, such as hazards, traps, or hidden items. The different areas within the exploration location should each be presented as a subsection with a consistent naming pattern. The body content of each area should be concise to avoid confusion, but may contain narrative consequences, battles, unique dialogues, etc.

Example:
```md
## 🗺️ Exploring The Lost City

> 📜 Having discovered a map of the lost city, the party can choose to explore each of the areas.

* **Golden Temple**
* **Council Chambers**
* **River Bridge**

### 📍 Golden Temple

...

### 📍 Council Chambers

...

### 📍 River Bridge

...
```

### Dungeon Master Notes Content

The Dungeon Master notes content is part of the body content of a section. They contain out-of-play guidance for the Dungeon Master, such as rules, mechanics, hidden logic, and reminders. Dungeon Master notes may also contain tips for the dungeon master.

Example:
```md
> 📜 The party has a limited amount of time to complete this section before the the chamber door closes. If they take too long, the consequences will be severe.
>
> 💡 To avoid an total party kill (TPK), consider accepting unique solutions to the puzzle. Adjust the difficulty and time limit based on the party's experience level (novice vs expert).
```

### Environmental Effects Content

Environmental effects content is part of the body content of a section. It contains information about the environment that may affect the party's actions, such as weather, terrain, and other environmental hazards. Environmental effects may also contain information about how the environment affects the party's abilities, such as movement speed, visibility, and other factors.

Example:
```md
> 📜 The chamber ahead contains numerous traps the players can avoid.
>
> 🌴 When a player pulls the wrong lever, a trap is triggered and they must make a DC 13 dexterity saving throw. On success, they leap out of the way before a blade emerges from the wall. On failure, they take 2D6 + 4 slashing damage.
> ...
```

## Consistency Checklist

Use this checklist to ensure that a campaign chapter file is complete and consistent:

- [ ] Title: Included at the top of the file and adheres to the expected format.
- [ ] Main Section(s): Each main section is a meaningful scene with a clear heading and body content.
- [ ] Sub Section(s): Each sub section is a meaningful part of a main section with a clear heading and body content.
- [ ] Body Content(s): Each main or sub section contains meaningful body content that is relevant to the section's purpose.
- [ ] Formatting: all headings and body conttent are formatted correctly and consistently with the rest of the campaign. Emojis are used properly.
- [ ] Consistency: All body content is verified against the [Campaign Overview] and previous chapters for consistency and accuracy.
- [ ] Horizontal Rule: Each main section is separated by a horizontal rule (`---`); no sub sections are separated by horizontal rules.

[Campaign Overview]: </1.0 - Overview.md>
[Monsters Guide]: </2.0 - Monsters.md>
[Emojis]: </.github/instructions/campaign.instructions.md#emojis>
