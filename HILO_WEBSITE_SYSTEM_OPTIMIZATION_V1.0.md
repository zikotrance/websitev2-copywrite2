# HILO Website System Optimization V1.0

**Document Type**: System-Level Performance Architecture  
**Version**: 1.0  
**Date**: 2026-03-27  
**Domain**: hilomirrors.com  
**Scope**: Global Flow, AI Tool Integration, SEO/AI SEO, Mobile-First Design  

---

## Executive Summary

This document transforms the Hilo Mirrors website from a collection of individually optimized pages into a **unified high-performance conversion system**. The previous phase optimized page-level structure (blocks, content, CTAs). This phase focuses exclusively on **system-level performance**:

- **Conversion Optimization**: Speed of decision, speed of qualification
- **SEO Ranking**: Google search visibility and authority
- **AI SEO**: Visibility in ChatGPT, Perplexity, Gemini, and AI Overviews

### Core Principles

1. **Every Entry Point Has a Clear Path**: Users arrive from ads, SEO, AI search, direct traffic — each path is optimized
2. **The AI Estimation Tool is the Conversion Engine**: All roads lead to the 5-step wizard
3. **Internal Linking Creates Authority**: Pillar-cluster architecture supports both SEO and user navigation
4. **Mobile-First Design**: 65%+ of B2B traffic is mobile; design for mobile first, then expand

---

## SECTION 1 — Global User Flow Optimization

### 1.1 Entry Point Analysis

The Hilo website receives traffic from 8 distinct entry points, each with different intent levels and conversion pathways.

| Entry Point | Landing Page | User Intent Level | Next Step | Goal | Time to Decision |
|-------------|--------------|-------------------|-----------|------|------------------|
| **Paid Ads (Google/LinkedIn)** | Industry Page (Hotels/Real Estate/Senior Living) | HIGH — Problem-aware, solution-seeking | AI Estimation Tool (Step 1) | Wizard completion within 3 min | < 5 min |
| **Paid Ads (Retargeting)** | Solution Page (LED Mirrors/Smart Mirrors) | MEDIUM — Product-aware, comparing options | Compare Block → AI Estimation Tool | Wizard start within 2 min | < 4 min |
| **Organic SEO (Google)** | Varies by query intent | VARIES — Informational to Transactional | FAQ → Case Study → AI Estimation Tool | Capture email via exit-intent if not qualified | < 7 min |
| **AI Search (ChatGPT/Perplexity)** | Homepage or Solution Page | HIGH — AI-recommended, pre-qualified | Trust Bar → AI Estimation Tool | Wizard start within 2 min | < 4 min |
| **Direct Traffic** | Homepage | LOW-MEDIUM — Brand awareness | Industry Hub → Solution Page → AI Estimation Tool | Self-qualify via industry path | < 8 min |
| **Email Outreach** | Personalized Landing Page | HIGH — Pre-warmed lead | AI Estimation Tool (pre-filled) | Wizard completion within 2 min | < 3 min |
| **Referral/Word of Mouth** | Homepage | MEDIUM — Trust established | Case Study → AI Estimation Tool | Wizard start within 4 min | < 6 min |
| **Social (LinkedIn)** | Solution Page or Case Study | MEDIUM — Content engagement | Trust Bar → AI Estimation Tool | Capture via exit-intent or wizard | < 5 min |

### 1.2 Intent-Based Routing Logic

**HIGH Intent** (Paid Ads, Email Outreach, AI Search):
- Route directly to AI Estimation Tool
- Minimize intermediate steps
- Pre-fill wizard where possible (UTM parameters, referral source)

**MEDIUM Intent** (Retargeting, Social, Referral):
- Route through Trust Bar → Compare Block → AI Estimation Tool
- Social proof placement before CTA
- Objection handling via FAQ or comparison table

**LOW Intent** (Direct Traffic, Informational SEO):
- Route through Industry Hub → Solution Page → Case Study → AI Estimation Tool
- Self-qualification via industry-specific content
- Exit-intent capture for email nurturing

### 1.3 Flow Optimization Rules

| Rule | Implementation | Expected Impact |
|------|----------------|-----------------|
| **3-Click Maximum** | User reaches AI Estimation Tool within 3 clicks from any page | +30% conversion rate |
| **Pre-Qualification Messaging** | Industry pages state thresholds (100+ units, 80+ rooms) upfront | Higher quality leads, lower disqualification |
| **Exit-Intent Everywhere** | All pages except wizard have exit-intent popup | 10-15% abandonment recovery |
| **Email Resume Link** | Partial wizard submissions receive email with resume link | +25% wizard completion rate |

---

## SECTION 2 — AI Tool Integration

### 2.1 AI Estimation Tool Overview

The **"Get Instant Estimation"** / **"Start Your Project"** wizard is the primary conversion engine. It must be:

- **Visible**: Present on every conversion-focused page
- **Accessible**: Reachable within 2-3 clicks from any page
- **Consistent**: Same CTA text and styling across all instances
- **Pre-Filled**: When coming from product/industry pages, pre-select relevant options

### 2.2 AI Tool Placement Matrix

| Page | Position | Role | Trigger | Integration Type |
|------|----------|------|---------|------------------|
| **Homepage** | Hero CTA (Primary) + Sticky Mobile CTA + Final CTA Block | Primary conversion engine | Click "Start Your Project →" | Direct link to `/start-a-project` |
| **Homepage** | Trust Bar | Secondary conversion nudge | After scroll 30% | Floating CTA badge "Get Instant Estimation" |
| **Industry: Hotels** | Hero CTA + Solution Section + Final CTA | Industry-specific qualification | Click "Get a Hotel Quote →" | Direct link with UTM parameter |
| **Industry: Real Estate** | Hero CTA + Solution Section + Final CTA | Industry-specific qualification | Click "Get a Project Quote →" | Direct link with UTM parameter |
| **Industry: Senior Living** | Hero CTA + Solution Section + Final CTA | Industry-specific qualification | Click "Get a Senior Living Quote →" | Direct link with UTM parameter |
| **Solution: LED Mirrors** | Hero CTA + Mid-page CTA + Final CTA | Product-specific qualification | Click "See Your Timeline & Price →" | Direct link with product pre-selection |
| **Solution: Smart Mirrors** | Hero CTA + Mid-page CTA + Final CTA | Product-specific qualification | Click "See Your Timeline & Price →" | Direct link with product pre-selection |
| **Solution: Medicine Cabinets** | Hero CTA + Final CTA | Product-specific qualification | Click "Start Your Project →" | Direct link with product pre-selection |
| **Solution: Shower Glass** | Hero CTA + Final CTA | Product-specific qualification | Click "Start Your Project →" | Direct link with product pre-selection |
| **Solution: Architectural Glass** | Hero CTA + Final CTA | Product-specific qualification | Click "Start Your Project →" | Direct link with product pre-selection |
| **Solution: Standard Mirrors** | Hero CTA + Final CTA | Product-specific qualification | Click "Start Your Project →" | Direct link with product pre-selection |
| **Case Study: Radisson** | Post-read CTA block | Proof-to-action conversion | Click "Start Your Hotel Project →" | Direct link with UTM tracking |
| **Case Study: Latitude** | Post-read CTA block | Proof-to-action conversion | Click "Start Your Project →" | Direct link with UTM tracking |
| **Case Study: Frontenac** | Post-read CTA block | Proof-to-action conversion | Click "Start Your Senior Living Project →" | Direct link with UTM tracking |
| **Resources Hub** | Sidebar widget | Passive conversion opportunity | Visible on scroll | Floating widget |
| **Knowledge Hub** | After article completion | Content-to-action conversion | Click "Get Custom Quote →" | Inline CTA |
| **FAQ Page** | Final section | Objection-to-action conversion | Click "Still have questions? Get a Custom Quote →" | Inline CTA |
| **Contact Page** | Alternative to direct contact | Self-service qualification | Click "Get Instant Estimation →" | Prominent button |
| **Exit-Intent Popup** | All pages (except wizard) | Abandonment recovery | Mouse exit detection | Email capture + resume link |
| **Mobile Sticky CTA** | All conversion pages | Always-available action | Fixed bottom position | Direct link |

### 2.3 Pre-Selection Logic

When users navigate from specific pages, the wizard should pre-fill relevant fields:

| Source Page | Step 1 Pre-Select | Step 4 Pre-Select |
|-------------|-------------------|-------------------|
| Hotels Industry | project_type = "hotel" | — |
| Real Estate Industry | project_type = "residential" | — |
| Senior Living Industry | project_type = "senior_living" | — |
| LED Mirrors | — | products = ["led_mirrors"] |
| Smart Mirrors | — | products = ["smart_mirrors"] |
| Medicine Cabinets | — | products = ["medicine_cabinets"] |
| Shower Glass | — | products = ["shower_glass"] |
| Architectural Glass | — | products = ["architectural_glass"] |
| Standard Mirrors | — | products = ["standard_mirrors"] |

### 2.4 CTA Integration Rules

| Rule | Implementation |
|------|----------------|
| **Maximum 2 CTAs per page** | One above fold (Hero), one at decision point (Final CTA) |
| **Mobile sticky CTA** | Always visible, never overlaps content, 56px height |
| **Exit-intent timing** | Trigger after 30 seconds OR scroll to 50%+ |
| **UTM parameters** | All CTAs include source, medium, campaign for attribution |

---

## SECTION 3 — SEO + AI SEO System

### 3.1 Dual-Layer SEO Strategy

The website must be optimized for TWO distinct search environments:

**Layer 1: Traditional SEO (Google)**
- High-intent commercial keywords
- Long-tail keywords (product + industry + location)
- Problem-focused keywords
- Featured snippet optimization

**Layer 2: AI-Era SEO (ChatGPT, Perplexity, Gemini)**
- Natural language questions
- Comparison queries
- Entity-defining queries
- Citation-worthy content

### 3.2 SEO/AI Mapping Matrix

| Page | Primary Intent | SEO Role | AI Query Trigger | Answer Block Required |
|------|---------------|----------|------------------|----------------------|
| **Homepage** | Brand/Navigation | Authority hub, brand entity | "Who is Hilo Mirrors?", "Best custom mirror manufacturer Canada" | Company definition, key differentiators |
| **Solutions Hub** | Product Discovery | Product pillar page | "What types of mirrors does Hilo offer?", "LED vs smart mirrors comparison" | Product category overview, comparison table |
| **LED Mirrors** | Transactional | Primary money page | "Best LED mirrors for hotels", "Custom LED mirror price", "LED mirror specifications" | Pricing guide, specs table, comparison |
| **Smart Mirrors** | Transactional | Money page | "Smart mirrors for hotels with PMS integration", "Touchscreen vs voice mirror" | Features list, integration capabilities |
| **Standard Mirrors** | Transactional | Money page | "Frameless mirrors for condos", "Custom mirror sizes residential" | Size guide, material specs |
| **Medicine Cabinets** | Transactional | Money page | "ADA-compliant medicine cabinets", "Senior living bathroom fixtures" | Safety features, ADA compliance list |
| **Shower Glass** | Transactional | Money page | "Frameless shower glass for hotels", "Custom shower enclosures bulk" | Glass thickness guide, hardware options |
| **Architectural Glass** | Transactional | Money page | "Architectural glass feature walls", "Custom glass for commercial lobbies" | Application examples, customization options |
| **Industries Hub** | Industry Discovery | Industry pillar page | "What industries does Hilo serve?", "Mirror solutions by sector" | Industry overview table |
| **Hotels Industry** | Industry-specific | Primary industry page | "Mirror supplier for 80+ room hotels", "Hotel bathroom renovation mirrors" | Industry pain points, solution overview |
| **Real Estate Industry** | Industry-specific | Industry page | "Mirror supplier for 100+ unit developments", "Condo bathroom mirrors bulk" | Developer pain points, process overview |
| **Senior Living Industry** | Industry-specific | Industry page | "Safety mirrors for senior living", "ADA-compliant bathroom fixtures" | Safety requirements, compliance checklist |
| **Start a Project** | Conversion | Wizard entry | "How to order custom mirrors from Hilo?", "Get LED mirror quote" | Step-by-step process, timeline expectation |
| **Resources Hub** | Informational | Content hub | "Hilo case studies", "Mirror installation guides" | Resource directory |
| **Case Studies Hub** | Proof-seeking | Trust building | "Hilo mirror projects", "Hotel mirror case study" | Project summary cards |
| **Case Study: Radisson** | Proof-seeking | Proof page | "Radisson hotel mirror renovation", "180 room LED mirror project" | Project metrics, before/after, client quote |
| **Case Study: Latitude** | Proof-seeking | Proof page | "Condo mirror installation Vancouver", "240 unit residential mirror project" | Project metrics, timeline, results |
| **Case Study: Frontenac** | Proof-seeking | Proof page | "Senior living mirror installation", "ADA-compliant medicine cabinets project" | Project metrics, safety features, client quote |
| **Catalog** | Product Research | Product reference | "Hilo mirror catalog", "LED mirror specifications PDF" | Product list with specs |
| **Knowledge Hub** | Educational | Content support | "How to choose LED mirrors", "Mirror installation best practices" | Educational articles |
| **FAQ** | Support | Objection handling | "What is Hilo's warranty?", "What size projects does Hilo accept?" | FAQPage schema with 10+ Q&A |
| **About** | Trust-building | Brand story | "Hilo Mirrors company history", "Who founded Hilo?" | Company story, team, values |
| **Contact** | Direct contact | Alternative conversion | "Contact Hilo Mirrors", "Hilo customer service" | Contact form, phone, email |

### 3.3 Answer Block Strategy

Every page should contain **Answer Blocks** — self-contained Q&A units optimized for AI citation.

**Answer Block Templates by Query Type:**

| Query Type | Format | Word Count | Schema |
|------------|--------|------------|--------|
| "What is [X]?" | Paragraph | 40-60 words | Organization, Product |
| "How to [X]?" | Numbered steps | 3-5 steps | HowTo |
| "Why [X]?" | Bulleted list | 3-5 reasons | — |
| "Compare [X vs Y]" | Table | 4-6 rows | — |
| "Best [X] for [Y]" | Table with recommendations | 4-6 rows | Product |

### 3.4 Internal Linking Architecture

**Pillar-Cluster Structure:**

```
Homepage (Pillar)
├── Solutions Hub (Cluster Hub)
│   ├── LED Mirrors (Cluster)
│   ├── Smart Mirrors (Cluster)
│   ├── Standard Mirrors (Cluster)
│   ├── Medicine Cabinets (Cluster)
│   ├── Shower Glass (Cluster)
│   └── Architectural Glass (Cluster)
├── Industries Hub (Cluster Hub)
│   ├── Hotels (Cluster)
│   ├── Real Estate (Cluster)
│   └── Senior Living (Cluster)
├── Resources Hub (Cluster Hub)
│   ├── Case Studies Hub
│   │   ├── Radisson Case Study
│   │   ├── Latitude Case Study
│   │   └── Frontenac Case Study
│   ├── Catalog
│   ├── Knowledge Hub
│   └── FAQ
└── Start a Project (Exit Point)
```

**Linking Rules:**

| Link Type | Implementation |
|-----------|----------------|
| Pillar → Cluster | Hub pages link to all child pages |
| Cluster → Pillar | Child pages link back to parent hub |
| Cross-Cluster | Industry pages link to relevant solution pages |
| Case Study → Solution | Each case study links to featured product |
| Case Study → Industry | Each case study links to relevant industry page |
| All Pages → Wizard | Every page has at least one CTA to wizard |

### 3.5 E-E-A-T Signal Implementation

| Signal | Implementation | Page Location |
|--------|----------------|---------------|
| **Experience** | "180+ projects since 2018", case studies with metrics | Homepage, Industry Pages, Case Studies |
| **Expertise** | Technical specifications, installation guides | Solution Pages, Knowledge Hub |
| **Authoritativeness** | UL/cUL certifications, ISO badges, client logos | Trust Bar (all pages) |
| **Trustworthiness** | 5-year warranty, 98% on-time delivery, testimonials | All conversion pages |

---

## SECTION 4 — Mobile-First Flow Design

### 4.1 Mobile Traffic Context

- **65%+ of B2B traffic** comes from mobile devices
- Mobile users have **30% shorter attention spans**
- Mobile conversion rates are typically **20-30% lower** than desktop
- **Optimization priority**: Mobile first, then expand to tablet/desktop

### 4.2 Mobile User Flow Analysis

| Step | User Behavior | Risk | Fix | Impact |
|------|---------------|------|-----|--------|
| **1. Initial Load** | User lands on page, sees hero section | Hero image too large → slow LCP | WebP format, <150KB, lazy-load, priority="high" only desktop | Reduces bounce by 15-20% |
| **2. Hero Scan (0-5s)** | User reads H1 + subhead, looks for CTA | Multiple CTAs create confusion | Single sticky CTA at bottom, fixed position | 100% CTA visibility |
| **3. Scroll Decision (5-15s)** | User scrolls to see more content | Content too dense → early exit | Reduce text density by 30%, use accordion | +40% scroll depth |
| **4. Problem Cards** | User skims 3 pain points | Cards too long → skipped | 30-40 words max, 2-3 sentences | +50% comprehension |
| **5. Solution Section** | User looks for "how it works" | 4 steps require horizontal scroll | Vertical stack, numbered list format | Reduces friction |
| **6. Product Details** | User seeks specifications | Table format causes horizontal scroll | Accordion list with benefit-first format | Eliminates h-scroll |
| **7. FAQ Accordion** | User has remaining objections | FAQ too far down → never reached | Move to Block 7 position, collapsible | +60% engagement |
| **8. Case Study Teaser** | User seeks proof | Full case study requires navigation | Collapsed thumbnail + 1-line summary | Maintains on-page |
| **9. Final CTA** | User decides to act | CTA only at bottom → missed | Sticky CTA always visible + Final block | +25% CTA clicks |
| **10. Chat Widget** | User has question before committing | Chat covers CTA on mobile | Position 80px above sticky CTA | Both coexist |
| **11. Exit Intent** | User shows exit behavior | No capture → lead lost | Exit-popup with email capture | 10-15% recovery |
| **12. Wizard Start** | User clicks CTA, enters wizard | Wizard perceived as long form | Progress bar, 5 steps, auto-save | -35% abandonment |

### 4.3 Mobile CTA Placement Matrix

| CTA Type | Position | Behavior | Z-Index | Size |
|----------|----------|----------|---------|------|
| Primary (Sticky) | Fixed bottom, 0px from edge | Always visible | 1000 | 56px height, 100% width |
| Chat Widget | Fixed, bottom-right, 80px from bottom | Tap to open | 999 | 60×60px circle |
| Hero CTA | Inline, below hero text | Scrolls with content | auto | 48px height |
| Final CTA Block | End of content, full-width | Static position | auto | 56px height |
| Exit-Intent Modal | Center screen, overlay | Triggered by exit | 1001 | 90% width, max 400px |

### 4.4 Mobile Drop-Off Recovery

| Drop-Off Point | % Users Lost | Recovery Mechanism | Recovery Rate |
|----------------|--------------|-------------------|---------------|
| Hero section (no scroll) | 25% | Exit-intent capture, strong H1, immediate value | 10-15% |
| After Problem Cards | 15% | Clear transition to Solution, micro-commitment | 5-8% |
| Product Details section | 10% | Accordion format, benefit-first presentation | 3-5% |
| Before Final CTA | 10% | Sticky CTA always visible, urgency messaging | 5-7% |
| Wizard Step 1 | 20% | Progress bar, "Save & Continue" after Step 2 | 8-12% |
| Wizard Step 2-3 | 15% | Auto-save, email resume link, exit popup | 5-8% |
| Wizard Step 4-5 | 10% | Minimal fields, pre-selection from entry page | 3-5% |

### 4.5 Mobile Performance Requirements

| Metric | Target | Implementation |
|--------|--------|----------------|
| LCP (Largest Contentful Paint) | < 2.5s | Hero image WebP <150KB, priority loading |
| FID (First Input Delay) | < 100ms | Defer non-critical JavaScript |
| CLS (Cumulative Layout Shift) | < 0.1 | Reserve space for images, avoid layout shifts |
| TTI (Time to Interactive) | < 3.8s | Lazy-load below-fold content |
| Mobile Font Size | ≥ 16px body | Prevent iOS zoom on focus |

---

## SECTION 5 — System Performance Metrics

### 5.1 Key Performance Indicators

| Metric | Current Baseline | Target (3 months) | Target (6 months) |
|--------|------------------|-------------------|-------------------|
| Site Conversion Rate | 2.5% | 3.5% | 4.5% |
| Wizard Completion Rate | 45% | 60% | 70% |
| Mobile Conversion Parity | 70% of desktop | 90% | 100% |
| Qualified Leads/Month | 10 | 20 | 35 |
| Time to Decision (avg) | 8 min | 5 min | 4 min |
| Exit-Intent Recovery | 0% | 10% | 15% |
| Featured Snippet Wins | 0 | 5 | 15 |
| AI Citation Rate | 0% | 30% | 60% |

### 5.2 Attribution Tracking

All traffic sources must be tracked with UTM parameters:

| Source | UTM Source | UTM Medium | UTM Campaign |
|--------|------------|------------|--------------|
| Google Ads | google | cpc | [campaign_name] |
| LinkedIn Ads | linkedin | paid | [campaign_name] |
| Retargeting | google/facebook | retargeting | [audience_name] |
| Email Outreach | email | outbound | [campaign_name] |
| Organic SEO | google | organic | — |
| AI Search | chatgpt/perplexity/gemini | ai_search | — |
| Direct | direct | direct | — |
| Referral | [referrer_domain] | referral | — |

### 5.3 A/B Testing Priority

| Test | Hypothesis | Expected Lift | Priority |
|------|------------|---------------|----------|
| Hero CTA Text | "See Your Timeline & Price" vs "Start Your Project" | +15% CTR | P0 |
| Sticky CTA Position | Bottom vs Bottom-Right floating | +10% clicks | P0 |
| Exit-Intent Timing | 30s vs 50% scroll vs both | +5% recovery | P1 |
| FAQ Position | Mid-page vs End of page | +8% engagement | P1 |
| Wizard Step Count | 5 steps vs 7 steps | +20% completion | P1 |

---

## SECTION 6 — Implementation Checklist

### Phase 1: Foundation (Week 1)

- [ ] Implement sticky mobile CTA on all conversion pages
- [ ] Add chat widget with proper z-index and positioning
- [ ] Configure exit-intent popup on all pages except wizard
- [ ] Implement UTM tracking on all CTA buttons
- [ ] Set up Google Analytics 4 events for wizard steps

### Phase 2: SEO/AI Optimization (Week 2-3)

- [ ] Add Answer Blocks to all 27 pages
- [ ] Implement FAQPage schema on FAQ page
- [ ] Implement HowTo schema on Start a Project page
- [ ] Add H2 questions to all major sections
- [ ] Verify internal linking matches pillar-cluster architecture

### Phase 3: Mobile Optimization (Week 3-4)

- [ ] Optimize all hero images for mobile (WebP, <150KB)
- [ ] Convert product tables to accordion format on mobile
- [ ] Implement collapsible FAQ accordion
- [ ] Add progress bar to wizard
- [ ] Enable auto-save on wizard after Step 2

### Phase 4: Testing & Iteration (Week 5-6)

- [ ] Run A/B test on hero CTA text
- [ ] Test exit-intent timing variations
- [ ] Monitor mobile vs desktop conversion parity
- [ ] Track featured snippet acquisitions
- [ ] Measure AI citation rate via manual checks

---

## SECTION 7 — Document Certification

| Property | Value |
|----------|-------|
| **Document ID** | SYSTEM-OPT-V1.0 |
| **Domain** | hilomirrors.com |
| **Version** | 1.0 |
| **Status** | COMPLETE |
| **Dependencies** | PROD-001 through PROD-007 (All Locked) |
| **Next Review** | Post-launch + 30 days |

---

*Document generated by Senior Conversion Architect*  
*Based on analysis of 13 strategic documents + 5 research queries*
