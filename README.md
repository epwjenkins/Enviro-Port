# Enviro-Port Website

A modern, static redesign of the Enviro-Port marketing site for a manufacturer of concrete reclaimer and ready-mix recycling systems for the ready-mix and precast concrete industries.

## Structure

Plain HTML/CSS/JS, no build step required.

```
index.html          Home
products.html        Aggregate Recovery Series, Complete Recovery Series, Components
how-it-works.html    Step-by-step reclamation process
about.html           Company overview
team.html            Team / departments
dealers.html         Dealer network & coverage
contact.html         Contact form, info, map
assets/css/styles.css  Design system & all page styles
assets/js/main.js      Mobile nav, scroll reveal, stat counters, contact form UI
assets/img/favicon.svg Site favicon
```

## Running locally

No build tools needed. Serve the folder with any static file server, e.g.:

```
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Deploying

Works as-is on any static host: GitHub Pages, Netlify, Vercel, S3 + CloudFront, etc. For GitHub Pages, enable Pages on this repo pointed at the root of the default branch.

## Content notes

This redesign was built without direct access to fetch the live enviro-port.com site (network restricted in the build environment), so copy was reconstructed from public search results, industry press coverage, and business directory listings referencing Enviro-Port, Inc. (Gratiot, WI). Before launch, please verify and update:

- **Team page**: currently organized by department rather than named staff, since no verified names/photos were available. Swap in real team bios/photos if desired.
- **Dealers page**: only the Western U.S. region (via D'Ambra Equipment) was confirmed in public sources; other regions are shown as "factory-direct" placeholders pending your actual dealer list.
- **Contact form**: the form UI is wired for a friendly front-end confirmation only; connect `assets/js/main.js`'s `#contact-form` submit handler to a real backend, form service (e.g. Formspree, Netlify Forms), or mailto endpoint.
- **Photography**: all visuals are CSS/SVG illustrations rather than real equipment photos. Swap in real product and facility photography for the strongest result.
- **Stats & specs** (23.1M tons/yr wasted, 15-25 yd/hr throughput, etc.): sourced from public references to the existing Enviro-Port site; confirm current figures before publishing.
