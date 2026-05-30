<div align="center">

<br>

# ia-practitioner

### A Claude skill for professional Information Architecture

Apply practitioner IA frameworks to any website, app, or content project — directly in conversation.

<br>

[![Version](https://img.shields.io/badge/version-2.0.0-c4a44a?style=flat-square)](https://github.com/sidhanth-povil/ia-practitioner/releases)
[![License](https://img.shields.io/badge/license-MIT-4a7a4a?style=flat-square)](./LICENSE)
[![Built by](https://img.shields.io/badge/built_by-designsuite.ai-1a4a7a?style=flat-square)](https://designsuite.ai)
[![Sources](https://img.shields.io/badge/sources-7_books-6a5acd?style=flat-square)](#source-literature)

<br>

</div>

---

## What this skill does

Install once and Claude becomes a working IA consultant. It applies a rigorous framework built from seven practitioner texts — covering the full lifecycle from user research through navigation design, search systems, taxonomy, testing, and client deliverables.

| Capability | What Claude does |
|---|---|
| **Nav audits** | Audits any site's navigation against IA principles — flags org-chart drift, label failures, pattern mismatches |
| **Classification** | Identifies which of the 8 classification schemes and 10 IA patterns best fit your content and users |
| **Search systems** | Designs search architecture — zones, result presentation, autocomplete, faceted navigation, no-dead-ends policy |
| **Vocabulary control** | Builds controlled vocabularies, synonym rings, authority files, and thesauri |
| **Research planning** | Runs card sort and tree test sessions — writes scenarios, advises on tools, analyses results |
| **Audit reports** | Generates client-ready `.docx` reports with before/after nav comparisons, issue cards, and roadmaps |
| **Labelling** | Tests every label against user terminology; catches internal jargon, audience-nav traps, junk drawers |
| **Cross-channel IA** | Applies Resmini & Rosati's five heuristics for consistent experiences across devices and channels |
| **Taxonomy design** | Documents controlled vocabularies, tagging systems, and faceted classification for CMS-driven sites |

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
"Design a search system for a 10,000-page university site"
"Build a controlled vocabulary for a healthcare clinic"
"What are the cross-channel IA heuristics I should apply?"
"How do I design faceted navigation for a product catalogue?"
```

---

## Skill structure

```
ia-practitioner/
├── SKILL.md                        ← Core — loaded on every relevant conversation
└── references/
    ├── classification-schemes.md   ← All 8 schemes; LATCH framework; controlled vocabulary; thesauri
    ├── ia-patterns.md              ← 10 IA patterns; cross-channel patterns; Glushko organising systems
    ├── user-analysis.md            ← Research methods; card sort analysis; structural audits; diagrams
    └── navigation-design.md        ← Nav types; search systems; wayfinding; faceted nav; anti-patterns
```

`SKILL.md` loads on every relevant conversation — kept tight and scannable. Reference files are loaded on demand when the depth of a question requires them.

---

## What's new in v2.0

This release incorporates **six additional books** on top of the Spencer foundation, adding material that was completely absent in v1.0.

| New capability | Source |
|---|---|
| Search systems (full chapter) | Morville & Rosenfeld |
| Controlled vocabularies, synonym rings, thesauri | Morville & Rosenfeld |
| Faceted classification and guided navigation | Morville & Rosenfeld |
| LATCH organisational framework | Wurman via Marquis |
| Criteria matching process for categorisation | Marquis |
| Four categorical considerations (user needs / business goals / current state / future) | Marquis |
| Structural audit methodology with spreadsheet template | Marquis |
| Labelling guidelines — clarity, specificity, inclusivity, consistency | Marquis |
| Conway's Law warning | Marquis |
| Folksonomy failure modes and controlled tagging | Marquis |
| Ontology as distinct from vocabulary | Covert |
| Nouns + verbs requirements model | Covert |
| Scales of abstraction (object → ecosystem) | Covert |
| Scanning, satisficing, muddling through | Krug |
| First-click testing | Krug |
| Organising systems framework vocabulary | Glushko |
| Resource description and aboutness theory | Glushko |
| Agent-type analysis (human vs algorithmic tagging) | Glushko |
| Five cross-channel heuristics | Resmini & Rosati |
| Internal vs external consistency | Resmini & Rosati |

See [CHANGELOG.md](./CHANGELOG.md) for full details.

---

## Source literature

Built from the actual practitioner texts. Decision rules and anti-patterns extracted from source material — not summaries.

**Primary source**

**A Practical Guide to Information Architecture** — Donna Spencer (UX Mastery, 2010)
Spencer's People × Content × Context model, classification scheme selector, and labelling principles form the backbone of this skill.

**v2.0 additions**

| Book | Author | What it added |
|---|---|---|
| *Information Architecture for the Web and Beyond* | Morville, Rosenfeld & Arango (4th ed.) | Search systems, controlled vocabularies, faceted classification, bottom-up IA |
| *Everyday Information Architecture* | Lisa Maria Marquis | LATCH, criteria matching, structural audits, labelling guidelines, Conway's Law |
| *How to Make Sense of Any Mess* | Abby Covert | Ontology, nouns + verbs model, scales of abstraction, "don't say" lists |
| *Don't Make Me Think* | Steve Krug | Scanning/satisficing/muddling, first-click testing, conventions, visual hierarchy |
| *The Discipline of Organizing* | Robert J. Glushko (4th ed.) | Organising systems framework, resource description, agent types, aboutness |
| *Pervasive Information Architecture* | Resmini & Rosati | Five cross-channel heuristics, internal/external consistency, ubiquitous ecologies |

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
- **Product designers** working on search and discovery experiences

---

## Further reading

| Book | Author | Why |
|---|---|---|
| *A Practical Guide to Information Architecture* | Donna Spencer | Best applied methodology — built this skill |
| *Information Architecture for the Web and Beyond* | Morville, Rosenfeld & Arango | Foundational vocabulary; search systems; controlled vocabularies |
| *How to Make Sense of Any Mess* | Abby Covert | Clearest intro to IA thinking; language-first approach |
| *Everyday Information Architecture* | Lisa Maria Marquis | Content-first IA; strongest on labelling, taxonomy, and audits |
| *Don't Make Me Think* | Steve Krug | Usability lens on navigation; billboards not books |
| *The Discipline of Organizing* | Robert J. Glushko (ed.) | Academic depth; bridges library science + HCI |
| *Pervasive Information Architecture* | Resmini & Rosati | Cross-channel IA across apps, devices, physical spaces |
| *Search Patterns* | Morville & Callender | Search as navigation; complements browse-first IA |

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
