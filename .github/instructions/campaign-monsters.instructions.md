---
name: Campaign Monsters
description: Guidelines for authoring a human-readable campaign monsters file.
applyTo: '**/2.0 - Monsters.md'
---

# Campaign Monsters Authoring Guide

The monsters guide is the human-readable bestiary for the campaign. It should let a Dungeon Master quickly find the correct creature statistics, understand where each version appears, and run the encounter directly from the document. Write it to be scannable, consistent, and faithful to the chapter-specific version being used.

## Structure

A monsters guide file should contain the following, in this order:

1. Title: The title of the campaign found in the [Overview] file, appended with `Monsters Guide`.
2. Reference: The reference includes an external link to the monster used as the base stats. The monster title and stats should be altered to create a variant that matches the campaign styling. Monsters can be unique and have no reference.
2. Description: A short paragraph explaining what the guide contains. This section needs no heading; it flows directly from the title.
3. Chapter Sections: Monster entries grouped by campaign chapter, in chapter order.
4. Monster Entries: Complete stat blocks using the same structure for every monster.
5. Horizontal Rule: Use the horizintal rule `---` to seperate Chapter Sections.

```md
# {Optional Emoji} {Title}: Monsters Guide

The monsters guide is a human-readable bestiary for the campaign. It contains all enemy stat blocks across the campaign, organized by chapter.

---

## 📖 {Chapter Number}: {Chapter Title}

### {Monster Emoji} {Monster Name} *({Monster Header Information})*

Reference: [{Base Monster}]({External Link})

{Monster Information}

---

## 📖 {Chapter Number}: {Chapter Title}

### {Monster Emoji} {Monster Name} *({Monster Header Information})*

{Monster Information}

### {Monster Emoji} {Monster Name} *({Monster Header Information})*

{Monster Information}

...
```

### Monster Structure

1. Name/Header: The monster emoji, name, and header information (size, type, subtype, alignment) are included in the heading. The monster can be a normal monster or a legendary monster identified by its emoji.
2. Description: A short paragraph describing the monster, its behavior, and any relevant lore.
3. Challenge Rating: The monster's challenge rating is included immediately below the heading.
4. Combat Statistics: The monster's combat statistics are included in a table.
5. Ability Scores: The monster's ability scores are included in a table.
6. General Statistics: The monster's general statistics are included in a table.
7. Traits/Actions: The monster's traits and actions are included in a list.

```md
## {Monster Emoji} {Monster Name} *({Size, Type, Subtype, Alignment})*

{Monster Reference}

{Monster Description}
{Challenge Rating}

{Combat Statistics Table}

{Ability Scores Table}

{General Statistics Table}

{Traits/Actions List}
```

### Monster Reference

Provide a name and link to the monster that was used as the base to the variant.

### Monster Description

Provide a short paragraph describing the monster, its behavior, and any relevant lore. The description should be concise and informative, providing context for the monster's role in the campaign.

### ☠️ Challenge Rating

The challenge rating is included immediately below the monster's heading. Provide the challenge rating, experience points, and proficiency bonus.

```md
☠️ **Challenge:** {Challenge Rating} ({Experience Points} XP; PB {Proficiency Bonus})
```

### 📊 Combat Statistics Table

The combat statistics table contains the monster's armor class, initiative, hit points, and speed. Use a four-column, headerless table. Align the raw Markdown columns with padding so the source remains human-readable.

```md
|                |                     |                |                     |
|:---------------|:--------------------|:---------------|:--------------------|
| 🛡️ Armor Class | {Armor Class Value} | ⏱️ Initiative | {Initiative Value}  |
| ❤️ Hit Points  | {Hit Points Value}  | 👟 Speed      | {Speed Value}       |
```

### 📊 Ability Scores Table

The ability scores table contains the monster's strength, dexterity, constitution, intelligence, wisdom, and charisma. Use an eight-column table. The first four columns contain strength, dexterity, and constitution; the last four contain intelligence, wisdom, and charisma. Leave the first and second header cells blank, and use `Mod` instead of `Modifier`. The modifier and save values can be positive (+), zero (+0), or negative (-). Align the raw Markdown columns with padding so the source remains human-readable.

```md
|        |     | Mod  | Save |         |     | Mod  | Save |
|:-------|----:|-----:|-----:|:--------|----:|-----:|-----:|
| 🏋️ STR | {N} | +{N} | +{N} | 🧠 INT | {N} | +{N} | +{N} |
| 🏃‍♂️ DEX | {N} | +{N} | +{N} | 🧘‍♂️ WIS | {N} | +{N} | +{N} |
| 🧬 CON | {N} | +{N} | +{N} | 🎭 CHA | {N} | +{N} | +{N} |
```

### 📊 General Statistics Table

The general statistics table contains the monster's skills, vulnerabilities, resistances, immunities, gear, senses, and languages. Use a headerless, aligned two-column table. Include every key in every monster entry, even when its value is not applicable. Use `(none)` for any missing or inapplicable value. Do not omit a row because a monster does not have that statistic.

```md
|                    |                                                         |
|:-------------------|:--------------------------------------------------------|
| 🤹 Skills          | (none) or {Skills}                                      |
| 💔 Vulnerabilities | (none) or {Vulnerabilities}                             |
| 🔰 Resistances     | (none) or {Resistances}                                 |
| 🚫 Immunities      | (none) or {Immunities}                                  |
| ⚒️ Gear            | (none) or {Gear}                                        |
| 👁️‍🗨️ Senses          | (none) or {Senses}                                      |
| 🗣️ Languages       | (none) or {Languages}                                   |
```

### Traits/Actions List

The traits and actions list contains the monster's traits, actions, legendary actions, bonus actions, and reactions in that order. Use list entries as key-value pairs. Prefix each key with the correct [Emoji] for the type of entry. Keep attack rolls, save DCs, ranges, damage, recharge limits, triggers, and responses in the value text:

```md
* ✨ **{Trait}:** {Trait Description}
* 🗡️ **{Action}:** {Melee Description}
* 👑 **{Legendary Action}:** {Legendary Action Description}
* ➕ **{Bonus Action}:** {Bonus Action Description}
* ⚡ **{Reaction}:** {Reaction Description}
```

#### ✨ Trait

Traits describe passive abilities, special rules, senses, resistances, or other effects that are always available or apply automatically. Include the trait name and a concise description. There is no required roll or special format unless the trait itself calls for an ability check, saving throw, attack roll, recharge, or usage limit.

#### 🗡️ Action

Actions describe what the monster can do on its turn. Include the action name, usage limit or recharge when applicable, range or area, attack roll or saving throw when applicable, and the result on a hit, failure, or success. Attack actions should include the attack type, attack bonus, reach or range, damage, and any conditions or additional effects.

#### 👑 Legendary Action

Legendary Actions must identify the action name, its cost in legendary action uses, and its recharge or available uses. Include the attack roll or saving throw, range or area, damage, conditions, and other effects when applicable. State the monster's total Legendary Action Uses before listing individual legendary actions.

#### ➕ Bonus Action

Bonus Actions describe abilities the monster can use as a Bonus Action. Include the action name, usage limit or recharge when applicable, range or area, required attack roll or saving throw, and the resulting effect. If no roll is required, state the effect directly.

#### ⚡ Reaction

Reactions must identify a **Trigger** and a **Response**. Include any required attack roll, ability check, or saving throw, along with the reaction's range, usage limit, recharge, and effect when applicable. A reaction that has no special roll should state the response directly.

## Additional Rules

* Keep separate entries for chapter-specific versions of a monster.
* Duplicate an entry when necessary to document a weaker, stronger, altered, or otherwise chapter-specific version.
* Do not consolidate variants merely to avoid duplication. The entry must reflect the statistics used in that chapter.
* Within each chapter, group related monsters together when practical.
* Keep every monster entry self-contained; do not rely on another entry for omitted statistics.

## Consistency Checklist

Use this checklist to ensure that the monsters guide is complete and consistent:

- [ ] Title: Included at the top of the file and adheres to the expected format.
- [ ] Referemce: Included immediately after the title; marked with `*(none)*` for unique monsters.
- [ ] Description: Included immediately after the reference.
- [ ] Chapters: The monsters are grouped by chapter in ascending order, with each chapter having its own subheading.
- [ ] Monsters: Each chapter contains the list of monsters as their own subheading.
- [ ] Monster Information: Each individual monster subheading and content adheres to structure specified.
- [ ] General Statistics: All required keys are present, using `(none)` where applicable.
- [ ] Additional Rules: All additional rules are followed.
- [ ] Traits/Actions: The list of traits, actions, bonus actions, reactions, and legendary actions are in one list and use the required [Emoji] to distinguish them apart.

[Emojis]: </.github/instructions/campaign.instructions.md#emojis>
