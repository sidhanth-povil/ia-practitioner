# Navigation Design — Reference

Sources: Spencer, Morville & Rosenfeld, Krug, Marquis, Resmini & Rosati

---

## Navigation vs IA

Navigation and IA are deeply connected but separate:
- **IA** = the groups, labels, and structure
- **Navigation** = how users get to those groups and content

Design IA first, then design navigation. Navigation is dependent on a stable IA.

---

## Navigation Types *(Morville & Rosenfeld / Marquis)*

### Primary / Main navigation
The main entry into the site structure. Exposes top-level IA categories.
- Should reflect user mental models and user terminology
- Typically 4-8 items (Hick's Law — more items = more decision time)
- Should be consistent across all pages
- The category labels here ARE part of the user experience — they tell a story about the organisation's purpose

### Secondary navigation
Sub-navigation within a section. Exposes second-level IA.
- Often contextual — appears only within a section
- Should always make parent section clear

### Utility navigation
Functional items like logins, account access, shopping carts, directories.
- Not every site needs it; often overlaps with secondary nav on smaller sites

### In-page / Contextual navigation
Links within body content (hypertext).
- Critical in hypertext and database patterns
- Anchor links for long pages
- Related content links

### Supplemental navigation (extras)
A-Z indexes, sitemaps, guides, breadcrumbs, "related articles", site search.
- **A-Z index**: high-value for known-item seeking; captures users who fail primary nav
- **Breadcrumbs**: essential in hierarchy patterns; shows current location and path back
- **Sitemap**: helps users with unusual mental models; rescue navigation
- **Search**: a navigation system in itself — see Search Systems section below

### Footer and header navigation
- Footer typically repeats main nav at first level, or surfaces important but secondary links (privacy, contact, sitemap)
- Header holds secondary or utility nav
- Footer is a way of exposing more content without distracting from main page layout

---

## Navigation Design Principles *(Spencer / Krug / Marquis)*

**1. Show where users are**
Users need to know: where am I, where can I go, where have I been.
Use: active states on nav items, breadcrumbs, page titles that match nav labels, clear visual hierarchy.

**2. Use consistent labels**
Navigation labels must match page headings. If the nav says "Our Services" and the page says "What We Offer", users question whether they're in the right place.

**3. Don't rely on hover**
Mobile users can't hover. All navigation must be accessible on touch.

**4. Reveal enough, hide enough**
Mega-menus can show more structure but overwhelm. Collapsed menus hide structure but reduce cognitive load. Test with real users.

**5. Match the IA pattern**
- Hierarchy → persistent top nav + breadcrumbs + section nav
- Database → filtering + sorting + multiple index views
- Hub & Spoke → clear "back to hub" always accessible
- Tagged → tag browsing + faceted filtering

**6. Every page needs a next step *(Marquis)***
Every page should have a clear primary call to action — a direction for the user. Pages without calls to action are dead ends. The more navigation structures on a page, the harder it is to see the primary action.

**7. Balanced pathways *(Marquis)***
- Too many paths → choice paralysis; users abandon
- Too few paths → dead ends; users hit back
- Less navigation is often more effective, not less (Seton Hill case: simplifying from 8 items to 3 doubled landing page sessions and increased new users 185%)

---

## Wayfinding Signals *(Marquis)*

Users look for these signals to orient themselves — often unconsciously:
- Navigation structures
- Page titles and headings
- **Breadcrumbs** — show hierarchical path; explicit placemaking; loved by SEO
- **URLs** — communicates location AND trustworthiness; misleading URLs undermine credibility
- Pagination and frames
- Buttons and calls to action
- Search results
- Imagery and captions
- Text links

**Information scent**: The cues that tell a user they're getting closer to what they need. Weak information scent → users go back and try a different path.

### Breadcrumbs
- Prominent enough to be spotted, subtle enough not to distract
- Spell out the established path (not necessarily the user's actual path, but a contextual anchor)
- Do not require strong design to work — explicit is better than clever
- Google likes breadcrumbs (structured data benefit)

### URL structures
- Clean, hierarchical URLs mirror the IA and provide navigational context
- Inconsistent URL structures (some with folders, some without) signal unreliability
- Misleading or masked URLs destroy trust — critical in post-misinformation web

---

## Designing Navigation — Process

1. Review the tested IA
2. Decide which IA levels to expose in primary vs secondary nav
3. Decide what supplemental navigation to add (A-Z, breadcrumbs, related links)
4. Sketch navigation in context of page layouts
5. Test navigation
6. Communicate navigation alongside IA (never IA alone)

---

## Testing Navigation *(Krug / Spencer)*

**Paper prototype / wireframe testing**
Show users navigation in the context of page layouts. Ask them to find specific things. Watch where they go and where they get confused. More realistic than tree testing because users can see the full page context.

**First-click testing**
Ask users: given this scenario, what's the first thing you'd click? Simple, fast, highly predictive. First click strongly correlates with overall task success.

**Analytics signals that navigation is failing:**
- High search use (users can't find via nav)
- High bounce rate from section landing pages
- Unexpected paths through the site
- High "back" button use from deep pages
- Direct URL entry for buried content

---

## Search Systems *(Morville & Rosenfeld)*

Search is a navigation system — design it as one.

**Search is not a band-aid** for poor information architecture. Bad navigation + good search = users who search instead of browse, never discovering what they didn't know to search for.

### When to add search

Add search when:
- Too much content to browse comfortably
- Content is fragmented across silos
- Content is highly dynamic (news, frequent updates)
- Users expect it (it's a standard convention)

**Fix navigation first, then add search.** A well-designed navigation + search works better than search compensating for broken navigation.

### Search system anatomy

**What to index:**
- **Search zones** — subsets indexed separately; reduces apples-and-oranges results
- **Destination vs navigation pages** — index destination pages; exclude navigation/listing pages from results (they clutter results with pages users didn't want)
- **Content components** — which fields in a document to search (title, body, tags, date)

**Retrieval algorithms:**
- **Recall vs precision tradeoff**: High recall = more results (some irrelevant); high precision = fewer but more relevant results. Match to user need.
- **Stemming**: Expands terms to word variants (lodge → lodging, lodger) — improves recall
- **Pattern matching**: Looks for exact text strings — simplest; doesn't handle synonyms
- **Relevance ranking**: Factors in term frequency, term proximity, location (title vs body), document popularity

**Query builders (invisible enhancements):**
- Spell checkers — correct typos before querying
- Stemming tools — expand to word variants
- Phonetic tools — handle name variations (Smith/Smyth)
- Controlled vocabulary / synonym rings — map user terms to preferred terms
- Autocomplete/autosuggest — surfaces vocabulary and reduces zero-result queries

### Presenting search results

**Which content components to display:**
- Known-item searchers: show less (title, date, location)
- Exploratory searchers: show more (summary, category, key metadata, image)
- When titles are similar: add distinguishing components (format, date, section)

**Listing/ranking approaches:**
- Alphabetical sort — good for name lookup
- Chronological sort — news, events, time-sensitive content
- Relevance ranking — understanding/research tasks
- Popularity ranking — discovery tasks, social signals
- Best bets — manually curated top results for high-frequency queries

**Grouping/clustering:**
- Cluster results by topic, audience, format — reduces overwhelm on large result sets
- Show total results count
- Allow search revision from results page (show query, allow editing)

**No dead ends policy:**
When users get zero results, always offer:
1. A way to revise the search
2. Search tips
3. A browse path (nav/sitemap)
4. A human contact option

### Search interface design

**The box**: One search box, one "Search" button. Simple. Users have been trained by Google — don't deviate without strong reason.

**Autocomplete/autosuggest**: Surfaces vocabulary terms and query patterns; modern replacement for "advanced search" in most cases; reduces misspellings and zero-result queries.

**Advanced search**: Reserve for power users (librarians, researchers, legal). If your default search is well-configured, most users should never need it.

**Supporting revision:**
- Repeat query in results page
- Explain what was searched (which zones, which filters)
- Show total results
- Allow narrowing within results

### Faceted navigation *(Morville & Rosenfeld / Marquis)*

Faceted classification = tagging resources along multiple independent dimensions simultaneously, then allowing users to filter by combining facets.

**Design requirements:**
1. The taxonomy must be documented and systematically applied to all content
2. Users must apply the taxonomy consistently (or it must be automated)
3. Facets must be mutually independent (filtering by one shouldn't invalidate another)
4. Clear display of which facets are active

**Best for:** Large structured content collections — e-commerce, recipe sites, academic databases, job boards, rental listings.

**Classic example:** Ravelry's pattern search allows filtering by craft type, product type, yarn weight, needle size, technique — each facet independent, combinations producing precise results.

---

## Navigation Anti-Patterns *(Spencer / Marquis / Krug)*

| Anti-pattern | Problem |
|---|---|
| Org chart nav | Users don't know which department owns what; Conway's Law in action |
| Clever/branded labels | "Explore" / "Discover" / "Moments" tell users nothing |
| Audience nav as primary | Users can't self-identify reliably; creates content duplication |
| Too many top-level items | Violates Hick's Law; decision paralysis |
| Nav-less pages / dead ends | Users feel trapped; can't get back |
| Inconsistent labels (nav vs page) | Creates doubt about location |
| "Quick links" modules | Junk drawer; signals underlying IA failure; often politically motivated |
| Navigation without calls to action | Pages with no next step are dead ends |
| Hiding nav behind hamburger (mobile) | Users don't know what navigation exists |
| Footer as only nav | Users don't scroll to find navigation |

### On "quick links" *(Marquis)*
Quick links are almost always a symptom of poor IA, not a solution. If content is hard to find, the right fix is better structure and clearer labels — not a list module that avoids the structural problem. When stakeholders request quick links, push back:
- What does "quick" mean? What are the criteria for inclusion?
- Quick for whom? Which audiences are being prioritised?
- Why can't this content be found through normal routes?

---

## Social Navigation *(Morville & Rosenfeld)*

Dynamically generated navigation based on collective user behaviour:
- Popularity-based ordering (Reddit votes, "most read" sections)
- Social graph filtering (Facebook's timeline, "recommended because X liked it")
- Collaborative filtering ("Users who viewed this also viewed...")

**Warning**: Systems too precisely tuned to one user's social graph become echo chambers. Global navigation still needs to provide some shared, consistent structure — for placemaking and collective orientation.

---

## Navigation for Elementor / WordPress (Sidhanth-specific)

**WordPress menu hierarchy maps to:**
- Primary nav = top-level menu items
- Secondary nav = sub-menus (mega-menu for large sites, max 2 levels)
- Footer nav = utility nav (privacy, contact, sitemap)

**Elementor nav widget considerations:**
- Use Elementor Pro Nav Menu widget for mega-menus
- Off-canvas nav for mobile — always test on actual mobile devices, not just browser responsive view
- Breadcrumbs: Yoast SEO or RankMath generate breadcrumb schema automatically
- A-Z index: usually a custom query loop or ACF relationship field
- Keep reduced-motion in mind for nav transitions: `prefers-reduced-motion` media query required

**Critical rule from Elementor GSAP work:**
Navigation transitions must use `prefers-reduced-motion` media query. Never animate navigation in a way that delays user feedback — especially for mobile nav open/close.

**For healthcare sites (medicalsuite.ai):**
- Regulatory labels (DHA, MOHAP, NABIDH) must be consistent throughout — use controlled vocabulary
- Patient-facing navigation must use plain language, not clinical terminology
- Search is essential: patients often don't know the correct medical category for their symptoms
- Audience-based navigation ("For Patients" / "For Doctors") — avoid as primary scheme; use focused entry points or task-based approach instead
