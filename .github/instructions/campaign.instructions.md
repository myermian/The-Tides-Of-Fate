---
name: Campaign Guidelines
description: Guidelines for authoring any campaign-related markdown files.
applyTo: '**/*.md'
---

# Campaign Guidelines

The campaign guidelines are the rules that apply to all campaign related files. These rules ensure that the campaign is consistent, readable, and playable. They contain the style, formatting, and structural rules that apply to all campaign files, including the overview, monsters, players guide, and campaign chapters.

## Style & Formatting Conventions

- Readability: Campaign files should be written primarily to be human readable in both markdown format and in the rendered markdown file.
- Headings: Each word in a heading is capitalized.
- Entities: Ensure that **bold** is used for entities: names, locations, key items.
- Flavoring: Ensure that *italics* is used for flavor.
- Bulleted Lists: Use `*` as the bullet marker.

## Emojis

Emojis act as visual markers that let the Dungeon Master (and any future tooling) quickly identify the type of section, action, or statistic. Use the following set consistently. Do not utilize any emojis that are not listed. The following table provides a reference for the emojis and their meanings:

| Emoji | Meaning          | Description                                       |
|:------|:-----------------|:--------------------------------------------------|
| `📖`  | Rule/Mechanic    | Campaign Rule & Mechanics                         |
| `💠`  | General          | General Information, Context, Background          |
| `💬`  | Narration        | Narrative Scenes, Dialogue, Roleplay              |
| `⚔️`  | Battle           | Encounters, Combat                                |
| `🗺️`  | Exploration      | Exploration Hub                                   |
| `📍`  | Locations        | Exploration Hub: Locations                        |
| `❓`  | Choice           | Branching Choices                                 |
| `📜`  | DM Notes         | Dungeon Master Guidance                           |
| `💡`  | Tips             | Dungeon Master Tips (Variations, Optional Flavor) |
| `👤`  | Character        | Character Entries                                 |
| `🐉`  | Bestiary         | Monster                                           |
| `👹`  | Legendary Beast  | Legendary Monster                                 |
| `🌴`  | Environment      | Environmental Effects                             |
| `🌟`  | Blessing         | Celestial Blessing                                |
| `📊`  | Statistics       | Stat-block: Key Statistics                        |
| `☠️`  | Challenge        | Stat-block: Challenge Rating                      |
| `🛡️`  | Armor Class      | Stat-block: Armor Class                           |
| `❤️`  | Hit Points       | Stat-block: Hit Points                            |
| `⏱️`  | Initiative       | Stat-block: Initiative                            |
| `👟`  | Speed            | Stat-block: Movement Speed                        |
| `🏋️`  | Strength         | Stat-block: Ability Score                         |
| `🏃‍♂️`  | Dexterity        | Stat-block: Ability Score                         |
| `🧬`  | Constitution     | Stat-block: Ability Score                         |
| `🧠`  | Intelligence     | Stat-block: Ability Score                         |
| `🧘‍♂️`  | Wisdom           | Stat-block: Ability Score                         |
| `🎭`  | Charisma         | Stat-block: Ability Score                         |
| `⚒️`  | Gear             | Stat-block: Equipment                             |
| `👁️‍🗨️`  | Senses           | Stat-block: Senses                                |
| `🗣️`  | Language         | Stat-block: Languages                             |
| `💔`  | Vulnerabilities  | Stat-block: Damage Vulnerabilities                |
| `🔰`  | Resistances      | Stat-block: Damage Resistances                    |
| `🚫`  | Immunities       | Stat-block: Damage Immunities                     |
| `✨`  | Trait            | Stat-block: Traits                                |
| `🤹`  | Skills           | Stat-block: Skills                                |
| `🗡️`  | Action           | Stat-block: Battle Information                    |
| `➕`  | Bonus Action     | Stat-block: Battle Information                    |
| `⚡`  | Reaction         | Stat-block: Battle Information                    |
| `👑`  | Legendary Action | Stat-block: Battle Information                    |

## File References

Ensure that all campaign files that reference other campaign files to use reference style links available in markdown. For example, if a campaign chapter references the campaign overview file, it should use the following syntax:

```md
This is a sample reference to [Campaign Overview].

This is a sample reference to [Guidance Section].

...

[Campaign Overview]: </path/to/1.0 - Overview.md>
[Guidance Section]: </path/to/1.0 - Overview.md#guidance-section>
```
