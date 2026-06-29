# Filling the Gap — Hero Section Upgrade Demo

A modern, cinematic full-bleed **video hero** demo for [fillingthegap.ca](https://fillingthegap.ca),
a Toronto dental charity. The header and footer are faithful replicas of the live site (unchanged);
only the hero section is new.

Built with the site's real brand palette and typography:

| Token | Value |
|-------|-------|
| Teal accent | `#00afd1` |
| Teal (hover) | `#008daa` |
| Navy | `#00406a` |
| Deep navy | `#002c44` |
| Display font | Alfa Slab One |
| Serif font | Arvo |
| Body font | Quicksand |

## Run locally

```bash
python3 -m http.server
# open http://localhost:8000
```

## Files

- `index.html` — full page (replica header + new hero + replica footer)
- `assets/styles.css` — all styling and brand tokens
- `assets/torontovid720.mp4` / `.webm` — optimized, muted hero video (audio stripped, faststart)
- `assets/hero-poster.jpg` — poster frame shown before video loads
- `assets/ftg-logo-white.png` — logo
- `assets/torontovid720.mov` — original source video (not used by the page)

## Deploy to GitHub Pages

The page is plain static files — no build step.

```bash
git init && git add . && git commit -m "Hero upgrade demo"
# push to a GitHub repo, then: Settings → Pages → Deploy from branch → main / root
```

`.nojekyll` is included so GitHub Pages serves all assets as-is.
