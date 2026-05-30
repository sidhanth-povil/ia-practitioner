# Changelog

---

## v2.0.0 — May 2026

Major expansion. Six additional source texts incorporated. Significant new content across all reference files.

### New capabilities

**Search systems** *(Morville & Rosenfeld)*
- Full search system design chapter added to `navigation-design.md`
- When to add search (and when not to)
- Search zones, navigation vs destination pages, content component indexing
- Retrieval algorithms: recall vs precision tradeoff, stemming, pattern matching
- Query builders: spell checkers, stemming, phonetic tools, synonym ring expansion
- Result presentation: content components to display, ranking strategies (relevance, popularity, chronological, best bets)
- Search interface design: the box, autocomplete/autosuggest, advanced search, supporting revision
- No dead ends policy

**Controlled vocabularies and thesauri** *(Morville & Rosenfeld)*
- Synonym rings, authority files, classification schemes, and full thesauri added to `classification-schemes.md`
- Technical lingo: PT, VT, BT, NT, RT, SN
- Faceted classification and guided navigation
- Polyhierarchy
- When controlled vocabulary improves recall; when it hurts precision

**LATCH organisational framework** *(Wurman via Marquis)*
- Five ways to organise anything: Location, Alphabet, Time, Category, Hierarchy
- Limitations of LATCH (conflates ordering and grouping; missing shape/mnemonic methods)
- Added to `SKILL.md` and `classification-schemes.md`

**Criteria matching** *(Marquis)*
- Categorisation as a two-step process: define criteria → assess content against criteria
- Four factors shaping category criteria: user needs, business goals, current state, future state
- Posse Foundation case study demonstrating verb-led categories over audience-based nav
- Added to `SKILL.md`

**Structural audit methodology** *(Marquis)*
- Distinction between content audit (process) and content inventory (output)
- Scoping audit, automated audit, structural audit as layered processes
- Spreadsheet template: page IDs, colour-coding by depth, tracking crosslinks/external links/on-page nav
- Visualising current sitemap with colour-coded cards before redesigning
- Added to `user-analysis.md`

**Labelling guidelines** *(Marquis)*
- Four qualities: clarity, specificity, inclusivity, consistency
- First/second person possessive pronoun rules ("our" vs "your")
- Parallel structure requirements for grouped labels
- Anti-pattern: Comcast "Products / Bundles / Programming / Customers" — consistency without meaning
- Added to `SKILL.md`

**Conway's Law warning** *(Marquis)*
- Organisations that design systems will reproduce their communication structures as those systems
- Explicit warning against org-chart navigation
- Added to `SKILL.md` and `classification-schemes.md`

**Folksonomy failure modes** *(Marquis)*
- The Toast: 8,182 unique tags, 6,152 used on only one post, 400+ unused
- Uncontrolled tagging creates near-duplicate terms, splits content streams, undermines measurement
- Solution: controlled vocabulary from day one, with documented process for additions and retirements
- Added to `ia-patterns.md`

**Ontology** *(Covert)*
- Ontology as declaring meaning for terms in a specific context — more precise than dictionary-level vocabulary
- Sticky note process for mapping term relationships
- "Don't say" lists as equally important as "do say" lists
- Added to `SKILL.md` and `classification-schemes.md`

**Nouns + verbs requirements model** *(Covert)*
- Identify nouns (objects) and verbs (actions) in your domain
- Combine into explicit requirements: "An author can write a post"
- Requirements inform navigation structure, permission systems, content types
- Added to `classification-schemes.md`

**Scales of abstraction** *(Covert)*
- Seven levels: object → interface → location → journey → structure → system → ecosystem
- Changes at one level ripple through others — zoom in and out deliberately
- Added to `user-analysis.md`

**Scanning, satisficing, muddling through** *(Krug)*
- Users scan not read; design for billboards not novels
- Satisficing: users click the first plausible link, not the best option
- Muddling through: users operate with incomplete mental models; "getting it" is materially better
- Added to `SKILL.md` under Understanding People

**First-click testing** *(Krug)*
- Added to user analysis and navigation testing sections

**Organising systems framework** *(Glushko)*
- New section in `SKILL.md`: resource, collection, organising principle, agent, interaction, interaction resource
- Intrinsic vs extrinsic properties; aboutness theory
- Agent types: human curators, self-tagging authors, automated algorithms, community tagging
- Why digital resources can be organised multiple ways simultaneously (iTunes/physical vs digital)
- Added to `SKILL.md` and `ia-patterns.md`

**Five cross-channel heuristics** *(Resmini & Rosati)*
- Place-making, consistency, resilience, reduction, correlation
- Internal consistency (serves its own context) vs external consistency (preserved across channels)
- Cross-channel IA designs semantic structures first, channel implementations second
- Added to `SKILL.md` and `ia-patterns.md`

### Updated files

| File | Changes |
|---|---|
| `skill/SKILL.md` | +200 lines; new sections: LATCH, scanning/satisficing, search systems overview, cross-channel heuristics, organising systems framework, criteria matching, ontology |
| `skill/references/classification-schemes.md` | +120 lines; LATCH expanded; full controlled vocabulary section (synonym rings → thesauri); ontology and nouns+verbs |
| `skill/references/navigation-design.md` | +160 lines; full search systems chapter; wayfinding signals section; faceted navigation; "quick links" anti-pattern; Elementor/WordPress healthcare notes |
| `skill/references/user-analysis.md` | +100 lines; structural audit methodology; scales of abstraction; diagram types; Marquis information-seeking modes |
| `skill/references/ia-patterns.md` | +110 lines; folksonomy failure modes; cross-channel patterns; Glushko organising system framework applied to pattern selection |
| `README.md` | Updated to v2.0.0; new source table; expanded capabilities table; new prompt starters |

### Source additions

- Morville, Rosenfeld & Arango — *Information Architecture for the Web and Beyond* (4th ed., O'Reilly, 2015)
- Marquis, Lisa Maria — *Everyday Information Architecture* (A Book Apart, 2019)
- Covert, Abby — *How to Make Sense of Any Mess* (Self-published, 2014)
- Krug, Steve — *Don't Make Me Think* (New Riders, 3rd ed., 2014)
- Glushko, Robert J. (ed.) — *The Discipline of Organizing* (4th ed., MIT Press, 2016)
- Resmini, Andrea & Rosati, Luca — *Pervasive Information Architecture* (Morgan Kaufmann, 2011)

---

## v1.0.0 — May 2026

Initial release.

### Skill files
- `SKILL.md` — Core skill with People × Content × Context model, IA project phases, classification scheme selector, IA pattern quick reference, labelling rules, design process, testing workflow, documentation guide, and quick decision checklists
- `references/classification-schemes.md` — All 8 classification schemes with full decision rules, tips, and common traps
- `references/ia-patterns.md` — Simple and combined IA patterns with a pattern selection guide
- `references/user-analysis.md` — Research methods, affinity mapping, card sort analysis, information-seeking behaviour types
- `references/navigation-design.md` — Navigation types, design principles, testing methods, anti-patterns, WordPress/Elementor-specific notes

### Audit report generator
- Full `.docx` audit report generation for any URL
- Example: GI Partners of Illinois audit (`examples/GI_Partners_IA_Audit_Report.docx`)

### Sources
Built from Donna Spencer, *A Practical Guide to Information Architecture* (UX Mastery, 2010).
