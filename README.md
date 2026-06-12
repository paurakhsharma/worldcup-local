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

> **Note:** All 48 squads confirmed as of June 8 2026. Post-deadline injury replacements applied for Czechia, South Korea, Bosnia & Herzegovina, Egypt, Scotland, Ivory Coast, Sweden, Germany, Austria, Jordan, Argentina, and Iraq (source: Wikipedia).
> When updating a squad in `SQUADS` in `index.html`, update the table below accordingly.

| Team | Group | Status | Notes |
|------|-------|--------|-------|
| **Mexico** | A | ✅ Confirmed | Announced May 31 2026. Full 26-player squad. Coach: Javier Aguirre. |
| **South Korea** | A | ✅ Confirmed | Announced May 16 2026. Coach: Hong Myung-bo. Cho Wi-je & Lee Gi-hyuk in for Cho Yu-min & Lee Ki-hyuk (June 2026). |
| **South Africa** | A | ✅ Confirmed | Announced May 27 2026. Full 26-player squad. Coach: Hugo Broos (Belgium). |
| **Czechia** | A | ✅ Confirmed | Full 26-player squad. Coach: Miroslav Koubek. Updated June 2026 (post-deadline changes). |
| **Canada** | B | ✅ Confirmed | Full squad added. Coach: Jesse Marsch (USA). Includes Alphonso Davies, Jonathan David. |
| **Switzerland** | B | ✅ Confirmed | Full 26-player squad added. Coach: Murat Yakin. |
| **Qatar** | B | ✅ Confirmed | Announced June 1 2026. Full 26-player squad. Coach: Julen Lopetegui (Spain). |
| **Bosnia & Herzegovina** | B | ✅ Confirmed | First team to announce (May 11 2026). Coach: Sergej Barbarez. Mladen Jurkas & Ermin Mahmić in for Osman Hadžikić (June 2026). |
| **Brazil** | C | ✅ Confirmed | Announced May 18 2026. Full 26-player squad. Coach: Carlo Ancelotti (Italy). |
| **Morocco** | C | ✅ Confirmed | Full 26-player squad added. Coach: Mohamed Ouahbi. Includes Hakimi, Bounou, Brahim Díaz. |
| **Haiti** | C | ✅ Confirmed | Full 26-player squad added. Coach: Sébastien Migné (France). |
| **Scotland** | C | ✅ Confirmed | Announced May 19 2026. Coach: Steve Clarke. Tyler Fletcher replaced Billy Gilmour (May 31 2026). |
| **USA** | D | ✅ Confirmed | Full 26-player squad added. Coach: Mauricio Pochettino (Argentina). Includes Pulisic, McKennie. |
| **Paraguay** | D | ✅ Confirmed | Announced June 1 2026. Full 26-player squad. Coach: Gustavo Alfaro (Argentina). |
| **Australia** | D | ✅ Confirmed | Full 26-player squad added. Coach: Tony Popovic. Includes Mathew Ryan, Leckie. |
| **Turkey** | D | ✅ Confirmed | Announced June 2 2026. Full 26-player squad. Coach: Vincenzo Montella (Italy). Includes Arda Güler, Çalhanoğlu. |
| **Germany** | E | ✅ Confirmed | Announced May 21 2026. Full 26-player squad. Coach: Julian Nagelsmann. Assan Ouédraogo replaced Lennart Karl (June 2026). |
| **Ecuador** | E | ✅ Confirmed | Full 26-player squad added. Coach: Sebastián Beccacece (Argentina). Includes Moisés Caicedo, Kendry Páez. |
| **Ivory Coast** | E | ✅ Confirmed | Announced May 15 2026. Full 26-player squad. Coach: Emerse Faé. Christopher Opéri replaced Clément Akpa (May 29 2026). |
| **Curacao** | E | ✅ Confirmed | Full 26-player squad added. Coach: Dick Advocaat (Netherlands). |
| **Netherlands** | F | ✅ Confirmed | Full 26-player squad added. Coach: Ronald Koeman. Includes Van Dijk, De Jong, Gakpo. |
| **Japan** | F | ✅ Confirmed | Announced May 15 2026. Full 26-player squad. Coach: Hajime Moriyasu. |
| **Sweden** | F | ✅ Confirmed | Full 26-player squad. Coach: Graham Potter (England). Herman Johansson replaced Emil Holm (June 2026). |
| **Tunisia** | F | ✅ Confirmed | Full 26-player squad added. Coach: Sabri Lamouchi (France). |
| **Belgium** | G | ✅ Confirmed | Announced May 15 2026. Full 26-player squad. Coach: Rudi Garcia (France). |
| **Egypt** | G | ✅ Confirmed | Announced May 30 2026. Full 26-player squad. Coach: Hossam Hassan. Includes Salah, Marmoush. Mohamed Alaa added (June 2026). |
| **Iran** | G | ✅ Confirmed | Announced June 1 2026. Full 26-player squad. Coach: Amir Ghalenoei. Includes Taremi. |
| **New Zealand** | G | ✅ Confirmed | Announced May 14 2026. Full 26-player squad. Coach: Darren Bazeley (England). |
| **Spain** | H | ✅ Confirmed | Announced May 25 2026. Full 26-player squad. Coach: Luis de la Fuente. |
| **Uruguay** | H | ✅ Confirmed | Full 26-player squad added. Coach: Marcelo Bielsa (Argentina). Includes Valverde, Darwin Núñez. |
| **Saudi Arabia** | H | ✅ Confirmed | Full 26-player squad added. Coach: Georgios Donis (Greece). Includes Salem Al-Dawsari. |
| **Cape Verde** | H | ✅ Confirmed | Full 26-player squad added. Coach: Bubista (Portugal). |
| **France** | I | ✅ Confirmed | Announced May 14 2026. Full 26-player squad. Coach: Didier Deschamps. |
| **Senegal** | I | ✅ Confirmed | Announced June 1 2026. Full 26-player squad. Coach: Pape Thiaw. Includes Mané, Jackson. |
| **Norway** | I | ✅ Confirmed | Full 26-player squad added. Coach: Ståle Solbakken. Includes Haaland, Ødegaard. |
| **Iraq** | I | ✅ Confirmed | Announced June 1 2026. Full 26-player squad. Coach: Graham Arnold (Australia). Ahmed Maknzi replaced Ahmed Yahya (June 2026). |
| **Argentina** | J | ✅ Confirmed | Announced May 28 2026. Full 26-player squad. Coach: Lionel Scaloni. Marcos Senesi in for Leonardo Balerdi (June 11 2026). |
| **Austria** | J | ✅ Confirmed | 25-player squad. Coach: Ralf Rangnick (Germany). Christoph Baumgartner withdrawn (June 2026). |
| **Algeria** | J | ✅ Confirmed | Full 26-player squad added. Coach: Vladimir Petković (Switzerland). Includes Mahrez, Gouiri. |
| **Jordan** | J | ✅ Confirmed | Announced June 2 2026. 25-player squad. Coach: Jamal Sellami (Morocco). Ibrahim Sabra withdrawn (June 2026). |
| **Portugal** | K | ✅ Confirmed | Announced May 19 2026. Full 26-player squad. Coach: Roberto Martínez (Spain). |
| **Colombia** | K | ✅ Confirmed | Announced May 25 2026. Full 26-player squad. Coach: Néstor Lorenzo (Argentina). Includes James, Luis Díaz. |
| **DR Congo** | K | ✅ Confirmed | Full 26-player squad added. Coach: Sébastien Desabre (France). Includes Wissa, Wan-Bissaka. |
| **Uzbekistan** | K | ✅ Confirmed | Announced June 2 2026. Full 26-player squad. Coach: Fabio Cannavaro (Italy). Includes Shomurodov, Khusanov. |
| **England** | L | ✅ Confirmed | Full 26-player squad added. Coach: Thomas Tuchel (Germany). Includes Kane, Bellingham, Saka. |
| **Croatia** | L | ✅ Confirmed | Full 26-player squad added. Coach: Zlatko Dalić. Includes Modrić, Kovačić, Gvardiol. |
| **Ghana** | L | ✅ Confirmed | Full 26-player squad added. Coach: Carlos Queiroz (Portugal). Includes Partey, Inaki Williams. |
| **Panama** | L | ✅ Confirmed | Full 26-player squad added. Coach: Thomas Christiansen (Spain). |

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

Known section indices (re-fetched June 8 2026 — may shift if Wikipedia adds/removes sections):

| Team | Index | Group |
|------|-------|-------|
| Czech Republic | 2 | A |
| Mexico | 3 | A |
| South Africa | 4 | A |
| South Korea | 5 | A |
| Bosnia & Herzegovina | 7 | B |
| Canada | 8 | B |
| Qatar | 9 | B |
| Switzerland | 10 | B |
| Brazil | 12 | C |
| Scotland | 15 | C |
| USA | 20 | D |
| Germany | 24 | E |
| Ivory Coast | 25 | E |
| Netherlands | 28 | F |
| Sweden | 29 | F |
| Egypt | 33 | G |
| Spain | 39 | H |
| France | 42 | I |
| Norway | 44 | I |
| Argentina | 48 | J |
| Austria | 49 | J |
| Colombia | 52 | K |
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
