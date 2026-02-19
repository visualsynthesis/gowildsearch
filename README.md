# GoWild Flight Finder

A single-file web tool for Frontier Airlines GoWild pass holders to find flights, check schedules, and get answers to common questions — all without fighting Frontier's website.

## What It Does

GoWild Flight Finder helps you quickly browse Frontier destinations from ATL, DEN, and MCO, filter by route type, check seasonal schedules, avoid blackout dates, and link directly to Frontier's booking page on the right date.

**The problem it solves:** Frontier's booking site doesn't make it easy to browse GoWild options. You can't easily see which routes fly on which days, when seasonal routes operate, or which dates are blacked out. This tool puts all of that in one place.

## Features

### Flight Search
- **100+ destinations** across ATL, DEN, and MCO hubs
- **Filter by route type:** domestic, international, or both
- **Filter by region:** Caribbean, Mexico, Central America, and more
- **Direct route detection** with visual indicators for nonstop flights
- **Low-frequency route warnings** for routes that only fly 1-2x/week

### Date Modes
- **Exact Dates** — pick specific travel dates and link directly to Frontier's booking page
- **Flexible Dates** — opens a popup showing all dates in your GoWild booking window (1 day for domestic, 10 days for international) with direct links for each date
- **Day-of-week filtering** — for routes with known schedules (e.g., Saturday-only flights), the popup only shows dates the route actually operates

### Calendar & Blackout Dates
- **Visual calendar carousel** showing the current and next month
- **Blackout dates highlighted in red** — covers 2025, 2026, and early 2027
- **Navigate months** to plan ahead

### Book Now Suggestions
- **Smart banner** suggesting destinations with upcoming non-blackout dates
- **Seasonal route awareness** — only suggests routes that are currently in season

### GoWild Help (FAQ Search)
- **66 curated Q&A entries** covering booking, bags, seats, pricing, policies, elite status, fleet info, seasonal schedules, and more
- **GPT-like search experience** — type a question, press Enter, get a clean answer with related topics
- **Smart keyword matching** with stop-word filtering and weighted scoring (tags > question > answer)
- **Suggestion chips** for common topics

## Seasonal Data

The tool includes detailed seasonal schedule data for international routes:

**ATL** — 15 international destinations with flight days and seasonal windows (Nov–Apr winter, May–Aug summer)

**DEN** — 8 international destinations including the only Frontier route to Honolulu

**MCO** — 12 international destinations with the most year-round coverage

Routes with confirmed day-of-week data (Saturday-only, daily, etc.) filter the flex popup to only show valid days. Routes without confirmed days show all dates with a warning.

## Tech Stack

- **Single HTML file** — no build step, no dependencies, no server needed
- HTML + CSS + vanilla JavaScript (~1,260 lines)
- Google-inspired Material Design aesthetic
- Fully responsive
- Works offline once loaded

## How to Use

1. Open `gowild-finder.html` in any web browser
2. Select your home airport (ATL, DEN, or MCO)
3. Use the filters to narrow destinations
4. Toggle between Exact and Flexible date modes
5. Click a destination card to go to Frontier's booking page
6. Use the search bar to ask questions about GoWild

## Data Sources

- Route data compiled from Frontier Airlines public schedules and press releases
- Blackout dates from official GoWild terms and conditions
- FAQ answers researched from Frontier's website, support pages, press releases, and public travel resources
- Day-of-week schedules from flight tracking sites (confirmed routes only)

## Limitations

- **No live availability data** — Frontier doesn't offer a public API, so the tool links to their booking page where you check actual seat availability
- **Schedules may change** — Frontier adjusts routes and frequencies seasonally; some day-of-week data may become outdated
- **GoWild-specific** — this tool is designed for GoWild pass holders, not general Frontier booking

## License

Personal use. Not affiliated with Frontier Airlines.
