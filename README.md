# Alexander Roman — Developer Portfolio

A modern, SaaS-style developer portfolio built with plain HTML, CSS, and
JavaScript (no framework or build step required).

## Structure

```
index.html                       Homepage — hero, project grid, about preview, contact
about.html                       Full About Me page
resume.html                      Printable resume (recruiter-ready, use Print / Save as PDF)
projects/
  roman-creative-studio.html     Case study: Roman Creative Studio
  4kingdom-podcast.html          Case study: 4Kingdom Podcast
css/style.css                    Design system + all page styles
js/main.js                       Mobile nav, scroll reveal, active states
```

## Running locally

No build step is needed. Either open `index.html` directly in a browser, or
serve the folder locally:

```
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploying

This is a static site, so it deploys as-is to GitHub Pages, Vercel,
Netlify, or Cloudflare Pages — no build command required.

## Before publishing

- `resume.html` has placeholders for phone, city/state, GitHub URL, and
  LinkedIn URL — search for `[Add` to find them.
- Update the social links in the contact section of `index.html` (GitHub,
  LinkedIn) once you have public profile URLs.
- Swap the browser-mockup placeholders for real screenshots if you'd like
  (`.browser-frame .surface` in `css/style.css`).
