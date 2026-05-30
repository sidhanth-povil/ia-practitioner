# Classification Schemes — Full Reference

Sources: Spencer, Morville & Rosenfeld, Marquis, Covert, Glushko

---

## Exact vs Ambiguous Schemes

**Exact schemes** — categories are predefined, unambiguous, items have one correct home:
- Time, Alphabetical, Geographical, Format, Organisational structure

**Ambiguous schemes** — you design the categories; items may fit multiple places; boundaries are fuzzy:
- Subject/Topic, Task, Audience, Metadata

Exact schemes need less testing. Ambiguous schemes require card sorting and tree testing.

---

## LATCH Expanded *(Wurman via Marquis)*

LATCH (Location, Alphabet, Time, Category, Hierarchy) is a meta-framework for organising anything.

**Limitation:** LATCH conflates ordering methods (L, A, T) with grouping methods (C, H). Once you create categories, you still need to order them — LATCH doesn't answer that question.

**Missing from LATCH:** Organisation by shape or visual fit; mnemonic organisation; algorithmic hierarchy (social media feeds sorted by engagement weight, not any of the five methods).

Real sites typically combine multiple LATCH methods. Netflix uses Category for primary browsing + Hierarchy (by engagement weight) for which categories appear + Time for new releases.

---

## The 8 Classification Schemes *(Spencer)*

### 1. Subject / Topic
Organises content around what it is about.

**Best for:** General-purpose sites; most website hierarchies use this at their core.

**Decision rules:**
- This is the default — use it unless you have strong evidence for another scheme
- Group according to user mental models, not org structure
- Test with card sorting to discover how users categorise
- Avoid creating categories from the org chart

**Common trap:** Building topic categories from internal team names ("Our Solutions", "Service Lines") rather than user-facing terminology ("Website Design", "SEO Audits").

---

### 2. Task
Organises content around what users are trying to do.

**Best for:** Sites where users have frequent, well-defined tasks (e.g. HR intranet: "Apply for leave", "Claim expenses", "Update my details").

**Decision rules:**
- Works best when all users do roughly the same tasks
- Breaks down when tasks overlap many content areas
- Often best as entry points over a subject hierarchy, not the sole scheme
- Validate task labels with real user language — "Apply for leave" vs "Leave request"

**Key insight from Marquis:** Focus on verbs, not audience labels. "Nominate a student", "Recruit scholars", "Support scholars" transcends audience groups and identifies commonalities in user needs better than "For Teachers", "For Universities".

---

### 3. Audience
Organises content by who it's for.

**Best for:** Sites with clearly distinct user groups who have fundamentally different needs and would never look at each other's content.

**Critical warnings:**
- Most content actually serves multiple audiences — don't force it into one group
- Audience schemes fail when users can't self-identify clearly ("Am I a 'Professional' or 'Researcher'?")
- Almost always better as **focused entry points** (landing pages by audience) over a subject hierarchy, rather than as the primary scheme
- Users are visiting to accomplish a task — not to select an identity. Having to first self-select a label adds a friction step
- Because audiences and their tasks overlap, content in audience-specific categories tends to overlap — leading to duplication, confusing search results, and maintenance errors
- Test: can every piece of content be unambiguously assigned to one audience? If not, don't use it as primary.

---

### 4. Time
Organises content by when it was published or when it occurs.

**Best for:** News, blogs, events listings, history, TV guides, scheduled content.

**Decision rules:**
- Two uses: time of publication (news) vs time as an attribute (events, history)
- Only use as primary if users genuinely want to browse by time
- Time adds meaning: when something was published changes how it's understood
- Always offer a secondary scheme (topic, author) so users can find older content
- Time can be a **sequencing method** (newest first) without being a **grouping method**

**Marquis warning on algorithmic time:** When platforms replace chronological with algorithmic ordering (Instagram, Facebook), they impose a hidden hierarchy — corporate valuation masquerading as relevance. Be transparent about your ordering.

---

### 5. Alphabetical
Organises content A-Z.

**Best for:** Known-item lookup when users know the exact name. Dictionaries, glossaries, A-Z indexes.

**Decision rules:**
- Almost never the PRIMARY scheme (only dictionaries/glossaries)
- Extremely high-value as a SECONDARY scheme (A-Z index alongside main nav)
- Users often say "don't take away the A-Z" even on well-designed intranets
- Include synonyms and common misnomers in A-Z (add both terms)
- Use user research to determine terminology — include the "wrong" word if users use it
- Don't list every page — list landing pages and key topics only

**Marquis note:** Alphabetising is for research, not discovery. Never use it as a primary browsing scheme unless users already know exactly what name they're looking for.

---

### 6. Geographical
Organises content by location.

**Best for:** Tourism, real estate, events, local services — any content where location is a primary attribute AND users understand the geography.

**Two criteria for success:**
1. Users actually want to access information geographically
2. Users understand the specific geographic boundaries you're using

**Common trap:** Assuming users know the boundaries. Water catchment areas, government regions, postcodes — users often don't know which one they're in.

**Marquis note:** State capitals are a list of literal locations, but are better organised alphabetically. A list of butcher cuts would be better as a locational illustration (forearm tattoo diagram) despite having nothing to do with geography. Geography as the organising principle is separate from whether content happens to be geographical.

---

### 7. Format
Organises content by its format type (articles, videos, downloads, tools, FAQs).

**Best for:** Instructional/resource sites as a secondary layer.

**Decision rules:**
- Users think "topic first, then format" — they want to find content about a topic before choosing whether to watch a video or read a guide
- Avoid as primary scheme (forces users to know the format before finding the topic)
- Excellent as a secondary filter after finding a topic
- Exception: if users have a strong format preference ("I only watch videos") it may work as primary entry point

---

### 8. Organisational Structure
Organises content by internal teams, departments, or org chart.

**Best for:** Intranets where the organisational structure genuinely maps to user mental models (rare).

**Decision rules:**
- Most users don't know (or care) which department owns what
- Common trap: building the site navigation from the org chart because it's easy internally
- Test rigorously: can users find HR content if it's under "People & Culture"?
- Better to expose org structure as metadata on content pages than as primary navigation
- **Conway's Law** (Marquis): Organisations that design systems will reproduce their communication structures as those systems. Fight this consciously.

---

## Combining Schemes

Most real sites need multiple classification schemes:
- **Primary**: subject hierarchy (or pattern appropriate to content)
- **Secondary**: A-Z index, audience entry points, task entry points, format filter, tag cloud

The primary scheme should serve 80%+ of user tasks. Secondary schemes serve edge cases and different user mental models.

---

## Metadata *(Morville & Rosenfeld / Glushko)*

Metadata = data about data. Three types *(Glushko)*:
- **Intrinsic**: what the object is (type, format, size, date)
- **Administrative**: how it's managed (author, owner, status, URL)
- **Descriptive/Aboutness**: what it's about (title, category, tags, summary)

Use metadata for:
1. Auto-generating content lists (all items in category X)
2. Creating multiple views from one dataset (by date / by author / by tag)

**Rule:** Only collect metadata you will actually use. Over-collecting metadata creates maintenance burden with no payoff.

**Aboutness** requires intellectual effort or statistical computation to determine — it is not directly apparent from looking at a document. Subject classification is intellectually intensive and in many cases requires human judgment.

---

## Controlled Vocabularies *(Morville & Rosenfeld / Covert / Marquis)*

Vocabulary control comes in increasing levels of sophistication:

### Synonym Ring
A set of equivalent terms defined as interchangeable for search retrieval. No preferred term — all are equal.

**Use case:** Product search. When user types "itouch" the search expands to also retrieve "ipod touch" results.

**Warning:** Synonym rings improve recall but can reduce precision. The query expansion happens behind the scenes, which can confuse users who don't see their exact term in results.

### Authority File
A list of preferred (authorised) terms, with variant terms mapped to the preferred form.

**Use case:** Drugstore.com mapping "tilenol" → "Tylenol". Corrects misspellings and teaches preferred terminology.

**Benefits:**
- Content authors use approved terms efficiently and consistently
- Preferred term serves as the unique identifier for each concept
- Navigation stays clean (only preferred terms appear in indexes and menus)
- Educates users toward shared vocabulary

### Classification Scheme / Taxonomy
An arrangement of preferred terms in hierarchical or other relationships.

**Two forms:**
- **Frontend** — a browsable hierarchy that's a visible part of the UI (Dewey Decimal, Netflix genres)
- **Backend** — a tool for authors and indexers to tag content (CMS tagging vocabulary)

**Polyhierarchy**: A concept belonging to more than one parent category. Common in practice; requires careful management to avoid inconsistency.

**Faceted classification**: Classifying resources along multiple independent dimensions simultaneously. Users combine facets to narrow results. Most powerful system for large, structured content collections.

→ See navigation-design.md for faceted navigation design

### Thesaurus
A controlled vocabulary in which equivalence, hierarchical, and associative relationships are all defined.

Technical terminology:
| Term | Meaning |
|---|---|
| **PT** — Preferred Term | The authorised term; all relationships defined with respect to it |
| **VT** — Variant Term | Synonym or near-synonym mapped to the PT |
| **BT** — Broader Term | Parent of the PT (one level up in hierarchy) |
| **NT** — Narrower Term | Child of the PT (one level down) |
| **RT** — Related Term | Associatively related (See Also) |
| **SN** — Scope Note | Definition restricting the PT's meaning to avoid ambiguity |

**When to use a thesaurus:** Large information environments with professional indexers, medical/legal/scientific content, enterprise search systems where vocabulary control dramatically improves retrieval.

---

## Ontology *(Covert)*

Ontology is the declaration of what terms mean in a specific context — more precise than a dictionary (lexicography), which collects varied meanings.

Examples of ontological decisions:
- Social networks redefining "like" and "friend" for their purposes
- The "folders" on a computer's "desktop" you use to organise "files"
- Fast food ordering by number

**Process:**
1. Write terms on sticky notes
2. Arrange by relationship on a surface
3. Test the arrangement with users and stakeholders
4. Document what you DO say and — equally importantly — what you DON'T say

**"Don't say" lists** can be more powerful than "do say" lists. Documenting forbidden terms — ones with historical baggage, internal jargon, alternative meaning to users — prevents the vocabulary from drifting back to org-speak.

**Nouns + verbs = requirements:**
Identify the nouns (objects) and verbs (actions) in your domain. Combine them into explicit requirements:
- "An author can write a post"
- "Any user can share a post"
- "An administrator can delete a post"

This forces clarity about who can do what — and directly informs navigation structure, permission systems, and content types.
