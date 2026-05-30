# Classification Schemes — Full Reference

Source: Donna Spencer, *A Practical Guide to Information Architecture*

---

## Exact vs Ambiguous Schemes

**Exact schemes** — categories are predefined, unambiguous, items have one correct home:
- Time, Alphabetical, Geographical, Format, Organisational structure

**Ambiguous schemes** — you design the categories; items may fit multiple places; boundaries are fuzzy:
- Subject/Topic, Task, Audience, Metadata

Exact schemes need less testing to implement. Ambiguous schemes require card sorting and tree testing.

---

## The 8 Schemes

### 1. Subject / Topic
Organises content around what it is about.

**Best for:** General-purpose sites; most website hierarchies use this at their core.

**Tips:**
- This is the default — use it unless you have strong evidence for another scheme
- Group according to user mental models, not org structure
- Test with card sorting to discover how users categorise
- Avoid creating categories from the org chart

---

### 2. Task
Organises content around what users are trying to do.

**Best for:** Sites where users have frequent, well-defined tasks (e.g. HR intranet: "Apply for leave", "Claim expenses", "Update my details").

**Tips:**
- Works best when all users do roughly the same tasks
- Breaks down when tasks overlap many content areas
- Often best as entry points over a subject hierarchy, not the sole scheme
- Validate task labels with real user language — "Apply for leave" vs "Leave request"

---

### 3. Audience
Organises content by who it's for.

**Best for:** Sites with clearly distinct user groups who have fundamentally different needs and would never look at each other's content.

**Tips (critical):**
- Most content actually serves multiple audiences — don't force it into one group
- Audience schemes fail when users can't self-identify clearly ("Am I a 'Professional' or 'Researcher'?")
- Almost always better as **focused entry points** (landing pages by audience) over a subject hierarchy, rather than as the primary scheme
- Test: can every piece of content be unambiguously assigned to one audience? If not, don't use it as primary.

---

### 4. Time
Organises content by when it was published or when it occurs.

**Best for:** News, blogs, events listings, history, TV guides, scheduled content.

**Tips:**
- Two uses: time of publication (news) vs time as an attribute (events, history)
- Only use as primary if users genuinely want to browse by time
- Check analytics: do users scan chronologically, or do they search by topic?
- Always offer a secondary scheme (topic, author) so users can find older content
- Time can be a **sequencing method** (newest first) without being a **grouping method** — distinguish the two

---

### 5. Alphabetical
Organises content A-Z.

**Best for:** Known-item lookup when users know the exact name. Dictionaries, glossaries, A-Z indexes.

**Tips:**
- Almost never the PRIMARY scheme (only dictionaries/glossaries)
- Extremely high-value as a SECONDARY scheme (A-Z index alongside main nav)
- Users often say "don't take away the A-Z" even on well-designed intranets
- Include synonyms and common misnomers in A-Z (add both terms)
- Use user research to determine terminology — include the "wrong" word if users use it
- Don't list every page — list landing pages and key topics only

---

### 6. Geographical
Organises content by location.

**Best for:** Tourism, real estate, events, local services, environmental data — any content where location is a primary attribute AND users understand the geography.

**Two criteria for success:**
1. Users actually want to access information geographically
2. Users understand the specific geographic boundaries you're using

**Common trap:** Assuming users know the boundaries. Water catchment areas, government regions, postcodes — users often don't know which one they're in.

**Tips:**
- Map for **displaying** information (precise) vs map for **navigating** to information (approximate) — two different use cases
- Offer topical scheme alongside geographical for when users don't know the geography
- Geography works well as secondary scheme ("Find events near me")

---

### 7. Format
Organises content by its format type (articles, videos, downloads, tools, FAQs).

**Best for:** Instructional/resource sites as a secondary layer.

**Tips:**
- Users think "topic first, then format" — they want to find content about varnishing a deck before choosing whether to watch a video or read a guide
- Avoid as primary scheme (forces users to know the format before finding the topic)
- Excellent as a secondary filter after finding a topic
- Exception: if users have a strong format preference ("I only watch videos") it may work as primary entry point

---

### 8. Organisational Structure
Organises content by internal teams, departments, or org chart.

**Best for:** Intranets where the organisational structure genuinely maps to user mental models (rare).

**Tips:**
- Most users don't know (or care) which department owns what
- Common trap: building the site navigation from the org chart because it's easy internally
- Test rigorously: can users find HR content if it's under "People & Culture"?
- Better to expose org structure as metadata on content pages than as primary navigation

---

## Combining Schemes

Most real sites need multiple classification schemes:
- **Primary**: subject hierarchy (or pattern appropriate to content)
- **Secondary**: A-Z index, audience entry points, task entry points, format filter, tag cloud

The primary scheme should serve 80%+ of user tasks. Secondary schemes serve edge cases and different user mental models.

---

## Metadata

Metadata = data about data. Three types:
- **Intrinsic**: what the object is (type, format)
- **Administrative**: how it's managed (author, date, owner, status, URL)
- **Descriptive**: what it's about (title, category, tags, summary)

Use metadata for:
1. Auto-generating content lists (all items in category X)
2. Creating multiple views from one dataset (by date / by author / by tag)

**Rule:** Only collect metadata you will actually use. Over-collecting metadata creates maintenance burden with no payoff.
