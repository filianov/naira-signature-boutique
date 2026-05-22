# Zargariyan / Naira Signature Boutique

Premium static boutique page for the Zargariyan / Naira Signature collection.

Main formula:

**Wiener Eleganz. Finanzielle Stärke. Persönlicher Stil.**

## What Is Included

- Static GitHub Pages-ready site: no build step, no backend dependency.
- German-first interface with RU/EN language switch.
- Mobile-first premium design for the boutique, Founder’s Drop, gifts, club edition and B2B inquiries.
- Real product catalog from local product photos: 22 grouped product cards and 75 gallery images.
- Cart, gift packaging option, promo code UI and demo checkout flow.
- Official links to `naira.wien` and `all-in-businessclub.at`.

## Project Structure

```text
.
├── index.html
├── styles.css
├── app.js
├── assets/
│   └── naira-signature-hero.png
├── images/
│   └── product photos
├── .gitignore
├── .gitattributes
├── .nojekyll
└── DEPLOY.md
```

## Local Preview

From the project folder:

```bash
python3 -m http.server 4174
```

Open:

```text
http://localhost:4174/
```

## Publish To GitHub Pages

Follow the detailed Russian instructions in [`DEPLOY.md`](DEPLOY.md).

Short version:

```bash
git init
git branch -M main
git add .
git commit -m "Publish Zargariyan boutique"
git remote add origin https://github.com/YOUR_USERNAME/naira-signature-boutique.git
git push -u origin main
```

Then enable GitHub Pages in repository settings:

`Settings` → `Pages` → `Deploy from a branch` → `main` → `/ (root)` → `Save`.

## Before Real Sales

This is ready as a static boutique page and visual product showcase. Before using it as a live commercial shop, replace the demo legal/payment parts:

- add real Austrian `Impressum`, `Datenschutz`, `AGB`, `Widerruf`;
- connect real Stripe/PayPal/Klarna checkout or an order backend;
- replace the demo Instagram URL with the real brand profile;
- confirm product prices, stock counts, shipping rules and alcohol sale/legal requirements.

