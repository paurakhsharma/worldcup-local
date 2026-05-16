# FIFA World Cup 2026 · Local Time Guide ⚽🌍

Single-file HTML app showing all 104 FIFA World Cup 2026 matches in **your local timezone** — auto-detected from your browser, with filters for favorable viewing hours, favorite teams, and more.

## Features

- **All 104 matches** — complete group stage (72) + Round of 32 → Final
- **Auto timezone detection** — kickoff times converted to your local timezone via browser's `Intl` API
- **Manual timezone override** — type any IANA timezone (e.g. `Asia/Tokyo`, `Europe/London`) to switch
- **Favorable window filter** — default 5:00 AM–10:00 PM, fully editable and saved in localStorage
- **Favorite teams** — pick your teams, filter to their matches, highlighted in gold
- **Color coding** — green cards = good time, red = late night/early morning
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

- Timezone auto-detected on load — shown in the header pill
- Click the pill or use the **Timezone (IANA)** input in controls to override
- Preferences (timezone, favorite teams, time window) saved per-browser via `localStorage`

## Timezone Support

Uses the browser's built-in `Intl.DateTimeFormat` API — works for every timezone worldwide, handles DST automatically.

```
Auto-detected:  Intl.DateTimeFormat().resolvedOptions().timeZone
Override:       type any IANA name → e.g. "Asia/Kathmandu", "America/Sao_Paulo"
Persisted:      localStorage key wc26_tz
```

## Data Sources

Match schedule sourced from Sky Sports, Al Jazeera, and worldcupwiki.com based on the official FIFA World Cup 2026 fixture list (updated February 2024 / December 2024 draw).
