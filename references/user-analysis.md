# User Analysis Methods — Reference

Sources: Spencer, Morville & Rosenfeld, Marquis, Krug, Glushko

---

## Analysis Goal

Convert raw research (interview transcripts, card sorts, surveys, analytics) into
actionable insights about:
- What people need
- How they think about the content
- The terminology they use
- Patterns across users

Analysis is not optional. Without it, you'll remember only what was most surprising or most recent, not what's most representative.

---

## Analysis Steps

1. **Immerse** — Read/listen to all raw data before sorting. Don't start analysing until you've seen everything.
2. **Extract** — Pull out observations, quotes, needs, behaviours. One idea per note/card.
3. **Cluster** — Group similar observations together (affinity mapping).
4. **Name clusters** — Write a short label that describes the pattern in each cluster.
5. **Identify themes** — Look for patterns across clusters: consistent needs, consistent language, consistent mental models.
6. **Prioritise** — Which insights affect the most users? Which affect the highest-stakes tasks?
7. **Document** — Write up findings in a form useful to your team.

---

## Affinity Mapping

Write each observation on a separate card/sticky note. Group cards that belong together. Label each group. Repeat at a higher level until you have 5-10 top-level themes.

Best done collaboratively — multiple people grouping catches more patterns and creates shared understanding.

---

## Card Sort Analysis

**Open card sort output:**
- Look for groups that appeared consistently across participants
- Pay special attention to the **words participants used for group names** — this is gold for labelling
- Note items that participants disagreed on — these are your IA problem areas
- Note items placed in unexpected groups — signals a mental model different from yours

**Closed card sort output:**
- High agreement on placement → item belongs there
- Low agreement → item is ambiguous; needs better labelling, a different home, or appears in multiple places
- Consistent "wrong" placement → consider moving the item to where users actually put it

**Key insight:** Users cluster by their mental models and use their own language. The group names they write are often better labels than anything you'd invent.

---

## Structural Audit *(Marquis)*

A structural audit reviews the site as a user would experience it — tracking hierarchy, crosslinks, navigation inconsistencies, and structural patterns.

**When to conduct:**
- Before building a new sitemap
- When redesigning an existing site
- When you need to understand how content is actually organised vs how it was intended

**What to track in the spreadsheet:**
- Page ID (decimal outline: 1.0, 1.1, 1.2, 2.0...)
- URL (periodic; used as anchor and duplicate detector)
- Navigation label / link text (captures mismatches between link and page heading)
- Page heading / H1 (what the page owner calls it)
- Page title (metadata title — often different from heading)
- Section (which top-level area the page lives in)
- Notes (structural anomalies, missing subnav, unexpected templates)

**What to watch for:**
- Crosslinks (same page accessible from multiple navigation paths)
- On-page links (pages accessible only via body content links, not navigation)
- External links (nav links leaving the domain)
- Unknown hierarchy (pages that don't fit anywhere obvious)
- Dynamic collections (mark with 'x' rather than listing every instance: 2.8.x for news articles)

**Process:** Start on the homepage. Explore main navigation before secondary. Move left to right, top to bottom. Record every page reachable from navigation.

---

## Content Audit for Categorisation *(Marquis)*

After inventory, evaluate the distribution and quality of content to inform category decisions.

**Questions the audit should answer:**
- How is content distributed across sections? (Does distribution reflect stated priorities?)
- Which sections are too large? Too small?
- Where is content depth vs. breadth? (Wide/shallow vs. narrow/deep)
- What's evergreen vs. dynamic?
- What's missing for the users you're trying to serve?

**Technique:** Visualise the current sitemap with cards (sticky notes, Trello, Boardthing). Colour-code by top-level category. Moving cards reveals how much content-shuffling is required and whether the new categories will have appropriate depth.

---

## Communicating About Users

### User profiles
Descriptions of user types, including:
- Typical goals and tasks
- Level of knowledge (topic + technology)
- Terminology they use
- Context of use (device, location, time pressure)
- Attitudes and pain points

Keep profiles realistic and grounded in research. Include verbatim quotes.

### Scenarios
Short narratives describing a specific user doing a specific task in a specific context.
Use to: test IA, brief authors, evaluate designs, communicate user needs to developers.

**Critical for tree testing:** Write scenarios that describe the user's situation without using the label words. "You've just found out you're having a baby. What are you entitled to?" — not "Find the maternity leave policy."

### Information needs diagrams
Map user needs against content types. Shows:
- What users want to do → what content serves that need
- Gaps (user needs with no matching content)
- Orphans (content with no identifiable user need)

Powerful for communicating to content authors — shows them why content matters.

---

## Information-Seeking Behaviours *(Spencer / Marquis)*

| Mode | Behaviour | IA support needed |
|---|---|---|
| **Known-item seeking** | Knows exactly what they want, not where to find it | A-Z index, search, direct labelling |
| **Exploratory seeking** | Browsing, learning, doesn't know exactly what's there | Clear categories, related links, serendipitous discovery |
| **Re-finding** | Looking for something previously found | Bookmarks, recent, search history, persistent URLs |
| **"Don't know what I need"** | Wants to learn but doesn't know what question to ask | Guided paths, curated entry points, progressive disclosure |

**Marquis on designing for mode:**
The question to ask: "What must users already know in order to find what they're looking for?" Systems that require specialised knowledge to navigate only support known-item seekers. Systems that support browsing lower the barrier to exploration.

**Krug on scanning behaviour:**
Users act like sharks — they have to keep moving. They scan for words that match their task or interests. They don't read page copy before deciding whether to click. They click the first plausible link (satisficing). Design for the billboard, not the novel.

---

## Mental Models *(Covert)*

A mental model is the internal belief structure and thought process a user uses to make sense of the world.

Users reference their mental model when navigating — they look for patterns matching what they already know. When the IA doesn't match their mental model, they get lost.

**Surfacing mental models:**
- Card sort group names reveal user mental models for content categories
- Interview probing ("walk me through how you'd think about finding X")
- Observation of navigation behaviour — where do users look first?
- Search log analysis — what do users type when looking for something?

**Mental models and taxonomies *(Glushko)*:**
The tomato problem: scientifically a fruit, culturally a vegetable. Classification systems that don't match user mental models create findability problems — even when the classification is technically "correct". Always verify your classification against user mental models, not just internal logic.

---

## Terminology Analysis

The most practically valuable output of user research for IA work.

Capture:
- What words users use to describe each content type
- What words they use for actions ("apply", "register", "enrol", "sign up")
- What words they use for categories
- What synonyms or near-synonyms exist
- What "official" terms are NOT used by users
- What acronyms users don't recognise

Use this directly in:
- Navigation labels
- Page titles and headings
- A-Z index terms
- Search synonyms / redirects
- Card sort design (use their terms, not yours)
- Controlled vocabulary "do say / don't say" lists

---

## Scales of Abstraction *(Covert)*

When making IA decisions, clarify what level you're working at:

| Level | What it means |
|---|---|
| **Object** | A specific thing (a document, a product page) |
| **Interface** | The point where a user affects that thing |
| **Location** | A specific place or position within the system |
| **Journey** | The steps within or between locations |
| **Structure** | A configuration of objects and locations |
| **System** | A set of structures working together |
| **Ecosystem** | A collection of related systems |

Zoom in to the appropriate level. When deep in detail, zoom out to check the broader effect. Changes at one level ripple through others.

---

## Diagrams for IA Work *(Covert)*

Useful diagram types for IA communication:

| Diagram | Use |
|---|---|
| **Block diagram** | How objects and attributes interrelate to create a concept |
| **Flow diagram** | Steps in a process, including conditions and connections |
| **Hierarchy diagram** | How objects, concepts, or pages relate in a parent-child structure (sitemaps) |
| **Swim lane diagram** | How multiple users/systems work together in a shared process |
| **Mind map** | Connections between concepts without an established hierarchy |
| **Journey map** | All steps and places that make up a user's experience |
| **Matrix diagram** | Capturing multiple variables against each other (good for facilitated discussions) |

**Principle:** Keep diagrams tidy enough for stakeholders to understand, flexible enough to change quickly. Don't over-polish early — polish locks in decisions.

**Scope and scale:** Define what the diagram covers (scope) and at what level of detail (scale) before drawing. "What are the edges of this map? What am I NOT mapping?"
