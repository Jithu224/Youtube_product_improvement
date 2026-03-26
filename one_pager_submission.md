# YouTube — What I'd Improve

**Jithendra Sarwad** | PM Internship Assignment | March 2026

---

### 1. Goal — YouTube's 2026 North Star

YouTube's CEO Neal Mohan stated the 2026 priority is **"Reinventing entertainment across ALL formats"** — Shorts, long-form, live, TV.

**The tension**: YouTube says "all formats" but acts "Shorts first" — long-form home feed slots cut by 80%, Shorts now account for 77% of global views. This gap is our opportunity.

> *Rationale: See [Supporting Document — Section 1](#) for goal credibility analysis (8/10).*

---

### 2. Problem Statement

YouTube's product decisions are pushing away intent-driven users — learners, researchers, and subscribers — by flooding the home feed with Shorts and degrading search quality through filter removals. This contradicts the platform's own stated goal and risks long-term engagement decline for its most valuable user segments.

> *Rationale: See [Supporting Document — Section 2](#) for thesis development.*

---

### 3. Pain Points (5 Identified → 2 Selected)

| Selected | Pain Point | Score |
|:--------:|-----------|:-----:|
| **P1** | **Home feed overwhelmed by Shorts** — long-form recs cut 80%, feed exhausts in 2 scrolls | **9.25/10** |
| **P4** | **Search quality degraded** — "Rating" and "Last Hour" filters removed Jan 2026, Shorts + AI slop pollute results | **8.00/10** |

**Excluded**: Excessive ads (7.75) — ads are YouTube's $40B revenue engine, not a product bug. Suggesting "reduce ads" shows no PM judgment.

> *Rationale: See [Supporting Document — Section 3](#) for all 5 pain points with evidence and scoring matrix.*

---

### 4. User Stories

- **The Learner**: *"I open YouTube to learn Python, but my feed is 80% Shorts. I can't find a quality tutorial without digging."*
- **The Subscriber**: *"I follow 50+ channels but their uploads are buried under algorithmic Shorts recommendations."*
- **The Researcher**: *"I search 'best laptop review' and get AI slop, clickbait, and Shorts — the filters I need were removed."*

> *Rationale: See [Supporting Document — Section 4](#) for full persona definitions.*

---

### 5. Features

**F1: Intent-Based Feed Modes** — Replace generic topic chips with intent chips: `Learn` | `Catch up` | `Discover` | `Quick watch` | `Deep dive`. Each mode changes what the algorithm serves. Users who want Shorts choose "Quick watch" — YouTube keeps Shorts revenue while serving all intents.

**F4: Enhanced Search Filters** — Restore removed "Rating" and "Last Hour" filters. Add `Long-form only` toggle, duration presets, and quality signals (% liked, verified badge, AI-generated label) on search results.

> *Rationale: See [Supporting Document — Section 5](#) for all 6 features considered.*

---

### 6. RICE Prioritization

| Feature | Reach | Impact | Confidence | Effort | RICE |
|---------|:-----:|:------:|:----------:|:------:|:----:|
| **F1: Intent-Based Feed Modes** | 9 | 9 | 7 | 3 | **189** |
| **F4: Search Format Filters** | 8 | 8 | 9 | 8 | **72** |

**F1** = primary (transformative). **F4** = quick win (low effort, high confidence).

> *Rationale: See [Supporting Document — Section 6](#) for RICE scoring of all 6 features.*

---

### 7. Prototype

**Live interactive prototype**: [jithu224.github.io/Youtube_product_improvement](https://jithu224.github.io/Youtube_product_improvement/)

Before/after toggle showing current YouTube vs proposed features. Mobile + desktop responsive. Try switching between Learn, Catch up, Discover, and Deep dive modes.

---

### 8. Key Trade-offs

1. **Replace topic chips, don't add a row** — Intent chips change algorithm behavior; topic chips don't. "All" mode preserves current experience as fallback.
2. **Session-reset, not permanent preference** — Protects YouTube's Shorts revenue while giving per-session control. Permanent mode = permanent Shorts revenue loss.
3. **Restore old filters + add new ones** — Signals YouTube is listening. Rebuild "Rating" using like-ratio (not deprecated like/dislike system).

> *Rationale: See [Supporting Document — Section 8](#) for all 5 trade-offs with options matrix.*

---

### 9. Edge Cases & Mitigation

| Edge Case | Mitigation |
|-----------|------------|
| Cold start: user has no educational watch history for "Learn" mode | Serve curated popular content + onboarding prompt "What do you want to learn?" |
| "Long-form only" + "Last hour" returns 0 results | Smart empty state: "No long-form in last hour. Try 'Today'?" with one-tap adjust |
| Creators game "Learn" mode with fake educational tags | Use engagement signals (watch-through, satisfaction) not just tags — leverage existing ML |
| AI-generated label false positives | Soft "suspected" label + creator appeal via YouTube Studio |
| "Catch up" mode overwhelming for 500+ subscriptions | Default to "Today" filter + "Priority channels" feature |

> *Rationale: See [Supporting Document — Section 9](#) for all 13 edge cases + 5 broader risks.*

---

### 10. Expected Impact

| Metric | Current (Est.) | Target (90 days) |
|--------|:--------------:|:-----------------:|
| Scroll depth before exit (home) | 2 scrolls | +40% |
| Long-form session duration | Declining | +15% |
| Search-to-watch conversion | Baseline | +10% |
| Shorts watch time | Current | No decline |

---

**Full Analysis** | [GitHub Repository](https://github.com/Jithu224/Youtube_product_improvement) | [Live Prototype](https://jithu224.github.io/Youtube_product_improvement/)

*Jithendra Sarwad — PM Internship Assignment for MioSalon via Airtribe*
