# Award-Winning Website

A high-fidelity, award-style landing page built with React, Vite, and Tailwind CSS. It features GSAP-powered animations, immersive video backgrounds, and polished UI components that emulate a premium interactive product experience.

## Features

- Dynamic hero section with animated video transitions
- Bento-style feature grid with subtle 3D tilt interactions
- Smooth scroll-triggered effects using GSAP + ScrollTrigger
- Responsive, mobile-first layout with Tailwind CSS
- Reusable components: `Navbar`, `Hero`, `About`, `Features`, `Story`, `Contact`, `Footer`
- Custom fonts, color system, and design tokens in Tailwind config

## Tech Stack

- React 18, Vite
- Tailwind CSS, PostCSS, Autoprefixer
- GSAP, @gsap/react, ScrollTrigger
- React Icons
- ESLint (React, Hooks, Refresh plugins)

## Project Structure

```
.
├── index.html
├── public/
│   ├── img/            # WebP images and icons
│   ├── videos/         # MP4 background/feature videos
│   └── fonts/          # Custom web fonts
├── src/
│   ├── components/     # Reusable UI components
│   ├── App.jsx         # Main app layout and sections
│   ├── index.css       # Tailwind and component styles
│   └── main.jsx        # React entry point
├── tailwind.config.js  # Theme, colors, fonts
├── postcss.config.js   # PostCSS pipeline
├── vite.config.js      # Vite configuration
└── package.json
```

## Getting Started

### Prerequisites
- Node.js 18+

### Install
```bash
npm install
```

### Development
```bash
npm run dev
```
This starts the Vite dev server with HMR at a local URL.

### Build
```bash
npm run build
```
Outputs a production build to `dist/`.

### Preview (local production)
```bash
npm run preview
```

## Configuration Notes

- Tailwind is configured in `tailwind.config.js` with custom fonts (`zentry`, `general`, `circular-web`, `robert-*`) and a branded color palette.
- GSAP `ScrollTrigger` is registered in components that use it (e.g., `Hero.jsx`), enabling scroll-based animation timelines.
- Media assets live in `public/` and are referenced in components via relative paths (e.g., `videos/hero-1.mp4`).

## Key Components

- `Hero.jsx`: Animated hero with layered videos and reveal transitions
- `Features.jsx`: Bento grid with 3D tilt (`BentoTilt`) and looping video cards
- `Navbar.jsx`, `Footer.jsx`: Site chrome
- `About.jsx`, `Story.jsx`, `Contact.jsx`: Section content
- `Button.jsx`, `AnimatedTitle.jsx`, `RoundedCorners.jsx`: UI primitives and effects

## Accessibility & Performance

- Uses semantic HTML within React components
- Optimized media formats (WebP, MP4)
- Responsive layout and typography
- Animations tuned for smoothness with GPU-accelerated transforms
