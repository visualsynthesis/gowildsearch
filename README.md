# GoWild Flight Finder

A single-file web tool for Frontier Airlines GoWild pass holders to find flights, check schedules, and get answers to common questions — all without fighting Frontier's website.

**Live:** [visualsynthesis.github.io/gowildsearch](https://visualsynthesis.github.io/gowildsearch/)

## What It Does

GoWild Flight Finder helps you quickly browse Frontier destinations from any hub, filter by route type, check seasonal schedules, avoid blackout dates, and link directly to Frontier's booking page on the right date.

**The problem it solves:** Frontier's booking site doesn't make it easy to browse GoWild options. You can't easily see which routes fly on which days, when seasonal routes operate, or which dates are blacked out. This tool puts all of that in one place.

## Features

### Flight Search
- **100+ destinations** with route data for ATL, DEN, and MCO hubs
- **Clickable stat box filters** — tap Direct Routes, Domestic, International, or All + Connecting to filter results instantly
- **Connecting flight support** — see every Frontier destination reachable with a layover, clearly labeled with a "Connecting" badge
- **Direct route detection** with visual indicators for nonstop flights
- **Low-frequency route warnings** for routes that only fly 1-2x/week
- **Seasonal route awareness** — inactive routes are automatically hidden based on the month you're searching

### Date Modes
- **Exact Dates** — pick specific travel dates and link directly to Frontier's booking page
- **Flexible Dates** — opens a popup showing all dates in your GoWild booking window (1 day for domestic, 10 days for international) with direct links for each date
- **Day-of-week filtering** — for routes with known schedules (e.g., Saturday-only flights), the popup only shows dates the route actually operates

### Calendar & Blackout Dates
- **Visual calendar carousel** covering 2025, 2026, and early 2027
- **Blackout dates highlighted in red** so you never waste a search
- **Navigate months** to plan ahead

### Book Now Suggestions
- **Smart banner** suggesting destinations with upcoming non-blackout dates
- **Seasonal route awareness** — only suggests routes that are currently in season

### GoWild Help (FAQ Search)
- **137 curated Q&A entries** covering booking, bags, seats, pricing, policies, elite status, fleet info, seasonal schedules, travel hacks, airport guides, and insider tips
- **Fact-checked** — every entry audited for accuracy against official Frontier sources
- **GPT-like search experience** — type a question, press Enter, get a clean answer with related topics
- **Smart keyword matching** with stop-word filtering and weighted scoring (tags > question > answer)
- **Airport code detection** — searching "ATL destinations" correctly prioritizes ATL-specific answers
- **Suggestion chips** for common topics

### GoWild in 30 Seconds
- **Collapsible rules panel** in the header — click to see a quick summary of how the GoWild pass works, booking windows, blackout dates, and key gotchas

## Seasonal Data

The tool includes detailed seasonal schedule data for international routes:

**ATL** — 15 international destinations with flight days and seasonal windows (Nov–Apr winter, May–Aug summer)

**DEN** — 8 international destinations including the only Frontier route to Honolulu

**MCO** — 12 international destinations with the most year-round coverage

Routes with confirmed day-of-week data (Saturday-only, daily, etc.) filter the flex popup to only show valid days. Routes without confirmed days show all dates with a warning.

## Tech Stack

- **Single HTML file** — no build step, no dependencies, no server needed
- HTML + CSS + vanilla JavaScript (~1,600 lines)
- Google-inspired Material Design aesthetic
- Google Analytics (GA4) with custom event tracking
- Fully responsive
- Works offline once loaded

## How to Use

1. Open the tool in any web browser
2. Select your home airport
3. Choose Exact or Flexible date mode
4. Click **Find Flights**
5. Use the stat boxes to filter by Direct, Domestic, International, or All + Connecting
6. Click a destination card to go to Frontier's booking page
7. Use the help search bar to ask questions about GoWild

## Data Sources

- Route data compiled from Frontier Airlines public schedules and press releases
- Blackout dates from official GoWild terms and conditions
- FAQ answers researched from Frontier's website, support pages, press releases, and public travel resources
- Day-of-week schedules from flight tracking sites (confirmed routes only)

## Limitations

- **No live availability data** — Frontier doesn't offer a public API, so the tool links to their booking page where you check actual seat availability
- **Schedules may change** — Frontier adjusts routes and frequencies seasonally; some day-of-week data may become outdated
- **GoWild-specific** — this tool is designed for GoWild pass holders, not general Frontier booking

## Version History

- **v1.1.0 "The Timber Wolf"** — 137 fact-checked FAQ entries, clickable stat filters, connecting flights, airport code search, bug fixes
- **v1.0.0 "The Flamingo"** — Initial release with flight search, flex dates, calendar, and 66 FAQ entries

## License

Personal use. Not affiliated with Frontier Airlines.
