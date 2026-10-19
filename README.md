# certificate portal

Serves **certificate.humanskills.in** — the branded certificate portal for
Human Skills by Sudeep Ghosh.

## What it does

A landing page that matches humanskills.in, with three entry points:

- **Submit your certificate request** -> https://ghoshsudeep.pythonanywhere.com/submit
- **Track your certificate** -> https://ghoshsudeep.pythonanywhere.com/track
- **Verify a certificate** -> https://humanskills.in/verify.html

## How it works

- `index.html` is the portal page. It links the main site's stylesheet
  (`https://humanskills.in/site.css`) and logo, so it always matches the site
  whenever the main stylesheet is updated.
- `CNAME` sets the custom domain `certificate.humanskills.in` for GitHub Pages.
- DNS: at Wix, a CNAME record `certificate` -> `ghoshsudeep27-commits.github.io`.

## Notes

- The certificate app itself is hosted separately on PythonAnywhere; this repo
  only serves the branded portal page.
- To change the destination links, edit the three `hero__cta` anchors in `index.html`.
