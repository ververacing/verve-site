# Verve Racing site

The landing page for Verve, the Assetto Corsa AI app. A static page on GitHub Pages.

- `index.html` — the page. Lap, car and track counts come live from the Verve Supabase `stats` view; the
  download count is GitHub's releases API plus the OverTake figure in `stats.json`.
- `stats.json` — the figures no browser can fetch for itself: recovery, frame cost, script errors, installs,
  CSP builds, and the OverTake download count with the date it was read. Regenerate with
  `python tools/site_stats.py --overtake N` in the verve-broadcast repo.
- `privacy.html` — what the visit beacon and the opt-in race reports hold.
