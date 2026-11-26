---
name: mylabs
description: Fill in MyLab Math answer boxes in Chrome one problem part at a time, then stop so the user reviews and clicks the Finish button. Use when the user is on mylab.pearson.com and wants help entering answers.
---

# MyLabs (Pearson MyLab Math) helper

Use when the user is on mylab.pearson.com and wants help entering answers.

## Flow (one part at a time)

1. Screenshot the user's current tab and zoom into the problem to read signs and exponents exactly.
2. Work out the answer. Keep the reply short: no step-by-step explanation unless the user asks (MyLab shows its own tutorial after a correct answer).
3. Fill the boxes (see below), then zoom to verify every box holds the right value.
4. Stop and tell the user: "Filled in, review and click Check answer." Always click Check answer, Submit, but never click Finish yourself.
5. When it says it's checked, screenshot. If correct, move to the next part or problem and repeat. If wrong, scroll down to read the feedback, fix only the wrong box, and stop again.

## Reading the page

- get_page_text often fails on MyLab, and find/read_page can't see the answer boxes (they are inside the math player). Use screenshots and zoom.

## Avoiding common mistakes

- Read the text right after an integrand box. If the Jacobian is already printed ("dz r dr dθ", "ρ² sin φ dρ dφ dθ"), the box gets only the density (often 1).
- Match the integration order shown. The leftmost integral is the outermost.
- Tries are limited, so double-check before handing off.

## Filling boxes reliably

- Click the LEFT side of a box (the typing area), not the small ∫Σ∂ icon.
- Type plain syntax: r^2, 2pi, sqrt(x). Press the Right arrow to leave an exponent.
- Lower-limit boxes most often miss input: zoom to confirm.
- Click a blank area to deselect when done.

## Style

- No em dashes in writing.
