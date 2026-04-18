<p align="center">
  <img src="https://img.shields.io/badge/HTML-5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS-3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/Zero_Build-Zero_Deps-22C55E?style=for-the-badge" alt="Zero build" />
  <img src="https://img.shields.io/badge/Studio_Builder-Ready-8B5CF6?style=for-the-badge" alt="Studio Builder Ready" />
  <img src="https://img.shields.io/badge/AI-Ready-F59E0B?style=for-the-badge" alt="AI Ready" />
</p>

<h1 align="center">VA Studio HTML Starter — Consultation Booking</h1>

<p align="center">
  <strong>A premium 1:1 consultation booking page with advisor showcase, date/time pickers, and live summary.</strong>
</p>

<p align="center">
  Hero imagery, advisor avatar stack, G2-style rating card, date pills, time-slot grid,<br/>
  and an order-summary sidebar — all in pure HTML/CSS with a tiny sprinkle of vanilla JS.
</p>

<p align="center">
  <a href="#quick-start">Quick Start</a> &bull;
  <a href="#sections">Sections</a> &bull;
  <a href="#studio-builder-integration">Studio Integration</a> &bull;
  <a href="#customizing">Customizing</a>
</p>

---

## Quick Start

```bash
python -m http.server 8000
# or
npx serve .
```

Open [http://localhost:8000](http://localhost:8000).

## Sections

- **Sticky nav** — brand mark + underlined active tab
- **Hero visual** — full-bleed Unsplash image with a floating advisor card (avatar stack, rating, 4.9 stars from 1,840 sessions)
- **Copy block** — eyebrow pill, Playfair Display headline, check-list perks
- **Booking form card** — service select, date strip (6 pills), time grid (6 slots), contact fields, notes textarea
- **Live summary** — service / when / total with a "Confirm booking" CTA
- **Success state** — appears on submit with confirmation message and manage-booking link

## Studio Builder Integration

- Form controls expose predictable IDs (`#service`, `#name`, `#email`, `#notes`) for Studio data-binding
- Date/time pills use semantic radio inputs — AI can read current selection without DOM scraping
- External imagery loads from Unsplash via stable photo IDs — safe to swap for Studio-hosted assets
- Event handlers (`submit`, `click`) are bundled in one script block at the bottom — easy to replace with Studio hooks

## Tech Stack

| Layer | Technology |
|-------|-----------|
| **Markup** | HTML5 forms with real `<input>`/`<select>` controls |
| **Styling** | CSS3, grid + flex layout |
| **Fonts** | Inter + Playfair Display (Google Fonts) |
| **Images** | Unsplash (stable photo IDs) |
| **Avatars** | pravatar.cc |
| **Icons** | Inline SVG |

## Project Structure

```
va_studio_html_starter_booking/
├── index.html      # Booking page
├── styles.css      # Design tokens, pill / grid styles
└── README.md
```

## Customizing

- **Services:** edit the `<option>` list inside `#service`
- **Dates:** the `.date-strip` pills — replace the hard-coded Mon-Sat with a Studio-driven loop
- **Time slots:** `.time-grid` — swap for your business hours
- **Hero image:** replace the Unsplash URL at the top of `.booking-visual`
- **Advisor avatars:** pravatar URLs inside `.advisor-stack`

## License

MIT

---

<p align="center">
  Part of the <strong>VA Studio</strong> starter family · Built for rapid prototyping with an AI copilot.
</p>
