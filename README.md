# Thrion Tactics - Press Kit

Static page. No build step, no dependencies. Open `index.html` in a browser to preview.

```
index.html          the whole page (CSS is inline)
images/logo-*.png   logo at 2400 / 1200 / 600 px, transparent background
images/screenshot-*.png   PLACEHOLDERS - replace with real captures
```

## Blanks to fill before publishing

Every blank is marked in the page with a red dashed `.todo` span. Search `index.html`
for `class="todo"` to find all of them.

| Placeholder | Appears in |
|---|---|
| `TEAM OR STUDIO NAME` | Factsheet, Team |
| `PUBLIC CONTACT EMAIL` | Factsheet, Contact |
| `GAME PAGE LINK` | Factsheet, Contact |
| `TRAILER OR GAMEPLAY VIDEO LINK` | Video |
| `THIS PAGE'S PUBLIC URL` | Contact |

The video section wants a YouTube link. Embed instead of link once the URL exists:

```html
<div style="position:relative;padding-bottom:56.25%;height:0">
  <iframe src="https://www.youtube.com/embed/VIDEO_ID" title="Thrion Tactics trailer"
    style="position:absolute;width:100%;height:100%;border:0" allowfullscreen></iframe>
</div>
```

## Screenshots

Six slots, 16:9. Replace the placeholder files in `images/`, keeping the same names,
or change the `<img src>` paths in the Images section.

Capture at 1920x1080 with the dev overlays off:
- FPS counter and the Pre-Alpha build label (both draw over the HUD)
- The tier info card that opens at run start

## Publishing

The page is plain HTML, so any static host works. Fastest route is the existing
GitHub Pages site, which is already live:

```bash
git clone https://github.com/D3vCrow/D3vCrow.github.io.git
cp -r F:/DevCrow/Dev/thrion-presskit D3vCrow.github.io/thrion
cd D3vCrow.github.io && git add thrion && git commit -m "add Thrion Tactics press kit" && git push
```

Live at `https://d3vcrow.github.io/thrion/` about a minute after the push.
Jekyll copies unknown folders through untouched, so no `_config.yml` change is needed.

Alternative: a dedicated `thrion-presskit` repo with Pages turned on, which lands at
`https://d3vcrow.github.io/thrion-presskit/`. Cleaner separation, longer URL, and
Pages has to be enabled first.

## Context

Built for the IGDA Greece "Game Developers Meetup #4" exhibitor form
(Larissa, 31 October 2026). The form asks for three links: game page, press kit,
and a trailer or gameplay video. Submission deadline 24 September 2026.
