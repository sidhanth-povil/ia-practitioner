# ia-practitioner — Claude Skill

> A Claude skill for applying professional Information Architecture principles to any website, app, or content project.

Built and maintained by **[designsuite.ai](https://designsuite.ai)** — UI/UX studio specialising in WordPress and healthcare web design.

---

## What this skill does

Install this skill and Claude becomes a working IA consultant. It knows how to:

- Audit any website's navigation structure and label system
- Identify which IA patterns and classification schemes suit your content
- Run card sort and tree test planning sessions
- Produce before/after nav comparisons and implementation roadmaps
- Generate client-ready audit reports as `.docx` files

It applies a rigorous framework built from the best practitioner literature in the field — covering the full lifecycle from user research through to navigation design and testing.

---

## Install

1. Download [`ia-practitioner.skill`](./ia-practitioner.skill)
2. In Claude.ai → Settings → Skills → Install from file
3. Drop the `.skill` file in

Done. Works across all your Claude chats.

---

## Example prompts after installing

```
"Audit the IA of gipartnersofil.com"
"What classification scheme suits a portfolio site?"
"How should I structure a healthcare clinic website?"
"Help me write tree testing scenarios for my new nav"
"What nav pattern suits an e-commerce site with 200 products?"
"Generate an IA audit report for [url] as a Word doc"
"My client's navigation feels wrong — how do I test it?"
```

---

## How we trained it

This skill was built by feeding Claude the full text of the best practitioner IA books and extracting the frameworks, decision rules, principles, and anti-patterns into a structured skill format.

The core sources that shaped the framework:

### Primary source

**A Practical Guide to Information Architecture** — Donna Spencer (UX Mastery, 2010)
The most applied, practitioner-focused IA book available. Spencer's People × Content × Context model, classification scheme selector, IA patterns library, and labelling principles form the backbone of this skill.

### Validated against

**Information Architecture for the World Wide Web** — Peter Morville & Lou Rosenfeld (O'Reilly, 3rd ed.)
The foundational "polar bear book" — the canonical reference for IA as a discipline. Morville and Rosenfeld's component model (organisation, labelling, navigation, search systems) underpins the vocabulary used throughout.

**How to Make Sense of Any Mess** — Abby Covert (Self-published, 2014)
The clearest introduction to IA thinking available. Covert's "intent → message → language" chain and her insistence on defining words before designing with them sharpened the labelling and terminology sections.

**Everyday Information Architecture** — Lisa Maria Marquis (A Book Apart, 2019)
Content-first IA with particular depth on labelling systems, taxonomy, and the relationship between content strategy and navigation design. Directly informed the labelling audit and classification scheme reference files.

**Don't Make Me Think** — Steve Krug (New Riders, 3rd ed.)
The usability perspective on navigation. Krug's billboards-not-books metaphor and his persistent scanning vs reading distinction are embedded in the nav design reference.

### Adjacent disciplines drawn from

- **Card sorting research** — Optimal Workshop methodology documentation
- **Tree testing** — Treejack research and first-click testing literature
- **Cognitive psychology** — Hick's Law (decision time vs choices), Miller's Law (working memory), and George Zipf's principle of least effort applied to navigation design

---

## Skill structure

```
ia-practitioner/
├── SKILL.md                          ← Core skill, always loaded
└── references/
    ├── classification-schemes.md     ← All 8 schemes with decision rules
    ├── ia-patterns.md                ← All IA patterns with selector guide
    ├── user-analysis.md              ← Research methods and analysis
    └── navigation-design.md         ← Nav types, principles, anti-patterns
```

The skill loads `SKILL.md` on every relevant conversation. Reference files are loaded on demand when a deeper question requires them (e.g. "which classification scheme should I use" loads `classification-schemes.md`).

---

## Audit report generation

The skill includes a full audit report generator that produces a professional `.docx` report covering:

- Executive summary with IA score
- User group analysis
- Issue cards (current state vs recommended fix)
- Labelling audit table
- Proposed IA structure
- Mobile-specific recommendations
- Prioritised implementation roadmap

See [`examples/GI_Partners_IA_Audit_Report.docx`](./examples/GI_Partners_IA_Audit_Report.docx) for a live example — a full audit of [gipartnersofil.com](https://gipartnersofil.com) produced entirely by Claude using this skill.

---

## Useful tools that pair with this skill

| Tool | Use |
|---|---|
| [Optimal Workshop](https://www.optimalworkshop.com) | Card sorting (OptimalSort) + tree testing (Treejack) |
| [UXtweak](https://www.uxtweak.com) | Card sort, tree test, usability — free tier available |
| [Maze](https://maze.co) | Card sorting + first-click testing + prototype tests |
| [Lyssna](https://www.lyssna.com) | Tree testing + first-click + preference tests |
| [UXMetrics](https://uxmetrics.com) | Lightweight focused card sort + tree test |
| [Miro](https://miro.com) | Affinity mapping, sitemap diagramming, sticky-note card sorts |
| [Figma](https://figma.com) | Navigation wireframing + IA structure visualisation |

---

## Further reading

These are worth reading front to back if you work on IA regularly:

| Book | Author | Why |
|---|---|---|
| A Practical Guide to Information Architecture | Donna Spencer | Best applied methodology — built this skill |
| Information Architecture for the Web and Beyond | Morville & Rosenfeld | Foundational vocabulary and component model |
| How to Make Sense of Any Mess | Abby Covert | Clearest intro to IA thinking; language-first approach |
| Everyday Information Architecture | Lisa Maria Marquis | Content-first IA; strongest on labelling and taxonomy |
| Don't Make Me Think | Steve Krug | Usability lens on navigation; billboards not books |
| The Discipline of Organizing | Robert J. Glushko (ed.) | Academic depth; bridges library science + HCI |
| Search Patterns | Morville & Callender | Search as navigation; complements browse-first IA |
| Pervasive Information Architecture | Resmini & Rosati | Cross-channel IA; apps, devices, physical spaces |

---

## Who this is for

Primarily built for:
- **Web designers and UX designers** working on site structure and navigation
- **WordPress / Elementor developers** making navigation and menu decisions
- **Healthcare and clinic websites** (medicalsuite.ai use case)
- **Agency teams** preparing client-facing IA audit deliverables

---

## About designsuite.ai

**designsuite.ai** is a UI/UX and WordPress studio building high-performance sites for clients across industries. Our sister brand **medicalsuite.ai** focuses on healthcare web design in the UAE and globally.

We build Claude skills as internal tools and release them publicly when we think they're useful to other practitioners.

→ [designsuite.ai](https://designsuite.ai) · [medicalsuite.ai](https://medicalsuite.ai)

---

## Contributing

Found a principle we missed? A better classification scheme example? A labelling anti-pattern worth documenting?

Open a PR against any of the `skill/references/*.md` files. Keep the tone practitioner-first — practical decision rules over theory.

---

## Licence

MIT. Use freely, attribution appreciated.
