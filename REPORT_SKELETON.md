# Report Skeleton

The binding fill-in template for a case study draft. Always fill this in
before writing flowing prose — it keeps quality consistent across pieces
and across writers.

The square brackets in section headings (`[H2 — …]`) are placeholders.
Replace them with your own content-specific, image-led headings. Do not ship
the bracket names.

---

```
TITLE: <short, with rhythm or a small wordplay; picks up the core theme>
SUBLINE: <more specific; often names the customer>

TEASER (2–4 sentences):
<orients the reader, makes them curious; names the customer and the core benefit>

[H2 — Opening / Portrait]
<image-led opening + industry, core product, headcount, sites,
  (Type 2 only) customer since>

[H2 — Starting point / (Type 2) Journey so far]
<Type 1: concrete pain points before the system.
 Type 2: how the partnership grew, then what brings us to today's topic>

[H2 — (Type 1) Decision / (Type 2) The challenge]
<Type 1: why this vendor was chosen.
 Type 2: the central challenge inside the focus topic>

[H2 — Solution 1]
<module / function paired with concrete effect in daily work; example from the source>

[H2 — Solution 2 (optional)]
<another module or topic with its effect>

[H2 — Outcomes & Outlook]
<verified improvements (minutes / hours / % / count) + forward-looking close>

PULL QUOTE (max. 2 sentences):
"…" — Name, Role, Company

OTHER QUOTES (1–3, distributed through the body):
"…" — Name, Role, Company
"…" — Name, Role, Company

FIGURES BOX:
Headcount · Users · Sites · Customer since · (optional standout figure)

— APPROVAL NOTE (at the end, not part of the body text) —
OPEN POINTS: <list of all [NEEDS INPUT] / [EDITORIAL] markers>
APPROVAL: Draft — quotes and statements to be approved by the customer before publication.
```

---

## Rules for the skeleton

- **Always fill in every slot.** If a slot is empty after reading the
  sources, mark it `[NEEDS INPUT: …]`. Do not silently delete sections.
- **Total H2 sections: four to six.** Adjust the number of Solution blocks
  to the material at hand.
- **Headings are not template names.** Write content-specific headings.
  "Solution 1" never appears in the final piece.
- **The figures box only contains what is verified.** Missing values appear
  as `[NEEDS INPUT]`.
- **Pull quote is exactly one.** Not zero, not three.
- **The approval note is always present.** No exceptions.

---

## Using the skeleton with an LLM

When you hand an interview transcript to an LLM, instruct it to fill the
skeleton above first — as a structured outline — *before* generating prose.
This catches missing material early and keeps the draft on the right arc.

The adapters in `/adapters/` (Claude skill, ChatGPT system prompt, universal
prompt) are configured to do this automatically.
