# YouTube Product Improvement — Full Analysis

> **Assignment**: One product you use frequently and what you would improve
> **For**: MioSalon PM Internship (via Airtribe)
> **Product**: YouTube (Mobile App)
> **Date**: March 25, 2026

---

## 1. YouTube's 2026 North Star Goal

### Goal Statement
**"Maximize viewer engagement & satisfaction across ALL formats (Shorts, long-form, live, TV) while growing creator economy revenue."**

> Credibility Rating: **8/10** — Directly sourced from CEO Neal Mohan's 2026 annual letter.

### YouTube's 4 Strategic Priorities (2026)

| # | Priority | Key Details |
| --- | --- | --- |
| 1 | **Reinventing Entertainment** | Creators = new stars & studios. #1 in US streaming watchtime for 3 consecutive years (Nielsen). Expanding Shorts + long-form + live + TV. |
| 2 | **Kids & Teens Safety** | Better parental controls, easier kid account setup, supervised experiences. |
| 3 | **Creator Economy Expansion** | $100B+ paid to creators in last 4 years. Growing shopping, brand partnerships, fan funding. |
| 4 | **AI + Creative Integrity** | 1M+ channels using AI tools daily. Fighting deepfakes, AI slop, misinformation. |

### The Critical Tension (Our Thesis)

YouTube **says** "all formats" but **acts** "Shorts first":
- Home feed long-form recommendations cut by **80%** (from 6/row to 2/row)
- Shorts account for **75-77% of global views**
- Trending page **killed** (July 2025)
- Shorts creators get only **45% rev share** vs 55% for long-form

**This gap between stated goal and actual product behavior is the core opportunity we're addressing.**

Sources:
- [Neal Mohan's 2026 Letter](https://blog.youtube/inside-youtube/the-future-of-youtube-2026/)
- [YouTube Home Feed Kills Long-Form Discovery — PPC Land](https://ppc.land/youtubes-home-feed-quietly-kills-long-form-video-discovery/)
- [YouTube Shorts Statistics 2026 — Loopex Digital](https://www.loopexdigital.com/blog/youtube-shorts-statistics)

---

## 2. Five Pain Points from Play Store Reviews, Trustpilot, Reddit & Tech Press

### P1: Home Feed Overwhelmed by Shorts — Killing Long-Form Discovery
**Credibility: 9/10**

| Evidence | Data |
| --- | --- |
| Long-form recs per row | 6 → 2 (**80% reduction**) |
| Shorts share of global views | 75-77% |
| Trending page | Killed July 2025 |
| Creator revenue impact | Shorts: 45% rev share vs Long-form: 55% |
| Monthly Shorts users | 2 Billion |
| User sentiment | Feed "exhausts in 2 scrolls" — Reddit |

**Why it matters**: Users who come to YouTube for tutorials, documentaries, deep-dives, and creator long-form are being force-fed Shorts. They either leave the app or switch to Shorts — neither outcome serves YouTube's "all formats" goal.

### P2: Excessive / Aggressive Ads
**Credibility: 7/10 — EXCLUDED from final selection**

| Evidence | Data |
| --- | --- |
| Ads per video | 2-3 (2020) → **5-7 (2025)** |
| Ad blocker usage | 27% (2020) → **47% (2025)** |
| Reddit complaints | 50,000+ posts in 2025 (200% YoY increase) |
| Hashtag trend | #YouTubeAdsWorstEver trended 3 weeks (April 2025) |
| Pause ads on TV | Introduced 2025, 68% of TV users annoyed |

**Why EXCLUDED**: Ads are YouTube's primary revenue engine ($40B+/year). Suggesting "reduce ads" tells the company to make less money — shows zero PM judgment. Ads are a **business decision**, not a product bug.

### P3: UI Redesign Backlash — "Squished," Confusing Layout
**Credibility: 6/10 — EXCLUDED from final selection**

| Evidence | Data |
| --- | --- |
| Media reaction | Called "most disgusting layout" by users |
| Changes | Upload dates removed, channel names hidden, bigger buttons |
| Desktop issue | Scrolling during video playback broken |

**Why EXCLUDED**: Cosmetic. Users always hate redesigns initially but adapt. YouTube A/B tests extensively — they likely have internal data supporting these changes. Hard to propose specific, measurable improvements.

### P4: Search Quality Degraded — Filters Removed, Shorts Pollute Results
**Credibility: 8.5/10**

| Evidence | Data |
| --- | --- |
| Filters removed (Jan 2026) | "Upload Date: Last Hour" and "Sort by Rating" officially removed |
| YouTube's reason | "Not working as expected" — no restoration planned |
| New filter | Shorts-only filter added (but no "Long-form only") |
| Sort change | "View count" replaced with "Popularity" (opaque metric) |
| AI slop | Clickbait + AI-generated content flooding search results |
| User reaction | "Swift and negative" — BetaNews |

**Why it matters**: Search is YouTube's **2nd largest traffic source**. Users with intent ("how to fix X", "best Y review") can no longer efficiently find quality content. This directly undermines YouTube's goal of being the world's learning and discovery platform.

Sources:
- [YouTube Updates Search Filters — 9to5Google](https://9to5google.com/2026/01/08/youtube-search-filters/)
- [YouTube New Search Filters — BetaNews](https://betanews.com/2026/01/09/youtube-introduces-new-search-filters-with-the-option-to-avoid-shorts/)

### P5: Watch Later / Queue is Broken
**Credibility: 5/10 — EXCLUDED from final selection**

| Evidence | Data |
| --- | --- |
| Queue persistence | Disappears on browser close |
| Mobile access | Premium-gated |
| Scale issues | Degrades above few hundred items, sync issues |

**Why EXCLUDED**: Affects power users only. Casual majority doesn't use Watch Later heavily. Doesn't directly conflict with any of YouTube's 4 strategic priorities.

---

## 3. Pain Point Prioritization Matrix

### Scoring Criteria (each 1-10)
- **Impact on Goal**: How directly does this pain point undermine YouTube's North Star?
- **Reach**: What % of YouTube's 2.7B users are affected?
- **Frequency**: How often does the user encounter this pain?
- **Severity**: How much does it degrade the experience when encountered?

| Pain Point | Impact on Goal | Reach | Frequency | Severity | **Total (avg)** |
| --- | --- | --- | --- | --- | --- |
| **P1: Shorts killing long-form** | 10 | 9 | 10 | 8 | **9.25** |
| **P4: Search quality degraded** | 8 | 8 | 7 | 9 | **8.00** |
| P2: Excessive ads | 4 | 10 | 10 | 7 | 7.75 |
| P3: UI redesign backlash | 5 | 8 | 10 | 5 | 7.00 |
| P5: Watch Later broken | 4 | 4 | 5 | 6 | 4.75 |

### Final Selection

| Rank | Pain Point | Score | Rationale |
| --- | --- | --- | --- |
| **1** | **P1: Shorts Killing Long-Form Discovery** | **9.25** | Highest impact. Directly contradicts CEO's "all formats" goal. Affects every user every session. |
| **2** | **P4: Search Quality Degraded** | **8.00** | YouTube officially broke this (removed filters Jan 2026). Intent-driven users losing trust. Specific and fixable. |

**Why P2 (Ads) was excluded despite high Reach+Frequency**: A PM who says "reduce ads" is telling a $40B ad business to make less money. P2 scores low on "Impact on Goal" because **ads ARE the goal** (revenue growth). Excluding P2 demonstrates PM judgment — distinguishing between user complaints and product opportunities.

---

## 4. Feature Solutions

### For P1: Shorts Killing Long-Form Discovery

#### F1: Intent-Based Feed Modes
**Description**: Horizontal toggle chips at the top of the Home feed:
`[Learn]` `[Catch up]` `[Discover]` `[Quick watch]` `[Deep dive]`

Each mode adjusts the algorithm's content weighting:
- **Learn**: Prioritizes tutorials, courses, educational long-form (10+ min)
- **Catch up**: Chronological feed from subscriptions only, no algo interference
- **Discover**: Surface new creators and channels outside your watch history
- **Quick watch**: Shorts-heavy feed for snackable content (current default behavior)
- **Deep dive**: Documentaries, podcasts, 30+ min content

**User control without killing Shorts**: Users who want Shorts can choose "Quick watch." Users who want depth can choose "Learn" or "Deep dive." YouTube keeps Shorts revenue while serving all user intents.

#### F2: Customizable Feed Ratio
**Description**: A slider in Settings letting users set their preferred Shorts:Long-form ratio (e.g., 30:70). Persists across sessions.

- Default: YouTube's current mix (~80:20 Shorts-heavy)
- User override: Drag to preferred ratio
- Smart default: Offer "Recommended for you" based on actual watch history distribution

#### F3: Subscriptions First Tab
**Description**: A dedicated tab showing **only** unwatched uploads from subscriptions, in chronological order. No algorithmic ranking, no Shorts injection, no recommendations.

- Shows channel avatar + title + duration + upload time
- Mark as "watched" to dismiss
- Filter by: All | Today | This week | Channel groups

---

### For P4: Search Quality Degraded

#### F4: Search Format Filters (Restore + Enhance)
**Description**: Bring back removed filters + add new ones:

**Restore**:
- "Upload Date: Last Hour" (removed Jan 2026)
- "Sort by Rating" (removed Jan 2026)

**Add new**:
- `[Long-form only]` toggle (Shorts already has a filter — long-form doesn't)
- `[Verified creators only]` — filter out reuploads, AI slop channels
- Duration presets: `<5min` `5-20min` `20-60min` `>1hr`

#### F5: AI Slop Shield
**Description**: Quality signals visible directly in search results:

- **Verified creator badge** (checkmark): Original content creator, not a reupload farm
- **Engagement quality indicator**: View-to-like ratio displayed (e.g., "92% liked")
- **"AI-generated" label**: Transparent labeling for AI-created content (aligns with YouTube's Priority #4)
- **"Community trusted" tag**: Videos with high comment engagement + positive sentiment

#### F6: Search Intent Clustering
**Description**: Group search results by detected user intent:

Search: "iPhone 16"
```
📚 Tutorials
├ Setup Guide (12min) — Channel A
└ Camera Tips (8min) — Channel B

⭐ Reviews
├ MKBHD Review (18min)
└ Unbox Therapy (14min)

📰 News
├ Sales Numbers Q4 (5min)
└ iOS 20 Update (7min)

🎬 Entertainment
├ Drop Test (3min)
└ Unboxing ASMR (10min)
```

Users jump directly to their intent category instead of scrolling through mixed, algorithm-ranked results.

---

## 5. RICE Scoring

### Formula
**RICE = (Reach × Impact × Confidence) / Effort**

| Dimension | Scale | Meaning |
| --- | --- | --- |
| **Reach** | 1-10 | % of YouTube's 2.7B users affected in next quarter |
| **Impact** | 1-10 | How much does this move the North Star metric (engagement + satisfaction)? |
| **Confidence** | 1-10 | How sure are we this will work? (data backing, precedent, clarity) |
| **Effort** | 1-10 | Engineering effort. **Lower = harder** (inverted: 1 = massive effort, 10 = trivial) |

### Scoring Table

| Feature | Reach | Impact | Confidence | Effort | **RICE Score** |
| --- | --- | --- | --- | --- | --- |
| **F1: Intent-Based Feed Modes** | 9 | 9 | 7 | 3 | **189.0** |
| **F6: Search Intent Clustering** | 8 | 8 | 6 | 4 | **96.0** |
| **F4: Search Format Filters** | 8 | 8 | 9 | 8 | **72.0** |
| **F2: Customizable Feed Ratio** | 7 | 7 | 8 | 6 | **65.3** |
| **F5: AI Slop Shield** | 7 | 7 | 5 | 4 | **61.3** |
| **F3: Subscriptions First Tab** | 6 | 6 | 9 | 7 | **46.3** |

### Feature Selection

| Priority | Feature | RICE | Rationale |
| --- | --- | --- | --- |
| **PRIMARY** | **F1: Intent-Based Feed Modes** | **189** | Highest RICE. Transformative. Solves P1 without killing Shorts. Gives users agency. Aligns with YouTube's satisfaction-over-watch-time metric shift. |
| **QUICK WIN** | **F4: Search Format Filters** | **72** | Highest confidence (9/10). Low effort — YouTube already has filter infrastructure. Restores removed functionality users are actively requesting. |
| **STRETCH** | **F6: Search Intent Clustering** | **96** | High RICE but lower confidence. Requires ML/NLP investment. Could be phased after F4. |

---

## 6. Prototype Wireframes

### F1: Intent-Based Feed Modes — Before vs After

**BEFORE (Current YouTube Home Feed)**:
```
┌─────────────────────────────────┐
│  YouTube                    🔔 👤│
│                                 │
│  [All] [Gaming] [Music] [News] │  ← Generic topic chips
│                                 │
│  ┌─────┐ ┌─────┐ ┌────────────┐│
│  │Short│ │Short│ │  Long-form ││
│  │ :15 │ │ :30 │ │  "How to.. ││
│  │     │ │     │ │   12:34    ││
│  └─────┘ └─────┘ └────────────┘│
│  ┌─────┐ ┌─────┐ ┌─────┐      │
│  │Short│ │Short│ │Short│       │  ← 80% Shorts
│  │ :22 │ │ :45 │ │ :18 │      │
│  └─────┘ └─────┘ └─────┘      │
│  ┌────────────────────────┐    │
│  │  Long-form (only 1)    │    │  ← Rare long-form
│  │  "React Tutorial" 45:00│    │
│  └────────────────────────┘    │
│  ┌─────┐ ┌─────┐ ┌─────┐      │
│  │Short│ │Short│ │Short│       │
│  └─────┘ └─────┘ └─────┘      │
│                                 │
│  ⚠️ Feed exhausted after 2     │
│     scrolls for long-form      │
│     seekers                     │
│                                 │
│  🏠    🔍    ➕    📺    👤    │
└─────────────────────────────────┘
```

**AFTER (With Intent-Based Feed Modes)**:
```
┌─────────────────────────────────┐
│  YouTube                    🔔 👤│
│                                 │
│  [Learn✓] [Catch up] [Discover]│  ← Intent chips
│  [Quick watch] [Deep dive]     │     (replaces topic chips)
│                                 │
│  ── "Learn" mode active ──     │
│                                 │
│  ┌────────────────────────┐    │
│  │ 📚 Python Full Course  │    │
│  │ freeCodeCamp · 4.2M    │    │
│  │ ⏱ 4:26:00 · Tutorial   │    │
│  └────────────────────────┘    │
│  ┌────────────────────────┐    │
│  │ 📚 System Design Guide │    │
│  │ ByteByteGo · 890K      │    │
│  │ ⏱ 28:15 · Deep dive    │    │
│  └────────────────────────┘    │
│  ┌────────────────────────┐    │
│  │ 📚 Excel for Beginners │    │
│  │ Leila Gharani · 2.1M   │    │
│  │ ⏱ 1:12:00 · Course     │    │
│  └────────────────────────┘    │
│  ┌────────────────────────┐    │
│  │ 📚 How Git Works       │    │
│  │ Fireship · 1.5M        │    │
│  │ ⏱ 12:34 · Explainer    │    │
│  └────────────────────────┘    │
│                                 │
│  ✅ Endless relevant long-form │
│     content for learners       │
│                                 │
│  🏠    🔍    ➕    📺    👤    │
└─────────────────────────────────┘
```

### F4: Search Format Filters — Before vs After

**BEFORE (Current YouTube Search)**:
```
┌─────────────────────────────────┐
│  🔍 how to learn python        │
│                                 │
│  Filters: [Shorts] [This year] │  ← No "Long-form" filter
│  [Creative Commons] [4K]       │    "Last Hour" REMOVED
│  Sort: Relevance | Popularity  │    "Rating" REMOVED
│                                 │
│  ┌─────┐                       │
│  │Short│ Python in 60 secs     │  ← Shorts pollute
│  │ :58 │ AI-generated channel  │     search results
│  └─────┘                       │
│  ┌─────┐                       │
│  │Short│ Python trick #47      │
│  │ :30 │                       │
│  └─────┘                       │
│  ┌────────────────────────┐    │
│  │ CLICKBAIT THUMB 🔥🔥   │    │
│  │ "I learned Python in   │    │  ← AI slop, no
│  │  1 day" · 2:34         │    │     quality signals
│  └────────────────────────┘    │
│  ┌─────┐                       │
│  │Short│ Another Short...      │
│  └─────┘                       │
└─────────────────────────────────┘
```

**AFTER (With Enhanced Search Filters)**:
```
┌─────────────────────────────────┐
│  🔍 how to learn python        │
│                                 │
│  Format: [All] [Long-form✓]   │  ← NEW: Long-form filter
│          [Shorts] [Channels]   │
│                                 │
│  Duration: [<5m] [5-20m✓]     │  ← NEW: Duration presets
│            [20-60m] [>1hr]     │
│                                 │
│  Sort: Relevance | Rating |    │  ← RESTORED: Rating
│        Upload date ▾           │    RESTORED: Last Hour
│        [Last hour] [Today]     │
│        [This week] [This year] │
│                                 │
│  ┌────────────────────────┐    │
│  │ ✅ Python for Beginners│    │
│  │ Corey Schafer · 12:34  │    │  ← Verified badge
│  │ ⭐ 96% liked · 2.1M   │    │  ← Quality signal
│  └────────────────────────┘    │
│  ┌────────────────────────┐    │
│  │ ✅ Python Tutorial 2026│    │
│  │ Tech With Tim · 18:45  │    │
│  │ ⭐ 94% liked · 800K   │    │
│  └────────────────────────┘    │
│  ┌────────────────────────┐    │
│  │ ✅ Learn Python Free   │    │
│  │ freeCodeCamp · 15:20   │    │
│  │ ⭐ 98% liked · 5.2M   │    │
│  └────────────────────────┘    │
│                                 │
│  ✅ Clean, relevant, quality   │
│     results for intent-driven  │
│     users                      │
└─────────────────────────────────┘
```

---

## 7. Trade-offs We Made (and Why)

### Trade-off 1: Replacing Topic Chips vs Adding a Second Row

| Option | Pros | Cons |
| --- | --- | --- |
| **A: Replace topic chips with intent chips (chosen)** | Clean UI, no added clutter, forces a clear mental model shift | Loses quick access to topic filters (Gaming, Music, News) |
| B: Add intent chips as a second row above topic chips | Preserves existing behavior | Adds vertical space, cognitive overload, users may ignore second row |

**Why we chose A**: YouTube's current topic chips are low-signal — they filter by content category but don't change the algorithm's behavior. Users still get Shorts-heavy feeds even when selecting "Gaming." Intent chips fundamentally change WHAT the algorithm serves, making topic chips redundant within each mode.

**Risk mitigation**: The "All" mode preserves the exact current experience including topic chips as a fallback during A/B testing.

### Trade-off 2: Session-Persistent Modes vs Permanent User Preference

| Option | Pros | Cons |
| --- | --- | --- |
| **A: Mode resets to "All" on app restart (chosen)** | Low commitment, encourages exploration, preserves YouTube's default behavior for most sessions | Power users must re-select their preferred mode each time |
| B: Mode persists permanently until changed | Reduces friction for repeat users | Users may forget they're in a mode, reducing content diversity. YouTube loses Shorts impressions permanently for users who set "Learn" once. |

**Why we chose A**: YouTube's ad revenue depends on Shorts impressions. Making "Learn" mode permanent would permanently reduce Shorts exposure for that user. Session-reset is a compromise — users get control per session without permanently opting out of YouTube's revenue model. This makes the feature more likely to be approved internally.

**Future iteration**: If data shows >60% of users re-select the same mode daily, introduce "Default mode" in Settings as a v2 feature.

### Trade-off 3: Restoring Removed Filters vs Building New Ones Only

| Option | Pros | Cons |
| --- | --- | --- |
| **A: Restore "Rating" and "Last Hour" + add new filters (chosen)** | Addresses the loudest user complaint directly, quick win, signals YouTube is listening | YouTube removed these for a reason ("not working as expected") — may resurface old bugs |
| B: Only add new filters (Long-form, Duration presets) | Avoids old bugs, forward-looking | Ignores the specific user pain point — feels tone-deaf |

**Why we chose A**: YouTube's stated reason for removal ("not working as expected") is vague and widely seen as dismissive. Restoring these filters — even in improved form — signals responsiveness to users. The "Rating" sort can be improved by using like-ratio instead of the old like/dislike system.

### Trade-off 4: Quality Signals on Search Results vs Clean Minimal UI

| Option | Pros | Cons |
| --- | --- | --- |
| **A: Show quality signals (% liked, verified, AI label) on results (chosen)** | Helps users make faster, better decisions. Fights AI slop passively. | Adds visual noise. YouTube may resist surfacing "AI-generated" label (discourages AI tool adoption). |
| B: Keep search results clean, let algorithm rank quality higher | Cleaner UI, less cognitive load | Users can't distinguish quality themselves — algorithm opacity continues |

**Why we chose A**: YouTube's own 2026 Priority #4 is "Supercharging and Safeguarding Creativity" — which explicitly includes labeling AI-generated content. Our quality signals ALIGN with YouTube's stated direction. The "% liked" metric is already available (like count is public) — we're just surfacing existing data.

### Trade-off 5: Picking P1 + P4 over P2 (Ads)

| Option | Pros | Cons |
| --- | --- | --- |
| **A: P1 (Shorts takeover) + P4 (Search degradation) — chosen** | Shows PM judgment, addresses structural product issues, specific and fixable | Ignores the #1 user complaint (ads) |
| B: P2 (Ads) + P1 (Shorts takeover) | Addresses the most complained-about issue | "Reduce ads" = telling YouTube to cut $40B revenue. Shows no PM sophistication. |

**Why we chose A**: The assignment is for a PM internship — we're being evaluated on product thinking, not user advocacy. Any user can say "too many ads." A PM identifies which user complaints represent **actual product opportunities** vs **intentional business decisions**. Ads are the latter.

---

## 8. Edge Cases & Risks

### Edge Cases for F1 (Intent-Based Feed Modes)

| # | Edge Case | Impact | Mitigation |
| --- | --- | --- | --- |
| 1 | **User selects "Learn" but has no educational watch history** | Algorithm has no signal to personalize — cold start problem | Serve curated "most popular educational" content by category (coding, cooking, finance). Show an onboarding prompt: "What do you want to learn?" |
| 2 | **Creator uploads content that spans multiple intents** (e.g., an entertaining tutorial) | Content may not appear in the mode the user expects | Allow content to appear in multiple modes with different ranking weights. A fun coding tutorial ranks in both "Learn" and "All." |
| 3 | **"Catch up" mode for users subscribed to 500+ channels** | Feed becomes overwhelming — hundreds of unwatched videos | Default to "Today" filter. Show channel group folders. Add "Priority channels" (user marks top 10-20 channels as priority). |
| 4 | **"Quick watch" mode cannibalizes Shorts tab** | Two entry points for Shorts creates redundancy | "Quick watch" differentiates by mixing trending Shorts + clips from long-form. Shorts tab remains pure Shorts. |
| 5 | **Metric gaming: creators tag content as "educational" to appear in Learn mode** | Low-quality content floods Learn mode | Use engagement signals (watch-through rate, satisfaction surveys) not just tags. YouTube already has content classification ML — leverage it. |
| 6 | **Mode switching on slow network** | Feed refresh feels broken — blank screen | Show skeleton loaders immediately. Pre-cache the first 3 videos for adjacent modes in the background. |
| 7 | **Accessibility: screen reader users navigating chips** | Horizontal chip scroll may not announce mode changes properly | Use proper ARIA roles: `role="tablist"` for chips, `role="tab"` for each chip, `aria-selected` for active state. Announce mode change: "Switched to Learn mode." |

### Edge Cases for F4 (Enhanced Search Filters)

| # | Edge Case | Impact | Mitigation |
| --- | --- | --- | --- |
| 1 | **"Long-form only" + "Last hour" returns 0 results for niche queries** | Empty state frustrates users | Show: "No long-form results in the last hour. Try 'Today' or 'All formats'?" with one-tap filter adjustment. |
| 2 | **"Sort by Rating" abused by creators using engagement bait** (e.g., "like this video if you breathe") | Artificially inflated ratings skew sort | Use weighted rating: factor in like ratio, watch-through rate, AND comment sentiment — not just raw like count. |
| 3 | **AI-generated label on results — false positives** | Legitimate creators flagged as AI → reputation damage | Use "Suspected AI-generated" with soft confidence signal. Allow creators to appeal via YouTube Studio. Only show hard "AI-generated" label for content created with YouTube's own AI tools (where labeling is automatic). |
| 4 | **Multiple filters combined produce contradictory results** (e.g., "Shorts" + "> 1 hour") | Impossible filter combination | Disable contradictory filters automatically. When "Shorts" is selected, hide duration presets. |
| 5 | **Verified creator badge creates a two-tier system** | Small creators feel penalized — verified gets more clicks | Badge indicates "original creator" not "quality." Show verification criteria transparently. Don't use verification in ranking — only as a visual signal. |
| 6 | **Filter state in URL shared to someone who expects default YouTube** | Shared URL opens with unexpected filters active | Show a subtle banner: "Viewing with filters: Long-form, 5-20min, Rating sort. [Clear all]" |

### Broader Risks

| Risk | Likelihood | Impact | Mitigation |
| --- | --- | --- | --- |
| **YouTube refuses to reduce Shorts visibility (internal politics)** | High | High | "All" mode = current behavior. We're not REMOVING Shorts — we're adding choice. Shorts revenue is protected via "Quick watch" mode. |
| **Feature adoption is low (<5%)** | Medium | Medium | Onboarding tooltip, A/B test placement, track intent chip engagement. If low, iterate on chip labels and positioning. |
| **Mode fragmentation reduces recommendation quality** | Medium | Medium | Each mode still uses collaborative filtering within its content pool. "Learn" mode has 2B+ educational videos — plenty of signal. |
| **Restored filters reintroduce old bugs YouTube removed them for** | Low | Medium | Rebuild "Rating" sort using like-ratio (not the old like/dislike system that was deprecated). Test "Last Hour" filter with proper time-zone handling. |
| **Cannibalization: users in "Learn" mode stop watching Shorts entirely** | Medium | High (revenue) | Monitor per-user Shorts watch time before/after. If significant decline, show a "Quick break?" Shorts card after 30 min in Learn mode. |

---

## Summary

| Step | Output |
| --- | --- |
| **Goal** | Maximize engagement across ALL formats + creator economy growth (8/10 credibility) |
| **Pain Points** | 5 identified → 2 selected: P1 (Shorts takeover, 9/10) + P4 (Search degradation, 8.5/10) |
| **Features** | 6 proposed → 2 winners: F1 (Intent Feed Modes, RICE 189) + F4 (Search Filters, RICE 72) |
| **Thesis** | YouTube's goal says "all formats" but the product says "Shorts first." Our features close this gap by giving users control over their content intent. |

---

---

## 10. Portfolio

### Project Links

| Asset | Link | Description |
| --- | --- | --- |
| **Live Prototype** | [jithu224.github.io/Youtube_product_improvement](https://jithu224.github.io/Youtube_product_improvement/) | Interactive before/after prototype with intent feed modes and enhanced search filters. Mobile + desktop responsive. |
| **GitHub Repository** | [github.com/Jithu224/Youtube_product_improvement](https://github.com/Jithu224/Youtube_product_improvement) | Full source code, analysis, and PRD |
| **This Analysis** | `youtube_painpoints_to_feature.md` | Pain points, prioritization, RICE scoring, trade-offs, edge cases |
| **PRD** | `PRD_intent_feed_modes.md` | Product Requirements Document with specs, personas, rollout plan |

### What This Project Demonstrates

| PM Skill | How It's Demonstrated |
| --- | --- |
| **Strategic Thinking** | Identified gap between YouTube's stated 2026 goal ("all formats") and actual product behavior (Shorts-first). Framed features as closing this gap. |
| **User Research** | Analyzed Play Store reviews, Trustpilot, Reddit, and tech press to source 5 pain points with quantified evidence. |
| **Prioritization** | Used a scoring matrix (Impact, Reach, Frequency, Severity) to select top 2 pain points. Deliberately excluded the #1 user complaint (ads) — demonstrating business judgment. |
| **Feature Design** | Proposed 6 features, RICE-scored them, selected 3 winners with clear rationale. |
| **Trade-off Analysis** | Documented 5 explicit trade-offs with options considered, decision made, and reasoning. |
| **Edge Case Thinking** | Identified 13 edge cases across both features with specific mitigations. |
| **Risk Assessment** | Mapped 5 broader risks with likelihood, impact, and mitigation strategies. |
| **Prototyping** | Built a working interactive prototype (HTML/CSS/JS) with before/after comparison, responsive design, and mode switching. |
| **Communication** | Structured the entire analysis as a clear narrative: Goal → Pain Points → Prioritization → Features → Scoring → Trade-offs → Edge Cases → Prototype. |

### About

**Jithendra Sarwad**
- PM Internship Assignment for MioSalon (via Airtribe)
- Product analyzed: YouTube Mobile App
- Date: March 25, 2026

*Next step: Condense this into a 1-page Google Doc submission for MioSalon via Airtribe.*
