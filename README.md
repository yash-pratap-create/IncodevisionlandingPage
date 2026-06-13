# ⬡ Incodevision — Landing Page

> **Build the Future, One Line at a Time.**  
> A sleek, animated product landing page for the Incodevision developer platform.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat&logo=three.js&logoColor=white)

---

## ✨ Overview

This is a fully static, single-page marketing site for **Incodevision** — a fictional developer tooling platform currently in Public Beta. It is designed to showcase the brand's core value proposition with a premium, modern UI that includes a live 3D interactive visualization, animated feature cards, a stats strip, and an email sign-up CTA.

No build tools or frameworks are required — just HTML, CSS, and vanilla JavaScript.

---

## 🚀 Features

| Feature | Description |
|---|---|
| **3D Hero Scene** | Interactive holographic crystal gem rendered with Three.js — responds to mouse movement in real time |
| **Animated Shader** | Custom GLSL vertex/fragment shader with Fresnel rim lighting, scanline shimmer, and animated colour blending |
| **Orbiting Rings & Satellites** | Torus rings and mini octahedron gems orbit the central crystal independently |
| **Particle Field** | 1,400 coloured particles drift slowly around the scene |
| **Scroll-Reveal Cards** | Feature cards fade-in via `IntersectionObserver` as they enter the viewport |
| **Sticky Navbar** | Header gains a frosted-glass backdrop on scroll; active link updates as you scroll through sections |
| **Mobile Hamburger Menu** | Responsive nav that collapses into a hamburger toggle on small screens |
| **Email CTA Form** | Validated email input with a success-state animation on submit |
| **Dark Mode Design** | Full dark palette with purple/cyan/emerald gradient accents throughout |
| **Zero Dependencies** | No npm, no bundler — opens directly in any modern browser |

---

## 📁 Project Structure

```
landingpage/
├── index.html   # Full page markup, Three.js scene, and page behaviour scripts
└── style.css    # All styling — design tokens, layout, animations, responsive rules
```

---

## 🖥️ Getting Started

Because this is a pure static site, there is no installation or build step needed.

### Option 1 — Open directly

Double-click `index.html` in your file explorer to open it in your default browser.

### Option 2 — Local dev server (recommended)

A local server avoids any CORS quirks with fonts or external scripts:

```bash
# Using Python (built into most systems)
python -m http.server 3000

# Using Node.js (if installed)
npx serve .

# Using VS Code
# Install the "Live Server" extension and click "Go Live" in the status bar
```

Then navigate to `http://localhost:3000`.

---

## 🎨 Design System

The visual identity is defined entirely through CSS custom properties in `style.css`:

| Token | Value | Usage |
|---|---|---|
| `--clr-purple` | `#a855f7` | Primary accent, gem shader colour A |
| `--clr-cyan` | `#06b6d4` | Secondary accent, gem shader colour B |
| `--clr-emerald` | `#10b981` | Tertiary accent, gem shader colour C |
| `--bg-base` | `#080810` | Page background |
| `--bg-card` | `rgba(255,255,255,0.04)` | Glassmorphism card surface |
| `--font-sans` | `Inter` | Body & UI text |
| `--font-display` | `Outfit` | Hero and section headings |

---

## 📐 Page Sections

1. **Navbar** — Logo, nav links (Home / About / Contact), and a "Get Started →" CTA button.
2. **Hero** — Headline, subtext, dual CTA buttons, social proof avatars, and the Three.js 3D canvas with floating stat badges.
3. **Stats Strip** — At-a-glance metrics: 10k+ Active Projects, 2.4k Developers, 99.9% Uptime, 4.9★ Rating.
4. **Features** — Three highlighted feature cards (Blazing Fast · Beautiful by Default · Secure & Reliable) plus a perks row.
5. **CTA / Contact** — Email sign-up form with validation and a success state.
6. **Footer** — Brand mark, navigation links, and copyright.

---

## 🛠️ Tech Stack

| Technology | Role |
|---|---|
| **HTML5** | Semantic page structure |
| **CSS3** | Layout, animations, glassmorphism, responsive design |
| **Vanilla JavaScript** | Navbar behaviour, scroll events, IntersectionObserver, form handling |
| **Three.js v0.158** | 3D WebGL scene (crystal gem, rings, particles, satellites) |
| **Google Fonts** | Inter (UI) + Outfit (Display) |

---

## 🌐 Browser Support

Works in all modern evergreen browsers that support:

- **WebGL** (for the Three.js scene)
- **CSS Custom Properties**
- **IntersectionObserver API**

| Browser | Support |
|---|---|
| Chrome / Edge | ✅ Full |
| Firefox | ✅ Full |
| Safari ≥ 15 | ✅ Full |
| IE / Legacy Edge | ❌ Not supported |

---

## 📄 License

© 2026 Incodevision. All rights reserved.
