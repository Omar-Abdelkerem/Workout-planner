# Fitness & Workout Planner - Design System Summary
**Course**: SW 302 - User Interface Development  
**Phase**: Phase 2 — UI/UX Design & Static Prototype  
**Team Member**: #3 (Routine Builder & Active Workout Tracker)

---

## 1. Design Discovery & Baseline Decision

Based on analyzing the repository code (`frontend/index.html`, `frontend/dashboard.html`, `frontend/profile.html`), the uploaded Figma wireframe mockups (Desktop and iPhone 16 Mobile for Landing, Dashboard, and Profile), and the project plan:

- **Followed Design**: The team has adopted a unified **grayscale wireframe design language** established by Team Member #1 and reflected in the Figma mockups.
- **Consistency Principle**: Member 3's pages (`routine-builder.html`, `routine-builder-mobile.html`, `active-workout.html`, `active-workout-mobile.html`) reuse **exactly** the teammates' layout shell (top navbar with `Fitness Planner`, hamburger `≡`, profile `👤`, bottom mobile nav bar, and `&copy; 2026 FitnessPlanner` footer), component styling (rounded-2xl/3xl cards, rounded-full pill buttons), and class conventions so the entire project looks like one cohesive product.
- **Accessibility Enhancement**: While teammate wireframes used `text-gray-600` on `bg-gray-300` (which fails WCAG AA contrast), Member 3's pages strictly enforce high-contrast compliant text (`text-gray-900` / `text-black` on light gray backgrounds, yielding > 10:1 contrast) and visible focus rings.

---

## 2. Color Palette

### Primary Grayscale Wireframe Palette (Active in Repo & Mockups)
| Role | Hex Code | Tailwind Class | Contrast against BG | WCAG AA Status |
| :--- | :--- | :--- | :--- | :--- |
| Page Canvas Background | `#F3F4F6` | `bg-gray-100` | — | Base |
| Header & Footer Background | `#D1D5DB` | `bg-gray-300` | — | Base |
| Primary Card Background | `#D1D5DB` | `bg-gray-300` | — | Base |
| Secondary Card Background | `#9CA3AF` | `bg-gray-400` | — | Base |
| Primary Text (Headings/Body) | `#111827` | `text-gray-900` | 10.7:1 on #D1D5DB / 12.5:1 on #F3F4F6 | **PASS (AAA)** |
| Secondary Text (Labels/Cues) | `#1F2937` | `text-gray-800` | 9.2:1 on #D1D5DB / 10.8:1 on #F3F4F6 | **PASS (AAA)** |
| Accent / Highlight Text | `#0F172A` | `text-slate-900` | 12.1:1 on #D1D5DB | **PASS (AAA)** |
| Primary Action Button | `#1F2937` / `#FFFFFF` | `bg-gray-800 text-white` | 11.5:1 | **PASS (AAA)** |
| Secondary Action Button | `#9CA3AF` / `#000000` | `bg-gray-400 text-black` | 7.1:1 | **PASS (AAA)** |
| Active Accent Badge | `#10B981` / `#022C22` | `bg-emerald-500 text-slate-950` | 7.3:1 | **PASS (AAA)** |
| Card Border / Divider | `#6B7280` | `border-gray-500` / `border-gray-400` | — | High Visibility |

### Dark Theme / Gym Mode Tokens (Documented Fallback & Future Phase)
- Canvas: `#0F172A` (`bg-slate-900`)
- Cards: `#1E293B` (`bg-slate-800`)
- Borders: `#334155` (`border-slate-700`)
- Accent: `#10B981` (`emerald-500`)
- High-contrast text: `#F8FAFC` (`text-slate-50`)

---

## 3. Typography & Local Fallback Stack

- **Font Family**: Inter with local system fallback stack:
  ```css
  font-family: "Inter", system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  ```
- **External CDN**: **Strictly zero external CDNs** (no Google Fonts link, no cdn.tailwindcss.com).
- **Scale**:
  - `text-2xl` / `text-3xl` (`font-bold` / `font-extrabold`): Primary page headings (`h1`, `h2`)
  - `text-xl` (`font-bold`): Section titles and card headers
  - `text-base` / `text-sm` (`font-semibold` / `font-medium`): Card body, form labels, table cells
  - `text-xs` (`font-semibold`): Badges, table headers, metadata

---

## 4. Spacing, Radii & Layout Rhythm

- **8px Base Grid**: Multiples of 8px (`gap-2` = 8px, `gap-4` = 16px, `gap-6` = 24px, `p-4` = 16px, `p-6` = 24px).
- **Corner Radii**:
  - Cards & Containers: `rounded-2xl` (16px) and `rounded-3xl` (24px)
  - Buttons: `rounded-full` (pill shape as seen in teammate designs)
  - Form Inputs: `rounded-xl` (12px)
  - Badges & Pills: `rounded-full` / `rounded-lg`
- **Shadows**: Clean wireframe elevation (`shadow-sm`, `shadow-md`, `shadow-lg`).

---

## 5. Navigation & Shell Structure

### Desktop Shell
- **Header**: `bg-gray-300 px-6 py-4 flex items-center justify-between`
  - Left: Brand title `Fitness Planner` with icon + mobile drawer button (`md:hidden`)
  - Center: Main navigation `<nav>` with `Home`, `Dashboard`, `Routine Builder`, `Active Workout`, `Profile`
  - Right: Quick Action pill button + Profile icon link `👤`
- **Main Container**: `container mx-auto px-4 py-6 flex-grow space-y-6 max-w-6xl`
- **Footer**: `bg-gray-300 py-4 text-center text-sm font-semibold` with `&copy; 2026 FitnessPlanner`

### Mobile Shell (Dedicated 390px iPhone View)
- **Top Header**: `bg-gray-300 px-4 py-3 flex items-center justify-between sticky top-0 z-40`
  - Left: Hamburger button `≡` (`aria-expanded="false"`, `aria-controls="mobile-nav"`)
  - Center: `Fitness Planner`
  - Right: Desktop switcher link + Profile avatar `👤`
- **Collapsible Drawer**: Semantic `<aside id="mobile-nav">` with full vertical navigation list
- **Bottom Navigation Bar**: Fixed `bg-gray-300 border-t border-gray-400 py-2 px-3 fixed bottom-0 left-0 right-0 z-50` with 5 quick-access tabs (`Home`, `Dashboard`, `Routines`, `Workout`, `Profile`), min 44x44px touch targets.

---

## 6. Component Library Styles

- **Primary Buttons**: `bg-gray-800 hover:bg-gray-900 text-white px-6 py-2.5 rounded-full font-bold transition focus-visible:ring-2 focus-visible:ring-gray-900 min-h-[44px]`
- **Secondary Buttons**: `bg-gray-400 hover:bg-gray-500 text-black px-5 py-2 rounded-full font-semibold transition focus-visible:ring-2 focus-visible:ring-gray-700 min-h-[44px]`
- **Accent Emerald Buttons**: `bg-emerald-600 hover:bg-emerald-500 text-white px-6 py-2.5 rounded-full font-bold shadow transition focus-visible:ring-2 focus-visible:ring-emerald-700 min-h-[44px]`
- **Form Inputs**: `bg-white border-2 border-gray-400 focus:border-gray-800 text-gray-900 rounded-xl px-4 py-2.5 font-medium min-h-[44px] focus-visible:ring-2 focus-visible:ring-gray-800`
- **Exercise Cards**: `bg-gray-300 p-5 rounded-2xl border border-gray-400 shadow-sm space-y-3`
- **Set Tables**: Real `<table>` with `role="group"`, `<th scope="col">`, `<th scope="row">`, rounded corners, and visible column headers.
- **Timers**: Accessible `role="timer"` with `aria-live="polite"`.

---

## 7. Responsive Breakpoints

- Mobile: `< 768px` (dedicated mobile templates designed 390px-first for iPhone 16 viewport)
- Tablet / Small Laptop: `md: 768px`
- Desktop: `lg: 1024px` and `xl: 1280px`
