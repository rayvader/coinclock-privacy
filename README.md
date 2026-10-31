# CoinClock privacy policy

The privacy policy for the CoinClock Android app (currency converter and world clock) by rayvader, published as a static GitHub Pages site.

Read it here: https://rayvader.github.io/coinclock-privacy/

## What the page covers

- A short summary: no sign-in, ads, analytics or tracking
- Data kept on the phone (saved currencies, cities, main currency, cached rates, settings)
- Data that leaves the phone: exchange rates from ExchangeRate-API (`open.er-api.com`) and city search via Open-Meteo geocoding (`geocoding-api.open-meteo.com`)
- Android backup and the "Copy lists to file" / "Load lists from file" features
- Permissions the app requests (internet, network state) and what it does not do
- Data retention and deletion, children, policy changes and contact

## Tech stack

- A single hand-written HTML page with inline CSS and an inline SVG logo
- No JavaScript, no external assets, no build step
- Light and dark themes via `prefers-color-scheme`

## Project structure

```
index.html   The privacy policy page (content and styles)
.nojekyll    Tells GitHub Pages to serve files as-is, without Jekyll
README.md    This file
```

## Prerequisites

None beyond a web browser. Git is needed to make changes.

## Preview locally

Open `index.html` in a browser, or serve the folder on localhost:

```
python3 -m http.server 8000 --bind 127.0.0.1
```

Then visit http://127.0.0.1:8000/.

## Configuration

There is no configuration, environment variables or secrets.

## Deploy

GitHub Pages serves the site from the root of the `gh-pages` branch. There is no CI workflow: changes go live once they are merged into `gh-pages`.

When the policy text changes, also update the "Effective" date near the top of `index.html`, as the page states that changes are posted with a new effective date.
