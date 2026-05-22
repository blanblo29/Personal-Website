# Pratyush Sharma — Author Portfolio & Interactive Audio Engine

A custom, responsive single-page web application built to showcase published literary works and explore browser-based digital signal processing. The project integrates vanilla web technologies with interactive design patterns, real-time audio synthesis, and a cinematic branded loading experience.

---

## 🚀 Key Features & Engineering Mechanics

### 🎬 Branded Animated Intro Loader (BLN-DSPTCH)
A fully custom splash screen featuring a staggered letter blow-in sequence with skew and blur transitions, followed by a **canvas-based particle disintegration system**. Each letter spawns dozens of physics-driven particles (with gravity, drag, wobble, and rotation) that crumble to dust before the main content loads. Built entirely with the Canvas 2D API and vanilla JS — no libraries.

### 🔊 Real-Time Audio Synthesis
Implements the native browser **Web Audio API** in two distinct contexts:
- **Loader sound design** — procedurally generated wind and crumble effects using `BiquadFilter`, `GainNode`, and `BufferSource` nodes, timed precisely to the visual animation sequence.
- **Ambient audio engine** — a toggleable atmospheric soundscape that runs independently of media files, synthesised in real time.

### 🔐 Cipher-Text Vault Mechanic
A hover-driven text decryption interaction on the Vault section. Scrambled placeholder characters progressively resolve into readable content as the user engages, with a configurable revert timeout on mouse leave. Driven by custom interval-based animation logic and CSS flicker keyframes.

### 🖱️ Cursor Spotlight Effect
A dynamic `radial-gradient` overlay that tracks the user's cursor position via CSS custom properties (`--cursor-x`, `--cursor-y`), casting a subtle ambient light effect across targeted sections for an immersive reading environment.

### 🌆 Handcrafted CSS/SVG Environmental Illustration
A fully code-rendered streetlight-in-the-rain scene on the hero section — built with layered CSS geometry, SVG turbulence filters, and animated rain — adding cinematic atmosphere without any image assets.

### ⚡ Asynchronous UI Interactions
Custom scroll-triggered reveal transitions and a marquee ticker driven by optimised Vanilla JavaScript event listeners and `IntersectionObserver`. Navigation, section transitions, and hover states are handled with clean, paint-efficient DOM manipulation.

### 📱 Fully Responsive Layout
Mobile-first breakpoints with a hamburger nav, fluid typography via `clamp()`, and adaptive grid restructuring across all content sections.

### 🚀 Production Deployment
Configured for automated production builds and secure hosting pipelines via Vercel.

---

## 🛠️ Tech Stack & Architecture

| Layer | Technology |
|---|---|
| **Structure** | HTML5, Semantic DOM |
| **Styling & Motion** | CSS3 — custom keyframe animations, CSS custom properties, viewport-relative transitions, SVG filters |
| **Logic & Interactivity** | Vanilla JavaScript (ES6+) |
| **Audio Engine** | Web Audio Context API — BiquadFilter, GainNode, BufferSource |
| **Visual Engine** | Canvas 2D API — particle system, physics simulation |
| **Fonts** | Google Fonts — Cormorant Garamond, Space Mono, Raleway |
| **Version Control** | Git |
| **Deployment** | Vercel |

---

## 📂 Repository Structure

```text
├── IMAGES/          # Optimised graphic assets and UI illustrations
├── .gitignore       # Production build and environment exclusion rules
├── index.html       # Application entry point — all structure, styles, and logic
└── README.md        # Technical project documentation
```

---

## 🤝 Development Note

This project was developed with the assistance of **Claude (Anthropic)**, an AI assistant, as a collaborative engineering and design tool. AI assistance was used to accelerate implementation of specific technical components — including the Web Audio synthesis logic, the canvas particle system, and the cipher-text animation mechanic — while all creative direction, content, architectural decisions, and final integration were authored and owned by me.

The use of AI tooling is treated here the same way one might use a reference implementation, a Stack Overflow answer, or a third-party library: as a resource that informs and accelerates work, not a replacement for the developer's understanding or intent.

---

*Built by Pratyush Sharma — author of* The Price of Silence: A Delhi Noir.
