# Yankee Gardener

A gardening blog for **yankeegardener.com** — written in the voice of Margaret "Maggie"
Whitfield, a retired New Yorker relearning how to garden in Florida's Zone 10 heat and
sandy soil. Tagline: *Northeast roots, Florida soil.*

A static, dependency-free site (plain HTML + CSS, inline SVG art). No build step.

## Pages

| Page | File | Notes |
| --- | --- | --- |
| Home | `index.html` | Hero, about teaser, featured posts, topics, newsletter CTA |
| About | `about.html` | Maggie's story |
| Blog | `blog.html` | Index of all posts |
| Contact | `contact.html` | Contact form + newsletter signup |

### Blog posts (`posts/`)

- `from-tulips-to-tropicals.html` — What this Yankee had to unlearn about Florida gardening
- `beating-the-florida-heat.html` — Plants that thrive in a Zone 10 summer
- `sandy-soil-salty-air.html` — Amending sand, salt tolerance, and coastal pests

## Structure

```
yankeegardener/
├── index.html, about.html, blog.html, contact.html
├── posts/            # individual blog articles
├── css/style.css     # design system + responsive layout
├── assets/           # favicon.svg, og-image.svg
├── server.js         # tiny static preview server (Node, no deps)
└── README.md
```

## Preview locally

The site is plain static files — open `index.html` directly in a browser, or run the
included zero-dependency server:

```bash
node server.js
# then visit http://localhost:8123
```

## Design

- **Palette:** garden green `#3a7d44`, coral accent `#e8743b`, citrus `#f2b134`,
  cream `#fdfaf3`, soft charcoal `#2f3733`
- **Type:** serif headings (Iowan/Palatino/Georgia stack) + system sans body
- **SEO:** every page has a unique title, meta description, Open Graph + Twitter card tags
- **Responsive:** mobile nav and stacked layouts under 860px

## Deploy

Any static host works (Netlify, GitHub Pages, Cloudflare Pages, S3). Point the host at the
repo root; no build command needed.
