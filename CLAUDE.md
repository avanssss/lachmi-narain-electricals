# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the website and business documentation for **Lachmi Narain Electricals**, an electrical cable and wire distributor based in Coimbatore, India (established 1998). The website is a single self-contained HTML file — no build system, no dependencies, no JavaScript.

## Files

- [index.html](index.html) — The working website. All CSS is embedded in `<style>`. Open directly in a browser to preview.
- [index_standalone.html](index_standalone.html) — Deployable version with all images base64-encoded inline. Share this single file for Vercel/Netlify deployment — no accompanying folders needed.
- [LOGOS/](LOGOS/) — `LACHMI NARAIN NEW LOGO 2.png` is the active navbar logo. Finolex and Polycab brand logos are also here.
- [Images for lachmi narain website/NEW IMAGES- higher quality/](Images%20for%20lachmi%20narain%20website/NEW%20IMAGES-%20higher%20quality/) — Three warehouse/product photos used across the site (image 1–3).
- [Images for lachmi narain website/resized image.png](Images%20for%20lachmi%20narain%20website/resized%20image.png) — Used in the products section banner.
- [lachmi_narain_electricals_detailed_profile.md](lachmi_narain_electricals_detailed_profile.md) — Source of truth for company info.
- [lachmi_narain_electricals_cable_catalogue.md](lachmi_narain_electricals_cable_catalogue.md) — Source of truth for products.

## Website Structure

Sections in order:

1. **Navbar** — white background, `LACHMI NARAIN NEW LOGO 2.png` at 100px height, anchor nav links in `--primary` blue
2. **Hero** — `--primary` blue background, headline, two CTAs, `image 2.png` (warehouse)
3. **Stats bar** — `--orange` strip, 4 stats (25+ years legacy, 25+ years Coimbatore, 4+ categories, 2 brands)
4. **About** (`#about`) — two-column: text left, `image 3.png` right (cable close-up, `object-fit: contain`)
5. **Products** (`#products`) — `--light` background, `resized image.png` banner, 4 product cards in a CSS grid
6. **Brands** (`#brands`) — centred rounded box, Finolex and Polycab logos side by side
7. **Why Us** (`#why`) — `--primary` background, 2×2 card grid left, `image 2.png` right
8. **Contact** (`#contact`) — address, phone, email, hours, embedded Google Maps iframe
9. **Footer** — `--primary` background

## Design Tokens

CSS variables at the top of `<style>`:

```
--primary: #1d407e   (blue — used for dark sections, headings, nav links)
--orange:  #e86c1a   (accent — buttons, icons, labels, stats bar)
--light:   #f4f6fb   (section backgrounds)
```

## Contact Details

- Email: sales@lnelectricals.com
- Mobile: +91 98430 14007
- Landline: 0422 232 1556
- Address: Sungam Bypass Road, Ramanathapuram, Coimbatore, Tamil Nadu

## Working with This Project

- Edit content and styles directly in [index.html](index.html).
- After any image or content change, re-run the base64 embed script to regenerate [index_standalone.html](index_standalone.html) — otherwise the standalone file will be out of date.
- The Markdown files are reference documents; keep the website in sync when updating product or company info.
- All image `src` attributes in `index.html` use `%20` URL-encoded paths (e.g. `Images%20for%20lachmi%20narain%20website/...`).
