<div align="center">

# KFC Landing Page Clone (KFC.pk UI)

A responsive **KFC.pk landing page clone** built with **HTML + Tailwind CSS** and bundled with **Vite**.  
Includes an interactive **mobile sidebar menu**, animated hover effects, and smooth in-page navigation.

<!-- Replace the demo link below with your actual Vercel URL if deployed -->
[Live Demo](https://your-project.vercel.app) · [Report Bug](../../issues) · [Request Feature](../../issues)

<img src="Image/.jpg" alt="Landing Page Preview" width="100%" />

</div>

---

## Table of Contents
- [About](#about)
- [Features](#features)
- [Responsive Design](#responsive-design)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Run Locally](#run-locally)
- [Build & Preview (Production)](#build--preview-production)
- [Customization](#customization)
- [Credits](#credits)
- [License](#license)

---

## About

This project recreates the look and feel of a **KFC-style promotional landing page** with:
- a fixed top navigation bar,
- a hero banner + CTA button,
- multiple product sections (Explore Menu, Best Sellers, Top Deals),
- promotional image blocks,
- and a footer with social + app store links.

It’s a great practice project for **Tailwind layouts**, **hover animations**, and **responsive UI composition**.

---

## Features

### Interactive UI
- **Mobile sidebar menu (hamburger → drawer)**
  - Implemented using a hidden checkbox + Tailwind `peer` / `peer-checked:*` utilities.
  - Drawer slides in/out with `transform` + `transition` classes.
- **Smooth scrolling navigation**
  - Anchor links scroll smoothly using a small jQuery script.

### Modern landing-page sections
- **Hero section**
  - Large banner image and a “REORDER” CTA button.
- **Explore Menu grid**
  - Category cards with hover elevation (`hover:-translate-y-3`) and scaling (`hover:scale-110`).
  - Decorative accent bars + dots animate on hover using `group-hover:*`.
- **Best Sellers + Top Deals**
  - Product cards with pricing ribbons, hover motion, and “Add to Bucket” CTA buttons.
- **Promo blocks**
  - Two-image row + a text/CTA panel (“Explore Menu”).
- **Footer**
  - Social icons + navigation links + store badges.

---

## Responsive Design

Your page uses Tailwind’s responsive utilities to progressively reveal more content as screen size increases:

- On **small screens**:
  - Focus is on essential content and fewer cards for readability.
  - Sidebar (drawer) navigation is available via hamburger icon.
- On **medium/large screens**:
  - More cards appear using patterns like:
    - `hidden md:block`
    - `hidden lg:block`
    - `hidden xl:block`

This keeps layout clean on mobile and richer on desktop, without needing extra JS.

---

## Tech Stack

- **HTML5**
- **Tailwind CSS** (via `style.css` using `@tailwind base/components/utilities`)
- **Vite** (dev server + production build)
- **PostCSS + Autoprefixer**
- **jQuery (CDN)** for smooth scrolling

---

## Project Structure

```text
.
├─ index.html              # Main landing page
├─ style.css               # Tailwind entry file (@tailwind directives)
├─ tailwind.config.js      # Tailwind config (content: index.html + root html/js)
├─ postcss.config.js       # PostCSS config
├─ package.json            # Vite scripts
├─ Image/                  # Images/icons used by the page
└─ dist/                   # Production build output (Vite)
```

---

## Run Locally

### 1) Install dependencies
```bash
npm install
```

### 2) Start dev server
```bash
npm run dev
```

Vite will print a local URL (commonly `http://localhost:5173`).

---

## Build & Preview (Production)

### Build
```bash
npm run build
```

### Preview the build
```bash
npm run preview
```

The production HTML is output to:
- `dist/index.html`
and references hashed assets under:
- `dist/assets/*`

---

## Customization

### Update images / icons
All visual assets are loaded from the `Image/` folder (example: `Image/main.jpg`, `Image/kfc.png`, menu icons, etc.).  
Replace files there (keeping names) or update the `<img src="...">` paths inside `index.html`.

### Change theme colors
Most of the theme is done using Tailwind utility classes:
- primary accents use `bg-red-600`, `text-red-600`
- backgrounds use `bg-white`, `bg-slate-100`, `bg-slate-200`

To globally redesign:
- adjust utility classes in `index.html`, or
- extend Tailwind theme in `tailwind.config.js`.

---

## Credits

UI inspired by KFC-style landing pages for educational and practice purposes.

---

## License

Add a license if you plan to distribute this publicly (MIT is common for UI clones/practice projects).
