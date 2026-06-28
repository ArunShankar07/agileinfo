# Agileinfo Techytern Solutions — Website

A single-page marketing site built with React + Vite, animated with Framer Motion,
and using Lucide icons + hand-built inline SVG brand logos for the tech stack section.

## Requirements

- Node.js 18+ (Node 20 LTS recommended)
- npm 9+ (comes with Node)

## Getting started

```bash
# 1. Install dependencies
npm install

# 2. Start the dev server (opens http://localhost:5173)
npm run dev
```

## Available scripts

| Command           | What it does                                      |
|--------------------|----------------------------------------------------|
| `npm run dev`      | Starts the Vite dev server with hot reload          |
| `npm run build`    | Builds an optimized production bundle into `dist/`  |
| `npm run preview`  | Serves the production build locally for a final check |
| `npm run lint`     | Runs ESLint over the project                         |

## Project structure

```
agileinfo-site/
├── index.html              # HTML entry point
├── package.json
├── vite.config.js
├── eslint.config.js
├── public/
│   └── favicon.svg
└── src/
    ├── main.jsx             # React root — mounts <App />
    └── App.jsx              # The entire site (Navbar, Hero, Services,
                              # Portfolio, Tech Stack, Testimonials, Footer, etc.)
```

Everything — sections, animations, color tokens, and the inline SVG tech-stack
logos (React, Next.js, Node.js, Python, Java, C, C++, Flutter, MongoDB, MySQL,
AWS, Firebase, Docker, GraphQL, TypeScript) — lives in `src/App.jsx`, exactly as
it was authored. Fonts (Inter + Space Grotesk) are loaded from Google Fonts via
a `<link>` tag rendered inside the component itself, so no extra setup is needed.

## Deploying

After `npm run build`, the `dist/` folder is a static site you can deploy to
Vercel, Netlify, GitHub Pages, S3/CloudFront, or any static host.

```bash
npm run build
npm run preview   # sanity-check the production build locally first
```
