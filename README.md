<div align="center">

<br>

# ia-practitioner

### A Claude skill for professional Information Architecture

Apply Donna Spencer's practitioner IA framework to any website, app, or content project — directly in conversation.

<br>

[![Version](https://img.shields.io/badge/version-1.0.0-c4a44a?style=flat-square)](https://github.com/sidhanth-povil/ia-practitioner/releases)
[![License](https://img.shields.io/badge/license-MIT-4a7a4a?style=flat-square)](./LICENSE)
[![Built by](https://img.shields.io/badge/built_by-designsuite.ai-1a4a7a?style=flat-square)](https://designsuite.ai)
[![Framework](https://img.shields.io/badge/framework-Donna_Spencer-6a5acd?style=flat-square)](#source-literature)

<br>

</div>

---

## What this skill does

Install once and Claude becomes a working IA consultant. It applies a rigorous framework built from the best practitioner literature — covering the full lifecycle from user research through navigation design, testing, and client deliverables.

| Capability | What Claude does |
|---|---|
| **Nav audits** | Audits any site's navigation against IA principles — flags org-chart drift, label failures, pattern mismatches |
| **Classification** | Identifies which of the 8 classification schemes and 10 IA patterns best fit your content and users |
| **Research planning** | Runs card sort and tree test sessions — writes scenarios, advises on tools, analyses results |
| **Audit reports** | Generates client-ready `.docx` reports with before/after nav comparisons, issue cards, and roadmaps |
| **Labelling** | Tests every label against user terminology from research; catches internal jargon and brand-speak |
| **Sitemap creation** | Produces both conceptual and detailed sitemaps with implementation rationale |

---

## Install

```
1. Download ia-practitioner.skill from Releases
2. Open Claude.ai → Settings → Skills → Install from file
3. Drop the .skill file in
```

Works immediately across all your Claude conversations. No configuration needed.

---

## Prompt starters

After installing, try any of these:

```
"Audit the IA of gipartnersofil.com"
"What classification scheme suits a portfolio site?"
"How should I structure a healthcare clinic website?"
"Help me write tree testing scenarios for my new nav"
"What nav pattern suits an e-commerce site with 200 products?"
"Generate an IA audit report for [url] as a Word doc"
"My client's navigation feels wrong — how do I test it?"
"Run an open card sort analysis on these 30 items"
"What's wrong with using an audience-based nav as the primary scheme?"
```

---

## Skill structure

```
ia-practitioner/
├── SKILL.md                        ← Core — loaded on every relevant conversation
└── references/
    ├── classification-schemes.md   ← All 8 schemes with decision rules and traps
    ├── ia-patterns.md              ← 10 IA patterns with a pattern selection guide
    ├── user-analysis.md            ← Research methods, card sort analysis, mental models
    └── navigation-design.md        ← Nav types, principles, testing, anti-patterns
```

`SKILL.md` loads on every relevant conversation — kept tight and scannable. Reference files are loaded on demand when the depth of a question requires them.

---

## Source literature

Built from the actual practitioner texts. Decision rules and anti-patterns extracted from source material — not summaries.

**Primary source**

**A Practical Guide to Information Architecture** — Donna Spencer (UX Mastery, 2010)
The most applied practitioner IA book available. Spencer's People × Content × Context model, classification scheme selector, and labelling principles form the backbone of this skill.

**Validated against**

| Book | Author | Why it's here |
|---|---|---|
| *Information Architecture for the World Wide Web* | Morville & Rosenfeld | Foundational vocabulary and component model |
| *How to Make Sense of Any Mess* | Abby Covert | Intent → message → language chain; language-first approach |
| *Everyday Information Architecture* | Lisa Maria Marquis | Content-first IA; strongest on labelling and taxonomy |
| *Don't Make Me Think* | Steve Krug | Usability lens on navigation; billboards not books |

**Adjacent disciplines**

- Card sorting — Optimal Workshop methodology documentation
- Tree testing — Treejack research and first-click testing literature
- Cognitive psychology — Hick's Law, Miller's Law, Zipf's principle of least effort applied to navigation design

---

## Live example

The skill ships with a full audit of **[gipartnersofil.com](https://gipartnersofil.com)** — a multi-location GI medical group in Illinois.

Five violations caught immediately:

- Locations organised by internal brand name, not geography
- `"Treatments"` label used where patients arrive to find symptoms
- `"Contact"` buried inside `About Us`
- `"In The News"` given equal nav weight to clinical sections
- No consolidated Patient Resources section

The audit proposed a full nav restructure, wrote before/after comparisons, produced an IA pattern rationale, and generated a 9-section Word report — all in one conversation.

→ See [`examples/GI_Partners_IA_Audit_Report.docx`](./examples/GI_Partners_IA_Audit_Report.docx)

---

## Useful tools that pair with this skill

| Tool | Use case |
|---|---|
| [Optimal Workshop](https://www.optimalworkshop.com) | OptimalSort (card sorting) + Treejack (tree testing) — the gold standard |
| [UXtweak](https://www.uxtweak.com) | Card sort, tree test, usability — free tier available |
| [Maze](https://maze.co) | Card sorting + first-click testing + prototype tests |
| [Lyssna](https://www.lyssna.com) | Tree testing + first-click + preference tests |
| [UXMetrics](https://uxmetrics.com) | Lightweight focused card sort + tree test |
| [Miro](https://miro.com) | Affinity mapping, sitemap diagramming, sticky-note card sorts |
| [Figma](https://figma.com) | Navigation wireframing + IA structure visualisation |

---

## Who this is for

- **Web designers and UX designers** working on site structure and navigation
- **WordPress / Elementor developers** making navigation and menu decisions
- **Healthcare and clinic websites** — medicalsuite.ai use case
- **Agency teams** preparing client-facing IA audit deliverables
- **Content strategists** building taxonomy and labelling systems

---

## Further reading

| Book | Author | Why |
|---|---|---|
| *A Practical Guide to Information Architecture* | Donna Spencer | Best applied methodology — built this skill |
| *Information Architecture for the Web and Beyond* | Morville & Rosenfeld | Foundational vocabulary and component model |
| *How to Make Sense of Any Mess* | Abby Covert | Clearest intro to IA thinking; language-first approach |
| *Everyday Information Architecture* | Lisa Maria Marquis | Content-first IA; strongest on labelling and taxonomy |
| *Don't Make Me Think* | Steve Krug | Usability lens on navigation; billboards not books |
| *The Discipline of Organizing* | Robert J. Glushko (ed.) | Academic depth; bridges library science and HCI |
| *Search Patterns* | Morville & Callender | Search as navigation; complements browse-first IA |
| *Pervasive Information Architecture* | Resmini & Rosati | Cross-channel IA across apps, devices, physical spaces |

---

## Contributing

Contributions are welcome — but keep the skill tight. The core file loads on every conversation and must stay scannable.

> **Write for a working designer, not an academic. Decisions over definitions.
> "Use X when Y" over "X is defined as…" — every addition should answer a real decision a designer faces.**

**What we want**
- Sharper decision rules for scheme and pattern selection
- Real-world examples — IA patterns applied to healthcare, e-commerce, SaaS, intranets
- Labelling anti-patterns worth documenting
- Practical notes from using Optimal Workshop, UXtweak, Maze, etc.
- Anything factually wrong or misleading corrected

**What we don't want**
- Pure theory without practical application
- Long additions to `SKILL.md` — it loads on every conversation
- Frameworks that haven't been tested in real projects

**How to contribute**

```
1. Fork the repo
2. Edit the relevant file in skill/references/
3. Keep the tone: practitioner-first, decision-rule focused, concrete examples
4. Open a PR with a one-line description of what changed and why
```

---

## About

Built and maintained by **[designsuite.ai](https://designsuite.ai)** — UI/UX studio specialising in WordPress and healthcare web design.

Our sister brand **[medicalsuite.ai](https://medicalsuite.ai)** focuses on healthcare web design in the UAE and globally.

We build Claude skills as internal tools and release them publicly when we think they're useful to other practitioners.

---

<div align="center">

MIT License · [designsuite.ai](https://designsuite.ai) · [medicalsuite.ai](https://medicalsuite.ai)

</div>
