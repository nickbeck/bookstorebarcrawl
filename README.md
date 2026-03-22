# Bookstore Bar Crawl NYC
### A Literary Drinker's Guide to New York City

**Live site:** [bookstorebarcrawl.com](https://bookstorebarcrawl.com)
**GitHub:** [github.com/nickbeck/bookstorebarcrawl](https://github.com/nickbeck/bookstorebarcrawl)

---

## About

Bookstore Bar Crawl NYC is an evergreen guide to the bars and bookstores where New York City's literary history was made — and is still being made. From the booth where O. Henry wrote *The Gift of the Magi* to the bar where Dylan Thomas drank his last whiskey, the guide maps the intersections of books, bars, and boroughs across Manhattan and Brooklyn.

The project originated as a live event on April 23, 2022 — Shakespeare's birthday — bringing together locals to celebrate NYC's literary and drinking traditions in a single day-long crawl. It has since been repurposed as a permanent city guide.

---

## Features

- 25+ venues across 7 neighborhoods in Manhattan and Brooklyn
- Curated venue cards with literary history and notable figures for each location
- Tappable Google Maps links on every address, resolving to the named business listing
- 4 suggested crawl routes with direct multi-stop Google Maps directions links
- Embedded Google Maps centered on NYC covering both boroughs
- Email signup powered by Formspree — captures submissions without a backend
- Fully responsive — mobile, tablet, and desktop
- Cache-control headers for consistent deploys

---

## Tech Stack

### Frontend
- **HTML5** — semantic, single-file static site with no frameworks or build tools
- **CSS3** — custom properties (variables), CSS Grid for 2-column venue layout, Flexbox for nav and forms, `@media` queries for mobile responsiveness
- **Vanilla JavaScript** — form submission handling via `fetch()`, scroll reveal animations via `IntersectionObserver` API

### Typography & Fonts
- **Google Fonts** — three typefaces loaded via CDN:
  - *Playfair Display* — display headlines and section titles
  - *IM Fell English* — body text and editorial prose
  - *Courier Prime* — monospace labels, badges, addresses, and metadata

### Form & Email Capture
- **Formspree** — serverless form backend; handles POST submissions from the email signup form and delivers them to the owner's inbox with zero backend code required

### Hosting & Deployment
- **GitHub Pages** — free static site hosting, auto-deploys on every push to `main`
- **Git** — version control; full commit history tracked on GitHub
- **Custom domain** — `bookstorebarcrawl.com` connected via DNS A records pointing to GitHub Pages servers
- **HTTPS** — SSL certificate auto-provisioned by GitHub Pages via Let's Encrypt
- **`_headers` file** — cache-control directives (`no-cache, must-revalidate`) to ensure users always receive the latest version on deploy

### Maps & Location
- **Google Maps Embed API** — iframe embed centered on NYC (`40.7282, -73.9857`) covering Manhattan and Brooklyn
- **Google Maps Search Links** — every venue address links directly to the named business listing on Google Maps (opens Maps app on mobile)
- **Google Maps Directions Links** — each crawl route pre-loads all stops as a multi-destination directions query

### Domain
- **Squarespace Domains** — domain registrar (pending transfer to Namecheap)
- DNS configured with 4 A records pointing to GitHub Pages IP addresses and a CNAME for `www`

---

## Deployment

The site is deployed via GitHub Pages from the `main` branch. Every push to `main` triggers an automatic redeploy within ~60 seconds.

To update the site locally:

```bash
# Make edits to index.html
git add index.html
git commit -m "describe your change"
git push
```

---

## Project Background

Built as a personal project to develop hands-on experience with Git, GitHub Pages, static site architecture, custom domain configuration, and third-party service integration (Formspree, Google Maps) — while creating something genuinely useful for NYC's literary community.

Started as a Squarespace event site for a one-day Shakespeare's birthday crawl in April 2022. Migrated off Squarespace, rebuilt from scratch, and repurposed as a permanent evergreen guide — reducing hosting costs from ~$200/year to $0.

---

*"In wine there is wisdom, in beer there is freedom, in water there is bacteria." — Benjamin Franklin*
