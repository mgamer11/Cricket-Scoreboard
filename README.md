# 🏏 Cricket Scoreboard

A live, mobile-first cricket scoreboard built as a single-page web app. Installs to your phone's home screen like a native app — no App Store needed.
## Features

- **Run pad** — 0, 1, 2, 3, 4, 6, with 4s and 6s visually called out
- **Wicket** — instant tap for a standard dismissal (bowled, caught, LBW, stumped)
- **Run Out** — arm it, then tap the number of runs the batters were attempting; automatically credits one fewer than what you tap (matches real cricket scoring rules)
- **No Ball** — arm it, then tap the runs scored; adds to the total without counting as a legal ball
- **Smart Undo** — reverses the *exact* last action (runs, wicket, no-ball, or run-out), including rewinding across an over boundary
- **Overs & wickets tracking** — auto-advances the over every 6 legal balls, locks scoring at 10 wickets
- **Ball-by-ball ledger** — scrolling log of everything bowled this innings
- **Teams & Players** — name two teams, add player rosters, and select who's on strike so runs get credited to individuals
- **New Innings** — freezes the current score as the target and flips the batting team, with a live "runs needed to win" tracker
- **Installable** — works as a full-screen home screen app on both iOS (via "Add to Home Screen") and Android (via the native install prompt)

## Files

| File | What it does |
|---|---|
| `index.html` | Page structure and all the game logic (JavaScript) |
| `style.css` | All visual styling — colors, fonts, layout, button styles |
| `manifest.json` | Tells Android/Chrome how to install this as an app (name, icon, colors) |
| `icon-180.png` | Home screen icon for iOS |
| `icon-192.png` | Home screen / browser tab icon for Android and Chrome |
| `icon-512.png` | Large icon Android uses for splash screens and app switchers |

## Installing on your phone

**iOS (Safari):**
1. Open the live site link above in Safari (not a downloaded file — if you're viewing a local file, first tap ••• → Open in Safari)
2. Tap **Share** → **Add to Home Screen**

**Android (Chrome):**
1. Open the live site link above
2. Tap the install prompt, or **⋮ menu → Install app**

## Making changes

- **Design/colors/spacing** → edit `style.css` only
- **New scoring rules or features** → edit the `<script>` section inside `index.html`
- **Icon** → replace `icon-180.png`, `icon-192.png`, and `icon-512.png` with new images of the same size and same filenames

All files need to live in the same folder in the repo for the relative links between them to work.
