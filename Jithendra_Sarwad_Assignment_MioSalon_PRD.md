# Product Requirements Document (PRD)
## YouTube Intent-Based Feed Modes + Enhanced Search Filters

---

### 1. Overview


| Field | Detail |
| --- | --- |
| **Product** | YouTube Mobile & Desktop App |
| **Features** | F1: Intent-Based Feed Modes, F4: Enhanced Search Format Filters |
| **Author** | Jithendra Sarwad |
| **Date** | March 25, 2026 |
| **Status** | Proposal |

### 2. Problem Statement

YouTube's home feed has become Shorts-dominated (80% of slots), alienating users who come for long-form content — tutorials, documentaries, reviews, deep-dives. Simultaneously, YouTube's search quality has degraded after removing key filters (Upload Date: Last Hour, Sort by Rating) in January 2026, with Shorts and AI slop polluting results.

**These problems directly contradict YouTube's 2026 stated goal**: "Reinventing entertainment across ALL formats."

### 3. Goals & Success Metrics

| Goal | Metric | Target |
| --- | --- | --- |
| Increase long-form engagement | Avg. session duration for non-Shorts content | +15% in 90 days |
| Reduce feed fatigue | Scroll depth before exit (home feed) | +40% more scroll depth |
| Improve search satisfaction | Search-to-watch conversion rate | +10% |
| Retain intent-driven users | DAU retention for users who use Learn/Deep dive modes | +8% vs control |
| Maintain Shorts revenue | Shorts watch time (global) | No decline (held flat) |

### 4. User Personas

| Persona | Description | Current Pain | Desired Outcome |
| --- | --- | --- | --- |
| **The Learner** | Uses YouTube to learn skills (coding, cooking, music). 25-35 age. | Drowns in Shorts when searching for tutorials. Feed doesn't match intent. | Dedicated learning feed with long-form educational content. |
| **The Subscriber** | Follows 50+ channels, wants to stay updated. | Subscribed creators buried under algorithmic Shorts recommendations. | Chronological feed of unwatched subscription uploads. |
| **The Explorer** | Casual browser, open to new content. | Feed is repetitive — same type of Shorts, no variety. | Discover new creators and formats outside their bubble. |
| **The Quick Scroller** | Wants snackable content during breaks. | Current default feed already serves this (Shorts-heavy). | No change needed — "Quick watch" mode = current experience. |
| **The Researcher** | Searches with specific intent ("best laptop 2026 review"). | Results polluted with Shorts, AI slop, clickbait. Filters removed. | Clean, filterable search with quality signals and format controls. |

### 5. Feature Requirements

---

#### Feature F1: Intent-Based Feed Modes

**Priority**: P0 (Primary feature)
**RICE Score**: 189

##### 5.1.1 Description
Replace the current generic topic chips (Gaming, Music, News, etc.) at the top of the home feed with **intent-based mode chips** that fundamentally change what content the algorithm serves.

##### 5.1.2 Feed Modes

| Mode | Icon | Algorithm Behavior | Content Mix |
| --- | --- | --- | --- |
| **All** | `🏠` | Current default behavior (status quo) | 80% Shorts, 20% long-form (unchanged) |
| **Learn** | `📚` | Weight toward educational, tutorial, how-to content | 90% long-form (10+ min), 10% short explainers |
| **Catch up** | `🔔` | Chronological subscription uploads only | 100% subscriptions, no algo ranking |
| **Discover** | `🧭` | Surface channels user has never watched, diverse topics | 70% new creators, 30% adjacent topics |
| **Quick watch** | `⚡` | Shorts-first feed | 90% Shorts, 10% trending clips |
| **Deep dive** | `🎯` | Documentaries, podcasts, long-form interviews (30+ min) | 100% long-form (30+ min) |

##### 5.1.3 UI Specifications

**Mobile**:
- Chips displayed in a horizontally scrollable row below the top nav bar
- "All" is the default selected chip (preserves current behavior)
- Active chip: filled background with white text
- Inactive chips: outlined/ghost style
- Sticky on scroll (remains visible as user scrolls feed)
- Chip order: All → Learn → Catch up → Discover → Quick watch → Deep dive

**Desktop**:
- Chips displayed in a horizontal row below the top nav bar, left-aligned
- Same behavior as mobile
- Wider chips with icon + label visible (mobile may abbreviate)

##### 5.1.4 Behavior Rules

1. **Default**: "All" mode = current YouTube experience (no disruption)
2. **Persistence**: Selected mode persists for the session. Resets to "All" on app restart.
3. **Mode switching**: Instant feed refresh on chip tap. Show skeleton loader during content fetch.
4. **First-time education**: Tooltip on first visit: "Choose how you want to browse today"
5. **Analytics**: Track mode selection frequency, session duration per mode, content engagement per mode
6. **A/B test**: Roll out to 10% of users first, measure engagement + satisfaction scores

##### 5.1.5 Content Cards per Mode

**Learn mode cards show**:
- Thumbnail with duration badge
- Title (max 2 lines)
- Channel name + verified badge
- View count + upload date
- **NEW**: Difficulty tag (Beginner / Intermediate / Advanced) — derived from video metadata
- **NEW**: Series indicator ("Part 3 of 8") if part of a playlist

**Catch up mode cards show**:
- Channel avatar (prominent, left-aligned)
- Thumbnail
- Title
- Upload time ("2 hours ago")
- **NEW**: "Mark as watched" swipe action

---

#### Feature F4: Enhanced Search Format Filters

**Priority**: P1 (Quick win)
**RICE Score**: 72

##### 5.2.1 Description
Restore removed search filters and add new format/quality controls to give users precise control over search results.

##### 5.2.2 Filter Groups

**Format Filters** (horizontal chips, single-select):
| Filter | Behavior |
| --- | --- |
| `All` | Default — shows everything |
| `Long-form` | Videos > 4 minutes only. No Shorts. |
| `Shorts` | Shorts only (already exists) |
| `Live` | Live streams and premiered content |
| `Channels` | Channel results only |

**Duration Presets** (horizontal chips, single-select, visible when Long-form selected):
| Filter | Range |
| --- | --- |
| `< 5 min` | 0-5 minutes |
| `5-20 min` | 5-20 minutes |
| `20-60 min` | 20-60 minutes |
| `> 1 hour` | 60+ minutes |

**Sort Options** (dropdown):
| Option | Status |
| --- | --- |
| Relevance | Existing |
| Upload date | Existing |
| View count | Existing (renamed from "Popularity") |
| **Rating** | **RESTORED** (removed Jan 2026) |

**Upload Date Sub-filters** (dropdown):
| Option | Status |
| --- | --- |
| **Last hour** | **RESTORED** (removed Jan 2026) |
| Today | Existing |
| This week | Existing |
| This month | Existing |
| This year | Existing |

**Quality Signals** (visible on each result card):
| Signal | Display |
| --- | --- |
| Verified creator | ✅ checkmark next to channel name |
| Like ratio | "94% liked" badge |
| AI-generated label | "🤖 AI-generated" tag (if applicable) |

##### 5.2.3 UI Specifications

**Mobile**:
- Format filters: horizontal scrollable chips below search bar
- Duration presets: appear as second row when "Long-form" is selected
- Sort/Upload date: accessible via "Filters" icon (funnel icon) → bottom sheet
- Quality signals: inline on result cards

**Desktop**:
- Format filters: horizontal chips below search bar
- Duration presets: inline second row
- Sort/Upload date: dropdown menus, inline
- Quality signals: inline on result cards

##### 5.2.4 Behavior Rules

1. **Default**: "All" format, "Relevance" sort (current behavior preserved)
2. **Filter persistence**: Filters reset per search session (don't carry between searches)
3. **Filter count badge**: Show active filter count on funnel icon (e.g., "2 filters active")
4. **Empty state**: If no results match filters, show "No results. Try adjusting your filters." with a "Clear all filters" button
5. **URL params**: Filters reflected in URL for shareability (`?format=longform&duration=20-60&sort=rating`)

---

### 6. Technical Considerations

| Area | Details |
| --- | --- |
| **Feed Modes (F1)** | Requires algorithm-side changes to support intent-weighted content ranking. Can leverage existing topic classification ML models. "Catch up" mode is simplest — just chronological subscription query. |
| **Search Filters (F4)** | Mostly frontend + API parameter changes. Filter infrastructure already exists. "Rating" sort was previously available — backend support likely still present. |
| **Performance** | Mode switching should feel instant (<500ms). Pre-fetch top 5 results for adjacent modes. |
| **Backward compatibility** | "All" mode = exact current behavior. Zero disruption for users who don't interact with new chips. |

### 7. Rollout Plan

| Phase | Timeline | Scope |
| --- | --- | --- |
| **Phase 1** | Week 1-2 | F4 (Search Filters) — frontend changes only, restore removed filters |
| **Phase 2** | Week 3-4 | F1 "Catch up" mode only — simplest (chronological subs, no ML) |
| **Phase 3** | Week 5-8 | F1 "Learn" and "Deep dive" modes — requires content classification |
| **Phase 4** | Week 9-12 | F1 "Discover" mode — requires new recommendation pipeline |
| **A/B Testing** | Throughout | 10% → 25% → 50% → 100% rollout per phase |

### 8. Out of Scope (v1)

- F2 (Customizable Feed Ratio slider) — deferred to v2
- F3 (Subscriptions First Tab) — partially addressed by "Catch up" mode
- F5 (AI Slop Shield) — deferred to v2, requires content classification pipeline
- F6 (Search Intent Clustering) — deferred to v2, requires NLP investment
- Personalized mode recommendations ("Based on your history, try Learn mode")
- Mode-specific notifications

### 9. Wireframe Reference

See working prototype: `prototype/index.html`
- Mobile view: < 768px
- Desktop view: >= 768px
- Interactive mode switching + search filter toggling
