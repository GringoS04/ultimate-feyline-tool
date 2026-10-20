# The Ultimate Feyline Tool

A living map of the Feyline, the magic of **Earlsdale**, for tabletop sessions. It shows where the Feyline runs strong or weak at any moment of your campaign. It turns that into **SWADE** modifiers for arcane skill rolls and helps plan journeys across the Fourth Age map.

Part of the [Earlsdale Compendium](https://swift-icon-9d6.notion.site/The-Earlsdale-Compendium-97725bbd1dd146f6892b755038b1a29a) by Grímur Fjeldsted · [mapventures.com](https://mapventures.com)

## Running it

It's a single web page with no build step and no server code.

- **Locally:** open `index.html` in a browser. If the map does not appear, serve the folder instead, for example with `python3 -m http.server`, then open `http://localhost:8000`.
- **GitHub Pages:** go to Settings → Pages and deploy from the `main` branch, root folder.

## What it does

### The Feyline
Currents of light flow between the **hotspots**, the places the Feyline is drawn to. Each hotspot swells and fades over one to four hours, its glow drifts around its place, and streams swirl around the strongest ones. The colour follows the season, and the four seasonal Turning days bring a convergence where every hotspot gains strength.

### Levels and SWADE modifiers
| Level | Modifier | Share of the map |
|---|---|---|
| Faint | −2 | about 20% |
| Weak | −1 | about 40% |
| Steady | ±0 | about 25% |
| Strong | +1 | about 10% |
| Surging | +2 | about 5% |

- **Measure:** click anywhere on the map for a live reading, its trend over the last minute and the hotspots it draws from.
- **Strength map:** an overlay with contour lines where the level changes, plus a key.

### Glimpses
Short flares of stronger Feyline, mostly in weak areas. Each lasts one to three hours, and any place gets one about once a day. They are seeded by date, so everyone sees the same ones, and the panel shows active and upcoming glimpses.

### The Turning calendar
The tool dates everything in the Turning: 12 months of 30 days and five Turning days, 365 days in all.

First Thaw · Thawrise · Seedwake · Blossomveil · **The Long Sun** · Suncrest · Highflame · Goldfield · **Harvest's End** · Reapfall · Amberwane · Mistveil · **The Long Night** · Frosthold · Longnight · Ashdawn · **The Nameless Day**

- **Real time** maps onto the Turning with First Thaw on 20 March, and the year from 20 March 2026 is year 23 of the Fourth Age.
- **Campaign time** is set by the GM. Run it, pause it, or jump by an hour, eight hours or a day. The same moment always gives the same Feyline.

### Party and travel log
- **Place party:** a banner with the party's live reading and modifier.
- **Plan route:** click stops on the map. The log assumes travel from 08:00 to 16:00 each day, lists the Feyline level every two hours on the road, marks camps and glimpses, and summarises the journey. Click a row to move the party there and set the clock. Set the map scale with *Days to cross the map*.

### GM tools (Map setup)
- **Add hotspot:** place your own hotspots for your campaign.
- **Edit:** for any hotspot, change its name, type, description, season, power (Minor, Normal or Major), and whether it is active in this campaign.
- **Move hotspots:** drag them into place.
- **Copy hotspots:** export all hotspots as JSON.
- **Load your map:** try another map image.

### Sound
*Hear the tone* plays a drone whose chords change with the season. It brightens as the Feyline strengthens, and chimes ring out more often near glimpses and on Turning days.

## Notes

- Campaign time, the party, routes and GM edits are saved in the **browser only** (`localStorage`). They are not shared between devices or players.
- Fonts load from Google Fonts. Everything else is in `index.html` and `earlsdale-map.webp`.

## Credits

Idea, world, map and lore: Grímur Fjeldsted (Mapventures). Built with Claude.
