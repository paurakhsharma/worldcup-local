# FIFA World Cup 2026 · Nepal Time Guide ⚽🇳🇵

Single-file HTML app showing all 104 FIFA World Cup 2026 matches in **Nepal Standard Time (UTC+5:45)** — with filters for favorable viewing hours, favorite teams, and more.

## Features

- **All 104 matches** — complete group stage (72) + Round of 32 → Final
- **Nepal Time** — every kickoff converted to NPT (UTC+5:45) automatically
- **Favorable window filter** — default 5:00 AM–10:00 PM, fully editable and saved in localStorage
- **Favorite teams** — pick your teams, filter to their matches, highlighted in gold
- **Color coding** — green cards = good time, red = late night
- **Group/round filter** — browse by group (A–L) or knockout round
- **Stats bar** — count of favorable matches, late-night matches, and your team's games
- **Fully offline** — no server, no framework, no build step

## Groups

| Group | Teams |
|-------|-------|
| A | Mexico, South Korea, South Africa, Czechia |
| B | Canada, Switzerland, Qatar, Bosnia & Herzegovina |
| C | Brazil, Morocco, Haiti, Scotland |
| D | USA, Paraguay, Australia, Turkey |
| E | Germany, Ecuador, Ivory Coast, Curacao |
| F | Netherlands, Japan, Sweden, Tunisia |
| G | Belgium, Egypt, Iran, New Zealand |
| H | Spain, Uruguay, Saudi Arabia, Cape Verde |
| I | France, Senegal, Norway, Iraq |
| J | Argentina, Austria, Algeria, Jordan |
| K | Portugal, Colombia, DR Congo, Uzbekistan |
| L | England, Croatia, Ghana, Panama |

## Tournament Dates

- **Group Stage:** June 11–28, 2026
- **Round of 32:** June 28–July 4
- **Round of 16:** July 4–7
- **Quarter-Finals:** July 9–12
- **Semi-Finals:** July 14–15
- **Third Place:** July 18
- **Final:** July 19, MetLife Stadium, New Jersey

## Usage

Open `index.html` in any browser. No installation needed.

To share with friends — just send the `index.html` file. Preferences (favorite teams, time window) are saved per-browser via `localStorage`.

## Time Zone Reference

Nepal is UTC+5:45. Many matches from North America kick off late at night in Nepal.

```
UTC 00:00  →  05:45 NPT  ✓ early morning
UTC 08:00  →  13:45 NPT  ✓ afternoon
UTC 14:00  →  19:45 NPT  ✓ evening
UTC 17:00  →  22:45 NPT  ✗ after 10 PM
UTC 20:00  →  01:45 NPT  ✗ past midnight
```

## Data Sources

Match schedule sourced from Sky Sports, Al Jazeera, and worldcupwiki.com based on the official FIFA World Cup 2026 fixture list (updated February 2024 / December 2024 draw).
