# FIFA World Cup 2026 · Local Time Guide ⚽🌍

Single-file HTML app showing all 104 FIFA World Cup 2026 matches in **your local timezone** — auto-detected from your browser. Also includes a **Squads tab** with player rosters, club info, and coach details for each team.

## Features

- **All 104 matches** — complete group stage (72) + Round of 32 → Final
- **Auto timezone detection** — kickoff times converted to your local timezone via browser's `Intl` API
- **Manual timezone override** — type any IANA timezone (e.g. `Asia/Tokyo`, `Europe/London`) to switch
- **Favorable window filter** — default 5:00 AM–10:00 PM, fully editable and saved in localStorage
- **Favorite teams** — pick your teams, filter to their matches, highlighted in gold
- **Color coding** — green cards = good time, red = late night/early morning
- **Group/round filter** — browse by group (A–L) or knockout round
- **Squads tab** — group accordion (A–L), click any team to see coach + player roster with clubs
- **Squad modal** — click any team name on a match card to view their squad inline
- **Wikipedia links** — player and coach names link to their Wikipedia pages
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
- Share with friends — just send the `index.html` file

## Timezone Support

Uses the browser's built-in `Intl.DateTimeFormat` API — works for every timezone worldwide, handles DST automatically.

```
Auto-detected:  Intl.DateTimeFormat().resolvedOptions().timeZone
Override:       type any IANA name → e.g. "Asia/Kathmandu", "America/Sao_Paulo"
Persisted:      localStorage key wc26_tz
```

## Squad Data Status

Squad data sourced from [Wikipedia — 2026 FIFA World Cup squads](https://en.wikipedia.org/wiki/2026_FIFA_World_Cup_squads).

> **Note:** Jersey numbers (1–26) are pending FIFA official squad submission deadline **June 2, 2026**.
> When adding a new squad to `SQUADS` in `index.html`, update the table below and mark it accordingly.

| Team | Group | Status | Notes |
|------|-------|--------|-------|
| **Mexico** | A | 🟡 Provisional | Trimmed to 26 from provisional list. Update after June 2. |
| **South Korea** | A | ✅ Confirmed | Announced May 16 2026. |
| **South Africa** | A | 🟡 Provisional | 32-man preliminary squad added. Coach: Hugo Broos (Belgium). |
| **Czechia** | A | ✅ Confirmed | Announced May 2026. |
| **Canada** | B | ⬜ TBD | Announcing May 29. |
| **Switzerland** | B | ✅ Confirmed | Full 26-player squad added. Coach: Murat Yakin. |
| **Qatar** | B | 🟡 Provisional | Partial data only — MF/FW rows missing from Wikipedia fetch. |
| **Bosnia & Herzegovina** | B | ✅ Confirmed | First team to announce (May 11 2026). |
| **Brazil** | C | ✅ Confirmed | Announced May 18 2026. Full 26-player squad added. Coach: Carlo Ancelotti (Italy). |
| **Morocco** | C | ⬜ TBD | Announcing May 26. Coach: Mohamed Ouahbi. |
| **Haiti** | C | ✅ Confirmed | Full 26-player squad added. Coach: Sébastien Migné (France). |
| **Scotland** | C | ✅ Confirmed | Announced May 19 2026. Full 26-player squad added. Coach: Steve Clarke. |
| **USA** | D | ⬜ TBD | Announcing May 26. Coach: Mauricio Pochettino. |
| **Paraguay** | D | 🟡 Provisional | Large preliminary squad added. Coach: Gustavo Alfaro (Argentina). |
| **Australia** | D | ⬜ TBD | Announcing June 1. |
| **Turkey** | D | 🟡 Provisional | 33-man provisional squad added. Coach: Vincenzo Montella (Italy). |
| **Germany** | E | ✅ Confirmed | Announced May 21 2026. Full 26-player squad added. Coach: Julian Nagelsmann. |
| **Ecuador** | E | ⬜ TBD | Preliminary May 24, final June 1. |
| **Ivory Coast** | E | ✅ Confirmed | Announced May 15 2026. Full 26-player squad added. Coach: Emerse Faé. |
| **Curacao** | E | ✅ Confirmed | Full 26-player squad added. Coach: Dick Advocaat (Netherlands). |
| **Netherlands** | F | ⬜ TBD | Announcing May 27. |
| **Japan** | F | ✅ Confirmed | Announced May 15 2026. Full 26-player squad added. Coach: Hajime Moriyasu. |
| **Sweden** | F | ✅ Confirmed | Full 26-player squad added. Coach: Graham Potter (England). |
| **Tunisia** | F | ✅ Confirmed | Full 26-player squad added. Coach: Sabri Lamouchi (France). |
| **Belgium** | G | ✅ Confirmed | Announced May 15 2026. Full 26-player squad added. Coach: Rudi Garcia (France). |
| **Egypt** | G | 🟡 Provisional | Provisional squad added. Coach: Hossam Hassan. Includes Mohamed Salah, Omar Marmoush. |
| **Iran** | G | 🟡 Provisional | 30-man provisional squad added. Coach: Amir Ghalenoei. Includes Mehdi Taremi. |
| **New Zealand** | G | ✅ Confirmed | Announced May 14 2026. Full 26-player squad with jersey numbers added. Coach: Darren Bazeley (England). |
| **Spain** | H | ⬜ TBD | Announcing May 25. Coach: Luis de la Fuente. |
| **Uruguay** | H | ⬜ TBD | Coach: Marcelo Bielsa. Not yet announced. |
| **Saudi Arabia** | H | ⬜ TBD | 30-man preliminary announced May 23. Coach: Georgios Donis. Players TBD. |
| **Cape Verde** | H | ✅ Confirmed | Full 26-player squad added. Coach: Bubista (Portugal). |
| **France** | I | ✅ Confirmed | Announced May 14 2026. Full 26-player squad added. Coach: Didier Deschamps. |
| **Senegal** | I | 🟡 Provisional | 28-man squad announced May 21 2026. Coach: Pape Thiaw. Includes Mané, Salah. |
| **Norway** | I | ✅ Confirmed | Full 26-player squad added. Coach: Ståle Solbakken. Includes Haaland, Ødegaard. |
| **Iraq** | I | 🟡 Provisional | 34-man provisional squad added. Coach: Graham Arnold (Australia). |
| **Argentina** | J | 🟡 Provisional | 55-man preliminary squad added. Coach: Lionel Scaloni. Includes Messi. |
| **Austria** | J | ✅ Confirmed | Full 26-player squad added. Coach: Ralf Rangnick (Germany). Includes Alaba, Arnautović. |
| **Algeria** | J | ⬜ TBD | Announcing May 31. |
| **Jordan** | J | 🟡 Provisional | 30-man provisional squad added. Coach: Jamal Sellami (Morocco). |
| **Portugal** | K | ✅ Confirmed | Announced May 19 2026. Full 26-player squad added. Coach: Roberto Martínez (Spain). |
| **Colombia** | K | 🟡 Provisional | Large provisional squad added. Coach: Néstor Lorenzo (Argentina). Includes James, Luis Díaz. |
| **DR Congo** | K | ✅ Confirmed | Full 26-player squad added. Coach: Sébastien Desabre (France). Includes Wissa, Wan-Bissaka. |
| **Uzbekistan** | K | 🟡 Provisional | Large provisional squad added. Coach: Fabio Cannavaro (Italy). Includes Shomurodov, Khusanov. |
| **England** | L | ✅ Confirmed | Full 26-player squad added. Coach: Thomas Tuchel (Germany). Includes Kane, Bellingham, Saka. |
| **Croatia** | L | ✅ Confirmed | Full 26-player squad added. Coach: Zlatko Dalić. Includes Modrić, Kovačić, Gvardiol. |
| **Ghana** | L | ⬜ TBD | Coach: Carlos Queiroz. Not yet announced. |
| **Panama** | L | ⬜ TBD | Announcing May 26. |

### How to fetch updated squad data

The Wikipedia squads page is too large for a single fetch. Use the **Wikipedia section API** to get individual team data:

**Step 1 — get section index for a team:**
```
https://en.wikipedia.org/w/api.php?action=parse&page=2026_FIFA_World_Cup_squads&prop=sections&format=json
```
Returns all section indices. Each team has its own subsection index (e.g. Scotland = 15, Portugal = 54, Brazil = 12).

**Step 2 — fetch that team's wikitext:**
```
https://en.wikipedia.org/w/api.php?action=parse&page=2026_FIFA_World_Cup_squads&prop=wikitext&section=<INDEX>&format=json
```

Known section indices (may shift if Wikipedia adds/removes sections):

| Team | Index | Group |
|------|-------|-------|
| Czech Republic | ~9 | A |
| Mexico | ~10 | A |
| South Africa | ~11 | A |
| South Korea | ~12 | A |
| Bosnia & Herzegovina | ~13 | B |
| Canada | ~14 | B |
| Qatar | ~15 | B (ish) |
| Brazil | 12 | C |
| Scotland | 15 | C |
| Germany | 24 | E |
| Netherlands | 28 | E/F |
| USA | 20 | D |
| Argentina | 48 | J |
| Spain | 39 | H |
| France | 42 | I |
| Norway | 44 | I |
| Portugal | 54 | K |
| England | 58 | L |

> Re-fetch the sections index if results look wrong — indices shift when new squads are added.

### How to add a squad

1. Find the team in `const SQUADS = { ... }` in `index.html`
2. Replace `{ status:"tbd", coach:null, players:[] }` with full data:

```js
"TeamName": {
  status: "confirmed",  // or "provisional"
  coach: { name: "Full Name", country: "Country", wiki: "/wiki/Full_Name" },
  players: [
    { pos: "GK", name: "Player Name", club: "Club Name", cc: "Club Country", wiki: "/wiki/Player_Name" },
    // ...
  ]
},
```

3. Update the status table above (✅ / 🟡 / ⬜)
4. Source: [Wikipedia — 2026 FIFA World Cup squads](https://en.wikipedia.org/wiki/2026_FIFA_World_Cup_squads)

## Data Sources

- Match schedule: Sky Sports, Al Jazeera, worldcupwiki.com (official FIFA 2026 fixture list)
- Squad data: Wikipedia — 2026 FIFA World Cup squads
