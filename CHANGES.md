# atdao.org — Upgrade Changes

**File:** `index.html`  
**Source:** Upgraded from current atdao.org (fetched April 2026)  
**Target:** `/Users/avielcarlos/.openclaw/workspace/web/atdao-upgrade/index.html`

---

## Summary

A major content and feature upgrade that preserves the entire existing design system (colors, fonts, tokens, dark theme, animations, component patterns) while adding significant new sections and updating existing content to reflect the current state of the build.

---

## Changes by Category

### 1. Navigation

**Before:** `Vision | Domains | How It Works | Governance | Membership | For AI | Directive | Docs`  
**After:** `Domains | Ora | Roadmap | How It Works | Contribute | Governance | Directive | Community ↗ (Telegram)`

- Added "Ora" nav link → `#connectome`
- Added "Contribute" nav link → `#contributions`
- Renamed "Vision" → "Roadmap" (clearer naming)
- Added "Community ↗" link directly to `t.me/ascensioncommunity` with distinct purple color
- Removed "Membership" as separate nav item (merged into "Contribute")
- Added community Telegram links to mobile nav (Community + AI Channel)
- Removed "For AI" from desktop nav (still in mobile nav via ai-builders section)

---

### 2. Hero (Updated)

- Primary CTA changed from "Join the DAO" → **"Join & Contribute"** (links to `#contributions`)
- Added **Telegram community CTA button** with Telegram icon (purple "Join Community" button)
- Kept "Read the Directive" secondary CTA
- Hero background gradient updated: replaced Eviva purple glow with Connectome purple (`rgba(168, 85, 247, 0.06)`)

---

### 3. Live Metrics Bar (NEW — below hero)

Added a persistent "Building in Public" stats bar immediately below the hero section:

| Metric | Value |
|--------|-------|
| Status | Building in Public (animated pulse dot) |
| Ora Agents Active | 10+ |
| Contributions Tracked | Live |
| Build Status | Phase 1 — Aventi Shipping |
| Community | t.me/ascensioncommunity |
| Founding Steward Spots | 10 Available (gold color) |

Styled with live pulse animations and edge fade-out gradients.

---

### 4. Domain Cards (Updated)

Added **live status badges** to each domain card:
- **Aventi** → `🟢 Live & Shipping` badge (animated green pulse)
- **iVive** → `🟡 Roadmap: Year 1–2` badge
- **Eviva** → `◯ Roadmap: Year 2–5+` badge

Updated feature list for Aventi to mention **Ora** ("Ora generates personalized experience feeds") and added "$3.14 CAD proven acquisition cost" bullet.

Updated iVive to mention **CoachingAgent integration**.

Updated REST description: added "Ora knows when you need to stop and helps you do it right."

Updated domains subtitle to reference Ora as the powering layer.

---

### 5. Connectome & Ora Section (NEW — major addition)

New full section between Domains and Roadmap (`id="connectome"`):

**Ora Hero Panel:**
- Animated brain visual with pulsing core labeled "Ora"
- 3 concentric animated rings
- 11 orbiting agent dots (interactive hover tooltips)
- Stats: 11 agents, 3 domains, ∞ screen variants
- "Live & Building" status indicator
- New color tokens: `--color-connectome: #A855F7` (purple), `--color-ora: #F59E0B` (amber/gold)

**Agent Network Grid (11 agents):**
1. DiscoveryAgent — finds and aggregates opportunities
2. CoachingAgent — personal evolution guidance
3. EnlightenmentAgent — consciousness expansion, mindfulness
4. UIGeneratorAgent — generates JSON screen specs
5. WorldAgent — maps global opportunities and local context
6. CollectiveIntelligenceAgent — synthesizes community patterns
7. ExploreAgent — serendipitous discoveries outside comfort zone
8. FeatureLabAgent — generates and A/B tests new features
9. FeedbackAnalystAgent — processes user signal and engagement data
10. RecommendationAgent — cross-domain personalized suggestions
11. DaoAgent — reads proposals, analyzes votes

**Server-Driven UI Panel:**
- Explains the JSON screen spec system
- 4-step flow: Ora analyses → UIGeneratorAgent outputs spec → Expo renders → User gets unique experience
- No App Store updates required

**Tech Stack Panel:**
- FastAPI (Backend)
- PostgreSQL (Database)
- pgvector (AI/Semantic search)
- Redis (Cache/Queues)
- Expo React Native (Mobile renderer)

**GitHub CTA:**
- Link to `https://github.com/AvielCarlos/ascension-site`
- "Join the Build" Telegram button

---

### 6. Roadmap / Vision (Updated)

**Typo fixed:** "Conncecome" → "Connectome" (appears in Phase 3 title and throughout)

**Phase 1 badge updated:** "Current Focus" → **"Live & Shipping"** (with animated green pulse dot)
- Description updated to reflect Connectome backend is running
- "AI Builds" section renamed to "Ora Builds"
- Updated to reference specific agents: UIGeneratorAgent, DiscoveryAgent, FeatureLabAgent, RecommendationAgent

**Phase 2 badge:** Updated to amber/building color style
- Updated to reference Ora's CoachingAgent and EnlightenmentAgent
- Mentions server-driven UI micro-apps

**Phase 3:** 
- Title fixed: "Connectome Systemic Directive" (was "Conncecome")
- Added "Connectome Full Deployment" highlight tag
- Updated to reference CollectiveIntelligenceAgent

---

### 7. How It Works (Updated)

Flow steps updated to reference Ora specifically:
- Step 1: "AI Agents Propose" → **"Ora Proposes"**
- Step 2: "A/B Variants Created" → **"FeatureLab Creates Variants"**
- Step 5: "Cycle Repeats" → **"Ora Learns"** (FeedbackAnalystAgent)

Vote type descriptions updated to reference Ora.

---

### 8. Contributions & Rewards Section (NEW — replaces/augments Membership)

Entirely new section (`id="contributions"`) replacing the simple 4-tier membership cards:

**Contribution Points (CP) — LTV Model:**
- 5 contribution types tracked: Code, Design, Research, Community, Ora Interactions
- Explained as a "living value" model — monthly re-evaluation by Ora

**Longevity Multiplier (animated bars):**
- 1.0× base
- 1.1× at 3 months
- 1.25× at 6 months
- 1.5× at 1 year+
- Animated bars that trigger on scroll into view

**5 Contribution Tiers (new design with tier cards):**
- 🔘 Observer — 0 CP
- 🔵 Contributor — 100+ CP
- 🟣 Builder — 500+ CP (can submit proposals)
- 🟡 Steward — 3,000+ CP
- ⚡ Founding Steward — First 10 to reach Steward (special gold styling)

**Founding Steward Spotlight:**
- Full callout panel with amber/gold styling
- 6 perks detailed: Founding Governance, Permanent Recognition, Ora Early Access, Multisig Authority, Ascension Direction, LTV Multiplier Lock
- Counter: "10 spots available — first come, first earned"

**Onboarding steps updated:**
- Step 1: Join Telegram community
- Step 2: Fork repo on GitHub
- Step 3: Make first contribution
- Step 4: Receive Contributor NFT
- Step 5: Watch CP grow monthly

---

### 9. Governance (Updated)

- Machine-Readable stack item description updated to reference "Ora's DaoAgent"
- Governance table: "Weighted voting by contribution" → "Weighted voting by CP tier"
- Emergency multisig: "Elected stewards" → "Founding Stewards"

---

### 10. For AI Builders (Updated)

- Section subtitle updated to reference Ora
- Added 7th "AI Can" item: "Measure contribution impact to inform CP allocation"
- Added 5th "AI Cannot" item: "Award or deduct CP from members"
- Structured JSON Proposals description updated to mention "Ora's DaoAgent"

---

### 11. Directive (Updated)

- Typo fixed: "Conncecome" → "Connectome" in section title
- Directive note updated: added "Every agent in Ora serves this unified vision. Every contribution to the DAO moves the mission forward."

---

### 12. Community Section (NEW)

New section (`id="community"`) before the docs section, with 3 link cards:

1. **Telegram Community** → `https://t.me/ascensioncommunity`
2. **Ascension AI Channel** → `https://t.me/ascensionai`  
3. **Get Involved (landing)** → `https://avielcarlos.github.io/ascension-site`

Each card has icon, title, description, and URL display.

---

### 13. Source Documents (Updated)

- Added **Connectome / Ascension GitHub** link card → `https://github.com/AvielCarlos/ascension-site` (styled in purple/connectome color)

---

### 14. Footer (Updated)

- GitHub link updated to real URL: `https://github.com/AvielCarlos/ascension-site`
- Added "powered by Ora" to domain list
- Added **footer community row** with Telegram Community, AI Channel, and Get Involved links
- Footer meta attribution updated: "Built with Ora — AI-Driven, Human-Governed." (removed Perplexity Computer attribution)

---

### 15. New Design Tokens

Added to `:root`:
```css
--color-connectome: #A855F7;
--color-connectome-glow: rgba(168, 85, 247, 0.15);
--color-connectome-glow-strong: rgba(168, 85, 247, 0.25);
--color-ora: #F59E0B;
--color-ora-glow: rgba(245, 158, 11, 0.15);
--color-ora-glow-strong: rgba(245, 158, 11, 0.25);
```

### 16. New CSS Components

- `.metrics-bar` — building-in-public stats bar
- `.metric-item` — individual stat with pulse animation
- `.connectome` — Connectome section wrapper
- `.ora-hero` — Ora hero panel with brain visual
- `.ora-brain` — animated brain with rings and orbiting agent dots
- `.ora-agent-dot` — individual agent dot (interactive)
- `.agents-grid` — 6-column responsive agent card grid
- `.agent-card` — individual agent card with hover effect
- `.sdui-panel` — server-driven UI explanation panel
- `.tech-stack` — tech stack listing
- `.contributions` — contributions section wrapper
- `.cp-model` — CP explanation grid
- `.longevity-bar` — animated longevity multiplier bars
- `.tiers-grid` — 5-column tier cards (responsive)
- `.tier-card` — individual tier with CSS custom property `--tier-color`
- `.founding-spotlight` — golden Founding Steward callout
- `.founding-perks` — 3-column perks grid
- `.founding-counter` — spots available counter
- `.community-links` — 3-column community link cards
- `.community-link-card` — individual community link card
- `.btn--community` — purple community CTA button
- `.footer__community` — footer community links row

### 17. New JavaScript

- **Longevity bar animation**: IntersectionObserver triggers animated bar fills on scroll into view

---

## Deployment Notes

- File is fully self-contained (no external dependencies beyond fonts + SVGs)
- Single HTML file, no build step required
- Deploy to Apache at 132.148.219.193 as `/var/www/html/index.html` (or equivalent document root)
- GoDaddy DNS pointing to the server — no DNS changes needed
- Test locally: `open /Users/avielcarlos/.openclaw/workspace/web/atdao-upgrade/index.html`
