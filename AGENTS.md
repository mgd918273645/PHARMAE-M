# Fruitables — AGENTS.md

Static HTML/CSS/JS website template. No build tools, no package manager, no server needed.

## Quick start

Open any `.html` file in a browser — no dev server required.

## Stack

- **Bootstrap 5** via CDN + `css/bootstrap.min.css`
- **jQuery 3.6** via CDN + custom JS in `js/main.js`
- **Owl Carousel**, **Lightbox**, **jQuery Easing**, **Waypoints** (local copies in `lib/`)
- **Font Awesome 5.15** + **Bootstrap Icons** via CDN

## Pages

| File | Route |
|---|---|
| `index.html` | Home |
| `shop.html` | Shop |
| `cart.html` | Cart |
| `chackout.html` | Checkout |
| `contact.html` | Contact |

All pages share the same `<head>` (CSS/CDN imports) and navbar/footer structure. Edit one, replicate across all.

## Key layout

- Navbar: `index.html:56-83`
- Hero section: `index.html:107-143`
- Product grid (tabbed): `index.html:201-555`
- Vegetable carousel (Owl): `index.html:608-684+`

## JS behavior (`js/main.js`)

- Spinner removal on load
- Fixed navbar shadow on scroll
- Back-to-top button
- Owl Carousel init for `.vegetable-carousel`
- Modal video handler

## Styling

- `css/style.css` — custom overrides (~460 lines)
- `css/bootstrap.min.css` — pre-compiled Bootstrap (do not edit directly)

## License

Creative Commons Attribution 4.0 — **must keep** credit link to HTML Codex in the footer.

## Git

Simple linear commits on `master`. No CI, no hooks, no conventions beyond descriptive messages.
