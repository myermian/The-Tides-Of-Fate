---
name: create-character
description: Creates a balanced, rules-accurate Dungeons & Dragons character sheet using standard character creation, while respecting any campaign-specific rules, homebrew mechanics, and sheet conventions in effect.
argument-hint: Create a character sheet (e.g. 'a level 5 tank' or 'a support healer'). Optional: name, level, role, party context, edition, save location.
user-invocable: true
---

# Character Creation

Create a balanced, rules-accurate Dungeons & Dragons character sheet. This skill serves any character built this way — a real player, a fill-in ally, or a test/playtest character — and is not limited to one table, setting, or edition.

The goal is a sheet that is (1) legal under the rules edition in use, (2) consistent with the table's campaign-specific rules and any homebrew mechanics, and (3) thematically coherent with the setting and party.

## When to Use

- The user asks to create, build, roll, or generate a character or character sheet.
- A player wants a coherent, ready-to-play build and does not want to do the math.
- Designing a fill-in or ally that fits the party and world.

Do not use this for NPC or monster stat blocks. Those are DM-authored content, not player character creation.

## Rules and Table Context

- Rules edition: default to the latest and most popular edition (D&D 5e, 2024 revision). Use a different edition only if the user requests it or the table context says so.
- Campaign rules: consult the table's campaign or overview files (if any exist in the workspace) for house rules, starting level, ability score method, HP rule (highest die vs average), and homebrew mechanics. Apply those rules when present; fall back to official rules when absent.
- Sheet conventions: match the format of existing character or companion sheets in the workspace when there are any (section names, structure). Otherwise use the template referenced below.
- If a rule is ambiguous or its exact text is unavailable, say so and apply the closest official ruling rather than inventing one.

## Character Creation Procedure

1. Gather intent. Determine (or ask about) the essentials before finalizing:
   - Role / playstyle: frontliner, ranged DPS, caster, control, support, healer, tank, utility.
   - Race/species or vibe preference, if any hard constraint.
   - Level: use the requested level, or the table's starting level; default to level 1 if neither is given.
   - Party context: what roles already exist, so the build fills a gap.
   - Name (or generate one fitting the setting).
   - Output location (see Where to Save).

   Use a clarifying question only if intent is genuinely unclear; otherwise proceed with sensible defaults and state your assumptions.

2. Choose race/species. Pick an official option for the edition in use that is thematically reasonable for the setting and does not break party balance. Note traits that affect ability scores, size, speed, senses, and languages.

3. Choose class and subclass. Select a single class and the subclass appropriate for the character's level that matches the desired role. Apply multiclassing only if the user asks or a table rule permits it; default to a single-class build for clarity and balance.

4. Ability scores. Use the table's agreed method if one is defined (point buy, standard array, or rolling); otherwise use the edition default. Show the final six scores (STR, DEX, CON, INT, WIS, CHA) with their modifiers.

5. Background. Choose an official background. Tie it lightly to the setting for flavor while keeping mechanics to the official background (feature, skills, starting gear).

6. Derive stats at the chosen level:
   - Armor Class (armor + DEX per rules, or natural/spell).
   - Hit Points using the class Hit Die + CON modifier per level, following the table's HP rule. State the formula.
   - Speed, Saving Throws (proficient saves + modifiers), Passive Perception, and the Proficiency Bonus for that level.
   - Skills: class + background + race selections, with modifiers.
   - Spell slots and known/prepared spells (for casters) at that level.
   - Class and subclass features in order of level.
   - Equipment: starting gear + sensible gear for the level.

7. Thematic and balance pass:
   - Add a short backstory hook that ties the character to the setting and party.
   - Check that the build fills a party gap rather than duplicating an existing member or ally.
   - Confirm the build is balanced at its level (no absurd power spike, no under-leveled build).
   - Include homebrew only when the table explicitly allows it; otherwise stick to official rules.

8. Write the sheet. Use the template at `#file:./assets/character-sheet-template.md` unless the table's existing sheets define a different format for user requested character creation. Fill every field; leave no required field blank. If the character creation was initiated for play testing, format the player file so it reads well for an AI Agent (yaml kvp based).

9. Validate against the checklist below, then report the sheet to the user with the file path and a 2-3 line summary of the build and its party role.

## Where to Save

- If the user names a location, use it.
- For a test/playtest character, save under the table's playtest/character folder if one exists.
- For a campaign or personal character, place it under a sensible characters folder, or confirm one with the user.
- Image: include the Image Placeholder section; reference a real image if one is provided.

## Validation Checklist

- [ ] Level matches the request or the table's starting level.
- [ ] Single, coherent class and subclass; multiclassing only if requested or permitted.
- [ ] All six ability scores present with modifiers, assigned sensibly.
- [ ] AC, HP (with formula), Speed, saves, Proficiency Bonus, and skills derived correctly for that level.
- [ ] Spell slots and spells correct if a caster.
- [ ] Background and race traits listed; equipment listed.
- [ ] Thematic hook present (setting/party).
- [ ] Build fills a party gap rather than duplicating an existing member or ally.
- [ ] Table house rules and homebrew applied only where permitted; ambiguous rules called out, not invented.
- [ ] No required field left blank; format matches the table's existing sheets or the template.

## Example Invocation

> "Create a level 5 character for the party — they need a solid frontline tank."

Build a level 5 Fighter (Battle Master or Chivalry) with high STR/CON and a defensive, controlling role that complements the rest of the party, a short setting-appropriate backstory, and write it to the confirmed location using the template.
