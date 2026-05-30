# IA Patterns — Full Reference

Source: Donna Spencer, *A Practical Guide to Information Architecture*

---

## Simple Patterns

### Hierarchy
Content organised into parent-child relationships (tree structure).

**Suits:** Varied content, small to large sites, general-purpose.
**Users:** Want to read broadly then drill into detail. Navigate top-down.

**Key design challenge — Breadth vs Depth:**
- Too shallow (2-3 levels, many items per level) → overwhelming choice at each node
- Too deep (6+ levels) → users get lost, can't remember where they are
- Ideal: 3-5 levels, 4-9 items per node (Hick's Law applies)

**Tips:**
- Test with tree testing to identify where users go wrong
- Every item should have one clear home — if it fits two places, it's a labelling or grouping problem
- Breadcrumbs are essential for hierarchy navigation

---

### Database
Content items share a consistent structure (same fields/attributes).

**Suits:** Products, articles, blog posts, events, employees, recipes — any content type where every item has the same pieces.
**Users:** Want to access content in more than one way (by date, by category, by author, by tag).

**Key challenge:** Every item must fit the same structure. Don't force diverse content into a database structure — it produces badly-fitting records.

**Tips:**
- Store once, display many ways — the core power of this pattern
- Only collect metadata fields you will actually use
- Index pages (listing views) are critical — they're where users make decisions
- Pair with a hierarchy for navigation into the database section

---

### Hypertext (Wiki)
Content pieces connected by associative links, no master hierarchy.

**Suits:** Documentation being developed over time; content where you don't know the full scope upfront; Wikipedia-style knowledge bases.
**Users:** Following links to related material; exploring rather than searching.

**Key challenge:** Success entirely depends on authors creating links. Unlike hierarchy (you can always go up a level) or database (you can list all items), hypertext has no automatic fallback if links are missing.

**Tips:**
- Good starting structure for knowledge that grows organically
- Plan to reorganise once the content is known
- Add entry pages and A-Z indexes as anchors

---

### Linear
One thing follows another in a fixed sequence.

**Suits:** Sequential instruction, tutorials where understanding step N requires step N-1.
**Users:** Need to complete a task in a defined order.

**Use sparingly.** If users don't genuinely need to follow sequence, a linear structure is just frustrating. Most web content does not require linear reading.

---

## Combined Patterns

### Hierarchy + Database (most common)
A hierarchical navigation for general content, with database-driven sections for structured content types.

**Example:** A medical clinic site — hierarchical pages for About, Services, Team + a database of blog articles filterable by category and date.

**When to use:** Almost any general website that also has content types (articles, products, team members, case studies).

**Key decision:** What content to structure as a database vs leave as flat pages.
- Use database when: you have 10+ items of the same type, users will want multiple views, or content will keep growing
- Leave as pages when: content is one-off, won't be reused, doesn't need filtering

---

### Catalogue
A hierarchy over a database — typically 2-3 levels of category hierarchy leading to database product/content records.

**Common in:** E-commerce, product catalogues, large article libraries.

**Jared Spool's three page types:**
- **Store pages** → top-level departments
- **Department pages** → sub-categories
- **Gallery pages** → direct access to individual items (hardest-working pages on the site — this is where users decide whether to go deeper)

**Tips:**
- Gallery pages need excellent labelling, imagery, and filtering
- 3 levels max before reaching items — deeper than that and users get lost

---

### Hub & Spoke
Users move from a central hub into detail pages, then return to the hub.

**Common in:** Apps with a home base (LinkedIn profile, dashboard, user account).

**Design note:** This is more about navigation behaviour than content structure. The hub (e.g. profile page, dashboard) must be consistently accessible. Design "return to hub" affordances clearly.

---

### Subsites
A large site as a collection of semi-independent subsites, unified by a home/top-level page.

**Common in:** Universities, government departments, large enterprises with multiple brands or business units.

**Key decisions:**
- Should subsites share navigation, layout, and brand? (Unified feel vs autonomy)
- How does the home page represent the full range of subsites without overwhelming?
- How do users who don't know which subsite to start from find what they need?

**Tips:**
- Each subsite can use its own pattern (some hierarchical, some database)
- Provide cross-subsite search as a safety net
- Top-level navigation must be audience/task-focused, not subsite-listing

---

### Focused Entry Points
A main structure (usually hierarchy) + additional entry points that cut across it for different audiences or task paths.

**Common in:** Government, utilities, information-heavy sites with multiple distinct user groups.

**Example:** A water authority site — main hierarchy of policies and programs + topical entry points (desalination, rainwater tanks, water saving) for users who don't know the program names.

**Why audience/task schemes work better as entry points than as primary structures:**
- Users often don't self-identify cleanly as "Audience A" or "Audience B"
- A task-based entry point ("I want to apply for X") can lead into a subject hierarchy beneath
- Entry points don't need to cover all content — just the most common or confusing paths

---

### Tagged
Content tagged with keywords; tags provide access pathways.

**Common in:** Blogs, photo libraries, large article collections, social content.

**Suits:** Large, diverse content sets where users don't know exactly what they're looking for, or want to explore related content.

**Key question:** Who tags, and how consistently?
- **Author tagging** — fast but inconsistent (authors use different terms)
- **Reader tagging** (folksonomies) — reflects user language but noisy
- **Controlled vocabulary tagging** — most consistent, requires governance overhead

**Tips:**
- Tag cloud navigation works for exploration, not known-item lookup
- Pair with search for known-item tasks
- Define a controlled vocabulary if you need consistency across authors

---

## Pattern Selection Guide

Ask these questions:

1. **How much content will there be, and how fast will it grow?**
   - Small, stable → flat hierarchy or simple pages
   - Large, growing → database or subsites

2. **Does the content have a consistent structure?**
   - Yes, all items same shape → database
   - No, each page different → hierarchy or hypertext

3. **Do users have multiple entry paths to the same content?**
   - Yes → database + metadata + multiple views
   - No → hierarchy is fine

4. **Are there distinct user groups with very different needs?**
   - Yes → focused entry points over a main hierarchy

5. **Is the content being created incrementally without a known full scope?**
   - Yes → hypertext (wiki), plan to reorganise later

6. **Is this primarily transactional (users have tasks to complete)?**
   - Yes → consider hub + spoke or task-based entry points
