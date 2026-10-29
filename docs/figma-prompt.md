# Figma AI Generation Prompt: Low-Fidelity Wireframes
**Project**: Fitness & Workout Planner Frontend  
**Course**: SW 302 - User Interface Development  
**Author**: Team Member #3 (Routine Builder & Active Workout Tracker)  
**Style**: Strict Grayscale Low-Fidelity Wireframes (Matching Teammate Design Exactly)

---

## Final Prompt Ready to Paste into Figma AI

```text
Create LOW-FIDELITY WIREFRAMES ONLY (not high-fidelity mockups). Strictly grayscale: no brand colors, no gradients, no shadows, no real images, no illustrations, and no icons other than simple outline placeholders. Font: Inter (or system-ui sans-serif). Rounded corners (12px) on all cards, boxes, and buttons. Plain text labels inside gray boxes describing elements (e.g. "[Routine name]", "[Drag handle]", "[Done]").

Palette (Grayscale wireframe only):
- Background: White #FFFFFF
- Headers, footers, navigation bars, and buttons: Light gray #D9D9D9
- Cards, form containers, and content boxes: Medium gray #B3B3B3
- Inner content areas and exercise rows: Darker gray #999999
- Text and stroke borders: Black #000000 / Dark charcoal #111827

Match the existing team wireframe style exactly:
- Desktop frames: Light gray top bar with "Fitness Planner" in bold at the left and a small text label "nav bar" centered; page title centered in bold; gray rounded boxes for every section; light gray bottom footer with centered text "© 2026 FitnessPlanner".
- Mobile frames (iPhone 16, 393x852): Top bar with outline hamburger icon [≡] on the left, "Fitness Planner" centered in bold, outline profile circle icon [👤] on the right; a light gray bottom bar fixed at the base with centered bold label "nav bar".

Generate 4 frames, desktop and its mobile version arranged side by side:

FRAME 1: "Routine Builder page - Desktop" (1440x1024 px)
- Top bar (Height 72px, Fill #D9D9D9, Padding 24px): "Fitness Planner" in bold 24px on the left; label "nav bar" centered in 16px.
- Centered bold title: "Build Your Routine" in 32px bold with 16px bottom margin.
- 2-Column main layout (centered, max width 1100px, 24px gap):
  * Left Column (Medium gray card #B3B3B3, 12px radius, 24px padding, width 380px):
    - Subtitle "Routine details" in 18px bold.
    - 3 stacked input boxes (White #FFFFFF fill, 1px black outline, 12px radius, height 48px each) with gray label text:
      1. [Routine name: Push Day Hypertrophy]
      2. [Day of week: Monday]
      3. [Notes: Warm up rotator cuffs, rest 90s on compound lifts] (Height 96px)
    - Action buttons row: "Save Routine" (Dark gray button #999999 with black text, 12px radius, height 44px) and "Cancel" (Light gray button #D9D9D9, 12px radius, height 44px).
  * Right Column (Large medium gray area #B3B3B3, 12px radius, 24px padding, flex-1):
    - Header: "Exercises in this routine (3 exercises)" in 18px bold.
    - 3 stacked exercise rows (Darker gray #999999, 12px radius, 16px padding, 12px gap):
      1. Row 1: [drag handle] icon, text "Barbell Bench Press", small tag box "[Chest]", small boxes: "[Sets: 4]" | "[Reps: 8]" | "[Rest: 90s]", and button "[Remove]".
      2. Row 2: [drag handle] icon, text "Incline Dumbbell Press", tag box "[Upper Chest]", small boxes: "[Sets: 3]" | "[Reps: 10]" | "[Rest: 75s]", button "[Remove]".
      3. Row 3: [drag handle] icon, text "Standing Cable Lateral Raise", tag box "[Shoulders]", small boxes: "[Sets: 4]" | "[Reps: 12]" | "[Rest: 60s]", button "[Remove]".
    - Button below rows: "+ Add Exercise" (Light gray #D9D9D9, 12px radius, height 44px, full width).
- Bottom Section (Max width 1100px, centered):
  - Section heading: "Saved Routines" in 22px bold.
  - 3 gray cards grid (#B3B3B3, 12px radius, 20px padding):
    * Card 1: "[Push Day Hypertrophy]", text "4 exercises • 14 sets • ~60m", row with buttons "[Edit]" and "[Start]".
    * Card 2: "[Pull Day Strength]", text "5 exercises • 18 sets • ~75m", row with buttons "[Edit]" and "[Start]".
    * Card 3: "[Legs & Core Blast]", text "6 exercises • 20 sets • ~70m", row with buttons "[Edit]" and "[Start]".
- Gray footer bar (Height 56px, Fill #D9D9D9, centered text "© 2026 FitnessPlanner").

FRAME 2: "iPhone 16 - Routine Builder page" (393x852 px)
- Top bar (Height 54px, Fill #D9D9D9, px-16): hamburger icon [≡] (left), "Fitness Planner" in 18px bold (center), profile icon [👤] (right).
- Centered title: "Build Your Routine" in 22px bold.
- Single-column scrollable stack (Padding 16px, 16px gap):
  * Routine Details Card (#B3B3B3, 12px radius, 16px padding): 3 stacked white input boxes labeled [Routine name], [Day of week], and [Notes].
  * Exercise List Card (#B3B3B3, 12px radius, 16px padding):
    - Title "Exercises (2)" and button "+ Add Exercise".
    - 2 compact cards (#999999, 12px radius, 12px padding):
      - Exercise 1: "Barbell Bench Press" with tag "[Chest]", grid of 3 boxes [Sets: 4] [Reps: 8] [Rest: 90s], button "[Remove]".
      - Exercise 2: "Incline DB Press" with tag "[Upper Chest]", grid of 3 boxes [Sets: 3] [Reps: 10] [Rest: 75s], button "[Remove]".
  * Action buttons: Full-width button "Save Routine" (Height 48px, Fill #999999, 12px radius, bold black text) and full-width button "Cancel" (Height 44px, Fill #D9D9D9).
  * Saved Routines: 2 compact cards (#B3B3B3, 12px radius, 12px padding) for "Push Day" and "Pull Day" with "[Edit]" and "[Start]" buttons.
- Bottom bar (Height 54px, Fill #D9D9D9, sticky bottom): centered bold text "nav bar".

FRAME 3: "Active Workout Tracker page - Desktop" (1440x1024 px)
- Top bar (Height 72px, Fill #D9D9D9): "Fitness Planner" (left) and "nav bar" (center).
- Header row (Height 72px, Fill #B3B3B3, 12px radius, 20px padding, max width 1100px, centered):
  * Left: Routine name "Leg Day" in 24px bold.
  * Center: Large elapsed digital timer "00:42:18" in 28px bold monospace.
  * Right: Button "Finish Workout" (Dark gray #999999 with black bold text, 12px radius, height 44px, padding 20px).
- Main Content 2-Column Split (Max width 1100px, centered, 24px gap):
  * Left Column (Large content area, width 720px, 16px gap):
    - Heading "Active Exercises".
    - Exercise Card 1 (#B3B3B3, 12px radius, 20px padding): Title "Barbell Squats", 3-row wireframe table:
      Columns: Set | Previous | Weight (kg) | Reps | Done [checkbox]
      Row 1: Set 1 | 100 kg x 8 | [102.5] | [8] | [X] (Checked box)
      Row 2: Set 2 | 100 kg x 8 | [102.5] | [8] | [X] (Checked box)
      Row 3: Set 3 | 100 kg x 7 | [102.5] | [8] | [ ] (Unchecked box)
    - Exercise Card 2 (#B3B3B3, 12px radius, 20px padding): Title "Romanian Deadlifts", 3-row table with completed sets.
  * Right Column (Width 356px, 16px gap):
    - Rest Timer Card (#B3B3B3, 12px radius, 24px padding, text-center):
      * Label "Rest Timer" in 16px bold.
      * Huge digital countdown "01:30" in 56px bold monospace text.
      * 3 control buttons row (Height 44px each): "[-15s]" (#D9D9D9), "[+15s]" (#D9D9D9), and "[Skip]" (#999999).
    - Workout Summary Card (#B3B3B3, 12px radius, 20px padding):
      * Label "Workout Summary" in 16px bold.
      * Stat row: "Sets done" -> "[11 / 14 sets]".
      * Stat row: "Total volume" -> "[8,450 kg]".
      * Stat row: "Estimated burn" -> "[345 kcal]".
- Gray footer bar (Height 56px, Fill #D9D9D9, centered text "© 2026 FitnessPlanner").

FRAME 4: "iPhone 16 - Active Workout Tracker page" (393x852 px)
- Top bar (Height 54px, Fill #D9D9D9): hamburger icon [≡], "Fitness Planner" bold, profile icon [👤].
- Header row (#B3B3B3, 12px radius, 12px padding): routine title "Leg Day" on left, timer "00:42:18" on right.
- Rest Timer Box (#B3B3B3, 12px radius, 12px padding, text-center): label "Rest Timer", big text "01:30", and 3 tap buttons: "[-15s]", "[+15s]", "[Skip]".
- Exercise Card (#B3B3B3, 12px radius, 16px padding):
  * Exercise title "Barbell Squats (1 of 3)".
  * Table (3 rows) with columns: Set | Prev | kg | Reps | Done (large 44px checkbox).
  * Navigation buttons row: "[Previous Exercise]" and "[Next Exercise]" (Height 44px each).
- Summary row (#B3B3B3, 12px radius, 10px padding): "Sets: 11/14" | "Volume: 8,450 kg".
- Large full-width button "Finish Workout" (Height 50px, Fill #999999, 12px radius, bold black text).
- Bottom bar (Height 54px, Fill #D9D9D9, sticky bottom): centered bold text "nav bar".

Layout & Accessibility Rules:
- Cleanly aligned on an 8px grid system with consistent margins and padding.
- All mobile interactive touch targets (buttons, checkboxes, inputs) are at least 44px high.
- Plain, short, descriptive text labels inside all boxes.
```
