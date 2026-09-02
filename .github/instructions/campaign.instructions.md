---
name: Campaign Guidelines
description: Guidelines for authoring any campaign-related markdown files.
applyTo: '**/*.md'
---

# Campaign Guidelines

The campaign guidelines are the rules that apply to all campaign related files. These rules ensure that the campaign is consistent, readable, and playable. They contain the style, formatting, and structural rules that apply to all campaign files, including the overview, monsters, players guide, and campaign chapters.

## Style & Formatting Conventions

- Readability: Campaign files should be written primarily to be human readable in both markdown format and in the rendered markdown file.
- Entities: Ensure that **bold** is used for entities: names, locations, key items.
- Flavoring: Ensure that *italics* is used for flavor.
- Bulleted Lists: Use `*` as the bullet marker.

## File References

Ensure that all campaign files that reference other campaign files to use reference style links available in markdown. For example, if a campaign chapter references the campaign overview file, it should use the following syntax:

```md

This is a sample reference to [Campaign Overview].

...

[Campaign Overview]: </path/to/1.0 - Overview.md>
```
