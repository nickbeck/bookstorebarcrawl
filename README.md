# Bookstore Bar Crawl NYC
### A Literary Drinker's Guide to New York City

**Live site:** [bookstorebarcrawl.com](https://bookstorebarcrawl.com)

---

## About

Bookstore Bar Crawl NYC is an evergreen guide to the bars and bookstores where New York City's literary history was made — and is still being made. From the booth where O. Henry wrote *The Gift of the Magi* to the bar where Dylan Thomas drank his last whiskey, the guide maps the intersections of books, bars, and boroughs across Manhattan.

The project originated as a live event on April 23, 2022 — Shakespeare's birthday — bringing together locals to celebrate NYC's literary and drinking traditions in a single day-long crawl. It has since been repurposed as a permanent city guide.

---

## Features

- 14 venues across 4 Manhattan neighborhoods (Greenwich Village, East Village, Midtown, Flatiron)
- Curated venue cards with literary history and notable figures for each location
- 3 suggested crawl routes with direct Google Maps links
- Embedded Google Maps with all venues plotted
- Email signup for future crawl events
- Fully responsive — mobile, tablet, and desktop
- Cache-control headers for consistent deploys

---

## Tech Stack

- **HTML / CSS / Vanilla JavaScript** — single-file static site, no frameworks or dependencies
- **Google Fonts** — Playfair Display, IM Fell English, Courier Prime
- **GitHub Pages** — free static hosting with custom domain
- **Git** — version control and deployment workflow

---

## Deployment

The site is deployed via GitHub Pages from the `main` branch. Every push to `main` triggers an automatic redeploy within ~60 seconds.

To update the site locally:

```bash
git add index.html
git commit -m "describe your change"
git push
```

---

## Domain

Custom domain `bookstorebarcrawl.com` is connected via DNS A records pointing to GitHub Pages servers, with HTTPS enforced via GitHub's automatic SSL certificate.

---

## Project Background

Built as a personal project to develop hands-on experience with Git, GitHub Pages, static site architecture, and custom domain configuration — while creating something genuinely useful for NYC's literary community.

---

*"In wine there is wisdom, in beer there is freedom, in water there is bacteria." — Benjamin Franklin*
