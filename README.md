# Customer Case Study Framework

A method for turning a customer interview into a publishable B2B case study —
documented end-to-end, with templates, a worked example, and three ready-to-use
adapters for Claude, ChatGPT, and any other LLM.

Most B2B case studies fail in the same ways: they read like brochures, they
invent numbers, they bury the customer's voice under product marketing. This
framework codifies the editorial moves that fix all three.

It is opinionated. It is tool-agnostic at its core. It produces drafts a
human still polishes — but a draft that already passes the quality bar that
matters.

---

## What's in this repo

```
.
├── METHODOLOGY.md            ← the editorial method (read this first)
├── QUALITY_CHECKLIST.md      ← the 16-point gate before shipping a draft
├── REPORT_SKELETON.md        ← the binding fill-in template
├── examples/
│   ├── input-transcript.md   ← a fictional interview, formatted like a Teams transcript
│   ├── output-report.md      ← the case study draft generated from that interview
│   └── module-glossary.example.md  ← example product-name glossary
└── adapters/
    ├── claude-skill/         ← drop-in Claude skill
    ├── chatgpt-system-prompt.md   ← paste into a ChatGPT Custom GPT
    └── universal-prompt.md   ← one-shot prompt for any LLM
```

## The shortest possible summary

**A case study has two types.** Type 1 is a new customer: the contrast
between *before* and *after* is the story. Type 2 is a long-term customer:
the depth of one topic, embedded in a partnership, is the story. Don't mix
them up. Don't force a Type 1 shape onto a Type 2 customer.

**A case study has one truth rule.** Anything not in your source material is
not claimed. Numbers, quotes, examples, module names — all from the source,
or marked as missing. A draft with marked gaps is better than a draft with
plausible-sounding filler.

**A case study has eight building blocks.** Company profile, interview
partner, leading topic, pain, solution, verified outcomes, quote candidates,
outlook. Extract them before drafting.

**A case study has a skeleton.** Title, subline, teaser, four to six H2
sections, one pull quote, a figures box, an approval note. The skeleton is
binding. Fill every slot, then write prose.

**A case study has a quality gate.** Sixteen points, every one of them a
specific failure mode neutralised. Walk it before you ship.

That's the whole method. The rest is detail.

---

## Three ways to use it

### 1. As a method, no tooling

Read [`METHODOLOGY.md`](./METHODOLOGY.md). Use
[`REPORT_SKELETON.md`](./REPORT_SKELETON.md) as your draft template. Run
[`QUALITY_CHECKLIST.md`](./QUALITY_CHECKLIST.md) on every draft. Write the
case study yourself in Word, Google Docs, or whatever you prefer.

This is the canonical use. Everything else is a wrapper around this.

### 2. With Claude

Install the skill in [`adapters/claude-skill/`](./adapters/claude-skill/).
Upload a transcript, ask Claude to make a case study, answer two clarifying
questions, get a draft. Setup takes about five minutes — see the
[skill README](./adapters/claude-skill/README.md).

### 3. With ChatGPT or any other LLM

For ChatGPT: paste
[`adapters/chatgpt-system-prompt.md`](./adapters/chatgpt-system-prompt.md)
into a Custom GPT's Instructions field. Done.

For any other LLM: copy
[`adapters/universal-prompt.md`](./adapters/universal-prompt.md), paste in
your transcript, send.

---

## A worked example

The clearest way to see what the framework does is to read the input and
the output side by side:

- **Input:** [`examples/input-transcript.md`](./examples/input-transcript.md) —
  a fictional Microsoft Teams transcript of an interview with the founder
  and production manager of *Northvale Brewing Equipment Ltd.*, a
  (fictional) Sheffield manufacturer of stainless steel brewing tanks.
- **Output:** [`examples/output-report.md`](./examples/output-report.md) —
  the case study draft generated from that interview, with every quote
  traceable, every number verified, every gap explicitly marked, and the
  approval note at the end.

Northvale, the people in the interview, the *Helios ERP* product they
adopted — all invented. Any resemblance to real companies or people is
coincidental.

---

## What this framework is for

- B2B SaaS, enterprise software, and vertical software vendors who
  publish customer case studies as part of their marketing.
- Content teams who want a method, not just a template.
- Solo writers and freelance content strategists who want to standardise
  the work without dumbing it down.

It works particularly well for ERP, CRM, manufacturing software, and any
domain where the story involves real operational change. It works less
well for purely consumer products or for short testimonial-style pieces.

## What this framework is *not*

- A publishing tool. Drafts go to a human writer for polish, then to the
  customer for approval, then a human ships.
- A way to skip interviews. The method is downstream of getting good
  source material. A weak transcript produces a weak draft, marked gaps
  and all.
- A guarantee. The checklist neutralises common failure modes; it does not
  replace editorial judgement.

---

## Customising for your product

The framework is intentionally generic. To make it write specifically for
your software:

1. Copy [`examples/module-glossary.example.md`](./examples/module-glossary.example.md)
   to your own glossary file. Replace the placeholder *Helios ERP* product
   and module names with yours.
2. Decide your house spelling conventions (capitalisation, brand mark,
   compound terms) and put them at the top.
3. If you use the Claude skill, drop your glossary in
   `adapters/claude-skill/references/`. If you use a Custom GPT, upload it
   as a knowledge file. If you use the universal prompt, paste it into the
   prompt.

The methodology, the checklist, and the skeleton stay the same.

---

## License

[MIT](./LICENSE). Use it, fork it, change it, ship it. No attribution
required, though it's appreciated.

---

## Contributing

This is a living document. If you find a failure mode the checklist
doesn't catch, a taboo word that slipped through, or a clearer way to
phrase a rule — open an issue or a PR.
