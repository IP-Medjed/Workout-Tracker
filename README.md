# Tension Protocol — PPL Workout Tracker

A single-file, zero-dependency workout tracker for a 6-day Push/Pull/Legs split built around heavy 5×5 anchor lifts, superset hypertrophy blocks, and separate midday conditioning sessions. No build step, no backend, no account — one HTML file.

**Live app:** `https://ip-medjed.github.io/Workout-Tracker/`

## Features

- **6-day PPL program** — each day opens with a unique 5×5 anchor (bench, deadlift, back squat, OHP, barbell row, front squat), followed by straight-set mains, paired supersets with transition/rest timing, and a burnout finisher
- **Two-session days** — AM lift + midday conditioning (track sprints, tempo intervals, Zone 2), structured with the same loggable card UI as the strength work
- **Per-set logging** — weight × reps for lifts, time × distance/RPE for conditioning; live volume (tonnage) totals per exercise and per day
- **Auto rest timers** — checking a set starts that exercise's rest countdown with sound + vibration; cooldown and mobility items have one-tap timers
- **Stats & history** — log sessions and graph any lift over time: estimated 1RM (Epley), top set, or total volume, with PR tracking
- **Exercise library** — browse 800+ exercises (filtered to the current day's muscle groups) with start/end position photos and step-by-step form notes, powered by [free-exercise-db](https://github.com/yuhonas/free-exercise-db)
- **Fully editable** — add, swap, reorder, remove, and re-program any exercise or conditioning piece; restore defaults per day
- **Offline-friendly data** — everything persists in your browser's `localStorage`; nothing leaves your device

## Usage

1. Serve the file over HTTP(S) — GitHub Pages works out of the box (Settings → Pages → Deploy from branch; name the file `index.html` for a clean URL)
2. Open the URL in your phone's browser
3. iOS: Share → **Add to Home Screen** for a fullscreen, app-like launch
4. Log sets, hit **✓ Finish & Log Session** when done, and watch the Stats tab fill in

> **Note:** opening the file directly from local storage (e.g. the iOS Files preview) won't render — Quick Look blocks JavaScript. Serve it from a real URL.

## Data & Privacy

All data lives in `localStorage` in your own browser. There is no server, no sync, no analytics, and no tracking. Clearing site data clears your logs — export/backup is on the roadmap.

External requests at runtime: Google Fonts (styling) and `raw.githubusercontent.com` (exercise database + demo images). Both are optional — the tracker itself works without them.

## Credits

- Exercise database and demonstration images from [yuhonas/free-exercise-db](https://github.com/yuhonas/free-exercise-db) (The Unlicense / public domain)
- Fonts: Anton, DM Sans, and DM Mono via Google Fonts
- Built with Claude (Anthropic)

## License

BSD 3-Clause — see [LICENSE](LICENSE).
