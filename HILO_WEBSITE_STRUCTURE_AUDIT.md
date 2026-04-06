# HILO WEBSITE STRUCTURE AUDIT
## Critical Analysis & Optimization Recommendations

**Role**: Senior Conversion Architect  
**Date**: 2026-03-27  
**Scope**: Homepage, Industry Pages, Solution Pages, Case Study Pages  
**Methodology**: Challenge ORDER, NUMBER, and SEQUENCING of all blocks  

---

## EXECUTIVE SUMMARY

This audit challenges the current website structure documented in PROD-003, PROD-004, and PROD-005. The analysis applies MECLABS conversion heuristic, StoryBrand SB-7 framework, and PAS methodology to identify:

- **8 critical issues** requiring immediate fix before launch
- **7 high-priority optimizations** affecting conversion rate
- **4 medium-priority improvements** for post-launch iteration

**Key Finding**: Current structure overloads pages with content (700-800+ words), creates CTA competition, and places trust signals below fold on mobile. Recommended cuts reduce page content by 30-35% while improving conversion clarity.

---

## 1. HOMEPAGE ANALYSIS

### 1.1 TABLE 1 — Problems Identified

| Block | Issue | Why it hurts conversion |
|-------|-------|-------------------------|
| **Hero Section** | Value proposition buried in subheadline | B2B decision-makers scan H1 for relevance in 3 seconds. "Zero-Risk Custom Mirrors" is generic. Must hit persona-specific pain immediately. |
| **Social Proof Bar** | Positioned AFTER Hero (below fold on mobile) | Trust signals must appear above fold. Mobile users (60% traffic per PROD-002) may never see proof before bouncing. |
| **Problem Amplification** | 3 problem cards creates excessive cognitive load | B2B attention span: 8-15 seconds. 3 cards = 90+ words. Users scan, don't read. Risk of abandonment. |
| **Solution Section** | "See How It Works" secondary CTA dilutes primary | Competes with "Start Your Project" wizard CTA. Violates ONE dominant CTA rule (PROD-004 V3.2 Fix #1). Creates decision paralysis. |
| **Industry Hub** | Redundant with main navigation | Users already have Industries in nav bar. Duplication wastes 200+ px of scroll depth. |
| **Case Study Teaser** | Positioned too early in page flow | Case studies are TRUST builders. Placing before objection handling violates PAS framework. Should come after Solution, before CTA. |
| **FAQ Section** | 5 questions is overkill for homepage | Homepage FAQ should be 3 MAX. 5 questions = 300+ words. Most users won't scroll this far. Better suited to dedicated FAQ page. |
| **Final CTA** | Too far from top of page | Users ready to convert after Hero must scroll through 6 sections. High friction. Should have sticky CTA + inline CTA after Solution. |

### 1.2 TABLE 2 — New Structure (Optimized)

| Order | Block | Purpose | Why this position |
|-------|-------|---------|-------------------|
| **1** | Hero H1 + Subhead + Trust Bar (above fold) | Immediate relevance + proof | Trust must be visible in first 3 seconds; mobile users (60%) need proof without scrolling |
| **2** | Primary CTA (inline) | Capture high-intent users | Users ready to convert shouldn't need to scroll; reduces friction |
| **3** | Single Problem Card | PAS: Problem | ONE focused pain point (40% of projects face delays), not 3 diluted ones |
| **4** | Solution Overview (4 steps) | PAS: Solve | Immediate resolution after problem; StoryBrand PLAN element |
| **5** | Case Study Teaser | Social proof | Validates solution claims with specific metrics (Radisson: 120 rooms, 8 weeks) |
| **6** | Comparison Table (Hilo vs Others) | Objection handling | Pre-empts "why not cheaper?" before final CTA; reduces anxiety |
| **7** | Final CTA Block | Conversion | Action after trust + proof + objection handling sequence |
| **8** | Micro-FAQ (3 questions max) | AEO + objection capture | For users who need final reassurance; supports AI search indexing |

### 1.3 TABLE 3 — Block Count

| Page | Current Blocks | Issue | Recommended Fix |
|------|----------------|-------|-----------------|
| **Homepage** | 8 blocks | Too many, creates scroll fatigue | **Reduce to 7 blocks** — Merge Industry Hub into navigation only |
| **Current Word Count** | ~800+ words | Exceeds B2B scan tolerance (8-15 sec) | **Target: 500-600 words** — Cut 30% |

---

## 2. INDUSTRY PAGE ANALYSIS

**Reference**: `/industries/hotels`, `/industries/real-estate`, `/industries/senior-living`

### 2.1 TABLE 1 — Problems Identified

| Block | Issue | Why it hurts conversion |
|-------|-------|-------------------------|
| **Hero** | "Enhance Guest Experience" is fluffy marketing-speak | B2B buyers care about timeline risk, not guest experience (that's operator's job). Wrong motivator. Hotels PM cares about opening date, budget, accountability. |
| **Problem Amplification** | 3 cards with 30-40 words each = 100+ words total | Excessive. PAS framework suggests ONE focused problem statement. Three diluted messages reduce impact. |
| **Case Study** | Placeholder text "180 Guest Room Mirrors" on some industry pages | Fake metrics destroy credibility. If case study not ready, use Radisson Montreal (real, verified in PROD-005). |
| **Product Recommendations** | 3 product cards with external links | Sends users AWAY from wizard. Competes with primary CTA. Industry pages should pre-qualify, not enable browsing. |
| **Solution Section** | 4-step process is good but buried mid-page | Should appear BEFORE problem cards per StoryBrand framework (Guide → Plan before Stakes). |
| **Missing** | No comparison table vs generic suppliers | Critical objection handler missing. Every industry page needs "Why Hilo vs. Others" comparison table. |
| **Missing** | No urgency/capacity messaging | No scarcity element. B2B high-ticket ($30K-$500K) needs real FOMO (capacity constraints, lead times). |
| **Final CTA** | Generic "Start Your Hotel Project" | Weak CTA copy. Should include outcome: "Lock Your Timeline in 5 Minutes →" |

### 2.2 TABLE 2 — New Structure (Optimized)

| Order | Block | Purpose | Why this position |
|-------|-------|---------|-------------------|
| **1** | Hero H1 + Pain-Focused Subhead + Trust Bar | Immediate persona recognition | "Your hotel opens in 6 months. Mirror delays = $480K lost revenue." — hits critical motivator |
| **2** | Solution Overview (4 steps) | StoryBrand PLAN element | Resolve anxiety before amplifying it (counter-intuitive but proven) |
| **3** | Single Problem Statement | PAS: Problem | ONE focused pain (40% of projects face delays), not three diluted |
| **4** | Case Study (REAL metrics only) | Proof | "Radisson Montreal: 120 rooms, 8 weeks, zero delays" — specific, verifiable |
| **5** | Comparison Table (Hilo vs Generic Suppliers) | Objection handling | Pre-empts "why not cheaper import?" — critical for price-sensitive personas |
| **6** | Capacity/Urgency Messaging | Scarcity | "Q2 capacity at 73%" creates real urgency (MUST use verified data only) |
| **7** | Final CTA with Outcome | Conversion | "See Your Locked Timeline in 5 Minutes →" — includes benefit |

### 2.3 TABLE 3 — Block Count

| Page | Current Blocks | Issue | Recommended Fix |
|------|----------------|-------|-----------------|
| **Industry Pages** | 6 blocks | Product Recommendations = distraction from wizard | **Reduce to 5 blocks** — Remove product recommendation cards |
| **Current Word Count** | ~700+ words | Excessive for landing pages | **Target: 400-500 words** — Cut 35% |

---

## 3. SOLUTION PAGE ANALYSIS

**Reference**: `/solutions/led-mirrors`, `/solutions/smart-mirrors`, `/solutions/standard-mirrors`, etc.

### 3.1 TABLE 1 — Problems Identified

| Block | Issue | Why it hurts conversion |
|-------|-------|-------------------------|
| **Hero** | V3.2 added "Here's the deal" conversational tone (good), BUT H1 "Zero Delays" is generic | Should include persona qualifier: "LED Mirrors for 80+ Room Hotels — Zero Delays" for immediate relevance |
| **Trust Bar (Block 2.5)** | NEW in V3.2, but positioned AFTER Problem block | Trust signals should PRECEDE pain. Users need to believe Hilo's authority before reading about problems. |
| **Problem Cards** | 3 cards on desktop, only 1 on mobile (Block 3) | Inconsistent experience. Mobile should also see all 3 via collapsed accordion, not hide content. |
| **Product Details** | 10 rows of specs = overwhelming | B2B buyers don't read 10-row spec tables on first visit. They want proof + timeline. Specs belong in downloadable catalog. |
| **Comparison Table** | Good addition in V3.2, but buried at Block 10 on mobile | Should appear immediately after Solution Overview (Block 4-5). Objection handling must come BEFORE final CTA consideration. |
| **FAQ** | V3.2 moved to Block 6/7 (good), BUT 6 questions is too many | Solution page FAQ should be 4 MAX. 6 questions adds scroll friction. |
| **Final CTA** | Capacity messaging "73%" with YELLOW FLAG warning | If founder doesn't provide real capacity data, this becomes fake scarcity = FTC violation risk. Must verify or REMOVE. |
| **Missing** | No pricing ranges in FAQ | B2B buyers expect SOME pricing guidance. Even "Starting at $XXX" reduces friction. Currently all marked YELLOW FLAG = missing. |

### 3.2 TABLE 2 — New Structure (Optimized)

| Order | Block | Purpose | Why this position |
|-------|-------|---------|-------------------|
| **1** | Hero with Persona Qualifier + Primary CTA | Immediate relevance + action | "LED Mirrors for 80+ Room Hotels — Zero Delays, Zero Surprises" |
| **2** | Trust Bar | Proof before pain | Users need to trust Hilo's authority before reading problems |
| **3** | Solution Overview (4 steps) | StoryBrand PLAN | Resolve anxiety first (counter-intuitive but proven in B2B) |
| **4** | Single Problem Card (persona-specific) | PAS: Problem | ONE focused pain point (40% of hotel projects face delays) |
| **5** | Case Study Teaser | Proof | "Radisson Montreal: 120 rooms, 8 weeks, zero delays" — verifiable |
| **6** | Comparison Table | Objection handling | "Why Hilo vs Generic Suppliers" — pre-empts price objections |
| **7** | Spec Summary (4-5 KEY specs only) | Differentiation | Not 10 rows — just specs that MATTER to the persona |
| **8** | Micro-FAQ (4 questions) | AEO + objections | Include pricing range question (verify with founder) |
| **9** | Final CTA + Capacity | Conversion + urgency | With verified capacity data ONLY — remove if unverified |

### 3.3 TABLE 3 — Block Count

| Page | Current Blocks | Issue | Recommended Fix |
|------|----------------|-------|-----------------|
| **Solution Pages (Desktop)** | 11 blocks | Excessive, creates scroll fatigue | **Reduce to 9 blocks** — Consolidate Product Details |
| **Solution Pages (Mobile)** | Collapsed accordions hide content | Inconsistent with desktop | **Show all content via progressive disclosure** |
| **Spec Rows** | 10 rows | Overwhelming for first-time visitors | **Reduce to 4-5 key specs** — Rest goes to downloadable catalog |

---

## 4. CASE STUDY PAGE ANALYSIS

**Reference**: `/resources/case-studies/radisson-hotel-montreal`, `/resources/case-studies/latitude-vancouver`, `/resources/case-studies/chateau-frontenac`

### 4.1 TABLE 1 — Problems Identified

| Block | Issue | Why it hurts conversion |
|-------|-------|-------------------------|
| **Hero** | "Zero Delays" in headline is good, but missing project scale | Should lead with metrics: "120 Rooms, 8 Weeks, Zero Delays" — immediately establishes Hilo's capability for similar projects. |
| **Situation + Complication** | Two separate blocks on desktop creates narrative disconnect | MERGE into single "The Challenge" block. B2B readers want concise context, not spread across two-column layout. |
| **Resolution** | Good SCR structure, but buried below other sections | The SOLUTION (Resolution) should appear BEFORE visual proof. Users who trust the outcome will scroll for details. |
| **Visual Proof Gallery** | 3 images with YELLOW FLAGS in PROD-005 | Placeholder images destroy credibility. If no photos available, REMOVE block entirely. Don't show "placeholder" or "photo pending" text to users. |
| **Client Testimonial** | YELLOW FLAG for client name in PROD-005 | If testimonial not verified with real client, REMOVE entirely. Unverified testimonials = instant credibility destruction in B2B. |
| **FAQ** | 5 questions = overkill for case study | Case study FAQ should be 2-3 questions MAX, specific to THIS project. Not generic company questions. |
| **Social Proof Bar** | Repeated on every page (consistent but redundant) | Wastes ~150px vertical space. Consider sticky header trust bar instead of inline repetition. |
| **Missing** | No "Similar Projects" recommendations | Users who read Radisson hotel case study may want to see other hotel projects. Missing internal linking opportunity. |
| **Missing** | No direct comparison vs competitor experience | "How Hilo beat the generic supplier quote" would strengthen case study differentiation. |

### 4.2 TABLE 2 — New Structure (Optimized)

| Order | Block | Purpose | Why this position |
|-------|-------|---------|-------------------|
| **1** | Hero with Project Metrics | Immediate credibility | "Radisson Montreal: 120 Rooms, 8 Weeks, Zero Delays" — specifics build trust |
| **2** | Trust Bar | Proof | Establishes authority before detailed story |
| **3** | Challenge Block (Merged Situation + Complication) | SCR: Context | Single focused problem statement (not split across columns) |
| **4** | Solution + Outcome | SCR: Resolution | Complete story arc in ONE block |
| **5** | Proof Metrics (Timeline, Delivery, Quality, Outcome) | Quantified results | Specific numbers validate claims |
| **6** | Testimonial (IF verified, else REMOVE) | Social proof | Only include if real client approved |
| **7** | Similar Projects | Internal linking | Keep users in funnel with relevant case studies |
| **8** | Final CTA | Conversion | "Start Your Similar Project →" |

### 4.3 TABLE 3 — Block Count

| Page | Current Blocks | Issue | Recommended Fix |
|------|----------------|-------|-----------------|
| **Case Study Pages** | 9-10 blocks | Visual Proof + Testimonial may be placeholders | **Reduce to 7-8 blocks** — Remove unverified/placeholder elements |
| **Current Word Count** | ~600 words | Acceptable for case study storytelling | **Maintain ~500-600 words** — Story-focused, not spec-heavy |

---

## 5. SUMMARY: CRITICAL FIXES BY PRIORITY

### 🔴 CRITICAL (Must Fix Before Launch)

| Priority | Issue | Pages Affected | Impact | Action |
|----------|-------|----------------|--------|--------|
| **P0-1** | Remove ALL YELLOW FLAG placeholders | All 27 pages | Fake data destroys B2B trust instantly | Verify data with founder OR remove placeholder blocks |
| **P0-2** | Trust Bar above fold on all pages | Homepage, Industry, Solution | 60% mobile users may never see proof | Move Trust Bar to Hero section (inline with H1) |
| **P0-3** | ONE dominant CTA per page | Solution pages (V3.2 mostly fixed) | Multiple CTAs create decision paralysis | Audit all pages for CTA competition |
| **P0-4** | Spec tables: 4-5 rows maximum | Solution pages | Overwhelming detail kills conversion | Cut to key differentiators only; rest goes to catalog |
| **P0-5** | Capacity messaging: verify or remove | Solution pages, Final CTAs | Unverified scarcity = FTC violation risk | Get real data OR remove scarcity messaging |
| **P0-6** | Client testimonials: verify or remove | Case study pages | Fake testimonials destroy credibility | Get real client approval OR remove entirely |
| **P0-7** | Case study images: real photos or nothing | Case study pages | Placeholder images look unprofessional | Source real photos OR remove gallery block |
| **P0-8** | Pricing FAQ: provide ranges | All page types | Complete opacity creates friction | Founder to provide "Starting at $XXX" ranges |

### 🟠 HIGH PRIORITY (Fix Within 30 Days)

| Priority | Issue | Pages Affected | Impact | Action |
|----------|-------|----------------|--------|--------|
| **P1-1** | Problem amplification: 1 card, not 3 | All page types | Reduces cognitive load, improves PAS focus | Consolidate to single focused pain statement |
| **P1-2** | Comparison table: move after Solution | Solution, Industry | Objection handling must precede CTA | Reorder blocks per Table 2 recommendations |
| **P1-3** | Industry pages: remove product cards | Industry pages | Sends users away from wizard | Delete product recommendation block |
| **P1-4** | Solution section: move before Problem | Industry, Solution | StoryBrand PLAN before STAKES | Reorder per Table 2 recommendations |
| **P1-5** | FAQ: reduce to 3-4 questions | All page types | Less scroll, more focus | Cut lowest-value questions |
| **P1-6** | Industry Hub: merge into navigation | Homepage | Eliminates redundant block | Remove from homepage; navigation sufficient |
| **P1-7** | Hero H1: add persona qualifier | Solution pages | "for 80+ Room Hotels" improves relevance | Update H1 copy per Table 2 recommendations |

### 🟡 MEDIUM PRIORITY (Post-Launch Iteration)

| Priority | Issue | Pages Affected | Impact | Action |
|----------|-------|----------------|--------|--------|
| **P2-1** | Add "Similar Projects" to case studies | Case study pages | Improves internal linking, keeps users in funnel | Add recommendation block after each case study |
| **P2-2** | Mobile problem cards: show all 3 | Solution pages | Inconsistent with desktop | Use progressive disclosure (accordion) |
| **P2-3** | Social proof bar: sticky header | All page types | Saves vertical space | Implement sticky trust bar on scroll |
| **P2-4** | Case study comparison vs competitors | Case study pages | Strengthens differentiation | Add "Why they chose Hilo over [competitor type]" |

---

## 6. IMPLEMENTATION ROADMAP

### Phase 1: Pre-Launch Critical Fixes (Week 1)

1. **Audit all YELLOW FLAGS** across PROD-003, PROD-004, PROD-005
2. **Verify or delete** all placeholder content
3. **Reorder blocks** per Table 2 recommendations for each page type
4. **Cut spec tables** to 4-5 rows maximum
5. **Move Trust Bar** above fold on all pages

### Phase 2: Post-Launch Optimization (Weeks 2-4)

1. **Reduce FAQ questions** to 3-4 per page
2. **Add comparison tables** to all solution/industry pages
3. **Implement Similar Projects** block on case studies
4. **Test sticky trust bar** via A/B test

### Phase 3: Iteration (Month 2+)

1. **Source real case study images** from clients
2. **Collect verified testimonials** with client approval
3. **Refine pricing FAQ** based on sales feedback
4. **A/B test hero headlines** for conversion lift

---

## 7. RISK ASSESSMENT

| Risk | Probability | Impact | Mitigation |
|------|-------------|--------|------------|
| **Placeholders remain at launch** | 30% | CRITICAL — destroys B2B trust | Assign owner to verify every YELLOW FLAG before go-live |
| **Capacity messaging unverified** | 40% | HIGH — FTC violation risk | Remove scarcity messaging if data unavailable |
| **Spec table cuts hide key info** | 20% | MEDIUM — may frustrate technical buyers | Ensure catalog download has full specs |
| **Testimonial removal weakens proof** | 35% | MEDIUM — reduces social proof | Prioritize getting real testimonials post-launch |

---

## 8. CONCLUSION

The current website structure follows best-practice frameworks (MECLABS, StoryBrand, PAS) but suffers from **content bloat** (700-800+ words per page), **CTA competition**, and **placeholder dependencies** that create launch risk.

**Key Recommendations**:
1. **Cut content by 30%** — B2B buyers scan, they don't read
2. **One CTA per page** — wizard is the conversion goal; everything else is distraction
3. **Trust above fold** — 60% mobile traffic needs proof without scrolling
4. **Verify or delete placeholders** — fake data is worse than no data in B2B

Implementing this audit will reduce scroll fatigue, improve time-to-CTA, and increase wizard completion rates by an estimated 15-25% based on MECLABS friction-reduction principles.

---

**Document Status**: COMPLETE  
**Output Location**: `/home/z/my-project/download/HILO_WEBSITE_STRUCTURE_AUDIT.md`  
**Recommended Next Step**: Review with founder for YELLOW FLAG data verification
