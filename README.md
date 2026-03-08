# D&D 5E Random Encounter Roller

## Explanation

In 1977 TSR published the first [Monster & Treasure Assortment book](https://en.wikipedia.org/wiki/Monster_%26_Treasure_Assortment) for level 1-3, they eventually published 4-6, and 7-9. These were simple tables designed to give the DM a quick and dirty encounter and treasure for the encounter. I used the heck out of these table through out the 1980. This provides similar fucntionality for a modern D&D 5E DM. Although designed specifically for the 2014 version of D&D, it should work just fine for the 2024 version as well. To see it in action go to https://carnifex.us. For anyone who wants copies of the tables I built, they are .md files in the data folder, so you can print them out and use them at your table without the need for a computer.

This is a browser-based tool for generating random monster encounters and treasure for D&D 5th Edition (2014 rules). Select a party level, roll a d100, and instantly see the encounter details and matching treasure assortment.

## Features

- **Levels 1–9** — 100 unique encounters and 100 treasure entries per level (1,800 total rows)
- **One-click rolling** — Roll button, Re-roll button, or press Space/Enter
- **Encounter details** — Monster name, CR, AC, HP, key attack, and adjusted XP
- **Treasure details** — Loot contents, magic item (highlighted), and total value
- **No installation required** — Single self-contained HTML file; works in any modern browser

## Usage

Open `encounter_roller.html` in any web browser. No server, no internet connection, and no dependencies required.

1. Select the party level from the dropdown (Level 1–Level 9)
2. Click **Roll Encounter (d100)** or press Space/Enter
3. View the encounter and treasure panels

### Web Deployment

To host the roller on a web server, rename `encounter_roller.html` to `index.html` and upload it to any static web host. No server-side configuration is needed.

## Data

The `data/` folder contains 18 Markdown tables — one encounter file and one treasure file per level:

```
data/
├── 1st Level Encounters.md
├── 1st Level Treasure Assortment.md
├── 2nd Level Encounters.md
├── 2nd Level Treasure Assortment.md
...
└── 9th Level Treasure Assortment.md
```

All encounter and treasure data is embedded directly into `encounter_roller.html` at build time. The Markdown source files are kept for reference and editing.

### Encounter Table Columns

| Column | Description |
|--------|-------------|
| `#` | d100 roll result (1–100) |
| `Name` | Encounter name |
| `Monsters (CR)` | Monster type(s) and Challenge Rating |
| `AC` | Armor Class |
| `HP` | Hit Points |
| `Key Attack` | Primary attack description |
| `Adj. XP` | Adjusted XP for the encounter |

### Treasure Table Columns

| Column | Description |
|--------|-------------|
| `#` | d100 roll result (1–100) |
| `Name` | Treasure name |
| `Contents` | Coins, gems, or other loot |
| `Magic Item` | Magic item (if any) |
| `Value` | Total monetary value |

## License

D&D 5th Edition content is © Wizards of the Coast. This tool is a fan project for personal use.
