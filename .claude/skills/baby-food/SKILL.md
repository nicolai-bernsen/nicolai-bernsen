---
name: baby-food
description: Plan homemade baby food (puree/porridge, baby-led weaning ideas) for a 6-month-old week by week, track new foods and reactions, and output the ingredients for the weekly-shop skill. Use when the user asks about the baby's meals, introducing a new food, or the baby's shopping list.
---

# Baby food planner

Draft v1. This is practical meal planning, **not medical advice**. For allergy, reaction or growth questions defer to the health visitor (sundhedsplejerske) / GP and the current guidance at sundhedsstyrelsen.dk, and say so when a reaction is logged.

## Context
- Baby is 6 months. Parents make their own **porridge/puree from boiled vegetables plus a base** such as buckwheat flour (boghvedemel), quinoa or oats. Oat milk is the household milk; breast milk/formula remains the main nutrition (ask which, do not assume).
- She **had stomach issues when lentils were introduced**. Reaction history lives in `foods.md` and wins over any generic suggestion.
- Ingredients should be **øko** (matches the weekly-shop rule).

## Rules
1. Read `foods.md` first: introduced foods, dates, reactions, status.
2. **One new food at a time**, then wait a few days before the next (so a reaction can be traced). Suggest the next new food only if the last one is logged "fine" or enough days have passed.
3. Never suggest foods logged as a problem. For a logged problem food, suggest only a cautious retry plan if guidance allows, and tell the user to check with the health visitor first.
4. Safety defaults: no added salt or sugar, no honey, no whole nuts or other choking hazards, texture appropriate for age. When unsure, say so and point to Sundhedsstyrelsen rather than guess.
5. Offer a batch-cooking plan (cook once, freeze in portions) to match the low-effort goal.
6. Ask before logging: when the user reports how a food went, update `foods.md` (date, food, outcome, notes).

## Output
- This week's baby menu (porridge combos, finger-food ideas), noting the single new food if any.
- **Ingredient list for weekly-shop** as plain items with quantities (øko veg, boghvedemel, quinoa, oats, etc.), ready to be merged into the shopping list. Include batch quantities for freezing.
- Short "watch for" note tied to the new food, with the health-visitor caveat.

## Questions to ask when missing
Breast milk or formula? Any allergies in the family? Which foods have been tried so far (to seed `foods.md`)? Freezer space?
