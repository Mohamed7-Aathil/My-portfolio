# Mohamed Aathil K — Portfolio

A single-file, responsive personal portfolio website built with plain **HTML, CSS, and JavaScript** (no frameworks, no build step). Just open `index.html` in a browser.

🔗 **Live Preview:** Open `index.html` directly, or deploy to GitHub Pages / Netlify / Vercel.

---

## ✨ Features

- **Single-file build** — HTML, CSS, and JS all combined in one `index.html` for easy hosting anywhere
- **Animated network background** — canvas-based particle system with connecting lines
- **Sticky navbar** — active-link highlighting on scroll + mobile hamburger menu
- **Hero section** — profile photo, name, role, and call-to-action buttons
- **About Me** — intro text + 3 highlight cards (Clean Code, Problem Solver, Fast Learner)
- **Education timeline** — alternating left/right timeline with degree, institution, and CGPA
- **Skills** — categorized (Frontend / Backend / Database & Tools) with animated progress bars that fill on scroll
- **Projects** — card grid with tech-stack tags and a "See More Details" button that opens a popup modal with full project abstracts
- **Contact section** — contact info cards (email, phone, LinkedIn, GitHub) + a working demo contact form
- **Fully responsive** — mobile, tablet, and desktop layouts
- **Scroll-reveal animations** — sections fade/slide in as you scroll

---

## 📁 Project Structure

```
├── assets        # Profileimage & Resume.
├── index.html    # Everything: HTML + CSS (inside <style>) + JS (inside <script>)
└── README.md     # This file
```

---

## 🚀 Getting Started

### Option 1 — Just open it

Double-click `index.html` or open it in any browser. No server, no build step required.

### Option 2 — Run with a local server (recommended for smoother dev experience)

```bash
# Using Python
python3 -m http.server 8000

# Using Node (http-server)
npx http-server .
```

Then visit `http://localhost:8000`.

---

## 🛠️ Customization Guide

| What to change       | Where in `index.html`                                                                                                                                                  |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Profile photo        | `<img class="avatar" src="...">` — replace the placeholder URL with your own image path/URL                                                                            |
| Name, role, tagline  | `<h1>`, `.role`, `.tagline` inside the `.hero` section                                                                                                                 |
| Resume download link | `#resumeBtn` — currently shows an alert; replace with `href="your-resume.pdf" download`                                                                                |
| About text & cards   | `#about` section                                                                                                                                                       |
| Education entries    | `.timeline-item` blocks inside `#education`                                                                                                                            |
| Skills & percentages | `.skill-row` blocks — edit the `%` text and the `data-width` attribute on `.bar-fill`                                                                                  |
| Projects             | `.project-card` blocks inside `#projects`, and matching `.modal-overlay` blocks below for the popup content                                                            |
| Contact details      | `.contact-item` links inside `#contact` (email, phone, LinkedIn, GitHub)                                                                                               |
| Contact form backend | `#contactForm` submit handler in the `<script>` — currently a demo; hook up [Formspree](https://formspree.io), [EmailJS](https://www.emailjs.com), or your own backend |
| Colors / theme       | CSS variables at the top of `<style>`: `--bg`, `--accent1`, `--accent2`, `--gradient`                                                                                  |

---

## 🎨 Color Palette

| Variable     | Value     | Usage                 |
| ------------ | --------- | --------------------- |
| `--bg`       | `#0a0a12` | Page background       |
| `--card`     | `#12121e` | Card backgrounds      |
| `--accent1`  | `#7c5cff` | Primary purple accent |
| `--accent2`  | `#3b8bff` | Secondary blue accent |
| `--text`     | `#e8e8f0` | Primary text          |
| `--text-dim` | `#9797ab` | Secondary/muted text  |

---

## 📱 Responsive Breakpoints

- Desktop: full multi-column layout
- `≤ 900px`: collapses to single-column grids, hamburger nav, stacked timeline

---

## 📌 Tech Used

- HTML5
- CSS3 (custom properties, grid, flexbox, animations)
- Vanilla JavaScript (IntersectionObserver for scroll reveals, Canvas API for background animation)

---

## 📄 License

Free to use and modify for personal portfolio purposes.

---

© 2026 K. Mohamed Aathil. All rights reserved.
