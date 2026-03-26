# Supporting Rationale Document
### YouTube Product Improvement — Decision Log

> This document explains the reasoning behind every decision in the [1-Pager Submission](one_pager_submission.md). Each section maps 1:1 to the 1-pager headings.

---

## Section 1: Goal Selection

**Decision**: YouTube's 2026 North Star = "Maximize engagement across ALL formats while growing creator economy revenue."

**Why this goal**:
- Directly sourced from CEO Neal Mohan's [2026 annual letter](https://blog.youtube/inside-youtube/the-future-of-youtube-2026/) — not our interpretation
- Covers all 4 of YouTube's stated priorities (entertainment, safety, creator economy, AI integrity)
- Creates a measurable thesis: if YouTube says "all formats" but acts "Shorts first," any feature that closes this gap is strategically aligned

**Credibility: 8/10**
- 10/10 for source authority (CEO's own letter)
- 6/10 for specificity (no public engagement targets)
- 7/10 for action alignment (YouTube's actions contradict the stated goal — 80% Shorts in feed)

**What we rejected**:
- "Increase watch time" — too generic, doesn't specify format
- "Grow Shorts" — contradicts the "all formats" framing YouTube itself uses
- "Improve creator monetization" — valid but narrower scope, harder to tie to user-facing features

---

## Section 2: Problem Statement (JTBD Framework)

**Decision**: Frame the problem using Jobs To Be Done — 3 core jobs that YouTube is failing at.

**Why JTBD**:
- JTBD focuses on what the user is TRYING TO ACCOMPLISH, not what they're complaining about
- "Too many Shorts" is a symptom. "I can't find a tutorial" is the unmet job
- Each job maps directly to a feature solution → clean traceability from problem to solution
- JTBD is a recognized PM framework — shows methodology, not just opinion

**The 3 Jobs and why they're broken**:

| Job | JTBD Statement | Why It's Broken | Maps to |
|-----|---------------|-----------------|---------|
| **The Learner** | When I open YouTube to learn a skill, I want to find quality long-form tutorials quickly, so I can build real knowledge | Home feed is 80% Shorts. Educational long-form buried. | F1: Learn mode |
| **The Subscriber** | When I have 15 min to catch up on creators, I want to see their latest uploads front and center, so I can stay connected | Subscription uploads buried under algorithmic Shorts recs. | F1: Catch up mode |
| **The Researcher** | When I search a specific topic, I want to filter by format/quality/recency, so I can find trustworthy content | "Rating" and "Last Hour" filters removed. No "Long-form only" toggle. AI slop pollutes results. | F4: Search filters |

**Why these 3 jobs, not others**:
- They represent YouTube's most valuable user segments (highest session duration, highest ad revenue)
- They are intent-driven — these users come to YouTube with a PURPOSE, not to casually scroll
- Each job has a direct, measurable failure point (80% Shorts in feed, filters removed)
- A 4th job ("The Casual Scroller") was excluded — it's already well-served by the current Shorts-heavy feed

**Evidence backing the gap**:
- Long-form recs: 6/row → 2/row (80% reduction) — [PPC Land](https://ppc.land/youtubes-home-feed-quietly-kills-long-form-video-discovery/)
- Shorts = 75-77% of global views — [Loopex Digital](https://www.loopexdigital.com/blog/youtube-shorts-statistics)
- Trending page killed July 2025
- Shorts rev share 45% vs long-form 55% — creators financially incentivized away from Shorts

---

## Section 3: Pain Point Selection

**Decision**: Selected P1 (Shorts takeover, 9.25/10) and P4 (Search degradation, 8.00/10) from 5 identified pain points.

**Why P1 — Shorts Killing Long-Form Discovery**:
- Highest Impact on Goal (10/10) — directly contradicts "all formats"
- Affects every user, every session (Reach: 9, Frequency: 10)
- Quantifiable: 80% reduction in long-form slots is a hard number
- Sources: Play Store reviews ("feed exhausts in 2 scrolls"), Reddit threads, PPC Land data analysis

**Why P4 — Search Quality Degraded**:
- YouTube officially removed "Rating" and "Last Hour" filters in Jan 2026 — [9to5Google](https://9to5google.com/2026/01/08/youtube-search-filters/)
- Search is 2nd largest traffic source — degraded search = lost sessions
- Specific and fixable — unlike vague complaints, we can name exact filters to restore
- AI slop + Shorts pollution in results is documented and worsening

**Why we excluded P2 — Excessive Ads** (despite 7.75 score):
- Ads are YouTube's primary business model ($40B+/year revenue)
- Suggesting "reduce ads" = telling YouTube to make less money
- Every user complains about ads — it's not an insight, it's obvious
- P2 scores 4/10 on "Impact on Goal" because ads ARE the goal (revenue growth)
- Excluding P2 shows we can distinguish user complaints from product opportunities

**Why we excluded P3 — UI Redesign Backlash** (6/10):
- Cosmetic issue — users historically adapt to redesigns
- YouTube A/B tests extensively; they likely have data supporting changes
- Hard to propose specific, measurable improvements for "make UI better"

**Why we excluded P5 — Watch Later Broken** (4.75/10):
- Affects power users only (<10% of user base)
- Doesn't conflict with any of YouTube's 4 strategic priorities
- Low reach, low frequency

---

## Section 4: User Stories

**Decision**: Defined 3 personas: The Learner, The Subscriber, The Researcher.

**Why these 3**:
- Each maps to a specific pain point AND a specific feature:
  - Learner → P1 → F1 (Learn mode)
  - Subscriber → P1 → F1 (Catch up mode)
  - Researcher → P4 → F4 (Search filters)
- These are YouTube's most valuable user segments (highest session duration, highest ad revenue per session)
- They represent intent-driven users — the segment most alienated by Shorts dominance

**What we rejected**:
- "The Casual Scroller" — already well-served by current Shorts-heavy feed
- "The Creator" — valid persona but our features are viewer-facing, not creator-facing
- "The Parent" — relevant to YouTube's Priority #2 but not our selected pain points

---

## Section 5: Feature Design

**Decision**: F1 (Intent-Based Feed Modes) as primary, F4 (Search Format Filters) as quick win.

**Why F1 — Intent-Based Feed Modes**:
- Solves P1 without killing Shorts (users self-select via "Quick watch")
- Gives users agency over their experience — aligns with YouTube's satisfaction metric shift
- "All" mode = current behavior = zero disruption for users who don't engage
- Precedent: Spotify has mood-based playlists; Netflix has "Watch Something" shuffle — intent-based UX works

**Why F4 — Search Format Filters**:
- Highest confidence (9/10) — YouTube already has filter infrastructure
- Directly restores what users are loudest about (removed "Rating" and "Last Hour")
- Low effort — mostly frontend + API parameter changes
- Quick win that can ship in Week 1-2 while F1 is being built

**What we rejected from the 6 features**:
- F2 (Customizable Feed Ratio slider): Good idea but slider UI is unusual for YouTube. Deferred to v2.
- F3 (Subscriptions First Tab): Partially addressed by "Catch up" mode in F1. Redundant.
- F5 (AI Slop Shield): Requires content classification pipeline investment. Elements included in F4 as quality signals.
- F6 (Search Intent Clustering, RICE: 96): High RICE but low confidence (6/10) — requires NLP investment. Deferred to v2 after F4 validates.

---

## Section 6: RICE Scoring

**Decision**: Used RICE formula with Effort inverted (lower = harder) for clearer differentiation.

**Why this scoring approach**:
- Standard PM framework — recognizable to any reviewer
- Effort inverted because F1 (highest impact) requires significant engineering investment — this naturally deprioritizes effort-heavy features unless their R×I×C is exceptionally high
- F1's RICE (189) is 2.6x higher than the next feature — clear winner, not a close call

**Key scoring justifications**:
- F1 Reach (9): Affects every home feed user — 2.7B monthly users see the feed
- F1 Effort (3): Requires algorithm-side changes to support intent-weighted ranking. "Catch up" mode is simpler (chronological query), but "Learn" and "Discover" need ML classification
- F4 Confidence (9): Highest — YouTube already had these filters, infrastructure exists, just restoring + extending
- F4 Effort (8): Mostly frontend changes + API params. Low engineering lift.

---

## Section 7: Prototype

**Decision**: Built a single-file HTML/CSS/JS interactive prototype with before/after toggle.

**Why this approach**:
- Zero dependencies — opens in any browser, no build tools needed
- Before/after toggle immediately shows the contrast between current YouTube and proposed features
- Responsive — works on mobile and desktop (reviewer can check on phone)
- Interactive mode switching demonstrates how intent chips would actually feel

**What the prototype covers**:
- F1: All 6 intent modes with different content per mode
- F4: Enhanced search filters with restored "Rating"/"Last Hour" highlighted
- Quality signals on search results
- First-time tooltip onboarding

---

## Section 8: Trade-offs

**Decision**: Documented 5 trade-offs. Top 3 in the 1-pager.

**Trade-off 1 — Replace topic chips vs add second row**:
- Chose: Replace. Topic chips are low-signal — selecting "Gaming" still gives 80% Shorts. Intent chips fundamentally change algorithm behavior.
- Risk mitigation: "All" mode = exact current behavior as fallback.

**Trade-off 2 — Session-reset vs permanent preference**:
- Chose: Session-reset. YouTube's ad revenue depends on Shorts impressions. Permanent "Learn" mode = permanent Shorts revenue loss for that user.
- This makes the feature more likely to be internally approved — we're not threatening revenue.
- Future: If >60% re-select daily, introduce "Default mode" in Settings (v2).

**Trade-off 3 — Restore old filters vs new only**:
- Chose: Restore + add new. YouTube's removal reason ("not working as expected") was vague and seen as dismissive. Restoring signals responsiveness.
- Improvement: Rebuild "Rating" using like-ratio (not deprecated like/dislike system).

**Trade-off 4 — Quality signals vs clean UI**:
- Chose: Show signals. Aligns with YouTube's Priority #4 (labeling AI content). "% liked" uses existing public data — just surfacing it.

**Trade-off 5 — P1+P4 over P2 (ads)**:
- Chose: P1+P4. Ads are intentional business decisions. PM judgment = knowing which complaints are product opportunities vs revenue levers.

---

## Section 9: Edge Cases & Risks

**Decision**: Identified 13 specific edge cases + 5 broader risks.

**Most critical edge cases**:

1. **Cold start in Learn mode** — No educational history → algorithm has no signal. Mitigation: curated popular content + onboarding prompt.
2. **0 results for combined filters** — "Long-form + Last hour" on niche query = empty. Mitigation: smart empty state with one-tap filter adjust.
3. **AI label false positives** — Legitimate creators flagged. Mitigation: soft "suspected" label + appeal via YouTube Studio. Hard label only for YouTube's own AI tools.
4. **Contradictory filters** — "Shorts" + "> 1 hour" = impossible. Mitigation: auto-disable contradictory options.
5. **Catch up overload** — 500+ subscriptions = hundreds of videos. Mitigation: default "Today" filter + priority channels.

**Most critical risks**:

1. **YouTube internal politics blocks Shorts visibility reduction** (High likelihood, High impact) — Mitigated: "All" mode = current behavior. We add choice, not remove Shorts.
2. **Users in Learn mode stop watching Shorts entirely** (Medium likelihood, High revenue impact) — Mitigated: monitor per-user Shorts time, show "Quick break?" card after 30 min.
3. **Low adoption (<5%)** (Medium likelihood) — Mitigated: onboarding tooltip, A/B test placement, iterate on labels.

---

## Section 10: Expected Impact

**Decision**: Conservative targets based on industry benchmarks.

**Why these numbers**:
- +40% scroll depth: Current feed exhausts in 2 scrolls for long-form seekers. Intent modes provide infinite relevant content within the selected mode.
- +15% long-form session duration: Users currently leave or switch to Shorts. With "Learn"/"Deep dive" modes, they stay in long-form content.
- +10% search-to-watch conversion: Restored filters + quality signals help users find what they want faster = fewer abandoned searches.
- Shorts watch time flat: "Quick watch" mode preserves current Shorts experience. "All" mode is the default. We're adding choice, not removing Shorts.

---

*This document supports the [1-Pager Submission](one_pager_submission.md). Full analysis: [youtube_painpoints_to_feature.md](youtube_painpoints_to_feature.md)*
