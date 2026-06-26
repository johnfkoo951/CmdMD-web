# cmdmd-web

Landing page for **[CmdMD](https://github.com/johnfkoo951/CmdMD)** — a review-first Markdown editor & Obsidian vault router for macOS.

🌐 Live: **https://cmdmd.cmdspace.work**

## Stack

- Single static `index.html` — CMDSPACE v4.3 design system (Apple SF Pro × CMDS Green/Pink), light/dark + KO/EN toggles.
- Real app screenshots in `assets/shots/` (synced from `CmdMD/docs/images/`).
- Dedicated OG image (1200×630) in `assets/og/`.

## Develop

```bash
# preview locally
python3 -m http.server 8799   # → http://localhost:8799

# regenerate the OG image after editing assets/og/templates/og-cmdmd-web.html
./scripts/build-og.sh         # Chrome headless → assets/og/og-cmdmd-web.png
```

## Deploy

```bash
vercel deploy --prod --yes    # Vercel project "cmdmd"
```

DNS: Cloudflare `cmdspace.work` → CNAME `cmdmd → cname.vercel-dns.com` (DNS only).

---
Built with the `cmdspace-web-builder` Landing template · © 2026 CMDSPACE · Yohan Koo
