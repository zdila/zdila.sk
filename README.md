# www.zdila.sk

Static homepage for **Ing. Martin Ždila s.r.o.** — GIS & full-stack development.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The single-page site |
| `styles.css` | All styling (no framework, no build step) |
| `main.js` | Mobile nav toggle + footer year |
| `favicon.svg` | Logo / favicon |

No build step — it's plain HTML/CSS/JS.

## Preview locally

```sh
cd homepage
python3 -m http.server 8080
# open http://localhost:8080
```

## Deploy

Upload the folder to any static host (Netlify, Cloudflare Pages, GitHub Pages,
or your own web server). Point the `www.zdila.sk` DNS / vhost at it.

## Status / TODO

Done:
- Company legal details in footer (IČO / DIČ / IČ DPH, registered address, OR SR entry).
- LinkedIn URL (`in/zdila`).
- Carpathia project description.
- English-only. Founder avatar (cropped from a casual photo) in the About sidebar —
  `martin-256/512.{jpg,webp}`; replace the files to swap the photo, no HTML changes needed.

- Experience section ("Companies we've worked with") built from CVs in `tmp/`:
  MapTiler, Gruveo, Fpt Slovakia, Encyklopedický ústav SAV, Hotovo, Nordlicht,
  Old Street Solutions. Text-only (no client logos without permission).
- LinkedIn export checked — saved profile page only, no recommendation texts.

Outstanding:
- Check NDAs before publishing the client list.
- Optional: a real Open Graph preview image (`og:image`) for nicer link sharing.
