# Output Contracts

## Concept Direction

Use this structure when the user asks for a creative direction, treatment, or concept:

```text
Product truth:
Audience:
Core promise:
Narrative spine:
Visual world:
Motion language:
Camera language:
Typography language:
Product UI treatment:
Proof beats:
Trust beat:
Ending:
Risks to avoid:
```

Keep the concept decisive. Do not provide many unrelated options unless the user asks.

## Storyboard or Shot Plan

Use this table structure:

```text
Time:
Shot name:
Narrative purpose:
First read:
Composition:
Camera and staging:
Primary motion:
Secondary motion:
Product/UI proof:
Copy or VO:
Transition in:
Transition out:
Taste notes:
```

Every shot must have a purpose, a focal hierarchy, and a transition logic. If any row cannot be filled concretely, the shot is not ready.

## Motion Spec

Use this for implementation-ready direction:

```text
Object:
Initial state:
Trigger:
Motion path:
Timing:
Easing feel:
Depth/layering:
Opacity/scale/blur behavior:
Settle state:
Attention target:
Reason:
```

Do not specify arbitrary values when the implementation stack is unknown. Specify behavior and taste intent unless the user asks for technical values.

## Critique

Use this structure:

```text
Overall diagnosis:
Top issues:
Recommended fixes:
Revised sequence:
Taste score:
Residual risk:
```

Lead with the issue that most affects product truth or viewer comprehension.

## Teardown

Use the format in `teardown-method.md`. After teardown, always extract reusable rules:

```text
Reusable pattern:
Why it works:
Where to use it:
Where not to use it:
Adaptation note:
```

## Polish Pass

Use this checklist:

```text
Hierarchy fixes:
Timing fixes:
Camera/staging fixes:
Typography fixes:
UI proof fixes:
Transition fixes:
Visual system fixes:
Cuts to remove:
Final quality gate:
```

Prefer removing weak complexity before adding new polish.

