# MASTER SYSTEM DOCUMENT — HILO Website Project

---

## SECTION A — Document Status and Immutability Rules

### A.1 Document Identity

| Field | Value |
|-------|-------|
| **Document ID** | 00_MASTER_SYSTEM |
| **Version** | 1.2 |
| **Created** | 2026-04-07 |
| **Created by** | Senior Conversion Architect (GLM) |
| **Owner** | zikotrance |
| **Status** | LOCKED — Source of Truth |
| **Repository** | github.com/zikotrance/websitev2-copywrite2 |
| **Path** | docs/00_MASTER_SYSTEM.md |

### A.2 Immutability Rules

This document is the **single source of truth** for the entire HILO website project. It governs all strategic, editorial, structural, and operational decisions.

```
IMMUTABILITY PROTOCOL:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

1. This document CANNOT be modified without explicit written approval from the owner.
2. No section may be deleted, reordered, or renamed without owner validation.
3. Any proposed modification must be submitted as a formal change request with rationale.
4. The companion document (docs/01_WORKPROGRESS.md) tracks all changes and deviations.
5. In case of conflict between this document and any other file, THIS DOCUMENT PREVAILS.
6. AI agents (GLM, Claude, or any other) must read this document in full before any intervention.

VIOLATION OF THESE RULES INVALIDATES THE ENTIRE PROJECT GOVERNANCE.
```

### A.3 Version Control Protocol

| Scenario | Action |
|----------|--------|
| Minor clarification (typo, formatting) | May be corrected without approval if meaning is unchanged |
| Content addition (new section, new rule) | Requires owner approval |
| Content modification (change to existing rule) | Requires owner approval |
| Full version upgrade (v1 to v2) | Requires owner approval + archive of v1 in docs/archive/ |

### A.4 Relationship with WorkProgress

- `docs/01_WORKPROGRESS.md` is the living companion to this document.
- The Master defines **what** and **why**. The WorkProgress tracks **when**, **how**, and **what's next**.
- Every production action must reference a rule or section from this Master.

---

## SECTION B — Project Mission

### B.1 Business Objective

Build and deploy a **top-tier B2B conversion website** for HILO, a North American manufacturer and distributor of premium glass and mirror products. The website's primary function is to **generate qualified commercial leads** through an AI-powered estimation tool, supported by conversion-optimized content architecture.

### B.2 Type of Site

| Characteristic | Definition |
|---------------|------------|
| **Type** | B2B Lead Generation Website |
| **Primary Audience** | Commercial buyers (hospitality, multi-family, senior living) |
| **Business Model** | Manufacturer-direct with AI estimation funnel |
| **Geographic Scope** | Canada and United States |
| **Language** | English (primary) |
| **Conversion Mechanism** | AI estimation tool → lead capture → sales follow-up |

### B.3 Definition of Success

The HILO website project will be considered successful when:

1. **Lead Generation**: The site consistently generates qualified B2B leads at a conversion rate exceeding 5% of visitors who reach the wizard/estimation tool.
2. **Lead Quality**: More than 70% of captured leads meet qualification criteria (commercial project, 50+ units, defined timeline).
3. **User Experience**: The wizard completion rate exceeds 65%, with average completion time under 90 seconds.
4. **Brand Authority**: The site positions HILO as the premium, reliable, and innovative choice in the glass and mirror industry.
5. **Content Depth**: Every page provides substantive value appropriate to its conversion role, awareness stage, and audience complexity — with clear conversion paths. See Section I.0 (Content Depth Doctrine) for the context-driven depth model.
6. **Operational Efficiency**: The AI estimation tool reduces pre-qualification calls by 50%, freeing sales resources for high-intent leads.

---

## SECTION C — Business Goals and KPIs

### C.1 Primary Goals

| Goal | Target | Measurement |
|------|--------|-------------|
| **Lead Generation** | 5%+ conversion rate from wizard visitors | Analytics: wizard starts → form submissions |
| **Lead Qualification** | 70%+ qualified leads | CRM: lead scoring on first follow-up |
| **Wizard Completion** | 65%+ completion rate | Analytics: step 1 starts → step 8 completions |
| **Friction Reduction** | < 90s average wizard time | Analytics: time from step 1 to submission |
| **Organic Traffic** | 3,000+ monthly visits within 6 months | SEO: Google Search Console data |
| **Repeat Engagement** | 15%+ return visitors | Analytics: 30-day return rate |

### C.2 Secondary Goals

| Goal | Description |
|------|-------------|
| **Brand Differentiation** | Establish HILO as the "engineered for reliability" choice vs. generic competitors |
| **Sales Enablement** | Provide sales team with well-qualified leads and supporting case study materials |
| **Market Expansion** | Attract inquiries from underserved verticals (healthcare, commercial office, mixed-use) |
| **Customer Retention** | Reduce support burden through clear FAQ, warranty, and shipping content |

### C.3 Anti-Goals (What We Do NOT Optimize For)

- Page views for vanity metrics
- B2C individual consumer sales (single-unit orders)
| Social media engagement metrics
- Content length for SEO stuffing purposes
- Feature comparison with irrelevant competitors

---

## SECTION D — ICP and Buying Committee

### D.1 Primary Buyer Personas

#### Persona 1: The Developer / Project Manager (PRIMARY)

| Attribute | Detail |
|-----------|--------|
| **Title** | VP of Development, Director of Procurement, Project Manager |
| **Company** | Hotel chain, multi-family developer, senior living operator |
| **Company Size** | 80+ rooms (hospitality), 100+ units (multi-family) |
| **Decision Authority** | Final or co-decision on FF&E and finishes |
| **Key Pain Points** | Product failures after handover, budget overruns, delivery delays, warranty complexity |
| **Buying Trigger** | New construction, renovation cycle, brand standards update |
| **Sales Cycle** | 2-8 weeks from inquiry to PO |
| **Awareness Level** | Solution-aware (Level 3) to Product-aware (Level 4) |

#### Persona 2: The Architect / Designer (INFLUENCER)

| Attribute | Detail |
|-----------|--------|
| **Title** | Project Architect, Interior Designer, Design Director |
| **Company** | Architecture firm, interior design studio, FF&E procurement |
| **Decision Authority** | Recommender, specifier, strong influence on final selection |
| **Key Pain Points** | Need reliable technical specs, custom options, design flexibility, sustainability data |
| **Buying Trigger** | Project specification phase, material selection milestone |
| **Sales Cycle** | Longer, often 2-6 months, integrated into overall project timeline |
| **Awareness Level** | Problem-aware (Level 2) to Solution-aware (Level 3) |

#### Persona 3: The Facility Manager / GM (END USER INFLUENCER)

| Attribute | Detail |
|-----------|--------|
| **Title** | General Manager, Director of Facilities, Director of Operations |
| **Company** | Operating hotel, residential property management, senior living community |
| **Decision Authority** | Initiator of replacement/renovation, may escalate to ownership |
| **Key Pain Points** | Constant maintenance issues, guest/resident complaints, replacement costs, downtime |
| **Buying Trigger** | Recurring failures, guest complaints, renovation budget approval |
| **Sales Cycle** | Short for replacement, longer for renovation projects |
| **Awareness Level** | Problem-aware (Level 2) — they feel the pain but may not know HILO exists |

### D.2 Buying Committee Dynamics

```
TYPICAL B2B BUYING COMMITTEE FOR HILO:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

1. INITIATOR:     Facility Manager / GM (feels the pain)
2. INFLUENCER:    Architect / Designer (specifies requirements)
3. DECIDER:       VP Development / Director of Procurement (approves budget)
4. BUYER:         Procurement Manager (issues PO, manages contract)
5. END USER:      Maintenance team (installs, maintains)
6. GATEKEEPER:    FF&E Coordinator (filters vendors, schedules reviews)

WEBSITE MUST ADDRESS: Primarily #1, #2, and #3
```

### D.3 Major Objections

| Objection | Root Cause | How the Website Addresses It |
|-----------|------------|------------------------------|
| "We already have a supplier" | Status quo bias, switching cost | Trust Line + case studies showing measurable improvement |
| "How do I know the quality is good?" | No physical inspection possible online | 5-year warranty, <0.5% failure rate, 180+ projects data |
| "Pricing is probably too high" | Association of quality with premium price | Competitive pricing section, direct-from-factory model, volume discounts |
| "I need to see it in person" | Need for tangible proof | Case studies with photos, specifications, samples available on request |
| "Custom will take too long" | Past experience with slow custom suppliers | 4-6 week custom turnaround, AI estimation in 60 seconds |
| "What about after installation?" | Fear of post-sale abandonment | Warranty details, 48-hour claims response, partner network |
| "We're too small / too large for you" | Uncertainty about fit | Clear project minimums (80+ rooms), enterprise-level case studies |

### D.4 Awareness Stage Strategy

The website is primarily designed for visitors at **Awareness Level 3 (Solution Aware)** and **Level 4 (Product Aware)** per the Eugene Schwartz framework. This means:

- They know they have a problem (mirror/glass failures, renovation needs)
- They know solutions exist (LED mirrors, smart mirrors, shower glass)
- They may not know HILO specifically
- They need evidence that HILO is the best choice

Content strategy must lead with **benefits and proof**, not education about the problem.

---

## SECTION E — Brand Positioning and Differentiation

### E.1 Why HILO Wins

HILO wins because it addresses the four anxieties that plague B2B glass and mirror buyers:

1. **Will it fail?** → 5-year warranty, <0.5% failure rate, 180+ projects
2. **Will it cost too much?** → Direct manufacturer pricing, 15-25% below premium competitors
3. **Will it arrive on time and intact?** → Door-to-door delivery, damage-free guarantee, multi-site coordination
4. **Will I be left alone after purchase?** → 48-hour claims response, partner installation network, ongoing support

### E.2 Differentiators (Ranked by Conversion Impact)

| Rank | Differentiator | Proof Point | Emotional Trigger |
|------|---------------|-------------|-------------------|
| **1** | **Documented Reliability** | <0.5% failure rate over 5 years, 180+ projects | Security / Peace of Mind |
| **2** | **5-Year Full Warranty** | No pro-rating, no exclusions for normal use | Confidence / Reduced Risk |
| **3** | **AI-Powered Estimation** | 60-second quotes, no sales call required | Control / Efficiency |
| **4** | **Direct Manufacturer Model** | 15-25% below premium competitors, no middlemen | Value / Smart Buying |
| **5** | **Door-to-Door Delivery** | Multi-site coordination, damage-free guarantee | Reliability / Convenience |
| **6** | **Full Product Range** | 6 categories, 200+ products, one supplier | Simplicity / Consolidation |
| **7** | **Canadian Design Origin** | Designed in Canada, distributed across North America | Quality / Trust |

### E.3 Central Message

```
PRIMARY BRAND MESSAGE:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

"Premium glass and mirror solutions engineered for commercial reliability.
Backed by a 5-year warranty. Delivered door-to-door.
Priced direct from the manufacturer."

SUPPORTED BY:
"Get your instant AI-powered estimate in 60 seconds.
No call required — unless you want one."
```

### E.4 Trust Anchors

The following trust elements MUST be deployed strategically across the site:

| Trust Anchor | Placement | Usage |
|-------------|-----------|-------|
| **180+ Projects** | Hero, footer, case study pages | Social proof at scale |
| **5-Year Warranty** | Hero subheadline, product pages, FAQ | Risk reduction |
| **<0.5% Failure Rate** | Solution pages, case studies | Performance proof |
| **Designed in Canada** | Footer, about page, trust bar | Origin credibility |
| **Distributed across North America** | Trust bar, shipping page | Geographic reach |
| **94% Maintenance Reduction** | Case studies, solution pages | Quantified benefit |
| **89% Repeat Customer Rate** | About page, case studies | Long-term trust |
| **48-Hour Claims Response** | Warranty page, FAQ | After-sale confidence |

### E.5 Mandatory Trust Line

```
THE FOLLOWING LINE MUST APPEAR UNMODIFIED ON EVERY PAGE:

🏆 180+ Projects | 🛡️ 5-Year Warranty | 🇨🇦 Designed in Canada. Distributed across North America.

PLACEMENT:
- Footer of every page
- Below hero CTA sections
- Below final CTA sections
- Never modified, never abbreviated, never omitted
```

### E.6 Brand Terminology Rules

| MANDATORY | FORBIDDEN | Reason |
|-----------|-----------|--------|
| "Designed in Canada" | "Canadian Made" | Legal accuracy — manufacturing spans Canada and US |
| "Distributed across North America" | "Ships across North America" | Implies professional distribution network |
| "Competitive pricing" | "Cheap" / "Low-cost" | Maintains premium positioning |
| "Industry-leading" | "Best" / "#1" | Credibility — avoid unprovable claims |
| "Engineered for..." | "Revolutionary" / "Innovative" | Specificity over marketing fluff |
| "Direct manufacturer" | "Factory direct" (acceptable but less preferred) | Professional B2B language |

---

## SECTION F — Offer Architecture

### F.1 What HILO Sells

HILO operates in two complementary offer modes:

#### Mode 1: Catalog Products (Ready-to-Ship)

| Category | Product Range | Price Visibility | Lead Time |
|----------|--------------|-----------------|-----------|
| LED Mirrors | 200+ designs, multiple sizes | Instant online pricing | 2-3 weeks |
| Smart Mirrors | 50+ configurations | Instant online pricing | 2-3 weeks |
| Medicine Cabinets | 100+ options | Instant online pricing | 2-3 weeks |
| Shower Glass | Frameless and semi-frameless | Quote-based | 2-4 weeks |
| Architectural Glass | Custom specifications | Quote-based | 4-8 weeks |
| Standard Mirrors | Wall, vanity, gym | Instant online pricing | 1-2 weeks |

#### Mode 2: Custom Products (Built-to-Spec)

| Parameter | Detail |
|-----------|--------|
| **Custom Dimensions** | Any size within manufacturing capabilities |
| **Custom Finishes** | Frame styles, LED color temperatures, glass tints |
| **Custom Features** | Integrated lighting zones, anti-fog, touch controls, ADA mounting |
| **Lead Time** | Typically 4-6 weeks |
| **Pricing** | AI-powered estimate in 60 seconds |

### F.2 Catalog vs. Custom Logic

The website must guide visitors through a clear decision tree:

```
CATALOG VS. CUSTOM DECISION FRAMEWORK:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

IF standard sizes fit the spec     → Catalog (faster, instant pricing)
IF brand standards require custom  → Custom (AI estimate in 60s)
IF mixed requirements              → Hybrid approach (most common for B2B)

ALL paths converge on:
→ AI Estimation Tool (unified quote)
→ Lead capture form
→ Sales follow-up (if needed)
```

### F.3 Estimate vs. Call Logic

| Trigger | Action | Rationale |
|---------|--------|-----------|
| Visitor lands on any page | CTA: "Get Instant AI Estimate" visible | Primary conversion path — always available |
| Visitor explores product detail | CTA: "Get AI Instant Quote" + "Book a Call" | Dual path for different buyer preferences |
| Visitor has complex requirements | CTA: "Book a Call" promoted | Some buyers need human interaction for confidence |
| Visitor completes wizard | Gate: contact form for full results | Value exchange — estimate details for contact info |

### F.4 Cross-Sell Architecture

| Current Category | Cross-Sell To | Rationale |
|-----------------|---------------|-----------|
| LED Mirrors | Smart Mirrors | Upsell to premium technology |
| LED Mirrors | Medicine Cabinets | Same buyer (bathroom renovation) |
| Shower Glass | LED Mirrors | Same buyer (bathroom renovation) |
| Smart Mirrors | LED Mirrors | Budget-conscious alternative |
| Any product | Installation service | Natural add-on |

Cross-sell recommendations must appear on:
- Product detail pages (related products section)
- Catalog pages (category navigation)
- AI estimation results (complementary products)
- Post-wizard confirmation (next steps)

---

## SECTION G — Conversion Doctrine

### G.1 The Conversion Equation

Every page on the HILO website must be designed around the MECLABS conversion equation:

```
CONVERSION = (Motivation + Value Proposition + Incentive) - (Friction + Anxiety)

WHERE:
- Motivation (M): The visitor's existing intent when they land on the page
- Value Proposition (V): How clearly HILO communicates superior value
- Incentive (I): The immediate benefit of taking action NOW (free estimate, 60 seconds)
- Friction (F): Every obstacle between intent and action (steps, typing, confusion)
- Anxiety (A): Every fear that prevents action (risk, commitment, uncertainty)

GOAL: MAXIMIZE (M + V + I) and MINIMIZE (F + A) on every page.
```

### G.2 Friction Management

| Friction Type | Strategy | Implementation |
|--------------|----------|----------------|
| **Too many steps** | Reduce to minimum viable steps | Wizard: 6 click-steps + 1 form (not 20 fields upfront) |
| **Too much typing** | Click-based interactions | 90%+ of wizard = clicks, only ZIP code requires typing |
| **Unclear next step** | Single CTA focus per viewport | One primary CTA visible above the fold on every page |
| **Information overload** | Progressive disclosure | Details revealed as visitor scrolls or clicks |
| **Generic messaging** | Audience-specific copy | Industry pages, persona-specific language |
| **Hidden pricing** | Transparent pricing or instant estimate | "Get your estimate in 60 seconds" everywhere |

### G.3 Anxiety Management

| Anxiety Type | Strategy | Implementation |
|-------------|----------|----------------|
| **"Am I making a mistake?"** | Social proof | Case studies with metrics, 180+ projects, 89% repeat rate |
| **"What if it breaks?"** | Warranty clarity | 5-year warranty, no pro-rating, simple claims process |
| **"Will I get spammed?"** | Privacy reassurance | "No spam, no sales call unless you request one" |
| **"Is this legit?"** | Authority signals | Trust Line on every page, specific metrics, company history |
| **"What happens after I submit?"** | Process transparency | "You'll receive your estimate immediately + a follow-up within 24 hours" |
| **"What if I need changes?"** | Flexibility signals | "Unlimited revisions in the AI tool", custom options available |

### G.4 Proof Doctrine

Every claim must be supported by at least one of the following proof types:

| Proof Type | Example | Usage |
|-----------|---------|-------|
| **Quantified Performance** | "<0.5% failure rate", "94% maintenance reduction" | Hero, solution pages |
| **Specific Case Studies** | "Radisson Montreal: 120 rooms, zero defects" | Case study pages, featured sections |
| **Aggregated Metrics** | "180+ projects", "89% repeat customer rate" | Trust Line, about page, footer |
| **Warranty Commitment** | "5-year full warranty, no exclusions" | Product pages, FAQ, warranty page |
| **Third-Party Framework** | Reference to MECLABS, Schwartz, etc. | Master document (not visible to end users) |
| **Process Transparency** | Step-by-step wizard, delivery timeline | Wizard, shipping page |

**FORBIDDEN**: Unsubstantiated claims. Every "we are X" must have a "because Y" attached.

### G.5 CTA Hierarchy

The HILO website uses a three-level CTA architecture:

```
LEVEL 1: ENTRY PAGES (Homepage, Industry Pages, Case Study Index)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
PRIMARY:   "Get Instant AI Estimate →"     → /estimate
SECONDARY: "Book a Call"                   → /contact

LEVEL 2: SOLUTION PAGES (LED Mirrors, Smart Mirrors, etc.)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
PRIMARY:   "See Our Products"              → /solutions/[category]/catalogue
SECONDARY: "Get AI Estimate"               → /estimate

LEVEL 3: PRODUCT DETAIL PAGES (Catalog Items)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
PRIMARY:   "Get AI Instant Quote"           → /estimate (pre-filled)
SECONDARY: "Book a Call"                   → /contact

LEVEL 4: CONVERSION TOOL (Wizard)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
PRIMARY:   "Get My Free Estimate →"        → Submit form
SECONDARY: (none — single-focus conversion)

LEVEL 5: SUPPORTING PAGES (About, FAQ, Warranty, Shipping)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
PRIMARY:   "Get AI Estimate"               → /estimate
SECONDARY: "Contact Us"                    → /contact
```

### G.6 CTA Mapping by Page Type

| Page Type | CTA Principal | CTA Secondaire | CTA Placement |
|-----------|---------------|----------------|---------------|
| Homepage | Get Instant AI Estimate → | Book a Call | Above fold + bottom |
| Industry Page | Get Instant AI Estimate → | Book a Call | Above fold + bottom |
| Solution Page | See Our Products | Get AI Estimate | Above fold + mid-page + bottom |
| Case Study | Start Your Project → | View All Case Studies | Bottom of study + bottom |
| Case Study Index | Start Your Project → | Book a Call | Above fold + bottom |
| Catalog Page | Get AI Instant Quote → | Book a Call | Above fold + per product + bottom |
| Product Detail | Get AI Instant Quote → | Book a Call | Above fold + mid-page + bottom |
| Support Page | Get AI Estimate → | Contact Us | Above fold + bottom |
| Wizard (final) | Get My Free Estimate → | — | End of flow |

---

## SECTION H — Information Architecture Doctrine

### H.1 Site Hierarchy

```
HILO WEBSITE INFORMATION ARCHITECTURE:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

L0: HOMEPAGE                              /
│
├── L1: INDUSTRIES                         /industries/
│   ├── Hotels                             /industries/hotels
│   ├── Real Estate                        /industries/real-estate
│   └── Senior Living                      /industries/senior-living
│
├── L1: SOLUTIONS                          /solutions/
│   ├── LED Mirrors                        /solutions/led-mirrors
│   │   └── Catalog                        /solutions/led-mirrors/catalogue
│   │       └── Product Detail             /solutions/led-mirrors/catalogue/[slug]
│   ├── Smart Mirrors                      /solutions/smart-mirrors
│   │   └── Catalog                        /solutions/smart-mirrors/catalogue
│   │       └── Product Detail             /solutions/smart-mirrors/catalogue/[slug]
│   ├── Medicine Cabinets                  /solutions/medicine-cabinets
│   │   └── Catalog                        /solutions/medicine-cabinets/catalogue
│   │       └── Product Detail             /solutions/medicine-cabinets/catalogue/[slug]
│   ├── Shower Glass                       /solutions/shower-glass
│   │   └── Catalog                        /solutions/shower-glass/catalogue
│   │       └── Product Detail             /solutions/shower-glass/catalogue/[slug]
│   ├── Architectural Glass                /solutions/architectural-glass
│   │   └── Catalog                        /solutions/architectural-glass/catalogue
│   │       └── Product Detail             /solutions/architectural-glass/catalogue/[slug]
│   └── Standard Mirrors                   /solutions/standard-mirrors
│       └── Catalog                        /solutions/standard-mirrors/catalogue
│           └── Product Detail             /solutions/standard-mirrors/catalogue/[slug]
│
├── L1: CASE STUDIES                       /case-studies
│   ├── Index                              /case-studies
│   ├── Hotel Rollup                       /case-studies/hotel-chain-rollup
│   ├── Multi-Family                       /case-studies/multi-family
│   ├── Senior Living                      /case-studies/senior-living
│   ├── Mixed-Use                          /case-studies/mixed-use
│   └── Boutique Hotel                     /case-studies/boutique-hotel
│
├── L1: ESTIMATE                           /estimate (Wizard)
│
└── L1: SUPPORT                            /
    ├── About                              /about
    ├── Contact                            /contact
    ├── FAQ                                /faq
    ├── Warranty                           /warranty
    ├── Shipping                           /shipping
    └── Returns                            /returns

MAXIMUM DEPTH: 4 levels (Homepage → Solutions → Catalog → Product Detail)
```

### H.2 Navigation Rules

| Rule | Description |
|------|-------------|
| **Maximum depth** | 4 levels from homepage |
| **Maximum items in main nav** | 7 top-level items (Industries, Solutions, Case Studies, Estimate, About, FAQ, Contact) |
| **Breadcrumb requirement** | All pages below L1 must show breadcrumb navigation |
| **No orphan pages** | Every page must be reachable from at least 2 navigation paths |
| **Cross-linking** | Solution pages must link to related solutions, industry pages must link to relevant solutions |

### H.3 URL Convention

| Type | Pattern | Example |
|------|---------|---------|
| Industry | `/industries/[slug]` | `/industries/hotels` |
| Solution | `/solutions/[slug]` | `/solutions/led-mirrors` |
| Catalog | `/solutions/[slug]/catalogue` | `/solutions/led-mirrors/catalogue` |
| Product Detail | `/solutions/[slug]/catalogue/[product-slug]` | `/solutions/led-mirrors/catalogue/fleuve-one-plus` |
| Case Study | `/case-studies/[slug]` | `/case-studies/hotel-chain-rollup` |
| Support | `/[slug]` | `/about`, `/contact`, `/faq` |
| Wizard | `/estimate` | `/estimate` |

### H.4 Page Addition/Removal Rules

```
BEFORE ADDING ANY NEW PAGE:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
1. Verify the page type exists in the Page-Type Frameworks (Section I)
2. Confirm the page serves a documented conversion goal (Section G)
3. Map the page into the Information Architecture (Section H)
4. Define CTA hierarchy for the new page (Section G.5)
5. Validate with owner BEFORE creation

BEFORE REMOVING ANY EXISTING PAGE:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
1. Check for inbound links from other pages
2. Assess SEO impact (existing rankings, backlinks)
3. Define redirect strategy (301 redirect to most relevant page)
4. Validate with owner BEFORE removal
```

---

## SECTION I — Content Depth Doctrine

### I.0 Depth Is Contextual, Not Numeric

Page depth must be determined by the conversion requirements of the specific page, not by a one-size-fits-all word count. A rigid "minimum 800 words" rule forces shallow filler on simple pages and may truncate complex pages that need more. Instead, depth is driven by five contextual factors.

The factors that determine how deep a page should go are:

1. **Buying stage of the target visitor** — A solution-aware visitor evaluating HILO as a vendor needs proof, comparison, and specificity. A problem-aware visitor needs credibility and relevance signals. Depth serves the stage.

2. **Complexity of the offer** — Smart mirrors with PMS integration and touchscreen technology require more explanation than standard wall mirrors. The more complex the product or service, the more depth is needed to resolve buyer uncertainty.

3. **Number of objections to resolve** — If a buyer has 7 objections (price, reliability, delivery, installation, custom options, after-sale support, switching cost), the page must address enough of them to reduce anxiety below the action threshold. More objections = more depth.

4. **Proof required** — A case study needs enough narrative depth to make metrics believable, not just a number. A solution page needs enough proof to back each of the 7 HILO criteria. The proof density required drives content depth.

5. **Scanning behavior** — B2B buyers scan before they read. Pages must be scannable first (clear structure, headings, visual hierarchy) and deep second (substantive paragraphs, evidence, reasoning). Scannability does NOT mean short — it means well-structured.

### I.0.1 Depth Guidance by Page Role

| Page Role | Depth Driver | Guidance | Typical Range |
|-----------|-------------|---------|-------------|
| **Homepage** | Breadth of value proposition across multiple personas | Deep enough to communicate all 7 criteria, establish credibility, and drive action. Not a data sheet. | 600-1,200 words |
| **Industry Page** | Industry-specific relevance + targeted objection handling | Must feel specific to the industry (not copy-paste). Depth serves to prove "we understand your sector." | 500-1,000 words |
| **Solution Page** | Category expertise + full 7-criteria coverage + proof density | This is the evaluation page. Buyers compare options here. Every HILO criterion deserves substantive treatment. Deeper is almost always better. | 1,000-2,000 words |
| **Case Study** | Narrative credibility + specific metrics | Must tell a complete story: challenge, approach, results. Metrics alone are not enough — the narrative context makes them believable. | 600-1,200 words |
| **Support Page** | Anxiety resolution + policy clarity | Depth serves the specific questions visitors came to answer. A warranty page needs complete terms. A contact page needs less. | 400-1,000 words |
| **Catalog Page** | Product comparison + decision facilitation | Overview depth with per-product summaries. Grid-based, not narrative-heavy. | 400-800 words (plus product summaries) |
| **Product Detail** | Full specification + conversion confidence | Buyers at this stage are ready to act. They need complete specs, clear pricing path, and trust reinforcement. | 800-1,500 words |

These are guidance ranges, not rigid minimums or maximums. A solution page with 900 words of dense, proof-backed copy is more valuable than a solution page with 1,500 words of filler. The content quality doctrine (Section J) — particularly the paragraph and section rules — remains the operative quality standard.

### I.0.2 When Depth Is Insufficient (Regardless of Word Count)

A page is too thin if ANY of the following are true:

- A visitor cannot determine what HILO offers and why it matters after scanning the page
- Fewer than 3 of the 7 HILO criteria are communicated (on any page)
- A section labeled as a major content block contains only a table or bullet list without explanatory copy
- The Trust Line is the only proof element on the page
- No objection-handling content is present (explicit or implicit)
- The page could apply equally to HILO and to a generic competitor

### I.0.3 When Depth Is Excessive (Regardless of Word Count)

A page is too long if ANY of the following are true:

- Content repeats the same point in multiple sections without adding new information
- Visitors must scroll more than 3 screens to reach the primary CTA on a page designed for action
- Sections exist primarily to hit a word target rather than to serve the buyer
- The page conflates multiple page types (e.g., a support page that contains full product specifications)

---

### I.1 Homepage Framework

| Attribute | Specification |
|-----------|--------------|
| **Objective** | Capture attention, communicate value proposition, drive to wizard |
| **Audience** | All buyer personas (Level 3-4 awareness) |
| **Awareness Stage** | Solution-aware to Product-aware |
| **CTA Principal** | "Get Instant AI Estimate →" |
| **CTA Secondaire** | "Book a Call" |
| **Depth Driver** | Breadth across 7 criteria, multiple persona relevance, credibility establishment |
| **Recommended Blocks** | Hero + Value Prop, 7 Key Advantages, Product Range, Process Steps, Case Study Teaser, FAQ (3 questions), Final CTA |
| **Expected Proof** | Trust Line, case study metrics, 7 HILO criteria |
| **Errors to Avoid** | Generic messaging, no clear path to conversion, missing Trust Line |

### I.2 Industry Page Framework

| Attribute | Specification |
|-----------|--------------|
| **Objective** | Establish relevance to specific industry, drive to wizard |
| **Audience** | Industry-specific buyers (developers, GMs, PMs) |
| **Awareness Stage** | Solution-aware (Level 3) |
| **CTA Principal** | "Get Instant AI Estimate →" |
| **CTA Secondaire** | "Book a Call" |
| **Depth Driver** | Industry-specific objection handling, sector-relevant proof, persona targeting |
| **Recommended Blocks** | Industry-specific hero, 7 advantages (industry-customized), recommended products, industry case study, industry FAQ, Final CTA |
| **Expected Proof** | Industry-specific case study, Trust Line, relevant metrics |
| **Errors to Avoid** | Generic content that could apply to any industry, no industry-specific case study, no sector-specific language |

### I.3 Solution Page Framework

| Attribute | Specification |
|-----------|--------------|
| **Objective** | Communicate category expertise, drive to catalog or wizard |
| **Audience** | Solution-aware buyers evaluating specific product category |
| **Awareness Stage** | Solution-aware to Product-aware (Level 3-4) |
| **CTA Principal** | "See Our Products" |
| **CTA Secondaire** | "Get AI Estimate" |
| **Depth Driver** | Full 7-criteria coverage, offer complexity, proof density, comparison need |
| **Recommended Blocks** | Product-specific hero with reliability stat, all 7 HILO criteria as dedicated sections, pricing callout, delivery section, catalog vs. custom decision box, AI estimate CTA box, product range cross-sell, installation section, Final CTA |
| **Expected Proof** | All 7 HILO criteria present, quantitative data, Trust Line |
| **Errors to Avoid** | Missing any of the 7 criteria, sections without explanatory copy, no decision box for catalog vs. custom |

### I.4 Case Study Framework

| Attribute | Specification |
|-----------|--------------|
| **Objective** | Provide social proof, support conversion on referring pages |
| **Audience** | Product-aware to Most-aware buyers (Level 4-5) |
| **Awareness Stage** | Product-aware (Level 4) — they're evaluating HILO as a vendor |
| **CTA Principal** | "Start Your Project →" |
| **CTA Secondaire** | "View All Case Studies" |
| **Depth Driver** | Narrative credibility to make metrics believable, specific enough to feel real |
| **Recommended Blocks** | Project overview, challenge/problem, HILO solution, results/metrics, testimonial (if available), product details, CTA |
| **Expected Proof** | Specific metrics (units delivered, time frame, failure rate), Trust Line |
| **Errors to Avoid** | Vague results ("they were happy"), no specific numbers, no project narrative, missing CTA |

### I.5 Support Page Framework

| Attribute | Specification |
|-----------|--------------|
| **Objective** | Reduce anxiety, answer objections, support conversion indirectly |
| **Audience** | All awareness levels — visitors seeking reassurance |
| **Awareness Stage** | Variable (2-5) — often anxiety-driven visits |
| **CTA Principal** | "Get AI Estimate →" |
| **CTA Secondaire** | "Contact Us" |
| **Depth Driver** | Number and complexity of questions the page must answer |
| **Recommended Blocks** | Clear page title, comprehensive FAQ-style content, relevant policies, Trust Line, CTA to return to conversion path |
| **Expected Proof** | Specific warranty terms, delivery details, clear policies |
| **Errors to Avoid** | Legal jargon, no CTA back to conversion, missing Trust Line, incomplete information |

### I.6 Catalog Page Framework

| Attribute | Specification |
|-----------|--------------|
| **Objective** | Showcase product range, drive to specific product pages or wizard |
| **Audience** | Product-aware buyers comparing options |
| **Awareness Stage** | Product-aware (Level 4) |
| **CTA Principal** | "Get AI Instant Quote →" |
| **CTA Secondaire** | "Book a Call" |
| **Depth Driver** | Number of products to compare, category complexity |
| **Recommended Blocks** | Category overview, product grid with images, key specs per product, comparison highlights, CTA |
| **Expected Proof** | Product specifications, warranty mention, Trust Line |
| **Errors to Avoid** | No pricing visibility, missing specs, no path to quote |

### I.7 Product Detail Page Framework

| Attribute | Specification |
|-----------|--------------|
| **Objective** | Provide full product information, convert to quote request |
| **Audience** | Most-aware buyers ready to evaluate specific products |
| **Awareness Stage** | Product-aware to Most-aware (Level 4-5) |
| **CTA Principal** | "Get AI Instant Quote →" |
| **CTA Secondaire** | "Book a Call" |
| **Depth Driver** | Specification completeness, feature differentiation, conversion confidence |
| **Recommended Blocks** | Product hero with image, key specifications table, features & benefits, dimensions/sizes, related products, warranty callout, CTA section |
| **Expected Proof** | Detailed specs, Trust Line, warranty terms |
| **Errors to Avoid** | Incomplete specs, no clear pricing or quote path, missing CTA |

---

## SECTION J — Copywriting Doctrine

### J.1 Tone and Voice

| Characteristic | Rule | Example |
|---------------|------|---------|
| **Professional** | B2B-appropriate language at all times | "Engineered for commercial reliability" NOT "Super awesome mirrors!" |
| **Direct** | No jargon, no fluff, no filler paragraphs | "Zero failures in 5 years" NOT "Leveraging best-in-class paradigm" |
| **Benefit-oriented** | Lead with what the customer gains | "Reduce maintenance calls by 94%" NOT "Our mirrors use quality components" |
| **Credible** | Every claim must be provable | "<0.5% failure rate across 180+ projects" NOT "The best mirrors ever" |
| **Scannable** | Short sentences, clear headings, strategic formatting | Bullet points, tables, callout boxes |

### J.2 Clarity Standards

| Rule | Standard |
|------|----------|
| **Reading level** | Grade 8-10 (Flesch-Kincaid) |
| **Sentence length** | Average 15-20 words |
| **Paragraph length** | 3-5 sentences minimum |
| **Section length** | 150-200 words minimum |
| **Heading clarity** | Headings must communicate value, not just label topics |

### J.3 Persuasion Framework

The HILO website uses a layered persuasion model:

```
LAYER 1: ATTENTION (Hero Section)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
H1 = Promise (what HILO delivers)
Subheadline = Proof summary (key metrics)
CTA = Action (immediate next step)
Trust Bar = Credibility anchors

LAYER 2: INTEREST (Value Propositions)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
7 HILO criteria communicated as benefits
Industry-specific relevance established
Problem → Solution → Benefit structure

LAYER 3: DESIRE (Proof & Comparison)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Case studies with specific metrics
Comparison tables (HILO vs. generic alternatives)
Pricing transparency or instant estimate access

LAYER 4: ACTION (CTA & Reassurance)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Friction-free path to conversion
Multiple CTA placements
Anxiety reduction at decision point
Trust Line reinforcement
```

### J.4 Paragraph and Section Rules

```
MANDATORY CONTENT STANDARDS:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

1. NO single-sentence paragraphs. Ever.
2. Every paragraph MUST contain 3-5 sentences minimum.
3. Every section MUST contain 150-200 words minimum of body content.
4. Bullet points are supplementary — they do NOT replace paragraph content.
5. Tables organize information — they do NOT substitute for explanatory copy.
6. Callout boxes highlight key information — they are NOT the primary content.
7. Every heading must be followed by substantive content within 2 lines.
```

### J.5 SEO Content Rules

| Rule | Description |
|------|-------------|
| **H1 per page** | Exactly one H1, containing primary keyword and value proposition |
| **H2 structure** | H2s must be descriptive, benefit-oriented, and contain relevant keywords |
| **Meta descriptions** | 150-160 characters, containing primary keyword and CTA |
| **Internal linking** | Minimum 3 internal links per content page |
| **Alt text** | Every image must have descriptive alt text |
| **Keyword density** | Natural usage, no stuffing. Target: mention primary keyword 3-5 times per page |

### J.6 Claims and Credibility Rules

| Rule | Description |
|------|-------------|
| **No unquantified superlatives** | Never "best", "fastest", "cheapest" without data |
| **Specific over generic** | "94% reduction in maintenance calls" NOT "significantly fewer issues" |
| **Past tense for proof** | Results are documented past events, not future promises |
| **Caveat when appropriate** | "subject to availability", "typical results" where applicable |
| **No fabricated data** | All metrics must be traceable to real HILO performance data |

### J.7 Words and Formulations to Avoid

| AVOID | USE INSTEAD | REASON |
|-------|------------|--------|
| "Amazing" / "Incredible" | "Reliable" / "Proven" | Credibility |
| "Cheap" / "Affordable" | "Competitive pricing" | Premium positioning |
| "Best" / "#1" | "Industry-leading" / "Engineered for..." | Provability |
| "Revolutionary" | "Purpose-built" / "Designed for..." | Specificity |
| "Cutting-edge" | "Advanced" / "Modern" | Overused buzzword |
| "No-brainer" | "Smart choice" / "Strategic decision" | Professionalism |
| "Stakeholder" | "Decision-maker" / "Project lead" | Clarity |
| "Leverage" | "Use" / "Apply" | Jargon avoidance |
| "Utilize" | "Use" | Simplicity |
| "Innovative" | "New" / "Improved" | Overused |
| "Synergy" | (remove entirely) | Meaningless filler |
| "Robust" | "Reliable" / "Durable" | Clarity |
| "Canadian Made" | "Designed in Canada" | Brand rule |

---

## SECTION K — UX/UI Doctrine

### K.1 Conversion-First Priorities

Every UX decision must be evaluated against its impact on conversion. The hierarchy of UX priorities is:

1. **Clarity** — Can the visitor immediately understand what HILO offers and what to do next?
2. **Trust** — Does the design reinforce credibility (professional imagery, clean layout, consistent branding)?
3. **Scannability** — Can a visitor extract key information in under 10 seconds?
4. **Navigation** — Can the visitor find what they need in 3 clicks or fewer?
5. **Mobile Performance** — Does the experience work flawlessly on mobile devices?
6. **Aesthetics** — Does the visual design support the premium B2B positioning?

### K.2 Above-the-Fold Structure

Every page must communicate the following above the fold (without scrolling):

```
ABOVE-THE-FOLD CHECKLIST:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

□ Value proposition headline (H1)
□ Key differentiator or proof point
□ Primary CTA (visible, actionable, benefit-oriented)
□ Secondary CTA (visible but subordinate)
□ Trust Line or trust indicators
□ Clear indication of what HILO does
□ Professional, uncluttered visual treatment
```

### K.3 Scannability Principles

| Principle | Implementation |
|-----------|---------------|
| **Inverted pyramid** | Most important information first, details below |
| **F-pattern scanning** | Key content on left side, supporting elements on right |
| **White space** | Generous padding between sections (48-64px) |
| **Typography hierarchy** | Clear H1/H2/H3 differentiation, readable body text |
| **Visual breaks** | Tables, callout boxes, and imagery to break up text walls |
| **Bullet formatting** | No more than 5-7 bullet items per list |

### K.4 Information Density

| Page Type | Content Density | Rationale |
|-----------|----------------|-----------|
| Homepage | Medium — scannable with clear sections | Broad audience, need to communicate breadth quickly |
| Industry Page | Medium — industry-specific depth | Targeted audience, need relevance |
| Solution Page | High — detailed product information | Evaluation stage, need comprehensive data |
| Case Study | Medium-High — narrative with data | Proof-driven, need specific metrics |
| Product Detail | High — full specifications | Decision stage, need complete information |
| Support Page | Medium — clear and organized | Utility-driven, need quick answers |
| Wizard | Very Low — minimal per screen | Conversion-focused, need zero distraction |

### K.5 Trust Element Placement

| Element | Placement | Frequency |
|---------|-----------|-----------|
| Trust Line | Footer, hero, final CTA | Every page |
| Warranty badge | Product pages, solution pages | Relevant pages |
| Project count | Hero, case study pages, about | High-impact pages |
| Case study metrics | Solution pages, homepage, case study pages | Proof-critical pages |
| Client logos | Homepage, about page | Authority pages |

### K.6 Mobile vs. Desktop Priorities

| Aspect | Mobile | Desktop |
|--------|--------|---------|
| **Navigation** | Hamburger menu, sticky CTA | Full nav, full CTA |
| **Wizard** | Mobile-first design, full-width CTAs, tap-friendly | Standard layout, side-by-side options |
| **Typography** | Minimum 16px body, 24px H2 | Standard web typography |
| **Images** | Smaller hero images, stacked layouts | Full-width hero, grid layouts |
| **Tables** | Stacked/scrollable on mobile | Standard grid tables |
| **CTA Buttons** | Full-width, sticky bottom | Inline, contextual |

---

## SECTION L — Technical and Deployment Governance

### L.1 Repository Structure

```
REPOSITORY STRUCTURE:
github.com/zikotrance/websitev2-copywrite2/
│
├── docs/
│   ├── 00_MASTER_SYSTEM.md          ← THIS DOCUMENT (immutable)
│   └── 01_WORKPROGRESS.md           ← Living progress tracker
│
├── [Page files by number prefix]    ← Content definition files
│   ├── 01_HOMEPAGE.md
│   ├── 02-04 Industries
│   ├── 05-10 Solutions
│   ├── 11-16 Case Studies
│   ├── 17-22 Support
│   ├── 23 Wizard
│   └── 31-51 Catalog Products
│
└── README.md
```

### L.2 GitHub / Deployment Relationship

| Aspect | Convention |
|--------|-----------|
| **Source of truth** | GitHub repository (this repo) |
| **Content definition** | Markdown files in repo (copywrite + structure specs) |
| **Deployment platform** | Vercel (or equivalent) |
| **Deployment trigger** | Commit to main branch → auto-deploy |
| **Branch strategy** | main (production), feature branches for development |

### L.3 Commit Rules

| Rule | Convention |
|------|-----------|
| **Format** | `[type]: brief description in English` |
| **Types** | `docs`, `content`, `structure`, `fix`, `chore` |
| **Example** | `docs: add MASTER_SYSTEM and WORKPROGRESS governance files` |
| **Language** | English for commits, regardless of content language |
| **No force push** | Never force-push to main branch |

### L.4 Quality Assurance Before Deployment

```
QA CHECKLIST — BEFORE ANY DEPLOYMENT:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

CONTENT QA:
□ All pages have Trust Line in footer
□ All pages have primary and secondary CTAs
□ All solution pages address all 7 HILO criteria
□ All pages pass the Depth Insufficiency Test (Section I.0.2) — depth is appropriate to page role, awareness stage, and offer complexity (see Section I.0 for the context-driven depth model)
□ All CTAs link to valid destinations
□ No broken internal links
□ No placeholder text ("Lorem ipsum", "TBD", "XXX")
□ Consistent terminology throughout ("Designed in Canada", not "Canadian Made")

FUNCTIONAL QA:
□ Wizard flow completes successfully end-to-end
□ Mobile responsive on 375px, 768px, 1024px, 1280px viewports
□ All interactive elements functional
□ Form submissions work
□ Page load under 3 seconds

SEO QA:
□ Unique H1 per page
□ Meta descriptions present (150-160 characters)
□ Alt text on all images
□ Proper heading hierarchy (H1 > H2 > H3, no skipping)
```

### L.5 Definition of "Ready for Deployment"

A page or feature is ready for deployment when:

1. Content meets all standards in this Master document (Sections I, J)
2. Copywriting has been reviewed for tone, clarity, and depth
3. All CTAs are functional and point to correct destinations
4. Trust Line is present
5. Mobile and desktop layouts are functional
6. No placeholder content remains
7. Internal linking is complete (minimum 3 links per content page)

---

## SECTION M — Roles and Workflow

### M.1 Role Definitions

#### Owner (zikotrance)
- **Authority**: Final decision-maker on all strategic, content, and structural matters
- **Responsibilities**: Approve master document changes, validate page completions, define priorities
- **Decision power**: Can override any recommendation, approve/deny change requests
- **Availability**: Asynchronous — responds within 24-48 hours typically

#### Prompt Architect / Auditeur
- **Authority**: Designs prompts, audits output quality, enforces master document compliance
- **Responsibilities**: Review all AI outputs against master standards, flag inconsistencies, propose improvements
- **Decision power**: Can request revisions, flag blockers, but cannot override owner decisions

#### GLM (AI Execution Agent)
- **Authority**: Executes tasks within the scope defined by the owner and prompt architect
- **Responsibilities**: Read master document, produce content, follow all rules without exception
- **Decision power**: NONE — must follow master document and owner instructions exactly
- **Constraint**: Must ask for validation when instructions are ambiguous or conflict with this document

### M.2 Decision Validation Protocol

```
WHEN TO ASK FOR VALIDATION:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

ALWAYS VALIDATE (Owner approval required):
- Any modification to this Master document
- Creation or deletion of a page
- Change to CTA hierarchy or wording
- Change to Trust Line text or placement
- Change to URL structure
- Decision that conflicts with any section of this Master
- Any assumption about HILO's business model, pricing, or capabilities

NEVER IMPROVISE:
- Brand terminology (use ONLY approved terms)
- HILO criteria wording (use ONLY approved wording)
- Trust Line text (use ONLY the exact approved text)
- Warranty terms or conditions
- Performance metrics or statistics
- New page types not defined in Section I
```

### M.3 Workflow for Content Production

```
STANDARD CONTENT PRODUCTION WORKFLOW:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

1. READ:    GLM reads 00_MASTER_SYSTEM.md in full
2. CHECK:   GLM reads 01_WORKPROGRESS.md for current context
3. PLAN:    GLM identifies the task and maps it to Master sections
4. EXECUTE: GLM produces content following all applicable rules
5. AUDIT:   GLM self-audits against QA checklist (Section L.4)
6. DELIVER: GLM presents output with compliance summary
7. VALIDATE: Owner reviews and approves or requests changes
8. COMMIT:  Approved content is committed with clear commit message
9. UPDATE:  01_WORKPROGRESS.md is updated with the change
```

---

## SECTION N — Definition of Done

### N.1 When Is a Page "Complete"?

A page is considered complete when ALL of the following are true:

| Criterion | Standard |
|-----------|----------|
| **Content depth** | Depth is appropriate to the page's role, buying stage, offer complexity, objection count, and proof requirements per Section I.0 (Context-Driven Depth Model). Page must NOT trigger any "insufficient depth" criterion in Section I.0.2. |
| **Copy quality** | No single-sentence paragraphs, no sections under 150 words |
| **CTA compliance** | Primary and secondary CTAs present and correct per mapping (Section G.6) |
| **HILO criteria** | Minimum 3 criteria present (5 for solution pages), criterion #1 always present |
| **Trust Line** | Present in footer and under CTAs |
| **Internal links** | Minimum 3 internal links to relevant pages |
| **SEO basics** | Unique H1, meta description, proper heading hierarchy |
| **Consistency** | Terminology, tone, and formatting consistent with Master document |
| **No placeholders** | No TBD, XXX, "placeholder", or Lorem ipsum remaining |
| **QA passed** | All items in QA checklist (Section L.4) checked |

### N.2 When Is a Phase "Complete"?

A project phase is complete when:

1. All pages assigned to the phase are individually "complete" per N.1
2. Internal linking between phase pages is verified
3. The WorkProgress document is updated with phase completion
4. Owner has validated the phase output

### N.3 When Is the Site "Ready for Deployment"?

The entire site is ready for deployment when:

1. All core pages are complete (homepage, solution pages, industry pages, case studies, support pages)
2. The wizard flow is functional end-to-end
3. All CTAs link to valid destinations
4. Mobile responsive design is verified
5. No placeholder content remains anywhere on the site
6. SEO fundamentals are in place (meta, headings, alt text)
7. Performance targets met (LCP < 2.5s, FID < 100ms, CLS < 0.1)
8. Owner gives explicit deployment approval

---

## SECTION O — Gate-Based Project Execution Model

### O.1 Gated Delivery Framework

The HILO website project follows a strict gated execution model. Each gate must be validated before work at the next gate begins. No gate may be skipped or collapsed without explicit owner approval.

```
GATE SEQUENCE:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

GATE 1 — GOVERNANCE FOUNDATION
  Deliverable:  Master System Document + WorkProgress (this document + companion)
  Validation:   Owner reads and approves both governance documents as-is or with noted amendments.
  Blocks:       ALL subsequent gates. Nothing proceeds without G1 approval.
  Status:       DRAFT — awaiting owner validation

GATE 2 — CONVERSION ARCHITECTURE
  Deliverable:  Final sitemap, primary/secondary navigation, page hierarchy,
                page family map, CTA flow by page family,
                rules for adding/removing/merging pages, production order.
  Validation:   Owner approves the conversion architecture as the structural blueprint.
  Blocks:       Gate 3 (no page models can be built without an approved architecture).

GATE 3 — PAGE MODELS AND PRIORITIZATION
  Deliverable:  Per-page-type content models derived from the architecture,
                production priority matrix, content briefs for each page.
  Validation:   Owner approves page models and production sequence.
  Blocks:       Gate 4 (no content production begins without approved models).

GATE 4 — CONTENT PRODUCTION
  Deliverable:  Full page content for all pages per approved models and production order.
  Validation:   Each page passes Definition of Done (Section N.1).
                Batch validation by owner per page family.
  Blocks:       Gate 5 (no site build begins without approved content).

GATE 5 — SITE BUILD
  Deliverable:  Functional website with all content integrated, navigation working,
                responsive layouts, wizard flow operational.
  Validation:   All pages render correctly, all CTAs functional, all links valid.
  Blocks:       Gate 6 (no QA begins without a build to test).

GATE 6 — QA / CRO / SEO VALIDATION
  Deliverable:  QA checklist passed (Section L.4), CRO review of conversion paths,
                SEO audit of all pages, accessibility check, performance benchmarks.
  Validation:   All QA items pass. Critical issues resolved.
  Blocks:       Gate 7 (no deployment without passing QA).

GATE 7 — DEPLOYMENT
  Deliverable:  Live website on production platform.
  Validation:   Smoke test on production, owner sign-off.
  Blocks:       None — project transitions to maintenance/optimization.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### O.2 Gate Validation Rules

| Rule | Description |
|------|-------------|
| **Sequential execution** | Gates must be completed in order (G1 → G2 → G3 → G4 → G5 → G6 → G7). |
| **No parallel gates** | Work on a later gate may not begin before the preceding gate is owner-validated. |
| **Gate deliverable required** | Each gate produces a defined deliverable. Vague or partial deliverables are not acceptable. |
| **Owner validation** | Every gate requires explicit owner approval. Agent self-validation is not sufficient. |
| **Backward impact** | If a validated gate needs revision, all subsequent gates must be re-evaluated for impact. |
| **WorkProgress reflection** | The companion WorkProgress document must reflect the current gate status at all times. |

### O.3 Current Gate Status

| Gate | Name | Status |
|------|------|--------|
| G1 | Governance Foundation | DRAFT — created, not yet owner-approved |
| G2 | Conversion Architecture | NOT STARTED |
| G3 | Page Models and Prioritization | NOT STARTED |
| G4 | Content Production | NOT STARTED |
| G5 | Site Build | NOT STARTED |
| G6 | QA / CRO / SEO Validation | NOT STARTED |
| G7 | Deployment | NOT STARTED |

---

## SECTION P — Mandatory Preserved Rules from Legacy Master

### P.1 The 7 HILO Criteria (PRESERVED VERBATIM)

These 7 criteria are the non-negotiable foundation of every page on the HILO website. They were defined by the owner and must never be altered, reworded, or deprioritized without explicit owner approval.

| Priority | Criterion | Key Message | Application Rule |
|----------|-----------|-------------|-----------------|
| **#1** | Fiabilité long terme | 5 ans sans bris de fonctionnement | Hero subheadline OR dedicated section — ALWAYS PRESENT |
| **#2** | Prix compétitif | Meilleur ROI du marché | Pricing section OR callout box |
| **#3** | Delivery porte-à-porte | Livraison on time, gérée de A à Z | Shipping section OR mentioned in copy |
| **#4** | Flexibilité | Catalogue ou sur mesure | Decision box when applicable |
| **#5** | Minimum d'interaction | Estimation AI instantanée | CTA "Get AI Estimate" visible |
| **#6** | Grand choix produits | Gamme complète verre & miroirs | Cross-sell to other categories |
| **#7** | Installation sur place | Via partenaires selon disponibilité | Installation section |

**Application Rule**: Every page MUST contain at minimum criteria #1 and #5, plus 3 additional criteria. Solution pages MUST contain all 7.

### P.2 Trust Line Exact Text (PRESERVED VERBATIM)

```
🏆 180+ Projects | 🛡️ 5-Year Warranty | 🇨🇦 Designed in Canada. Distributed across North America.

This exact text, with these exact emoji, must appear on every page.
NEVER modify the wording, order, or emoji.
NEVER abbreviate or omit any part.
```

### P.3 CTA Architecture (PRESERVED)

The three-level CTA hierarchy from the legacy master is preserved:

| Level | CTA Principal | CTA Secondaire |
|-------|---------------|----------------|
| Solution Page | See Our Products | Get AI Estimate |
| Product Detail | Get AI Instant Quote | Book a Call |
| Case Study | Start Your Project | View All Case Studies |

### P.4 "Designed in Canada" Terminology (PRESERVED)

```
MANDATORY: "Designed in Canada"
FORBIDDEN: "Canadian Made"

REASON: Legal accuracy. HILO products are designed in Canada but manufactured
and distributed across Canada and the United States.

Always pair with: "Distributed across North America"
or "Canada and US facilities"
```

### P.5 Conversion Frameworks (PRESERVED)

The 7 conversion frameworks from the legacy master continue to inform all content decisions:

| # | Framework | Primary Application |
|---|-----------|-------------------|
| 1 | MECLABS | Value proposition, conversion equation |
| 2 | Hormozi | Offer structure, value stacking |
| 3 | Dan Kennedy | Direct response, urgency |
| 4 | Eugene Schwartz | Awareness levels, copy stages |
| 5 | StoryBrand | Hero journey, clear messaging |
| 6 | PAS (Problem-Agitate-Solution) | Content structure |
| 7 | AIDA (Attention-Interest-Desire-Action) | Page flow |

### P.6 Copywriting Standards (PRESERVED)

| Rule | Standard |
|------|----------|
| Minimum paragraph length | 3-5 sentences |
| Minimum section length | 150-200 words |
| No single-line sections | EVER |
| Tone | Professional, direct, benefit-oriented |
| No slang or excessive emojis | Professional B2B standard |
| Claims must be credible | Data-backed, no hyperbole |

### P.7 Quality Checklists (PRESERVED)

The legacy quality checklist for page validation is preserved and incorporated into Section L.4 of this document. The wizard-specific checklist is preserved in the Wizard flow document.

---

## APPENDIX A — Quick Reference Card

```
HILO MASTER SYSTEM — QUICK REFERENCE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

TRUST LINE (every page):
🏆 180+ Projects | 🛡️ 5-Year Warranty | 🇨🇦 Designed in Canada. Distributed across North America.

7 CRITERIA (every page, min 5 of 7, #1 and #5 always):
1. 5-Year Warranty     5. AI Estimate in 60s
2. Competitive Pricing 6. Full Product Range (200+)
3. Door-to-Door        7. Installation Available
4. Catalog or Custom

CTA HIERARCHY:
Homepage/Industry:    "Get Instant AI Estimate →"  + "Book a Call"
Solution:             "See Our Products"           + "Get AI Estimate"
Product Detail:       "Get AI Instant Quote"       + "Book a Call"
Case Study:           "Start Your Project"         + "View All Case Studies"
Wizard (final):       "Get My Free Estimate →"
Support:              "Get AI Estimate"            + "Contact Us"

TERMINOLOGY:
✓ "Designed in Canada"     ✗ "Canadian Made"
✓ "Competitive pricing"    ✗ "Cheap"
✓ "Industry-leading"       ✗ "Best"
✓ "Engineered for..."      ✗ "Revolutionary"

CONTENT RULES:
- Depth is contextual, not numeric (see Section I.0)
- Depth depends on: buying stage, offer complexity, objections to resolve, proof required, scanning behavior, primary CTA goal
- Use guidance ranges in Section I.0.1 as reference, NOT as rigid minimums
- A page must NOT trigger any "insufficient depth" test in Section I.0.2
- Min 150 words per section body content
- Min 3-5 sentences per paragraph
- No single-sentence paragraphs

BEFORE ANY ACTION:
1. Read 00_MASTER_SYSTEM.md
2. Check 01_WORKPROGRESS.md
3. Follow rules exactly
4. Ask owner if unsure
```

---

*This document is the definitive operational system for the HILO website project. It must be read in full before any production work begins.*
