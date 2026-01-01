Mood Tracker (calendar, client-only)

This is a single-page, client-only mood tracker that stores daily ratings in the browser.

Live app

- Open `index.html` in a browser, or enable GitHub Pages for the repository root so `index.html` is served.

What it does

- Calendar UI: click any day to rate it 1 (very sad) → 5 (very happy).
- Analytics: per-month distribution, share bars, and averages (month and all-time) are calculated from stored ratings.
Storage details

- Primary storage is browser `localStorage` under key: `mood-tracker:v1`.
- The app relies on browser `localStorage` only (no file linking).
 - On app load the code will not attempt to read or write external files; it reads/writes `localStorage` only.

Privacy and backup

- All data is stored locally in your browser. Nothing is sent to external servers by default.
- To back up data manually: open your browser dev tools and copy the JSON value from `localStorage` (key: `mood-tracker:v1`) or save the browser profile.

Quick tips

- Use the ◀ / ▶ buttons to move between months. The "Today" button jumps to the current month/day.
- Click a rated day again to change or clear the rating.

Developer notes

- The app stores data only in `localStorage` under the key `mood-tracker:v1`.

License

MIT
