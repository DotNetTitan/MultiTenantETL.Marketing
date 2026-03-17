# ETL Portal — Marketing Site

Static marketing website for [ETL Portal](https://etlportal.io), a multi-tenant data pipeline platform. Built with plain HTML, CSS, and vanilla JavaScript — no build step required.

## Project Structure

```
├── index.html      # Main page
├── styles.css      # All styles (dark theme, CSS custom properties)
├── app.js          # Vanilla JS (navbar, animations, counters, smooth scroll)
├── robots.txt      # Search engine crawl rules
├── sitemap.xml     # XML sitemap for SEO
└── assets/
    └── images/     # Logos and other static images
```

## Page Sections

| Section | ID | Description |
|---|---|---|
| Hero | `#hero` | Headline, sub-copy, and primary CTA |
| Features | `#features` | Key platform capabilities |
| Maeve AI | `#maeve` | AI assistant feature highlight |
| How It Works | `#how-it-works` | Step-by-step pipeline walkthrough |
| Connectors | `#connectors` | Supported data source/destination tiles |
| CTA | `#cta` | Final call-to-action / sign-up prompt |

## Getting Started

Open `index.html` directly in a browser, or serve the folder with any static file server:

```bash
# Node.js (npx)
npx serve .

# Python
python -m http.server 8080
```

Then visit `http://localhost:3000` (or whichever port is reported).

## Key Features of the Site

- **Scroll animations** — fade-up elements driven by `IntersectionObserver`
- **Animated stat counters** — ease-out counter animation triggered on scroll
- **Responsive navbar** — burger menu for mobile with fixed overlay
- **Smooth scrolling** — all `#anchor` links scroll smoothly
- **SEO-ready** — canonical tag, Open Graph meta, JSON-LD structured data, `robots.txt`, and `sitemap.xml`

## Deployment

The site is purely static and can be deployed to any CDN or static host (Netlify, Vercel, Azure Static Web Apps, GitHub Pages, etc.). No server-side processing is needed.

The canonical URL is configured as `https://etlportal.io/` — update the `<link rel="canonical">` tag and Open Graph/JSON-LD URLs in `index.html` if deploying to a different domain.
