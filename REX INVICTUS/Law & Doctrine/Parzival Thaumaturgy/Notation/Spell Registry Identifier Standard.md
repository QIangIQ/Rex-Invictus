---
tags:
  - rex-invictus/magic-system
  - rex-invictus/spell-notation
  - source/rex-invictus
aliases:
  - Spell ID Standard
  - Registry Tag
updated: 2026-11-16
---

**[[Spell Registry Identifier Standard]]** fixes how every working in the [[Spell Registry]] is named and tagged. A short tag in the note name lets a reader see a working's tier, affinity and handling grade from any link; a full attribute code in each note gives all six attributes.

---

## Hierarchical Placement

- [[Parzival Thaumaturgy]]
  - [[Spell Attribute Set]]
    - **Spell Registry Identifier Standard** (this note)

---

## Short tag

**Name (Tier-Affinity-Grade-Shorthand)**, for example `Magic Missile (1-P-L-MM)` or `Dream of the Blue Veil (7-C-M-DBV)`.

The note file carries this name. Each note also has the aliases "Tier Spell: Name" (for example "1st Tier Spell: Magic Missile"), the plain name and the tag on its own, so a search for any of them finds it. A colon cannot appear in a file name on Windows, so the "1st Tier Spell:" form is an alias and not the file name.

### Tier

The working's tier, 0 to 14, as in [[Caster Capacity and Tiers]].

### Affinity

| Code | Affinity | Code | Affinity |
|---|---|---|---|
| A | [[Abjuration]] | I | [[Illusion]] |
| C | [[Conjuration]] | N | [[Necromancy (School)\|Necromancy]] |
| D | [[Divination]] | T | [[Transmutation]] |
| E | [[Enchantment]] | P | [[Pure]] (raw force construct, no school lean) |
| V | [[Evocation]] | X | [[Composite]] (combination) |

A working is tagged P when its only output is magical force or a bare field construct (Magic Missile, Shield, Mage Armor, Wall of Force, Mage Hand, Magic Link), whatever school the source gave it. A divine affinity can follow after a slash where it matters, for example `/Ap` for an Apollonian working.

### Grade

The grade measures how hard a working is to run, from its energy against its tier and its handling.

**Score = clamp(0.5 × (T_E − T), −1, 3) + handling points**

| Grade | Score | Meaning |
|---|---|---|
| L (Low) | ≤ 0.5 | Basic; fits easily inside its quantum |
| M (Medium) | ≤ 1.5 | Over its curve or fragile |
| H (High) | ≤ 3.0 | Strongly over-curve or hard to hold |
| X (Extreme) | > 3.0 | Runs far past its tier; strategic or prohibited |

Handling points are listed in [[Parzival Energy Budget#Handling points]]. Fragility (the working ends if the caster or target is injured or intercepted) counts a full point, so Dream of the Blue Veil grades M on fragility alone, as its source description requires.

### Shorthand

Initials of the significant words, skipping of, the, and, with, from, to, via, or, a, an, on, in: Magic Missile → MM, Dream of the Blue Veil → DBV, Lance of Longinus → LL. A one-word name takes its first letter and the next two consonants: Fireball FRB, Shield SHL, Grease GRS, Alarm ALR. Shorthands are unique across the registry. When two collide, the later one (by source, tier, then name) adds its next letter or a number. Shorthands for the workings named in field doctrine are fixed first.

## Combination tags

A combination is named with its members' letters in the field's own style, for example `Magical Railcannon (SM-S-G-A-C)`. Its registry ID adds the composite prefix and the highest member tier: `X-2-SM-S-G-A-C`. See [[Combat Combination Analysis]].

## Attribute code

The long form lists all six attributes in glyph order: **Tier·School·Damage·Area·Range·Duration**, for example `3·Evo·Fire·sphere (20)·150 feet·Instantaneous`. It is stored in each note's frontmatter as `attribute_code`, next to `registry_id`, `incantation`, `pz_total`, `t_e` and `grade`, so the vault can be queried by any field.

## Browsing

Every note links to its tier page, its school page and its function and element families. See [[Spell Families]].

---

## Related

[[Spell Registry]] · [[Spell Families]] · [[Spell Attribute Set]] · [[Parzival Energy Budget]]
