---
name: ia-practitioner
description: >
  Apply Donna Spencer's practical Information Architecture framework to any
  design project. Use this skill whenever Sidhanth (or any designer) is working
  on site structure, navigation, content organisation, labelling, card sorting,
  IA testing, sitemap creation, classification schemes, or any UX task that
  involves deciding how to group, label, or connect content. Also trigger when
  the user asks: "how should I structure this site", "what nav should I use",
  "help me organise this content", "how do I label these categories", "should I
  do card sorting", "how do I test my IA", "help me create a sitemap", "what
  classification scheme should I use", or any variant. Apply even when the
  question is phrased as a WordPress/Elementor design question — IA underpins
  all navigation and menu decisions.
---

# IA Practitioner — Donna Spencer Framework

A practical guide to applying *A Practical Guide to Information Architecture*
(Donna Spencer / UX Mastery) to real projects.

---

## Core Model: People × Content × Context

Every IA decision lives at the intersection of three things:

| Dimension | What to understand |
|---|---|
| **People** | Tasks, mental models, terminology, knowledge level, where they use the site |
| **Content** | What exists, what's needed, structure, format, length, accuracy |
| **Context** | Business goals, constraints, tech stack, stakeholders, org culture |

Missing any one of these = guaranteed IA failure. Start here before touching any nav or sitemap.

---

## The Three Jobs of IA

1. **Organise** content into groups that make sense to users (not to the org)
2. **Describe** those groups with labels users recognise
3. **Provide paths** for users to reach what they need

Every deliverable (sitemap, nav, labels, metadata) serves one of these three jobs.

---

## IA Project Phases

```
1. Define    → Goals, constraints, stakeholders, tech, culture
2. Research  → Learn about People + Content
3. Design    → Draft IA, labels, nav
4. Test      → Validate before building
5. Build     → Implement + communicate rationale
6. Maintain  → Document decisions + guidelines
```

Research + communication take more time than design. Never skip them.

For **Agile projects**: focus on big-picture IA + detail for current sprint only.
Use sticky notes / lo-fi artefacts; conversation > documentation.

---

## Understanding People

### What to learn
- What tasks they need to do (not what they think they need)
- Their terminology for things (critical — use their words, not yours)
- What they already know (topic + technology)
- Where and when they use the site (device, context, urgency)
- Their mental model of how things group together

### Research methods — when to use each

| Method | Best for |
|---|---|
| **Interview** | Rich, contextual understanding; exploring why |
| **Observation** | Seeing real behaviour (call centres, fast-paced tasks) |
| **Card sorting** | How users mentally group content; terminology |
| **Survey** | Volume; collecting common info needs in users' words |
| **Web analytics** | What's being used; entry points; popular terms |
| **Search logs** | What people call things; unmet needs |
| **Existing data** | Fast start: emails, help-desk tickets, forums |

Use at least **two methods**. Direct (interview/observation) reveals why. Indirect (analytics/search) reveals what.

### The 5 Whys technique
Start from something you know people want → ask "why do they need that?" → repeat until you hit "I don't know". That's your research question.

### If you can't do research
Write down what you already know. Describe users concretely. Bad decisions come from vague assumptions, not from lack of research tools.

→ For deep analysis methods: see `references/user-analysis.md`

---

## Understanding Content

### Content audit steps
1. Inventory everything (spreadsheet: title, URL, type, owner, last updated, analytics)
2. Assess quality and accuracy
3. Identify structured vs unstructured content
4. Colour-code by usage data to reveal what's working
5. Identify what can be deleted, what needs rewriting, what's missing

### Structured vs unstructured
- **Structured**: all items of a type share the same pieces (database model). Use when content will be generated automatically, displayed in multiple views, or managed at scale.
- **Unstructured**: one-off pages. Fine for low-volume, static content.

Only structure content when you'll actually use that structure (auto-generated lists, multiple views, filtering).

### Content planning — what to define per content type
- Format (article, video, tool, PDF, FAQ)
- Length (check longest + shortest examples)
- Target audience
- Tasks it supports
- Accuracy / update frequency
- Structured fields (if applicable)

### Content priorities
Use one of: value vs cost matrix, scoring system (importance × freshness × availability × author speed), cyclical/seasonal schedule, or core-first release.

Content is the website. Involve authors from day one.

---

## Classification Schemes

Read `references/classification-schemes.md` for the full breakdown.

Quick selector:

| Scheme | Use when |
|---|---|
| **Hierarchical (subject/topic)** | General-purpose; most common |
| **Task-based** | Users have clear, frequent tasks |
| **Audience** | Clearly distinct user groups with very different needs |
| **Time** | News, events, history, sequential content |
| **Alphabetical** | Known-item lookup; best as secondary scheme (A-Z index) |
| **Geographical** | Content where location is a primary attribute AND users understand the geography |
| **Format** | Secondary only — users think topic first, then format |
| **Organisational** | Intranets where dept is genuinely meaningful to users (rare) |

Rules:
- Audiences rarely work as the **only** scheme — pair with subject
- Geography only works if users know the boundaries you use
- Format is almost always secondary, not primary
- A-Z indexes are high-value secondary navigation — never underestimate them

---

## IA Patterns

Read `references/ia-patterns.md` for full pattern details + examples.

Quick reference:

| Pattern | Suits | Key challenge |
|---|---|---|
| **Hierarchy** | Varied content, small/medium sites | Breadth vs depth balance |
| **Database** | Consistent-structure content, large sets | Don't over-collect metadata |
| **Hypertext (wiki)** | Evolving content, unknown structure upfront | Authors must link actively |
| **Linear** | Sequential instruction (use sparingly) | Frustrating unless truly sequential |
| **Hierarchy + Database** | Most real sites | Decide what to structure vs leave flat |
| **Catalogue** | E-commerce, product listings | Gallery page is the hardest-working page |
| **Hub & Spoke** | Apps with a central home base | Navigation style, not structure |
| **Subsites** | Large orgs, diverse content, multiple brands | Consistent nav/brand across subsites |
| **Focused Entry Points** | Multiple audiences, no single best path | Audience/task entry points over a main hierarchy |
| **Tagged** | Large diverse collections, user-driven discovery | Who tags, and how consistently |

Most real sites are **Hierarchy + Database**. Don't over-engineer.

---

## Labels and Language

### What makes a good label
- **Uses your users' exact terminology** (not internal jargon, not invented terms)
- Consistent throughout the site
- Calls things by the correct name (boring is good)
- As clear as possible — no cleverness, no brand-speak

### Getting label ideas
1. User research transcripts — capture verbatim what users say
2. Search logs — what terms do users type?
3. Card sort labels — what did users write on the cards?
4. Competitor sites (for language, not IA)
5. Internal stakeholders — then test against users

### Common labelling traps
- Using internal/org terminology instead of user language
- Trying to be creative or branded ("Our Solutions", "Explore")
- Inconsistency across levels (same thing, two names)
- Labels too broad ("Information", "Resources")
- Labels too narrow (hiding sub-content)

### Label testing
- Show users top-level labels, ask what they'd expect to find inside
- Use tree testing to find where users go wrong
- Check search logs — searches on a site usually mean navigation failed

---

## How to Create IA — The Design Process

1. **Review research** — people needs, content inventory, context
2. **Choose a classification scheme** — match to user mental models
3. **Choose an IA pattern** — match to content + site scale
4. **First draft** — brainstorm groups using user language (sticky notes, index cards)
5. **Gut check** — does every piece of content fit? Does anything fall in two places?
6. **Test with users** (tree test or card sort validation)
7. **Iterate** — change labels, move items, test again
8. **Document rationale** — why this structure, what you tried and rejected

Never show an IA to stakeholders without navigation and page layouts alongside it — too abstract on its own.

---

## Testing IA

### Tree testing (recommended first)
Show users the IA as a hierarchy. Give them a scenario (not using your labels). Ask where they'd look.

**Preparation:**
- Draft IA (can still be rough)
- 8–12 realistic scenarios (avoid using label words in scenario text)
- 5–8 participants minimum

**Scenario writing rule:** describe the user's situation, not the object. "You need the maternity leave policy" → "You've just found out you're having a baby. What are you entitled to?"

**Tools:** Optimal Workshop Treejack, C-inspector, or paper cards (write categories on index cards, walk through with users face to face).

**When to change the IA:**
- Consistent wrong choice → move the content there
- Inconsistent choices → the label is ambiguous, rewrite it
- Everyone goes backwards → the category above is misleading

### Card sorting
**Open card sort** → users create their own groups from content cards. Use to discover mental models early.
**Closed card sort** → users sort into your predefined categories. Use to validate an existing IA.

Tools: Optimal Workshop OptimalSort, or physical index cards.

Analyse for: clusters (what goes together), outliers (where people disagree), and — critically — the **language users wrote** on group headers.

---

## Documenting and Communicating IA

### Two sitemap types

**Conceptual sitemap** — high-level, shapes + connectors, shows overall pattern. Use for team alignment early in the project. Don't share with clients alone — too abstract.

**Detailed sitemap** — every page, numbered, with templates noted. Can be a diagram (good for visual overview) or spreadsheet (better for large sites + project tracking + content migration).

### What to document beyond the sitemap
- **Rationale**: why this structure, what each section contains, what you tried and rejected
- **Maintenance guide**: rules for adding new content, what goes where, how to handle scale
- **What you decided NOT to do** — this is as important as what you did. Document rejected ideas and why.

### Cross-links
Don't try to draw cross-links on sitemaps — too messy. Track them in the content document alongside the copy.

---

## Quick Decision Checklists

### Starting an IA project
- [ ] Do I know the business goals and constraints?
- [ ] Do I understand who the users are and what they need?
- [ ] Do I have a content inventory (or at least a content list)?
- [ ] Do I know which content is structured vs unstructured?

### Choosing a classification scheme
- [ ] What mental model do users have? (Check card sort / interview data)
- [ ] Are there clearly distinct tasks? → task scheme
- [ ] Are there distinct audiences with very different needs? → audience entry points (not primary scheme)
- [ ] Is there a natural, exact scheme (time/geography)? → verify users care about it

### Before designing navigation
- [ ] Is the IA tested and stable?
- [ ] Do I have user terminology confirmed?
- [ ] Do I know the IA pattern I'm using?

---

## Reference Files

| File | When to read |
|---|---|
| `references/classification-schemes.md` | Choosing how to organise content; all 8 schemes with tips |
| `references/ia-patterns.md` | Choosing a structural pattern; all combined patterns with examples |
| `references/user-analysis.md` | Deep analysis methods: affinity mapping, mental models, personas |
| `references/navigation-design.md` | Navigation types, design patterns, testing nav |
