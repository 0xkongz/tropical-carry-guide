# 🌴 The Tropical Carry Guide

A curated, editorial-style guide to the **best waist bags and sling bags** for tropical travel — optimized for heat, humidity, and monsoon seasons.

## 🔗 Live Site

👉 **[View the guide](https://{USERNAME}.github.io/tropical-carry-guide/)**

> Replace `{USERNAME}` with your GitHub username after deploying.

## What's Inside

**10 expert-picked bags** across two categories:

### Waist Bags (1.5L – 3L)
| # | Bag | Brand | Price |
|---|-----|-------|-------|
| 1 | Mantis 2 Waist Pack | Arc'teryx | $55–65 |
| 2 | UL Black Hole Mini Hip Pack | Patagonia | $35–45 |
| 3 | Venture Ready 2.5L | Bellroy | $60–89 |
| 4 | Allpa X 3L Hip Pack | Cotopaxi | $50–60 |
| 5 | Tanker Waist Bag | Porter-Yoshida | $150–200 |

### Sling Bags (3L – 8L)
| # | Bag | Brand | Price |
|---|-----|-------|-------|
| 1 | Day Sling 3 | Aer | $80–90 |
| 2 | Atom Sling 8L | Patagonia | $60–70 |
| 3 | Daylite Sling 6L | Osprey | $40–50 |
| 4 | Venture Sling 6L | Bellroy | $99–125 |
| 5 | Tanker Sling W Zip (L) | Porter-Yoshida | $200–280 |

Plus: scenario comparison table, material guide, and regional picks for SE Asia.

## Tech Stack

- Single-file HTML — no build tools, no dependencies
- Dark editorial design (DM Serif Display + Instrument Sans)
- Inline SVG illustrations as fallback visuals
- Product photos loaded from Pack Hacker CDN
- Sticky navigation with scroll-spy
- Fully responsive (mobile-first)

## Deploy

### Option 1: GitHub Pages (recommended)
```bash
gh repo create tropical-carry-guide --public --clone
cp index.html tropical-carry-guide/
cd tropical-carry-guide
git add . && git commit -m "Initial commit" && git push
gh api repos/{OWNER}/tropical-carry-guide/pages -X POST -f source.branch=main -f source.path=/
```

### Option 2: Just open it
Download `index.html` and open in any browser. Product photos load from CDN — internet connection required.

## License

Content compiled for personal reference. Product names and images belong to their respective brands.
