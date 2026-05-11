# pi-x-pixel.com — Brand homepage

Single-screen brand presence for [pi-x-pixel.com](https://pi-x-pixel.com).
Static HTML, no build step, no JavaScript framework.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Brand homepage — single screen, links to GitHub + (future) Gumroad |
| `impressum.html` | Legal — § 5 TMG (German Gewerbe requirement) |
| `datenschutz.html` | Legal — DSGVO (PLACEHOLDER, must be filled before launch) |
| `404.html` | Branded 404 page |
| `robots.txt` | Crawler config — allow all, advertise sitemap |
| `netlify.toml` | Netlify deploy config — security headers + www-redirect |

## Before going live (mandatory)

- [ ] **Fill placeholders in `impressum.html`** — name, address, phone, USt-ID/Steuernummer
- [ ] **Generate full `datenschutz.html`** via [e-recht24.de](https://www.e-recht24.de/muster-datenschutzerklaerung.html) generator with these aspects checked:
  - Hosting: Netlify (server logs, IP addresses)
  - Google Fonts: embedded via fonts.googleapis.com
  - No cookies, no tracking, no contact forms
- [ ] **Add `sitemap.xml`** if more pages are added later (currently only 4 pages — sitemap optional)

## Deploy — option A: drag & drop (fastest)

1. Open [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag this entire folder onto the page
3. Netlify deploys instantly, returns a `*.netlify.app` URL
4. In the resulting site dashboard:
   - **Domain management → Add custom domain → `pi-x-pixel.com`**
   - Netlify shows DNS instructions
5. At Porkbun DNS, replace existing A records with Netlify's:
   - `A pi-x-pixel.com → 75.2.60.5`
   - `A www.pi-x-pixel.com → 75.2.60.5`
6. SSL is auto-provisioned by Netlify (Let's Encrypt) within 5–30 min after DNS propagates

## Deploy — option B: Git-linked (after first launch)

1. Create repo `pi-x-pixel/homepage` on GitHub (private OK)
2. Push this folder
3. In Netlify: **Add new site → Import from Git → select `pi-x-pixel/homepage`**
4. Build command: leave empty
5. Publish directory: `.`
6. Custom domain setup as above

## DNS — current state vs. target

| Record | Current (Hetzner placeholder) | Target (Netlify) |
|---|---|---|
| `A pi-x-pixel.com` | `37.27.212.196` | `75.2.60.5` |
| `A www.pi-x-pixel.com` | `37.27.212.196` | `75.2.60.5` |

The redirect `www → apex` is handled by `netlify.toml` once on Netlify.

## Brand tokens (consistent with other surfaces)

```
Brand display: pi-X-pixel  (capital X in Persimmon)
Colors:
  --surface:    #FAF9F6  (off-white)
  --text:       #1A1A1A  (charcoal)
  --secondary:  #5C6471  (slate)
  --accent:     #D5582C  (Persimmon)
Typography:
  Display: Newsreader (serif)
  Body:    Inter
```

Mood: editorial-clinical, NEJM-meets-Anthropic-docs.
Anti-mood: tech-bro / wellness-Instagram / SaaS-illustrated-humans.

## Related artifacts

- Brand decisions: `passive-income-research/docs/marketing/BUILD-DECISIONS.md`
- Visual system: `passive-income-research/docs/marketing/Visual-Direction.md`
- Page wireframes (incl. this homepage): `passive-income-research/docs/marketing/Gumroad-Page-Wireframe.md` Surface C

## License

The site code (HTML/CSS) is MIT.
The brand name "Pi mal Pixel" / "pi-x-pixel" and associated marks are reserved.
