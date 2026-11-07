# vibo-site

Landing page for ViBo — modular skills for AI agents.

Static site: one HTML file and an SVG mark. No build step, no dependencies.
Served by GitHub Pages from the `main` branch root.

## Structure

```
index.html    page
favicon.svg   three-module mark (agent / skill / result)
```

## Design

Built from the ViBo light brand book (2026, v2.0):

- Cobalt `#1557FF` — platform, infrastructure, navigation, primary action
- Action Orange `#FF642F` — skills, execution; one orange element per screen
- Graphite `#171D27` — text, result module
- Warm White `#FAF9F6` background, Pure White `#FFFFFF` surfaces
- Blue Surface `#EEF3FF`, Peach Surface `#FFF0EA`, Muted `#5E6878`, Border `#DFE4EC`
- Space Grotesk for text, IBM Plex Mono for code and identifiers

Layout follows the frontend-design skill: the mark opens the page instead of a
stat block, memory leads the skill grid instead of six equal cards, and the page
avoids the usual generated-page tells (all-caps eyebrows, dot-separated meta
strings, arrow suffixes on buttons).

## Local preview

```bash
python3 -m http.server 8000
```
