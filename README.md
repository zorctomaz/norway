# Norway Arctic Expedition — 10-Day Guided Trip

A self-contained, single-page website (HTML5 + CSS + vanilla JavaScript, no build step, no dependencies) advertising a 10-day guided small-group trip through Arctic Norway.

## What's on the page

- **Hero** — trip headline, key stats (10 days, up to 8 guests, aurora season).
- **Highlights** — whale watching, Northern Lights, Tromsø sightseeing, van road trip, small-group guiding.
- **Your Guide** — bio section highlighting 5 years as icebreaker crew, skiing, mountaineering and paragliding experience.
- **Itinerary** — expandable day-by-day plan for all 10 days.
- **What's included / not included**.
- **Gallery** — placeholder tiles (swap for real photos, see below).
- **Countdown** — live countdown to the next departure date.
- **Pricing & booking** — interactive group-size stepper with live price/discount calculation, plus a client-side-validated inquiry form (no backend attached yet).
- **FAQ** — expandable accordion.

## Running it

Just open `index.html` in a browser, or serve the folder with any static file server:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Customizing

- **Your name/contact/email**: replace the placeholder `hello@example.com` in the footer and the guide bio text in the `#guide` section.
- **Photos**: the hero, guide portrait, and gallery currently use CSS/SVG placeholders. Swap the relevant elements for `<img>` tags pointing at your own photos (e.g. `assets/` folder) once you have them.
- **Itinerary / FAQ content**: edit the `itinerary` and `faqs` arrays near the top of the `<script>` block in `index.html`.
- **Pricing**: adjust `BASE_PRICE`, `MAX_GROUP`, and the `discountFor()` tiers in the same script block.
- **Booking form**: currently client-side only (shows a success message but sends nothing). Wire `form#inquiry`'s submit handler to your email service / booking backend / form endpoint of choice.
- **Next departure date**: auto-computed to the 1st of the next aurora-season month; override `computeNextDeparture()` if you want a fixed date instead.

## Tech

Pure HTML5, CSS3 and vanilla JavaScript — no frameworks, no build tools, no external CDN dependencies.
