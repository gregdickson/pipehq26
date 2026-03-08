# PipeHQ Website

The official website for **PipeHQ** — The AI Operating System for Trade Businesses.

Built with [Astro](https://astro.build), [Tailwind CSS v4](https://tailwindcss.com), and TypeScript.

## Getting Started

```bash
# Install dependencies
npm install

# Start the dev server (http://localhost:4321)
npm run dev

# Build for production
npm run build

# Preview the production build
npm run preview
```

## Project Structure

```
src/
├── assets/              # Images, fonts, and other static assets
├── components/
│   ├── Header.astro     # Sticky navigation with CTA
│   ├── Footer.astro     # Footer with final CTA banner
│   └── sections/        # Reusable page sections
│       ├── Hero.astro
│       ├── SocialProofBar.astro
│       ├── ProblemAgitation.astro
│       ├── HowItWorks.astro
│       ├── FeaturesGrid.astro
│       ├── Testimonials.astro
│       └── FAQ.astro
├── layouts/
│   └── BaseLayout.astro # Base HTML layout with SEO meta tags
├── pages/
│   ├── index.astro      # Homepage
│   ├── pricing.astro
│   ├── demo.astro       # Lead capture / booking page
│   ├── contact.astro
│   ├── how-it-works.astro
│   ├── faq.astro
│   ├── about/
│   ├── platform/        # Feature pages (9 product pillars)
│   ├── industries/      # Industry-specific pages (10 trades)
│   ├── compare/         # Comparison pages (vs competitors)
│   ├── blog/
│   └── case-studies/
├── styles/
│   └── global.css       # Tailwind import + design tokens
public/
├── favicon.svg
└── images/
```

## Design System

Design tokens are defined in `src/styles/global.css` using Tailwind CSS v4's `@theme` directive:

- **Primary:** `#2563eb` (Blue — trust, reliability)
- **Accent:** `#f97316` (Orange — energy, action)
- **Font:** Inter (system-ui fallback)

## VS Code Setup

This project includes recommended VS Code settings. When you open the project, VS Code will suggest installing the recommended extensions:

- Astro
- Tailwind CSS IntelliSense
- Prettier
- GitLens
- ESLint

## Architecture Notes

This site follows the **9-section page anatomy** from the `blue-collar-conversion-design` skill, combined with the aesthetic principles from the `polished-astro-theme-design` skill. Every page is structured for conversion:

1. Navigation & Header (sticky, with CTA)
2. Hero Section (above the fold)
3. Authority & Social Proof Bar
4. Problem & Agitation
5. Solution & How It Works
6. Deep Social Proof (Testimonials)
7. The Offer & Pricing
8. Objection Handling (FAQ)
9. Final CTA & Footer
