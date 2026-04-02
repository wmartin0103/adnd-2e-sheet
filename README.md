# ⚔️ Advanced Dungeons & Dragons 2nd Edition — Interactive Character Sheet

A lightweight, browser-based character sheet for AD&D 2nd Edition. No server required — just open `index.html` and play. Built to handle the math and lookups so you can focus on the adventure.

---

## Features

**Character Identity**
- Name, player, race, class, kit, alignment, and level tracking
- Multi-class and dual-class support
- Race and class selections drive automatic rule lookups

**Ability Scores**
- All six ability scores with full modifier breakdowns
- Exceptional Strength (percentile) for fighters
- Per-score detail cards showing every derived bonus (hit, damage, encumbrance, etc.)

**Combat**
- Auto-calculated THAC0 based on class and level
- Armor Class with base + Dexterity adjustment + equipped armor
- Hit point tracking with current / max / temporary HP
- Strength hit/damage adjustments and Dexterity missile adjustment shown at a glance
- Movement rate calculator
- **Combat Scenarios** — build multiple attack setups (weapon + modifiers) and compare THAC0-to-AC hit matrices in real time

**Weapons & Proficiencies**
- Weapon inventory with attack/damage/speed/range pre-filled from the weapons database
- Weapon proficiency tracker with slots used vs. available
- Non-weapon proficiency (NWP) tracker with ability check targets

**Spells**
- Wizard and Priest spell lists sourced from the PHB and *Tome of Magic*
- Memorized-spell tracking per level
- Searchable spell lookup with full descriptions

**Class Features**
- Thieving skills panel (auto-shown for Thieves/Bards) with percentage trackers
- Racial traits panel populated from race selection

**Equipment & Gear**
- Equipment list with quantity and weight
- Magic items inventory
- Encumbrance tracking

**Data & Persistence**
- Auto-saves to browser `localStorage` — your sheet is there when you come back
- **Export JSON** — download your full character as a portable `.json` file
- Extensive reference data bundled locally: races, classes, kits, weapons, armor, equipment, proficiencies, spells, magic items, and psionics

---

## Getting Started

```bash
git clone https://github.com/your-username/adnd-2e-sheet.git
```

Open `adnd-2e-sheet/index.html` in any modern browser. No build step, no dependencies, no internet connection required after the initial font load.

---

## Project Structure

```
adnd-2e-sheet/
├── index.html          # The entire app — HTML, CSS, and JS in one file
└── rules_data/
    ├── rules_data.js                       # Data loader
    ├── adnd2e_ability_scores.json
    ├── adnd2e_classes.json
    ├── adnd2e_classes_additional.json
    ├── adnd2e_races.json
    ├── adnd2e_races_additional.json
    ├── adnd2e_kits.json
    ├── adnd2e_combat.json
    ├── adnd2e_weapons_armor.json
    ├── adnd2e_weapons_additional.json
    ├── adnd2e_equipment.json
    ├── adnd2e_proficiencies.json
    ├── adnd2e_proficiencies_additional.json
    ├── adnd2e_spells_wizard.json
    ├── adnd2e_spells_wizard_additional.json
    ├── adnd2e_spells_priest.json
    ├── adnd2e_spells_tome_of_magic.json
    ├── adnd2e_magic_items.json
    ├── adnd2e_psionics.json
    └── adnd2e_index.json
```

---

## Browser Compatibility

Works in any modern browser (Chrome, Firefox, Safari, Edge). Uses standard Web APIs — no frameworks, no bundler.

---

## Contributing

Pull requests welcome. The `rules_data/` JSON files are designed to be easy to extend — add new entries following the existing structure and they'll appear automatically in the relevant dropdowns and lookups.

---

*This project is a fan-made tool for personal use. Advanced Dungeons & Dragons and related trademarks are the property of Wizards of the Coast.*
