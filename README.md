# certificate portal

Serves **certificate.humanskills.in** — the branded certificate portal for
Human Skills by Sudeep Ghosh.

## What it does

A landing page that matches humanskills.in, with:

- three entry points — **Submit**, **Track** and **Verify**
- a **How it works** 3-step strip
- **Good to know** notes (3 working days turnaround, keep your tracking code, what to have ready)
- a **sample certificate** preview

## Files

- `index.html` — the portal page (self-contained)
- `assets/` — bundled stylesheet, hero artwork, sample certificate, OG image, favicon
- `robots.txt` — allows crawling and points to the sitemap
- `sitemap.xml` — single-URL sitemap for the portal
- `CNAME` — custom domain for GitHub Pages
- `.nojekyll` — skip Jekyll processing

## SEO / indexing

- **Title:** "Certificate Portal - Human Skills by Sudeep Ghosh"
- **Site name (structured data):** "Human Skills by Sudeep Ghosh Certificate Portal"
- **H1:** "Human Skills by Sudeep Ghosh Certificate Portal"
- **Structured data:** schema.org `WebSite` + `WebPage` + `Person` (JSON-LD)
- `robots` meta: `index, follow`

## Notes

- Assets are **bundled**, not hot-linked, so the page works even if humanskills.in
  is slow or unavailable.
- To re-sync styling after a change to the main site's stylesheet, replace
  `assets/site.css` with a fresh copy.
- The certificate app itself is hosted on PythonAnywhere; this repo serves only
  the portal page.
