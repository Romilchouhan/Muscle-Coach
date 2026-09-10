# Muscle Coach PWA — v0.2

Standalone, offline-capable protein + workout coach.

## Included
- Apple-Health-inspired daily protein progress ring
- Adjustable protein target (default 130g)
- One-tap meal checkpoints
- Rotating Indian meal suggestions with veg / egg / quick / light filters
- Recent-meal avoidance so suggestions do not feel identical every day
- 3-session rotating strength plan instead of a fixed weekday calendar
  - A: Chest + Triceps
  - B: Back + Biceps
  - C: Legs + Shoulders
- Each session is about 60–80 minutes with 5 exercises
- Exercise completion tracker and session progress bar
- One-tap exercise substitutions
- Rest-day option that preserves the next session in the rotation
- Local device storage and offline support
- No ChatGPT subscription or API key required

## Training model
Aim for three strength sessions per week with a rest day between sessions when practical. Your easy/moderate weekly run can sit on a rest day. Most sets use 3 working sets; compounds generally use 6–12 reps and isolation work 10–20 reps.

## Deploy on GitHub Pages
1. Create a GitHub repository.
2. Upload all files in this folder to the repository root.
3. GitHub → Settings → Pages → Deploy from a branch.
4. Select `main` and `/ (root)`.
5. Open the Pages URL in Safari on iPhone.
6. Share → Add to Home Screen.

A PWA can launch like an app and work offline, but it cannot provide a true native WidgetKit Home Screen widget.

## v0.3 changes
- Workout A/B/C cards are now directly selectable. The suggested rotation is guidance, not a lock.
- Exercise completion is kept separately for each workout while you switch between plans.
- Protein meal checkpoints are independent and toggleable, so breakfast never blocks lunch/snack/dinner.
- Checkpoints can no longer accidentally add protein repeatedly; tapping again removes that checkpoint.
- Added a Reset today's protein control for correcting a day's state.

## v0.4 changes
- Meal suggestions are now strictly scoped by meal type: breakfast, lunch, snack, and dinner never cross over.
- Selecting a checkpoint also switches the suggestion panel to that meal.
- “What should I eat now?” picks the next unchecked meal and shows only options for that meal.
- Recent-meal avoidance is tracked separately for each meal type.
- Added larger meal-specific Indian option pools for more variety.


## v0.5
- Added rough daily estimates for calcium, magnesium, iron, zinc, potassium, fiber, vitamin B12 and vitamin D.
- Added compact micronutrient progress bars and a food-first nutrition gaps card.
- Meal recommendations now rank options using both remaining protein and the largest tracked nutrient gaps.
- Expanded each meal-specific Indian food pool while preserving strict breakfast/lunch/snack/dinner separation.
- Added a local 7-day protein trend.
- Kept all workout behavior from v0.4, including free A/B/C session selection.
- Remains offline-first and stores data only in the browser.

### Important
Micronutrient values are approximate standard-serving estimates. Do not use the app alone to decide whether you need a supplement; supplement decisions, especially iron and vitamin D, are better based on diet history and appropriate clinical testing/advice.
