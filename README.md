# certificate-redirect

Redirects **certificate.humanskills.in** to the training certificate app at
**https://ghoshsudeep.pythonanywhere.com**.

## How it works

- `index.html` issues the redirect (JavaScript, with a `<meta http-equiv="refresh">` fallback).
  It preserves the path, query string and fragment.
- `CNAME` tells GitHub Pages to answer for `certificate.humanskills.in`.
- DNS: at Wix, a CNAME record for host `certificate` points to `ghoshsudeep27-commits.github.io`.

## Notes

- GitHub Pages cannot issue a true HTTP 301 from static hosting; this is a
  client-side redirect (HTTP 200 + immediate forward). For a vanity link that is
  fine, but it is a "soft" redirect as far as search engines are concerned.
- To change the destination, edit the URL in `index.html` (both the script and the meta tag).
