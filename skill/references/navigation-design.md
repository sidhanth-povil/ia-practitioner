# Navigation Design — Reference

Source: Donna Spencer, *A Practical Guide to Information Architecture*

---

## Navigation vs IA

Navigation and IA are deeply connected but separate:
- **IA** = the groups, labels, and structure
- **Navigation** = how users get to those groups and content

Design IA first, then design navigation. Navigation is dependent on a stable IA.

---

## Navigation Types

### Primary navigation
The main entry into the site structure. Exposes top-level IA categories.
- Should reflect user mental models and user terminology
- Typically 4-8 items (Hick's Law — more items = more decision time)
- Should be consistent across all pages

### Secondary navigation
Sub-navigation within a section. Exposes second-level IA.
- Often contextual — appears only within a section
- Should always make parent section clear

### In-page navigation
Links within body content (hypertext).
- Critical in hypertext and database patterns
- Anchor links for long pages
- Related content links

### Supplementary navigation (extras)
A-Z indexes, sitemaps, tag clouds, breadcrumbs, "related articles".
- A-Z index: high-value for known-item seeking; captures users who fail primary nav
- Breadcrumbs: essential in hierarchy patterns; shows current location and path back
- Sitemap: helps users with unusual mental models; rescue navigation
- Tag cloud: aids exploration in database/tagged patterns

### Search
A navigation system in itself. Always offer search as a complement to browse navigation — don't treat it as a substitute.

Search is not a workaround for bad IA. Bad navigation + good search = users who search instead of browse, never discovering what they didn't know to search for.

---

## Navigation Design Principles

**1. Show where users are**
Users need to know: where am I, where can I go, where have I been.
Use: active states on nav items, breadcrumbs, page titles that match nav labels.

**2. Use consistent labels**
Navigation labels must match page headings. If the nav says "Our Services" and the page says "What We Offer", users question whether they're in the right place.

**3. Don't rely on hover**
Mobile users can't hover. All navigation must be accessible on touch.

**4. Reveal enough, hide enough**
Mega-menus can show more structure but overwhelm. Collapsed menus hide structure but reduce cognitive load. Test with real users to find the right balance for your content volume.

**5. Match the IA pattern**
- Hierarchy → persistent top nav + breadcrumbs + section nav
- Database → filtering + sorting + multiple index views
- Hub & Spoke → clear "back to hub" always accessible
- Tagged → tag browsing + faceted filtering

---

## Designing Navigation — Process

1. Review the tested IA
2. Decide which IA levels to expose in primary vs secondary nav
3. Decide what supplementary navigation to add (A-Z, breadcrumbs, related links)
4. Sketch navigation in context of page layouts
5. Test navigation (see below)
6. Communicate navigation alongside IA (never IA alone)

---

## Testing Navigation

**Paper prototype / wireframe testing**
Show users navigation in the context of page layouts. Ask them to find specific things. Watch where they go and where they get confused.

More realistic than tree testing because users can see the full page context (not just the hierarchy).

**Tree testing with nav context**
Tools like PlainFrame allow testing navigation as positioned on-screen rather than just as a hierarchy tree. Good for testing whether visual placement of nav affects findability.

**First-click testing**
Ask users: given this scenario, what's the first thing you'd click? Simple, fast, highly predictive — the first click is strongly correlated with task success.

**Analytics signals that navigation is failing:**
- High search use (users can't find via nav)
- High bounce rate from nav pages
- Unexpected paths through the site
- High "back" button use from section landing pages
- Direct URL entry for content buried in the hierarchy

---

## Navigation Anti-Patterns

| Anti-pattern | Problem |
|---|---|
| Org chart nav | Users don't know which department owns what |
| Clever/branded labels | "Explore" / "Discover" tell users nothing |
| Too many top-level items | Violates Hick's Law; decision paralysis |
| Nav-less pages | Users feel trapped; can't get back |
| Inconsistent labels (nav vs page) | Creates doubt about location |
| Mobile nav hidden behind hamburger with no peek | Users don't know what navigation exists |
| Audience nav as sole primary nav | Users can't self-identify reliably |

---

## Navigation for Elementor / WordPress (Sidhanth-specific)

**WordPress menu hierarchy maps to:**
- Primary nav = top-level menu items
- Secondary nav = sub-menus (mega-menu for large sites)
- Footer nav = utility nav (privacy, contact, sitemap)

**Elementor nav widget considerations:**
- Use Elementor Pro Nav Menu widget for mega-menus
- Anchor + off-canvas nav for mobile — always test on actual mobile
- Breadcrumbs: Yoast SEO or RankMath generate breadcrumb schema automatically
- A-Z index: usually a custom query loop or ACF relationship field

**Critical rule from Elementor GSAP work:**
Navigation transitions must use `prefers-reduced-motion` media query. Never animate navigation in a way that delays user feedback.
