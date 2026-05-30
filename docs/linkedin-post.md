We turned one of the best UX books ever written into a Claude skill — and it just saved us 3 hours on a client nav audit.

Here's what we built, how, and why it matters for anyone doing web design work 👇

---

**The problem we kept running into:**

Every client project starts with the same question: is this navigation actually right for users, or just for the organisation that built it?

Most of the time, it's the latter. Navigation structured around internal brand names, departments, and org charts. Labels that make sense to the CEO but not to a first-time visitor.

We knew the principles. We just weren't applying them systematically.

---

**What we built:**

An `ia-practitioner` skill for Claude — a structured framework that Claude uses when evaluating any site's information architecture.

We fed Claude the full text of practitioner IA books, extracted the key decision frameworks, and packaged them as a `.skill` file that installs in one click.

Now when we ask Claude to audit a client site, it:
→ Identifies which user groups are being underserved by the current nav
→ Tests every label against "the word in their head" principle
→ Flags which IA patterns and classification schemes are being violated
→ Proposes a restructured nav with specific before/after comparisons
→ Generates a client-ready Word report in minutes

---

**Live example:**

We ran it on a real client site — a multi-location GI medical group in Illinois.

The audit caught 5 violations immediately:
- Locations organised by internal brand name, not geography
- "Treatments" used for a section patients enter to find symptoms
- "Contact" buried inside About Us
- In The News given equal nav weight to the clinical sections
- No consolidated Patient Resources section

The skill proposed a full nav restructure, wrote the before/after comparison, produced an IA pattern rationale, and generated a 9-section Word doc — all within one conversation.

---

**The sources that trained it:**

The frameworks in the skill come from:
- A Practical Guide to Information Architecture (Spencer)
- Information Architecture for the Web and Beyond (Morville & Rosenfeld)  
- How to Make Sense of Any Mess (Abby Covert)
- Everyday Information Architecture (Lisa Maria Marquis)
- Don't Make Me Think (Steve Krug)

These aren't summaries. The skill contains the actual decision rules, anti-patterns, classification scheme selectors, and labelling tests from the source material.

---

**It's open source.**

Repo: github.com/sidhanth-povil/ia-practitioner

Install the skill, use it on client projects, contribute improvements back.

If you work on websites — as a designer, developer, or agency — this will change how you approach navigation decisions.

---

What's the worst navigation mistake you've seen on a client site? Drop it below 👇

#InformationArchitecture #UXDesign #WebDesign #WordPress #DesignTools #Claude #AI
