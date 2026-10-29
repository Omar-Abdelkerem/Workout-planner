# Workout-planner

A collaborative university course project for **SW 302: User Interface Development** (Fall 2026).  
**Fitness & Workout Planner** frontend application built with HTML5 and Tailwind CSS.

---

## Member 3: Routine Builder and Active Workout Tracker

### Pages Delivered
1. **Routine Builder (Desktop)**: [`frontend/routine-builder.html`](file:///mnt/c/Users/oa304/OneDrive/Desktop/UI%20project/frontend/routine-builder.html)
   - Desktop and tablet responsive layout for creating, reordering, and configuring routine sets, target reps, and rest intervals.
2. **Routine Builder (Mobile)**: [`frontend/routine-builder-mobile.html`](file:///mnt/c/Users/oa304/OneDrive/Desktop/UI%20project/frontend/routine-builder-mobile.html)
   - Dedicated 390px-first mobile view (iPhone 16 viewport) with collapsible drawer and fixed bottom navigation bar.
3. **Active Workout Tracker (Desktop)**: [`frontend/active-workout.html`](file:///mnt/c/Users/oa304/OneDrive/Desktop/UI%20project/frontend/active-workout.html)
   - Live workout session interface with elapsed timer, workout volume metrics, rest timer widget, and set performance tables.
4. **Active Workout Tracker (Mobile)**: [`frontend/active-workout-mobile.html`](file:///mnt/c/Users/oa304/OneDrive/Desktop/UI%20project/frontend/active-workout-mobile.html)
   - Ergonomic gym-mode mobile interface designed for one-handed operation with sticky top bar, 44px+ tap targets, and large checkboxes.

### Setup and Build Instructions
All Tailwind CSS styles are compiled locally via the Tailwind CLI without any external CDN dependencies.

```bash
# Navigate to the frontend directory
cd frontend

# Install dependencies (Tailwind CLI v4)
npm install

# Build compiled CSS bundle
npm run build:css

# Watch for real-time CSS changes during development
npm run watch:css
```

The compiled CSS output is committed to [`frontend/dist/output.css`](file:///mnt/c/Users/oa304/OneDrive/Desktop/UI%20project/frontend/dist/output.css) so the pages render out-of-the-box in any browser without requiring an active build process.

### Accessibility (WCAG 2.1 AA) Highlights
- **100% Automated Axe-Core Conformance**: 0 accessibility violations across all Member 3 pages.
- **Strict Semantic Landmarks**: `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`, exactly one `<h1>` per page.
- **Form Controls & ARIA**: Visible linked `<label for="id">` on every input; explicit `aria-label` on all icon-only buttons; `aria-current="page"` on active navigation links; `aria-expanded` and `aria-controls` on mobile drawer buttons.
- **Accessible Timers & Tables**: Timers implement `role="timer"` with `aria-live="polite"`; set tables use real semantic HTML `<table>` elements with `<th scope="col">` and `<th scope="row">`.
- **Keyboard Navigation & Hit Targets**: Visible focus rings (`focus-visible:ring-2`), "Skip to main content" links, and minimum 44×44px touch targets.

### Documentation Links
- **Design System Summary**: [`docs/design-summary.md`](file:///mnt/c/Users/oa304/OneDrive/Desktop/UI%20project/docs/design-summary.md)
- **Accessibility Audit Report**: [`docs/a11y-report.md`](file:///mnt/c/Users/oa304/OneDrive/Desktop/UI%20project/docs/a11y-report.md)
- **Figma AI Prompts**: [`docs/figma-prompt.md`](file:///mnt/c/Users/oa304/OneDrive/Desktop/UI%20project/docs/figma-prompt.md)
- **Figma Links**: [`docs/figma-link.md`](file:///mnt/c/Users/oa304/OneDrive/Desktop/UI%20project/docs/figma-link.md)
- **Lighthouse / Axe Audit Artifacts**: [`docs/lighthouse/`](file:///mnt/c/Users/oa304/OneDrive/Desktop/UI%20project/docs/lighthouse/)
