# Sunil Hegde — Portfolio Site

A single-file portfolio site, styled around a "program blueprint" theme —
your programs presented like technical schematics: roadmaps, spec sheets,
a legend, and a timeline.

No build step, no dependencies to install. It's one HTML file with
everything (CSS + JS) inline, using Tailwind-style utility patterns by hand
and Google Fonts loaded via CDN link.

## Deploy to Netlify (fastest way — no account setup needed beyond signing in)

1. Go to https://app.netlify.com/drop
2. Drag the `index.html` file straight onto the page
3. Netlify gives you a live URL immediately (something like `random-name-123.netlify.app`)
4. Optional: in Site settings → Domain management, click "Options" → "Edit site name"
   to get a custom subdomain like `sunilhegde.netlify.app`

## Deploy via GitHub (better if you want to keep editing it over time)

1. Create a new GitHub repo (e.g. `portfolio`)
2. Add `index.html` to the repo and push
3. In Netlify: "Add new site" → "Import an existing project" → connect GitHub → pick the repo
4. Build command: leave blank. Publish directory: leave as `/` (root)
5. Deploy — from now on, every push to the repo auto-updates the live site

## Editing the content

Everything is in `index.html` — no separate content files. Search for these
sections to update them:

- `<h1>Sunil Hegde</h1>` — name/hero text
- `id="about"` — bio + the four stat numbers
- `id="programs"` — the four case-study cards (situation / action / result)
- `id="skills"` — the three-column skills legend
- `id="experience"` — the work history timeline
- `id="contact"` — email, phone, LinkedIn

Colors and fonts are defined once at the top of the `<style>` block under
`:root { ... }` if you want to adjust the palette.

## Notes

- Fully responsive down to mobile (nav collapses, grids stack to one column)
- Respects `prefers-reduced-motion` for anyone with that OS setting on
- No tracking, no analytics, no external JS beyond Google Fonts — add your
  own analytics snippet before `</body>` if you want visit data later
