# NEXUS // Human Evolution Initiative
### Cyborg-Themed Responsive Landing Page

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Responsive](https://img.shields.io/badge/Responsive-Yes-00F5FF?style=for-the-badge)

> A fully responsive, single-file cyborg/sci-fi themed landing page built with pure HTML, CSS, and vanilla JavaScript — no frameworks, no dependencies, no build step.

---

## 🔗 Live Demo

> _[Add your GitHub Pages / Vercel / Netlify link here]_

📹 **Demo Recording:** [Google Drive Link](https://drive.google.com/your-link-here) *(viewer access enabled)*

---

## 📸 Preview

| Section | Description |
|---|---|
| Hero | Animated HUD reticle, glitch headline, live stat bar |
| Augmentation | Annotated cyborg body SVG + feature cards |
| Specifications | 6-metric performance grid |
| Phases | 4-step augmentation timeline |
| Enlist | Full-bleed CTA with terminal badge |

---

## ✨ Features

- **Animated HUD targeting reticle** — multi-ring SVG with independently rotating dashed arcs and a pulsing core
- **Glitch text effect** — CSS `clip-path` animation on the hero headline, fires periodically via JS
- **CRT scanline overlay** — full-page `repeating-linear-gradient` with slow scroll animation
- **Scan beam** — neon cyan sweep across the hero on loop
- **Annotated cyborg body diagram** — inline SVG with glowing callout lines for each augmentation module
- **Scroll-reveal animations** — staggered `IntersectionObserver` reveals on all content blocks
- **HUD nav** — fixed top bar with hexagonal clip-path CTA button and underline hover animations
- **Corner bracket decorators** — tactical UI corner accents on hero and CTA sections
- **Blinking terminal cursor** — after hero subtext
- **Fully responsive** — adapts to mobile at 900px and 500px breakpoints
- **`prefers-reduced-motion` support** — all animations disabled for accessibility

---

## 🎨 Design System

### Color Palette

| Token | Hex | Usage |
|---|---|---|
| `--black` | `#050A0E` | Page background |
| `--dark` | `#0A1520` | Alternate section bg |
| `--steel` | `#1A2A3A` | Cards, borders |
| `--cyan` | `#00F5FF` | Primary accent, glow |
| `--magenta` | `#FF006E` | Secondary accent, alerts |
| `--titanium` | `#8A9BAE` | Body text, labels |
| `--chrome` | `#E8F4F8` | Headings, highlights |

### Typography

| Role | Font | Notes |
|---|---|---|
| Display | `Orbitron` (900) | Hero + section headings |
| UI Labels | `Rajdhani` (600–700) | Nav, buttons, eyebrows |
| Body / Data | `Share Tech Mono` | Body copy, terminal readouts |

---

## 📁 File Structure

```
cyborg-landing/
├── index.html     # Complete single-file page (HTML + CSS + JS)
└── README.md      # This file
```

All styles and scripts are embedded in `index.html` — no external files needed beyond Google Fonts (loaded via CDN).

---

## 🚀 Getting Started

### Option 1 — Open directly
```bash
# Clone the repo
git clone https://github.com/your-username/cyborg-landing.git

# Open in browser
open cyborg-landing/index.html
```
No server required — just open the file.

### Option 2 — Local dev server (optional)
```bash
cd cyborg-landing

# Python
python -m http.server 3000

# Node.js (npx)
npx serve .
```
Then visit `http://localhost:3000`.

### Option 3 — Deploy to GitHub Pages
1. Push repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your site will be live at `https://your-username.github.io/cyborg-landing`

---

## 🧩 Sections Breakdown

### 1. Navigation
Fixed HUD-style top bar with logo, nav links (underline on hover), and a hexagonal clip-path CTA button. Becomes translucent with `backdrop-filter: blur` over content.

### 2. Hero
Full-viewport grid layout (text left, visual right). Features:
- Glitch-animated `Orbitron` headline with `::before` / `::after` clip-path layers
- Animated targeting reticle SVG with 3 independently rotating rings
- Cyan scan beam sweeping the section on a 4s loop
- Circuit-board SVG background with dashed paths and node markers
- Stats bar: 847% strength / 12ms neural latency / ∞ uptime

### 3. Augmentation Modules
Two-column grid: feature list on the left, annotated cyborg body diagram on the right. The SVG body diagram uses `filter: feGaussianBlur` glow effects and dashed callout lines for each augment zone.

### 4. Technical Specifications
3-column card grid (collapses to 2 then 1 on mobile). Each card has a left-border reveal animation on hover via CSS `::before` height transition.

### 5. Phases Timeline
4-step roadmap with diamond markers connected by a neon gradient horizontal rule. Markers are styled as `clip-path: polygon` diamonds — filled for completed phases, outlined for pending.

### 6. Enlist CTA
Centred full-bleed section with radial glow background, terminal badge, and dual CTA buttons.

---

## ♿ Accessibility

- Semantic HTML5 elements (`<nav>`, `<section>`, `<footer>`)
- `prefers-reduced-motion` media query disables all animations
- Keyboard-navigable links and buttons
- Sufficient color contrast between `--cyan` / `--magenta` on dark backgrounds
- `crosshair` cursor maintained consistently for thematic immersion

---

## 🛠 Customization

**Change the brand name:** Find `NEXUS` in `index.html` and replace globally.

**Swap accent color:** Override `--cyan` and `--magenta` in `:root`.

**Add a section:** Copy any `<section>` block and adjust content. The `.reveal` class on child elements will auto-animate on scroll via the existing `IntersectionObserver`.

**Change fonts:** Replace the Google Fonts `<link>` and update the `:root` font-family references.

---

## 📋 Browser Support

| Browser | Support |
|---|---|
| Chrome 90+ | ✅ Full |
| Firefox 88+ | ✅ Full |
| Safari 14+ | ✅ Full |
| Edge 90+ | ✅ Full |
| IE 11 | ❌ Not supported |

---

## 📜 License

This project is open source under the [MIT License](LICENSE).

---

<p align="center">
  Built with pure HTML · CSS · JS &nbsp;|&nbsp; No frameworks &nbsp;|&nbsp; No build tools
  <br><br>
  <code>SYS STATUS: ONLINE // BUILD: v4.2.1-ALPHA</code>
</p>
