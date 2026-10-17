# marcusmaximus.ca

Personal site. Static, no build step.

## Deploy (GitHub Pages)

1. Copy the contents of this folder into the repo root (or into `/docs`).
2. Settings → Pages → Source: `Deploy from a branch`, branch `main`, folder `/ (root)`.
3. `CNAME` is already set to `marcusmaximus.ca` — point an ALIAS/A record at GitHub Pages, or a CNAME record at `<user>.github.io`.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Whole site, self-contained (CSS, JS, images inlined) |
| `og.png` | Social share card (1200×630) |
| `Marcus-Maximus-Resume.pdf` | Linked from the contact section |
| `CNAME` | Custom domain for Pages |
| `.nojekyll` | Skips Jekyll processing |
| `robots.txt`, `sitemap.xml` | Crawling |

Runtime dependencies loaded from CDNs: three.js (unpkg) for the 3D scene, and the Calendly widget (loaded only when someone books a call).

## Editing

`index.html` is compiled output. Do not edit it. Edit `Marcus Reyes v12 Cockpit 3D.dc.html` and re-export.
