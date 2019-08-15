# Magic
MagicSpells configuration for server

ORGANISATIONAL TASKS:
- Standardise spell descriptions.  e.g.
    - (Colour code)Spellname: Lv(memory) spell
    - Descriptive text
    - [Requires (prerequisites)]
- Standardise spell layouts:
    - spell-class
    - cast-item
    - spell-icon
    - casting costs (cost, cast-time, cooldown)
    - learning requirements (prerequisites, precludes, replaces, and memory)
    - spell-specific configuration (range, damage, etc)
    - modifiers
    - description and other strings
    - effects (particles, sound effects, etc)
- Most vital strings to write:
    - Descriptions
    - str-cost
    - str-modifier-failed (if spell has require/denied modifiers)

DESIGN TASKS:
- Technology tree
    - Novice level spells have a memory cost of 3 or less, have no MagicXP requirements, and can be cast with a stick.
    - Apprentice level spells have a memory cost of 4-7, have a Novice MagicXP requirement of 1000x the memory cost, and can be cast with either specific cast items or a stick.
    - Master level spells have a memory cost of 7 and up, have requirements of Apprentice MagicXP 1000x the memory cost PLUS Novice MagicXP 10,000x the memory cost.
    - Cast item creation spells are Apprentice level, must be cast with a grimoire, and are not bindable.
    - Grimoires should be thematic with appropriate item creation spells tied to them
- Spell effects
    - Visual and sound effects are a great way to make spells characterful and "feel" magical.  If a spell doesn't have any built-in and obvious effects (like a fireball or particle projectile spell) it should have some effects.
    - Spell effects should give some hint as to the school they come from
    - Even simple spells like eating or item creation benefit from spell effects
    - You can accompany spell effects with str-cast-self, str-cast-target, or str-cast-others, but often these will not be necessary

