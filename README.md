# Thrion Tactics - Press Kit

Live at **https://pyles-studio.github.io/thrion-tactics/**

Static page. No build step, no dependencies. Open `index.html` in a browser to preview.

```
index.html                 the whole page (CSS is inline)
images/logo-*.png          logo at 2400 / 1200 / 600 px, transparent background
images/screenshot-*.jpg    1920x1080, full quality, linked for download
```

## Publishing

Push to `main`. GitHub Pages rebuilds in about a minute.

```bash
git add -A && git commit -m "update press kit" && git push
```

## Screenshots

Six 1920x1080 captures, each clickable on the page for the full-size file.

Debug overlays were painted out before publishing: the FPS counter, the
"Work in Progress" build box with its Close button, the "Development Build"
watermark, and the PlayFab account ID on the menu screens. If you recapture,
turn those off in the build instead and the edit step goes away.

To replace one, drop a 1920x1080 JPEG over the matching `screenshot-0N.jpg`
and push. Order on the page is menu, champion select, combat, dungeon,
altar chamber, run summary.

## Video

The Video section embeds `https://youtu.be/5jNCCWCWdOY` through
youtube-nocookie. To swap it, change the video ID in the `<iframe src>`
and in the "Watch on YouTube" link below it.

## Context

Built for the IGDA Greece "Game Developers Meetup #4" exhibitor form
(Larissa, 31 October 2026). The form asks for three links: game page,
press kit, and a trailer or gameplay video. Submission deadline
24 September 2026.

Form answers used:

| Field | Value |
|---|---|
| Team / company | Pyles Studio |
| Contact | pylesstudio@gmail.com |
| Game Link | https://gamejolt.com/games/ThrionTactics/807396 |
| Press Kit | https://pyles-studio.github.io/thrion-tactics/ |
| Trailer | https://youtu.be/5jNCCWCWdOY |
