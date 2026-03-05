<div align="center">

# 🍗 KFC Landing Page Clone (KFC.pk UI)

A responsive **KFC.pk landing page clone** built with **HTML + Tailwind CSS** and bundled with **Vite**.  
Includes an interactive **mobile sidebar menu**, animated hover effects, and smooth in-page navigation.

<!-- Replace the demo link below with your actual URL if deployed -->
🌐 **Live Demo:** https://your-project.vercel.app  
🐛 **Report Bug:** ../../issues · ✨ **Request Feature:** ../../issues

<img src="" alt="Landing Page Preview" width="100%" />

</div>

---

## 🧭 Table of Contents
- [📌 About](#-about)
- [✨ Features](#-features)
- [📱 Responsive Design](#-responsive-design)
- [🧰 Tech Stack](#-tech-stack)
- [🗂️ Project Structure](#️-project-structure)
- [🚀 Run Locally](#-run-locally)
- [🏗️ Build & Preview (Production)](#️-build--preview-production)
- [🎨 Customization](#-customization)
- [🙏 Credits](#-credits)
- [📄 License](#-license)

---

## 📌 About

This project recreates the look and feel of a **KFC-style promotional landing page** with:
- 🧭 a fixed top navigation bar
- 🖼️ a hero banner + CTA button
- 🍔 multiple product sections (Explore Menu, Best Sellers, Top Deals)
- 🧱 promotional image blocks
- 🔗 a footer with social + app store links

It’s a great practice project for **Tailwind layouts**, **hover animations**, and **responsive UI composition**.

---

## ✨ Features

### 🧩 Interactive UI
- 🍔 **Mobile sidebar menu (hamburger → drawer)**
  - Implemented using a hidden checkbox + Tailwind `peer` / `peer-checked:*` utilities.
  - Drawer slides in/out with `transform` + `transition` classes.
- 🧭 **Smooth scrolling navigation**
  - Anchor links scroll smoothly using a small jQuery script.

### 🛍️ Landing-page sections
- 🦸 **Hero section**
  - Large banner image and a “REORDER” CTA button.
- 🧾 **Explore Menu grid**
  - Category cards with hover elevation (`hover:-translate-y-3`) and scaling (`hover:scale-110`).
  - Decorative accent bars + dots animate on hover using `group-hover:*`.
- ⭐ **Best Sellers**
  - Product cards with price ribbons and hover animations.
- 🔥 **Top Deals**
  - Deal cards with “+ ADD TO BUCKET” CTA buttons.
- 🖼️ **Promo blocks**
  - Image grid + featured CTA panel (“Explore Menu”).
- 🧾 **Footer**
  - Social icons + quick links + store badges.

---

## 📱 Responsive Design

The page uses Tailwind’s responsive utilities to progressively reveal more content as the screen gets larger:

- 📲 **Small screens**
  - Clean layout and fewer visible cards for readability.
  - Sidebar (drawer) navigation available via hamburger.
- 💻 **Medium / Large screens**
  - Extra cards and UI elements appear using:
    - `hidden md:block`
    - `hidden lg:block`
    - `hidden xl:block`

This keeps the UI minimal on mobile and richer on desktop without additional JS.

---

## 🧰 Tech Stack

- 🧱 **HTML5**
- 🎨 **Tailwind CSS** (via `style.css` using `@tailwind base/components/utilities`)
- ⚡ **Vite** (dev server + production build)
- 🧪 **PostCSS + Autoprefixer**
- 🌀 **jQuery (CDN)** for smooth scrolling

---

## 🗂️ Project Structure

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

## 🚀 Run Locally

### 1️⃣ Install dependencies
```bash
npm install
```

### 2️⃣ Start dev server
```bash
npm run dev
```

Vite will print a local URL (commonly `http://localhost:5173`).

---

## 🏗️ Build & Preview (Production)

### 📦 Build
```bash
npm run build
```

### 🔍 Preview the build
```bash
npm run preview
```

The production HTML is output to:
- `dist/index.html`  
and references hashed assets under:
- `dist/assets/*`

---

## 🎨 Customization

### 🖼️ Update images / icons
All visual assets are loaded from the `Image/` folder (example: `Image/main.jpg`, `Image/kfc.png`, menu icons, etc.).  
Replace files there (keeping names) or update `<img src="...">` paths inside `index.html`.

### 🎯 Change theme colors
Most of the theme is done using Tailwind utility classes:
- 🟥 primary accents: `bg-red-600`, `text-red-600`
- ⚪ backgrounds: `bg-white`, `bg-slate-100`, `bg-slate-200`

To globally redesign:
- edit classes in `index.html`, or
- extend Tailwind theme in `tailwind.config.js`.

---

## 🙏 Credits

👨‍🍳 UI inspired by KFC-style landing pages for educational/practice purposes.

---

## 📄 License

📌 Add a license if you plan to distribute this publicly (MIT is common for practice projects).
