# Samsara Monetization Studio

An interactive, single-file HTML prototype of a global monetization platform, inspired by Material Design 3. This is an unofficial concept, not a Samsara product.

## Run locally

Open `dist/index.html` in a modern browser, or serve it locally:

```sh
python3 -m http.server 8000 --directory dist
```

Then open http://localhost:8000. No package installation or build step is required.

## Explore

- Revenue overview with reporting-month, region, and currency filters.
- Product catalog, regional rate cards, and browser-local pricing-plan drafts.
- AI usage simulator comparing standard and committed credit pricing.
- Customer, billing-entity, organization, and location hierarchy.
- Billing exceptions, assignment actions, and draft invoice previews.
- Searchable activity log, calculation traces, and CSV exports.

## Project structure

```text
dist/
  index.html    # Complete application: HTML, CSS, JavaScript, and inline SVG
README.md
.gitignore
```

## Prototype boundaries

All revenue, customers, prices, usage, exchange rates, and audit events are illustrative. The prototype does not connect to Samsara, payment processing, production metering, or live billing. Pricing plans and new audit events are stored in browser localStorage; other demo interactions may reset on reload. Data stored in one browser is not synchronized with other users or browsers.

Regional list prices are distinct from the fixed exchange rates used for consolidated reporting. The pricing simulator excludes taxes, negotiated discounts, and prorations.

## Hosting

Serve the `dist` directory with any static web host. The existing private Sites preview is deployed separately; commits to this repository do not automatically update that preview. No deployment workflow or GitHub Pages configuration has been enabled.
