# Personal Portfolio — Jeffry

A high-performance, minimalist personal portfolio built with **Vue 3**, **Vite**, and **Tailwind CSS**. Designed with a **Black Glossy / Glassmorphic** aesthetic, fully responsive, and optimized for ultra-fast static rendering.

## Technical Architecture & Stack

- **Framework:** Vue 3 (Composition API)
- **Build Tool:** Vite 5
- **Styling:** Tailwind CSS 3 (Custom Monochromatic Theme)
- **State Management:** Vue Reactive Store (`src/store.js`) for Bilingual Switching (ID / EN)
- **Form Handling:** Formspree API Integration
- **Deployment:** Vercel via GitHub Integration

## File Structure

- `src/components/Navbar.vue`: Responsive Header, Drawer, and Language Switcher
- `src/components/Hero.vue`: Intro Section & Resume Link
- `src/components/AboutSkills.vue`: Philosophy & Monochrome Pill Badges
- `src/components/Projects.vue`: Featured Projects, Metric Bars, and Action CTAs
- `src/components/Experience.vue`: Career Storytelling & Credentials
- `src/components/Contact.vue`: Contact Cards & Message Transmission Form
- `src/store.js`: Global Reactive Store for Language Switching

## Maintenance Workflow

Push changes directly to the `master` branch to trigger an automatic Vercel build:

```bash
git add .
git commit -m "Update documentation and content"
git push -u origin master
```
