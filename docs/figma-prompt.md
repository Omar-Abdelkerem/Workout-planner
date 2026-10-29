# Figma AI Generation Prompts: Routine Builder & Active Workout Tracker
**Project**: Fitness & Workout Planner Frontend  
**Course**: SW 302 - User Interface Development  
**Author**: Team Member #3  
**Frames Included**:
1. Routine Builder Desktop (1440×1024)
2. Routine Builder Mobile (390×844)
3. Active Workout Desktop (1440×1024)
4. Active Workout Mobile (390×844)

---

## (A) High-Fidelity Mockups Prompt (Ready to Paste into Figma AI)

```text
Design a clean, professional, high-fidelity UI mockup for a web application called "Fitness Planner" consisting of 4 frames. Use a modern grayscale aesthetic matching the existing codebase with subtle dark accents.

Global Design System Specifications:
- Color Palette:
  * Page Canvas: #F3F4F6 (Light gray)
  * Header, Footer, and Primary Card Backgrounds: #D1D5DB (Medium gray)
  * Secondary Containers & Badges: #9CA3AF (Muted gray)
  * Card Borders: #6B7280 (1px solid border)
  * Primary Text & Headings: #111827 (Near black, 10.7:1 contrast)
  * Secondary Text: #374151 (Dark gray, 5.5:1 contrast)
  * Primary Action Buttons: #1F2937 (Charcoal black) with #FFFFFF (Pure white) bold text
  * Secondary Action Buttons: #9CA3AF (Gray) with #000000 bold text
  * Focus State Indicator: 2px solid ring in #111827 with 2px offset
- Typography: Inter / system sans-serif font stack. Clean hierarchy with bold weights (700/800) for headers and medium (500) for body text.
- Radii: Cards and containers use 24px (rounded-3xl) or 16px (rounded-2xl). Buttons are pill-shaped (rounded-full). Inputs are 12px (rounded-xl).
- Spacing: 8px grid system (16px and 24px padding).

Frame 1: Routine Builder Desktop (1440x1024 px)
- Top Navigation Bar (Height 72px, BG #D1D5DB, Padding 24px):
  * Left: Brand title "Fitness Planner" in bold 22px text.
  * Center: Horizontal navigation links: "Home", "Dashboard", "Routine Builder" (active state with bold text and 2px black bottom border), "Active Workout", "Profile".
  * Right: Pill button "📱 Mobile View" (BG #9CA3AF) and round user profile avatar circle with "👤" icon.
- Main Content Area (Max width 1024px, centered, 32px vertical spacing):
  * Header Section: Title "Routine Builder" in 30px bold, subtitle "Design and configure custom workout routines with targeted sets, reps, and rest intervals", and a pill button "▶ Launch Active Workout" (#1F2937 BG, white text).
  * Section 1 - Routine Details Card (BG #D1D5DB, 24px border radius, 24px padding):
    - Title "Routine Details" with bottom divider.
    - 2-Column form grid: Left field "Routine Name" with white text input containing "Push Day Hypertrophy". Right field "Assigned Day" with select dropdown showing "Monday - Push (Chest & Triceps)".
    - Full-width textarea "Routine Notes & Coaching Tips" with white background containing warmup instructions.
  * Section 2 - Ordered Exercise List Card (BG #D1D5DB, 24px border radius, 24px padding):
    - Header with title "Ordered Exercise List (4 Exercises)" and button "+ Add Exercise" (#1F2937 BG, white text).
    - 4 stacked exercise items (BG #F3F4F6, 16px radius, border #9CA3AF):
      1. Barbell Bench Press: drag handle icon (⠿), title, badge "Chest", number inputs for Sets (4), Target Reps (8), Rest sec (90s), and "✕" remove button.
      2. Incline Dumbbell Press: drag handle, title, badge "Upper Chest", Sets (3), Reps (10), Rest (75s), remove button.
      3. Standing Cable Lateral Raise: drag handle, title, badge "Shoulders", Sets (4), Reps (12), Rest (60s), remove button.
      4. Tricep Rope Pushdown: drag handle, title, badge "Triceps", Sets (3), Reps (12), Rest (60s), remove button.
    - Bottom Actions: "Cancel" button (#9CA3AF BG) and "Save Routine" button (#1F2937 BG, white text). Focus state demonstrated on Save Routine with a 2px outer ring.
  * Section 3 - Saved Workout Routines (3 Cards in a row, BG #D1D5DB, 24px radius):
    - Card 1: "Push Day Hypertrophy", Monday badge, ~60 min, 4 exercises, 14 sets. Buttons: "Edit" and "Start".
    - Card 2: "Pull Day Strength", Tuesday badge, ~75 min, 5 exercises, 18 sets. Buttons: "Edit" and "Start".
    - Card 3: "Legs & Core Blast", Thursday badge, ~70 min, 6 exercises, 20 sets. Buttons: "Edit" and "Start".
- Footer (Height 56px, BG #D1D5DB, center aligned text "© 2026 FitnessPlanner").

Frame 2: Routine Builder Mobile (390x844 px, iPhone 16 Viewport)
- Top Bar (Height 56px, BG #D1D5DB, sticky): Hamburger button "≡", brand "Fitness Planner", and "👤" avatar.
- Main Scrollable Body (Padding 16px, spacing 16px):
  * Title: "Routine Builder" in 20px bold.
  * Card 1: Routine Details (BG #D1D5DB, 24px radius) with input for routine name, day dropdown, and notes.
  * Card 2: Exercises (4) with "+ Add Exercise" button. 4 stacked compact exercise cards (BG #F3F4F6) with drag handle, title, badge, 3-column input row (Sets, Reps, Rest), and remove button. Min 44px touch targets.
  * Action buttons: Full-width "Save Routine" (#1F2937 BG, white text, 48px height) and "Cancel" button.
  * Card 3: Saved Routines with compact cards for Push Day and Pull Day.
- Fixed Bottom Navigation Bar (Height 60px, BG #D1D5DB, border-t #9CA3AF): 5 tabs with icons and text: "Home", "Dashboard", "Routines" (Active state with darker gray highlight #9CA3AF), "Workout", "Profile".

Frame 3: Active Workout Desktop (1440x1024 px)
- Top Navigation Bar (Identical to Frame 1, with "Active Workout" highlighted as active link).
- Main Content Area (Max width 1024px, centered, 24px spacing):
  * Header Banner (BG #D1D5DB, 24px radius, 24px padding):
    - Left: Badge "IN PROGRESS", routine title "Push Day Hypertrophy" in 28px bold, "Started at 10:15 AM".
    - Right: Elapsed Time box (BG #F3F4F6, text "00:42:18" in 28px bold monospace) and large button "✓ Finish Workout" (#1F2937 BG, white text, 48px height).
  * 3 Summary Metric Cards Grid (BG #D1D5DB, 16px radius, centered text):
    - Sets Completed: "11 / 14" (78% routine progress)
    - Total Volume Lifted: "8,450 kg" (+420 kg vs last week)
    - Estimated Burn: "345 kcal" (Average HR: 132 bpm)
  * Rest Timer Widget Card (BG #D1D5DB, 24px radius, 24px padding):
    - Section header "Active Rest Timer".
    - Huge countdown display "01:30" in 64px bold monospace font.
    - Quick control pill buttons: "- 15s" (BG #9CA3AF), "+ 15s" (BG #9CA3AF), "Skip Rest" (BG #1F2937, white text).
  * Exercise Performance Logs Section (2 Large Cards, BG #D1D5DB, 24px radius):
    - Card 1 "Barbell Bench Press": Title, target info, "3 of 4 Sets Completed". Clean HTML table with columns: Set, Previous (80 kg × 8), Weight kg (input 82.5), Reps (input 8), Complete (large checked checkboxes).
    - Card 2 "Incline Dumbbell Press": Title, target info, "3 of 3 Sets Completed", table with completed sets.
- Footer (Height 56px, BG #D1D5DB, "© 2026 FitnessPlanner").

Frame 4: Active Workout Mobile (390x844 px, iPhone 16 Viewport)
- Sticky Top Header (Height 56px, BG #D1D5DB): Hamburger "≡", live elapsed timer "00:42:18", and pill button "Finish" (#1F2937 BG, white text).
- Main Body (Padding 16px, spacing 16px):
  * Title: "Push Day Hypertrophy" in 20px bold.
  * Rest Timer Card (BG #D1D5DB, 24px radius): Big countdown "01:30" and 3 touch buttons: "- 15s", "+ 15s", "Skip".
  * Summary Cards (2 columns): "Sets Done: 11/14", "Volume: 8,450 kg".
  * Exercise Card 1 (BG #D1D5DB, 24px radius): Table with Set #, Prev, kg input, Reps input, and large 44px checkbox targets.
  * Exercise Card 2 (BG #D1D5DB, 24px radius): Incline Dumbbell Press table.
- Fixed Bottom Navigation Bar (Height 60px, BG #D1D5DB): 5 tabs, with "Workout" tab active.
```

---

## (B) Low-Fidelity Wireframes Prompt (Grayscale Wireframe Style)

Use this prompt when you need Figma AI to generate **clean wireframes ONLY** without colorful mockups or illustrations:

```text
Create a low-fidelity grayscale wireframe system in Figma consisting of 4 frames for a web and mobile workout planner.

Styling Rules for Low-Fidelity Wireframe:
- Strict grayscale only: Pure white (#FFFFFF), Light gray (#F3F4F6), Neutral medium gray (#D1D5DB), Border gray (#9CA3AF), and Dark charcoal for text (#111827).
- No saturated colors, no gradients, no photorealistic images.
- Image placeholders must be gray rectangles with an "X" drawn diagonally from corner to corner and labeled in brackets (e.g., "[Exercise Diagram]").
- Buttons must be simple gray rounded rectangles or pill outlines with centered text labels.
- Simple system sans-serif typography (Inter or Roboto) with high contrast text.

Frames to generate:

1. "Wireframe - Routine Builder Desktop" (1440x1024):
   - Wireframe Header: Gray bar (#D1D5DB) with text logo "Fitness Planner", text nav links ("Home", "Dashboard", "Routine Builder" bolded, "Active Workout", "Profile"), and a circular placeholder "[User]".
   - Form Container: Outlined box containing "Routine Name" input wireframe, "Day" dropdown wireframe, and "Notes" box.
   - Exercise List: 4 stacked wireframe rows. Each row has a grip icon (⠿), exercise title, placeholder badge box "[Chest]", input boxes for Sets, Reps, and Rest, and an "[X]" remove button.
   - Action Bar: Wireframe buttons "[+ Add Exercise]", "[Cancel]", and solid charcoal button "[Save Routine]".
   - Bottom Section: 3 wireframe cards representing saved routines with text placeholders and action buttons "[Edit]" and "[Start]".
   - Wireframe Footer: Gray text bar "© 2026 FitnessPlanner".

2. "Wireframe - Routine Builder Mobile" (390x844):
   - Top Bar: Hamburger icon "[≡]", title "Fitness Planner", and user icon.
   - Stacked wireframe form cards for Routine Name, Day select, and Notes.
   - Vertical list of 4 exercise cards, each with sets/reps/rest wireframe number steppers.
   - Primary full-width wireframe button "[Save Routine]" and secondary button "[Cancel]".
   - 2 saved routine wireframe boxes.
   - Bottom Bar: Fixed wireframe navigation bar with 5 icon/label slots: Home, Dashboard, Routines (highlighted with gray fill), Workout, Profile.

3. "Wireframe - Active Workout Desktop" (1440x1024):
   - Top Header: Same wireframe nav bar.
   - Status Header: Box with title "Push Day Hypertrophy", elapsed time wireframe box "[00:42:18]", and button "[Finish Workout]".
   - 3 Summary Stat Boxes: "[Sets Completed: 11/14]", "[Total Volume: 8,450 kg]", "[Calories: 345 kcal]".
   - Rest Timer Wireframe Box: Large centered digital countdown "[01:30]" with 3 wireframe buttons: "[- 15s]", "[+ 15s]", and "[Skip]".
   - Set Tables: 2 wireframe table cards. Table 1 has columns Set #, Prev, Weight, Reps, and square Checkboxes (3 checked with an X, 1 unchecked). Table 2 has 3 completed set rows.
   - Wireframe Footer.

4. "Wireframe - Active Workout Mobile" (390x844):
   - Sticky Top Bar: "[≡]", elapsed timer "[00:42:18]", and button "[Finish]".
   - Rest Timer card with big "[01:30]" and 3 tap buttons.
   - 2-column stats box.
   - 2 exercise cards with simplified mobile wireframe set rows and large touch-friendly checkboxes.
   - Bottom Bar: 5-tab wireframe bar with "Workout" active.
```
