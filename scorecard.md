# Layr Scorecard

Use this scorecard after applying the Layr rules.

A score is not valid unless it includes evidence from the UI.

---

## Hard Gates

If any hard gate fails, the screen cannot score above 84.

- one clear primary action exists
- primary action is visually dominant
- screen is understandable within 3 seconds
- clickable targets are at least 40x40px on desktop or 44x44px on touch interfaces
- interactive states are visible
- text contrast is accessible
- layout does not require unnecessary decisions before the primary action
- empty, loading, error, and success states are handled when relevant

---

## Scoring

Score every screen out of 100:

- Clarity: 0-20
- Cognitive Load: 0-20
- Time to Value: 0-20
- Hierarchy: 0-15
- Feedback: 0-10
- Accessibility: 0-10
- Trust: 0-5

Pass: 85+
Fail: below 85

---

## Evidence Requirements

For each score category, identify:

- what improved
- what still creates friction
- what was changed or should be changed next

Do not award high scores for intentions.
Score the actual interface, not the explanation.

---

## Score Guidance

### 95-100

Exceptional. The screen is obvious, fast, accessible, visually focused, and strongly aligned with the user's goal.

### 85-94

Strong. The screen is usable and clear, with only minor improvements remaining.

### 70-84

Not good enough. The screen may work, but important friction remains.

### Below 70

Failed. The user is likely to hesitate, misunderstand, abandon, or make errors.

---

## Improvement Loop

If the score is below 85:

1. identify the lowest scoring category
2. fix the largest source of friction
3. remove unnecessary elements before adding new ones
4. rescore using evidence
5. repeat until the score is at least 85
