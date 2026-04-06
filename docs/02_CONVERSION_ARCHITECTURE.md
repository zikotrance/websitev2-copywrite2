# CONVERSION ARCHITECTURE — HILO Website Project

**Gate**: 2 — Conversion Architecture
**Status**: DRAFT — Owner validation required
**Created**: 2026-04-07
**Created by**: Senior Conversion Architect (GLM)
**Governing Document**: docs/00_MASTER_SYSTEM.md (v1.2)
**Companion**: docs/01_WORKPROGRESS.md

---

## 1. Executive Summary

### What Gate 2 Solves

Gate 1 established the rules. Gate 2 builds the blueprint. This document defines the **complete structural architecture** of the HILO website — every page, every navigation path, every conversion flow, and every relationship between page families. It converts the Master System's strategic doctrine into an actionable site map and execution plan.

### What Is Being Decided Now

- Final sitemap with every page the site will contain at launch
- Primary, secondary, and footer navigation structure
- Page family map defining each page's conversion role
- Disposition of every existing content file (keep, merge, split, rename, remove, or defer)
- Missing pages justified by conversion value
- Complete CTA flow architecture across all page families
- Rules for hierarchy, naming, and page creation
- Production sequence for Gate 3 (page models) and Gate 4 (content production)

### What Remains Blocked

- **Page content writing** — no final copy may be produced until Gate 3 validates page models
- **Code, build, or deployment** — not actionable until Gate 5
- **Pricing data** — placeholder values require owner input (cannot be fabricated)
- **Product naming reconciliation** — existing catalog files use inconsistent product names that require owner arbitration (see Section 6)
- **New industry page decisions** — mixed-use and commercial office require owner direction

---

## 2. Current-State Audit of Site Structure

### 2.1 Repository Content Inventory

| Page Family | Files | Existing Pages | Assessment |
|-------------|-------|----------------|------------|
| Homepage | 1 | 01_HOMEPAGE.md | Structure sound, content comprehensive. H1 is metadata not a page headline. French metadata mixed with English content. |
| Industries | 3 | Hotels, Real Estate, Senior Living | Consistent template structure. All critically thin (~470-500 words). Fail Section I.0.2 depth tests. No cross-linking between industry pages. |
| Solutions | 6 | LED, Smart, Cabinets, Shower, Arch Glass, Standard | Good to strong depth (1,472-2,435 words). All 7 HILO criteria addressed. No cross-linking to /industries/ pages. No case study blocks. "See All Products" CTA has no target path. |
| Case Studies | 6 | Index + 5 individual studies | Consistent structure. Adequate depth. No cross-linking between studies. CTA link targets unspecified. |
| Support | 6 | About, Contact, FAQ, Warranty, Shipping, Returns | Mixed quality. Contact page thin (709 words). Heavy content overlap between Warranty and Returns. Placeholder phone/address data throughout. |
| Wizard | 1 | 23_WIZARD-ESTIMATE.md | Comprehensive specification (5,926 words). French metadata. Step count inconsistency (8 vs 9). Technical spec document, not a content page. |
| Catalog (LED) | 4 | Files 31-34 | Multi-product bundles (4-5 products per file). Filenames reference WRONG product names. No parent catalogue links. No breadcrumb navigation. French metadata + HTML template code mixed in. |
| Catalog (Smart) | 4 | Files 41-44 | Same issues as LED. Filenames reference "NEXA" brand names but content uses different names (INTELLI, GENIUS, etc.). Chinese text leak in file 43. |
| Catalog (Cabinet) | 1 | File 51 | Multi-product bundle (5 products). Filename references "RITUAL" brand but content uses different names (ESSENTIAL, DELUXE, etc.). |
| Catalog (Shower) | 0 | — | No catalog or product detail files exist. Solution page is dead-end. |
| Catalog (Arch Glass) | 0 | — | No catalog or product detail files exist. Solution page is dead-end. |
| Catalog (Standard) | 0 | — | No catalog or product detail files exist. Solution page is dead-end. |

### 2.2 Structural Strengths

1. **Solution pages are well-crafted** — all 6 follow consistent structure, address all 7 HILO criteria, and provide substantive depth appropriate to their conversion role.
2. **Trust Line is present on every page** — consistent deployment across all content files.
3. **Case studies follow a consistent narrative structure** — project overview, challenge, solution, results, testimonial format.
4. **Industry pages follow a consistent template** — hero, 7 advantages, recommended products, case study, FAQ, CTA. Template is correct; execution is thin.
5. **Wizard specification is comprehensive** — detailed step-by-step flow with psychological mechanics and UX writing.
6. **Homepage is strong** — broad value proposition coverage, multiple CTAs, multiple persona relevance.

### 2.3 Structural Weaknesses

1. **No catalogue listing pages exist** — The Master defines a 3-level product hierarchy (Solution → Catalog → Product Detail), but NO catalogue listing pages exist. The 9 existing catalog files are multi-product bundles, not catalogue pages. The primary CTA on every solution page ("See Our Products → /solutions/[category]/catalogue") leads to a dead end.

2. **No individual product detail pages exist** — All 9 catalog files contain 4-5 products bundled together. The Master defines product detail pages at `/solutions/[slug]/catalogue/[product-slug]`, but these do not exist as individual pages.

3. **Three solution categories are dead-ends** — Shower Glass, Architectural Glass, and Standard Mirrors have solution pages but zero catalog or product content. A buyer reaching these pages has no product pages to navigate to.

4. **Zero cross-linking between /industries/ and /solutions/** — These page families are completely siloed. An industry page visitor cannot discover relevant solutions, and a solution page visitor cannot see industry-specific relevance.

5. **Catalog filenames are systematically wrong** — Every catalog file references product names that don't match their content. LED files reference "ILLUMA", smart files reference "NEXA", cabinet file references "RITUAL", but the actual content uses different product names (FLEUVE, INTELLI, GENIUS, ESSENTIAL, etc.).

6. **French metadata leakage** — 12 of 35 content files contain French labels ("Titre", "Projet", "Statut", "LIVRABLE", "Table des Matières") that are collaboration artifacts, not website content.

7. **Placeholder data throughout** — Phone numbers ("1-800-HILO-XXX"), addresses ("[Street Address]"), pricing ("$XXX", "$XX"), and CTA link targets are unresolved.

8. **Content overlap between Warranty and Returns pages** — Claims process content is duplicated almost verbatim between files 20 and 22.

### 2.4 Obvious Redundancies

| Redundancy | Location | Impact |
|------------|----------|--------|
| Claims process duplicated | 20_SUPPORT-WARRANTY.md (Section 4) + 22_SUPPORT-RETURNS.md (Section 3-4) | Maintenance burden, user confusion if content diverges |
| FAQ content overlaps with support pages | 19_SUPPORT-FAQ.md overlaps with Warranty, Shipping, Returns | Same answers in multiple places |
| Phone placeholder repeated | 9 files | Must be updated everywhere when real number is available |
| Product data in catalog bundles vs. product detail pages | Catalog files contain full product specs that should live on individual product pages | Will need reconciliation when individual pages are created |

### 2.5 Structural Contradictions

| Contradiction | Detail |
|--------------|--------|
| Master defines catalogue pages at depth 2, but none exist | `/solutions/[slug]/catalogue` is referenced in CTAs but has no content file |
| Master defines product detail pages at depth 3, but none exist | `/solutions/[slug]/catalogue/[product-slug]` is referenced but has no content file |
| Wizard spec says "8 steps" but flow shows 9 | Step count inconsistency between rationale table and detailed flow |
| Master says "Industries" in nav, but no mixed-use or commercial office pages | About page references these verticals but no dedicated pages exist |

---

## 3. Final Recommended Sitemap

```
FINAL HILO WEBSITE SITEMAP
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

L0: HOMEPAGE                                    /
│
├── L1: SOLUTIONS                               /solutions/
│   ├── LED Mirrors                             /solutions/led-mirrors
│   │   └── Catalogue                           /solutions/led-mirrors/catalogue
│   │       └── Product Detail ×N               /solutions/led-mirrors/catalogue/[slug]
│   ├── Smart Mirrors                           /solutions/smart-mirrors
│   │   └── Catalogue                           /solutions/smart-mirrors/catalogue
│   │       └── Product Detail ×N               /solutions/smart-mirrors/catalogue/[slug]
│   ├── Medicine Cabinets                       /solutions/medicine-cabinets
│   │   └── Catalogue                           /solutions/medicine-cabinets/catalogue
│   │       └── Product Detail ×N               /solutions/medicine-cabinets/catalogue/[slug]
│   ├── Shower Glass                            /solutions/shower-glass
│   │   └── Catalogue                           /solutions/shower-glass/catalogue
│   │       └── Product Detail ×N               /solutions/shower-glass/catalogue/[slug]
│   ├── Architectural Glass                     /solutions/architectural-glass
│   │   └── Catalogue                           /solutions/architectural-glass/catalogue
│   │       └── Product Detail ×N               /solutions/architectural-glass/catalogue/[slug]
│   └── Standard Mirrors                        /solutions/standard-mirrors
│       └── Catalogue                           /solutions/standard-mirrors/catalogue
│           └── Product Detail ×N               /solutions/standard-mirrors/catalogue/[slug]
│
├── L1: INDUSTRIES                              /industries/
│   ├── Hotels                                 /industries/hotels
│   ├── Real Estate                            /industries/real-estate
│   └── Senior Living                          /industries/senior-living
│
├── L1: CASE STUDIES                            /case-studies
│   ├── Index                                  /case-studies
│   ├── Hotel Chain Rollup                     /case-studies/hotel-chain-rollup
│   ├── Multi-Family Development               /case-studies/multi-family
│   ├── Senior Living Facility                 /case-studies/senior-living
│   ├── Mixed-Use Development                  /case-studies/mixed-use
│   └── Boutique Hotel Renovation              /case-studies/boutique-hotel
│
├── L1: ESTIMATE                                /estimate
│   └── (Multi-step wizard — single URL with client-side routing)
│
└── L1: SUPPORT                                 /
    ├── About                                  /about
    ├── Contact                                /contact
    ├── FAQ                                    /faq
    ├── Warranty                               /warranty
    ├── Shipping                               /shipping
    └── Returns                                /returns

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

PAGE COUNT SUMMARY:
┌─────────────────────────────────┬───────────┬────────────┐
│ Page Type                       │ Count     │ Status     │
├─────────────────────────────────┼───────────┼────────────┤
│ Homepage                        │ 1         │ EXISTS     │
│ Solution overview pages         │ 6         │ EXISTS     │
│ Catalogue listing pages         │ 6         │ CREATE     │
│ Product detail pages            │ TBD       │ CREATE     │
│ Industry pages                  │ 3         │ EXISTS     │
│ Case study index                │ 1         │ EXISTS     │
│ Case study pages                │ 5         │ EXISTS     │
│ Wizard / Estimate               │ 1         │ EXISTS     │
│ Support pages                   │ 6         │ EXISTS     │
├─────────────────────────────────┼───────────┼────────────┤
│ TOTAL DEFINED PAGES             │ 28+       │            │
│ PAGES TO CREATE                 │ 6+TBD     │            │
│ PAGES EXISTING                  │ 28        │            │
└─────────────────────────────────┴───────────┴────────────┘

MAXIMUM DEPTH: 4 levels (Homepage → Solutions → Catalogue → Product Detail)
             ↳ 3 levels (Homepage → Industries → Industry Page)
             ↳ 3 levels (Homepage → Case Studies → Individual Study)
```

### 3.1 Sitemap Decisions vs. Master Section H.1

The sitemap above is **fully consistent** with the Master's information architecture (Section H.1). No pages were added, removed, or relocated from the Master's hierarchy. The key gap this sitemap exposes is that the Master's hierarchy assumes catalogue listing pages and product detail pages exist, but they have never been created. This is the single largest structural deficit in the current repository.

### 3.2 Pages Explicitly NOT Recommended

| Page Considered | Decision | Rationale |
|----------------|----------|-----------|
| Mixed-Use industry page | **DEFER** | Mixed-use case study exists but a dedicated industry page requires industry-specific content, proof, and buyer persona work. Not justified until core pages are production-ready. |
| Commercial Office industry page | **DEFER** | Referenced in About page but no case study, no buyer persona work, and no commercial office specific proof exists. Premature to create. |
| Blog / Resources section | **DEFER** | Content marketing capability. Does not serve the immediate conversion goal. Revisit post-launch. |
| Individual product comparison pages | **NOT RECOMMENDED** | Product comparison is handled within catalog listing pages via grid/table UI. Separate comparison pages add depth without conversion value. |
| Installation services page | **MERGE INTO SUPPORT** | Installation is covered in solution pages (Criterion #7) and could have a dedicated section within /about or /shipping. Does not warrant its own page. |
| Pricing page | **NOT RECOMMENDED** | Pricing is handled through the wizard/estimation tool and within catalog/product pages. A standalone pricing page would either duplicate wizard content or be too vague for B2B custom pricing. |

---

## 4. Primary Navigation

### 4.1 Top Navigation Bar

```
╔══════════════════════════════════════════════════════════════════════════╗
║  HILO (logo)                                                    [Get Instant AI Estimate →]  ║
╠══════════════════════════════════════════════════════════════════════════╣
║  Solutions ▾    Industries ▾    Case Studies    About    Contact       ║
╚══════════════════════════════════════════════════════════════════════════╝
```

| Position | Item | Type | URL | Notes |
|----------|------|------|-----|-------|
| Left | HILO (logo) | Logo/Brand | `/` | Links to homepage |
| Center-left | Solutions | Dropdown | `/solutions/` | 6 solution categories in mega-menu |
| Center | Industries | Dropdown | `/industries/` | 3 industry pages in dropdown |
| Center-right | Case Studies | Link | `/case-studies` | No dropdown — index page handles navigation |
| Right | About | Link | `/about` | Support page |
| Far-right | Contact | Link | `/contact` | Support page |
| Far-right (CTA) | Get Instant AI Estimate | Button | `/estimate` | Always visible. Highest visual prominence. NOT a nav item — a conversion button. |

**Total nav items: 5 + 1 CTA button.** The Master specifies 7 top-level items. This recommendation reduces to 5 nav links + 1 persistent CTA button for the following reasons:

1. **Estimate moves from nav item to CTA button** — The wizard is the primary conversion mechanism. Burying it as a nav item reduces its visibility. A persistent CTA button in the nav bar ensures it's always one click away.
2. **FAQ removed from top nav** — FAQ content is anxiety-reduction, not navigation. It belongs in the footer and is reachable from relevant support pages. Adding it to the top nav dilutes the conversion-focused navigation.
3. **Fewer items = faster decisions** — B2B buyers scanning the nav should see 5 clear paths, not 7. The CTA button handles the most important action separately.

**This navigation change requires owner validation** — the Master Section H.2 specifies 7 items including Estimate and FAQ. This recommendation deviates. Owner approval required.

### 4.2 Solutions Mega-Menu

When the user hovers or clicks "Solutions", a mega-menu panel opens displaying all 6 solution categories in a 2×3 or 3×2 grid:

```
┌──────────────────────────────────────────────────────────────────┐
│  LED Mirrors          Smart Mirrors        Medicine Cabinets      │
│  Engineered for       Touchscreen &        Storage solutions      │
│  commercial           PMS-integrated       for hospitality        │
│  reliability          smart mirrors        & residential         │
│                                                                  │
│  Shower Glass         Architectural Glass   Standard Mirrors      │
│  Frameless &          Custom specifications Wall, vanity,         │
│  semi-frameless       for commercial       gym & custom          │
│  enclosures           projects             dimensions            │
│                                                                  │
│  [Get Your Instant AI Estimate →]                                  │
└──────────────────────────────────────────────────────────────────┘
```

Each category tile shows: product name, 1-line description, and links to `/solutions/[slug]`.

The CTA at the bottom of the mega-menu reinforces the primary conversion path.

### 4.3 Industries Dropdown

```
┌──────────────────────────────────────────────────┐
│  Hotels & Hospitality                            │
│  Real Estate Developers                          │
│  Senior Living Facilities                        │
└──────────────────────────────────────────────────┘
```

Simple dropdown. Each item links to `/industries/[slug]`.

### 4.4 Footer Navigation

```
┌──────────────────────────────────────────────────────────────────┐
│ HILO                                                            │
│                                                                  │
│  SOLUTIONS              INDUSTRIES           SUPPORT             │
│  LED Mirrors            Hotels              About                │
│  Smart Mirrors          Real Estate         Contact              │
│  Medicine Cabinets      Senior Living       FAQ                  │
│  Shower Glass                               Warranty             │
│  Architectural Glass                        Shipping             │
│  Standard Mirrors                          Returns              │
│                                                                  │
│  CASE STUDIES              ESTIMATE                                 │
│  All Case Studies          Get Instant AI Estimate                │
│  Hotel Chain Rollup       Book a Call                              │
│  Multi-Family                                                     │
│  Senior Living           🏆 180+ Projects | 🛡️ 5-Year Warranty   │
│  Mixed-Use               🇨🇦 Designed in Canada.                   │
│  Boutique Hotel           Distributed across North America.       │
│                                                                  │
│  © 2026 HILO. All rights reserved.                                │
└──────────────────────────────────────────────────────────────────┘
```

### 4.5 Breadcrumb Navigation

All pages below L1 display breadcrumbs:

| Page Type | Breadcrumb Pattern |
|-----------|-------------------|
| Industry page | Home > Industries > [Industry Name] |
| Solution page | Home > Solutions > [Category Name] |
| Catalogue page | Home > Solutions > [Category] > Catalogue |
| Product detail | Home > Solutions > [Category] > Catalogue > [Product Name] |
| Case study | Home > Case Studies > [Study Name] |
| Support page | Home > [Page Name] |

---

## 5. Page Family Map

### 5.1 Homepage

| Attribute | Value |
|-----------|-------|
| **Route** | `/` |
| **Conversion Role** | Entry point — captures attention, communicates full value proposition, routes visitors to their most relevant next step |
| **Audience Intent** | "I need glass/mirror solutions for my commercial project. Is HILO credible? What do they offer?" |
| **Core CTA Path** | → `/estimate` (primary) or → `/solutions/[category]` (secondary, via solution cards) |
| **Relationships** | Links TO: all 6 solution pages, wizard. Linked FROM: footer of every page, logo. |
| **Persona Reach** | All 3 buyer personas (Developer/PM, Architect/Designer, Facility Manager/GM) |

### 5.2 Solutions

| Attribute | Value |
|-----------|-------|
| **Route** | `/solutions/[slug]` |
| **Conversion Role** | Category evaluation — the most content-heavy conversion page. Buyers compare HILO against alternatives here. |
| **Audience Intent** | "I'm looking at [LED mirrors / smart mirrors / etc.]. Why should I choose HILO? What proof do they have?" |
| **Core CTA Path** | → `/solutions/[slug]/catalogue` (primary) or → `/estimate` (secondary) |
| **Relationships** | Links TO: catalogue page, wizard, related solution pages, relevant industry pages. Linked FROM: homepage, industries, mega-menu. |
| **Persona Reach** | Primary: Developer/PM, Architect/Designer. Secondary: Facility Manager. |
| **Critical Gap** | Links to relevant industry pages are missing. Must be added during content production (G4). |

### 5.3 Catalogue Listing Pages

| Attribute | Value |
|-----------|-------|
| **Route** | `/solutions/[slug]/catalogue` |
| **Conversion Role** | Product comparison — grid-based selection page. Buyers compare products within a category and select one for detailed evaluation. |
| **Audience Intent** | "Show me what HILO offers in this category. Which product fits my project?" |
| **Core CTA Path** | → `/solutions/[slug]/catalogue/[product-slug]` (primary, per product) or → `/estimate` (secondary) |
| **Relationships** | Links TO: product detail pages, wizard. Linked FROM: parent solution page. |
| **Persona Reach** | Product-aware buyers (Level 4-5). |
| **Status** | **DO NOT EXIST. Must be created.** 6 catalogue pages needed. |

### 5.4 Product Detail Pages

| Attribute | Value |
|-----------|-------|
| **Route** | `/solutions/[slug]/catalogue/[product-slug]` |
| **Conversion Role** | Conversion-ready — the last content stop before the wizard. Provides full specifications, pricing, and trust reinforcement. |
| **Audience Intent** | "This is the product I want. Give me the specs, pricing, and let me get a quote." |
| **Core CTA Path** | → `/estimate` (pre-filled with product selection) (primary) or → `/contact` (secondary) |
| **Relationships** | Links TO: wizard, related products (cross-sell), parent catalogue page. Linked FROM: parent catalogue page, solution page. |
| **Persona Reach** | Most-aware buyers ready to act (Level 5). |
| **Status** | **DO NOT EXIST. Must be created.** Exact count depends on owner's product catalog decisions. |

### 5.5 Industries

| Attribute | Value |
|-----------|-------|
| **Route** | `/industries/[slug]` |
| **Conversion Role** | Audience segmentation — proves HILO understands the visitor's specific industry. Drives to wizard. |
| **Audience Intent** | "I work in [hotels / real estate / senior living]. Does HILO have experience in my sector?" |
| **Core CTA Path** | → `/estimate` (primary) or → `/contact` (secondary) |
| **Relationships** | Links TO: relevant solution pages, relevant case studies, wizard. Linked FROM: homepage, industries dropdown, mega-menu. |
| **Persona Reach** | Industry-specific: Hotel GMs, Real Estate developers, Senior Living operators. |
| **Critical Gap** | No cross-linking to solution pages currently. Must be added. Also, case study links have no targets. |

### 5.6 Case Studies

| Attribute | Value |
|-----------|-------|
| **Route** | `/case-studies` (index), `/case-studies/[slug]` (individual) |
| **Conversion Role** | Social proof — provides narrative evidence that HILO delivers on its promises. Supports conversion on referring pages. |
| **Audience Intent** | "Show me proof that HILO can deliver for a project like mine." |
| **Core CTA Path** | → `/estimate` (primary, "Start Your Project") or → `/case-studies` (secondary, "View All Case Studies") |
| **Relationships** | Links TO: wizard, related solution pages, related industry pages. Linked FROM: homepage, solution pages, industry pages, case study index. |
| **Persona Reach** | Product-aware to Most-aware buyers (Level 4-5). |

### 5.7 Support Pages

| Attribute | Value |
|-----------|-------|
| **Route** | `/about`, `/contact`, `/faq`, `/warranty`, `/shipping`, `/returns` |
| **Conversion Role** | Anxiety reduction — answers objections, resolves uncertainties, supports conversion indirectly. |
| **Audience Intent** | "I have a specific question about warranty / shipping / returns / pricing." or "Who is HILO?" |
| **Core CTA Path** | → `/estimate` (primary) or → `/contact` (secondary) |
| **Relationships** | Links TO: wizard, relevant solution pages. Linked FROM: footer, nav. |
| **Persona Reach** | All awareness levels (2-5). Often anxiety-driven visits. |
| **Internal Relationship** | FAQ overlaps with Warranty, Shipping, Returns. Content should be consolidated: FAQ answers link to dedicated support pages rather than duplicating content. |

### 5.8 Estimate / Wizard

| Attribute | Value |
|-----------|-------|
| **Route** | `/estimate` |
| **Conversion Role** | Primary conversion mechanism — captures qualified lead information in exchange for an AI-powered estimate. |
| **Audience Intent** | "I want to know how much this will cost for my project. Give me an estimate." |
| **Core CTA Path** | Internal multi-step flow → lead capture form → submission |
| **Relationships** | Linked FROM: every page on the site (primary CTA). Links TO: none (terminal conversion point). |
| **Persona Reach** | All personas at any awareness level — this is the universal conversion path. |

---

## 6. Existing-Page Disposition Matrix

### 6.1 Homepage

| File | Disposition | Rationale |
|------|-------------|-----------|
| 01_HOMEPAGE.md | **KEEP — REWRITE** | Structure and content breadth are sound. Must be rewritten to: (1) fix H1 which is currently document metadata, (2) remove French sections, (3) remove strategy/analysis content that is not page copy, (4) add cross-links to industry pages, (5) ensure all CTAs have valid targets. |

### 6.2 Industry Pages

| File | Disposition | Rationale |
|------|-------------|-----------|
| 02_INDUSTRIES-HOTELS.md | **KEEP — REWRITE** | Template structure is correct (hero, 7 advantages, products, case study, FAQ, CTA). Content is critically thin (~499 words). Must be expanded with industry-specific depth, objection handling, and proof per Section I.0. Must add cross-links to solution pages and target case study URL. |
| 03_INDUSTRIES-REAL-ESTATE.md | **KEEP — REWRITE** | Same assessment as Hotels. Must expand and add cross-linking. |
| 04_INDUSTRIES-SENIOR-LIVING.md | **KEEP — REWRITE** | Same assessment as Hotels. Additionally, the "Château Frontenac" case study reference should be fact-checked — Château Frontenac is a famous Quebec hotel, not a senior living facility. |

### 6.3 Solution Pages

| File | Disposition | Rationale |
|------|-------------|-----------|
| 05_SOLUTIONS-LED-MIRRORS.md | **KEEP — REVISION** | Good depth and structure. Must: (1) add cross-links to relevant industry pages, (2) add case study or social proof block, (3) add link targets to "See All Products" CTA, (4) resolve pricing placeholders. |
| 06_SOLUTIONS-SMART-MIRRORS.md | **KEEP — REVISION** | Good depth. 8 sections may be slightly long — consider consolidating Sections 2 and 3 (Features + Pricing). Same cross-link and CTA target issues. |
| 07_SOLUTIONS-MEDICINE-CABINETS.md | **KEEP — REVISION** | Good depth. Same cross-link and CTA target issues. |
| 08_SOLUTIONS-SHOWER-GLASS.md | **KEEP — REVISION** | Strong depth. Same cross-link and CTA target issues. |
| 09_SOLUTIONS-ARCHITECTURAL-GLASS.md | **KEEP — REVISION** | Strongest solution page but longest (9 sections + subsections). Consider consolidating to reduce scroll depth while maintaining proof density. |
| 10_SOLUTIONS-STANDARD-MIRRORS.md | **KEEP — REVISION** | Good depth. Trust Line missing from body copy (only in hero/footer). Add reinforcement in body. |

### 6.4 Case Studies

| File | Disposition | Rationale |
|------|-------------|-----------|
| 11_CASE-STUDIES-INDEX.md | **KEEP — REVISION** | Adequate structure. Must: (1) add actual link targets to case study cards, (2) add industry filter links, (3) remove French "SECONDAIRE" label, (4) remove duplicate Trust Line. |
| 12_CASE-STUDIES-HOTEL-ROLLUP.md | **KEEP — REVISION** | Adequate depth and consistent structure. Must add: (1) cross-links to other case studies, (2) link target for "View All Case Studies", (3) link targets for "Book a Call". |
| 13_CASE-STUDIES-MULTI-FAMILY.md | **KEEP — REVISION** | Same as Hotel Rollup. |
| 14_CASE-STUDIES-SENIOR-LIVING.md | **KEEP — REVISION** | Same as Hotel Rollup. |
| 15_CASE-STUDIES-MIXED-USE.md | **KEEP — REVISION** | Same as Hotel Rollup. Additionally, verify #railings fragment link target. |
| 16_CASE-STUDIES-BOUTIQUE-HOTEL.md | **KEEP — REVISION** | Same as Hotel Rollup. |

### 6.5 Support Pages

| File | Disposition | Rationale |
|------|-------------|-----------|
| 17_SUPPORT-ABOUT.md | **KEEP — REVISION** | Good structure. Must: (1) add actual link targets to industries and solutions sections, (2) add CTA link targets, (3) remove French "Titre" labels. |
| 18_SUPPORT-CONTACT.md | **KEEP — REWRITE** | Thin (709 words). Must be expanded to cover: contact form specification, booking process, office location details, and clearer CTA paths. Phone/address placeholders must be resolved by owner. |
| 19_SUPPORT-FAQ.md | **KEEP — REVISION** | Good content coverage. Must: (1) add in-page anchor navigation, (2) add link targets to CTAs, (3) resolve phone placeholder, (4) ensure answers link to dedicated support pages rather than duplicating content. |
| 20_SUPPORT-WARRANTY.md | **KEEP — REVISION** | Adequate structure. Must: (1) remove French "Titre" labels, (2) resolve phone placeholder, (3) add link target for "Download Warranty PDF", (4) coordinate claims content with Returns page to eliminate duplication. |
| 21_SUPPORT-SHIPPING.md | **KEEP — REVISION** | Adequate structure. Must: (1) remove French "Titre" labels, (2) resolve phone placeholder, (3) define "Track Order" action. |
| 22_SUPPORT-RETURNS.md | **KEEP — MERGE with Warranty** | Heavy content overlap with Warranty page (claims process duplicated). Recommendation: **consolidate claims process into Warranty page**. Returns page should focus exclusively on: return eligibility, return initiation, shipping costs for returns, refund/replacement process. Claims (warranty-related) should link to Warranty page. This reduces content duplication and simplifies maintenance. |

### 6.6 Wizard

| File | Disposition | Rationale |
|------|-------------|-----------|
| 23_WIZARD-ESTIMATE.md | **KEEP — REVISION** | Comprehensive specification. Must: (1) reconcile step count (8 vs 9), (2) remove French metadata, (3) resolve phone placeholder, (4) confirm URL structure matches final routing decisions. This is a technical specification document — it should be preserved as-is for developer reference during Gate 5, but the actual wizard page content will be built from this spec. |

### 6.7 Catalog Files (Critical Disposition)

All 9 existing catalog files share the same structural issues: multi-product bundles with wrong filenames, no parent catalogue links, and French metadata leakage. The disposition is consistent across all:

| File | Disposition | Rationale |
|------|-------------|-----------|
| 31_CATALOG-LED-FLEUVE-ONE-PLUS.md | **SPLIT → individual product detail pages** | Contains 5 products (One, Plus, Pro, Ultra, Round) but filename references only 2. Must be split into 5 individual product detail pages + product data used to build the LED catalogue listing page. |
| 32_CATALOG-LED-FLEUVE-PRO-ULTRA.md | **SPLIT → individual product detail pages** | Contains 5 products (Pure, Rise, Pan, Tilt, Star). Filename references wrong products. Same treatment as file 31. |
| 33_CATALOG-LED-FLEUVE-ROUND-ILLUMA.md | **SPLIT → individual product detail pages** | Contains 4 products (Spa, Grand, Frame, Layer). Filename references wrong products. Same treatment. |
| 34_CATALOG-LED-ILLUMA-PLUS-PRO.md | **SPLIT → individual product detail pages** | Contains 4 products (Modular, Color, Deep, Sense). Filename references wrong products. Same treatment. |
| 41_CATALOG-SMART-NEXA-ONE-PLUS.md | **SPLIT → individual product detail pages** | Contains 5 products (INTELLI, CONNECT, VUE, AURA SMART, HUB). Filename references "NEXA" brand that doesn't exist in content. Same treatment. |
| 42_CATALOG-SMART-NEXA-PRO-HOTEL.md | **SPLIT → individual product detail pages** | Contains 5 products (GENIUS, SYNC, MIRROR AI, STREAM, PIVOT). Same issues. |
| 43_CATALOG-SMART-NEXA-SUITE-ROUND.md | **SPLIT → individual product detail pages** | Contains 5 products (CLARITY SMART, MINI SMART, DUAL, SENSORY, BASIC SMART). Same issues. Also contains Chinese text leak that must be removed. |
| 44_CATALOG-SMART-NEXA-CUSTOM-INTEGRATION.md | **SPLIT → individual product detail pages** | Contains 5 products (MIRROR LITE, CONFERENCE, RETAIL, FAMILY, PRO SMART). Same issues. Also has 7-year warranty reference inconsistent with standard 5-year. |
| 51_CATALOG-CABINET-RITUAL-SERIES.md | **SPLIT → individual product detail pages** | Contains 5 products (ESSENTIAL, DELUXE, RECESS, SURFACE, CORNER). References 5 additional products (DOUBLE, TRIPLE, MIRROR CAB, STORAGE PRO, SLIM) in a "Next Steps" section that don't have a file. |

### 6.8 Legacy Files

| File | Disposition | Rationale |
|------|-------------|-----------|
| 00_MASTER-GUIDELINES.md | **REMOVE — ARCHIVE** | Superseded by docs/00_MASTER_SYSTEM.md. Has no role in the final architecture. Should be moved to docs/archive/ or deleted. |

### 6.9 Disposition Summary

| Disposition | Count | Files |
|-------------|-------|-------|
| **KEEP — REVISION** | 20 | 05-10 (solutions), 11-16 (case studies), 17, 19-21 (support), 23 (wizard) |
| **KEEP — REWRITE** | 5 | 01 (homepage), 02-04 (industries), 18 (contact) |
| **SPLIT → new pages** | 9 | 31-34, 41-44, 51 (catalog bundles → individual product pages) |
| **MERGE** | 1 | 22 (Returns) — claims content merged into 20 (Warranty) |
| **CREATE** | 6 | Catalogue listing pages for all 6 solution categories |
| **CREATE** | ~38 | Individual product detail pages (extracted from catalog bundles) |
| **REMOVE** | 1 | 00_MASTER-GUIDELINES.md (archive) |
| **DEFER** | 2 | Mixed-use industry page, Commercial office industry page |

---

## 7. Missing Pages / Recommended Additions

### 7.1 P0 — Must Create Before Production (Conversion Blockers)

| Page | Route | Purpose | Justification |
|------|-------|---------|---------------|
| LED Mirrors Catalogue | `/solutions/led-mirrors/catalogue` | Grid-based product comparison page for LED mirror category | **Conversion blocker.** Solution page primary CTA ("See Our Products") links here. Without this page, the primary CTA on the highest-traffic solution category is a dead end. |
| Smart Mirrors Catalogue | `/solutions/smart-mirrors/catalogue` | Grid-based product comparison page for smart mirror category | Same blocker logic as LED. |
| Medicine Cabinets Catalogue | `/solutions/medicine-cabinets/catalogue` | Grid-based product comparison page for medicine cabinet category | Same blocker logic. |
| Shower Glass Catalogue | `/solutions/shower-glass/catalogue` | Product overview for shower glass category | **Conversion blocker + content gap.** No catalog content exists at all. Solution page has no product pages to link to. |
| Architectural Glass Catalogue | `/solutions/architectural-glass/catalogue` | Product overview for architectural glass category | Same blocker logic. |
| Standard Mirrors Catalogue | `/solutions/standard-mirrors/catalogue` | Product overview for standard mirror category | Same blocker logic. |

### 7.2 P0 — Must Create (Product Detail Pages)

Individual product detail pages must be extracted from the 9 existing catalog bundle files. The exact count depends on owner's product catalog decisions, but based on existing content:

| Category | Products Identified in Existing Files | Product Detail Pages Needed |
|----------|---------------------------------------|---------------------------|
| LED Mirrors | ~18 products (across files 31-34) | ~18 |
| Smart Mirrors | ~20 products (across files 41-44) | ~20 |
| Medicine Cabinets | ~10 products (file 51 + 5 unreferenced) | ~10 |
| Shower Glass | 0 products defined | **Owner must define product catalog** |
| Architectural Glass | 0 products defined | **Owner must define product catalog** |
| Standard Mirrors | 0 products defined | **Owner must define product catalog** |

### 7.3 P1 — Recommended (Not Blocking)

No additional pages are recommended at this time. The 6 catalogue listing pages and ~48+ product detail pages represent a significant content production workload. Adding more pages before these are complete would dilute execution quality.

The mixed-use and commercial office industry pages are deferred (Section 3.2) because they lack supporting case studies and industry-specific proof.

---

## 8. CTA Flow Architecture

### 8.1 Primary Conversion Flow (The Happy Path)

```
                    HOMEPAGE
                       │
          ┌────────────┼────────────┐
          ▼            ▼            ▼
    SOLUTIONS    INDUSTRIES    CASE STUDIES
          │            │            │
          ▼            │            │
    CATALOGUE          │            │
          │            │            │
          ▼            │            │
  PRODUCT DETAIL ◄─────┴────────────┘
          │
          ▼
      WIZARD ──→ FORM SUBMISSION ──→ LEAD CAPTURED
```

This is the optimal conversion path: a visitor enters through the homepage or an industry page, evaluates solutions, browses the catalogue, selects a specific product, and enters the wizard with a product pre-selected. This path provides maximum context and trust before the conversion event.

### 8.2 Shortcut Conversion Flow (From Any Page)

```
    ANY PAGE ──→ WIZARD ──→ FORM SUBMISSION ──→ LEAD CAPTURED
```

The "Get Instant AI Estimate" CTA button is available on every page. A visitor who is already convinced can convert from any entry point without navigating through the full evaluation path. This is by design — it captures high-intent visitors who don't need the full evaluation sequence.

### 8.3 Secondary Conversion Flow (Human Interaction)

```
    ANY PAGE ──→ CONTACT ──→ BOOK A CALL FORM ──→ SALES TEAM
```

The "Book a Call" secondary CTA is available on most pages. Some buyers — particularly those with complex custom requirements or enterprise-level projects — need human interaction before converting. This path captures these buyers.

### 8.4 CTA Flow by Page Type

| Source Page | Primary CTA | Primary CTA Target | Secondary CTA | Secondary CTA Target |
|-------------|-------------|-------------------|---------------|---------------------|
| Homepage | Get Instant AI Estimate → | `/estimate` | Book a Call | `/contact` |
| Industry Page | Get Instant AI Estimate → | `/estimate` | Book a Call | `/contact` |
| Solution Page | See Our Products | `/solutions/[slug]/catalogue` | Get AI Estimate | `/estimate` |
| Catalogue Page | Get AI Instant Quote → | `/estimate` (pre-filled) | Book a Call | `/contact` |
| Product Detail | Get AI Instant Quote → | `/estimate` (pre-filled) | Book a Call | `/contact` |
| Case Study Index | Start Your Project → | `/estimate` | Book a Call | `/contact` |
| Case Study | Start Your Project → | `/estimate` | View All Case Studies | `/case-studies` |
| Support Page | Get AI Estimate → | `/estimate` | Contact Us | `/contact` |
| Contact | Submit Message | Form submission | Book a Call | Form section |
| FAQ | Get AI Estimate → | `/estimate` | Contact Support | `/contact` |
| Wizard (final step) | Get My Free Estimate → | Form submission | — | — |

### 8.5 Cross-Linking Requirements

| From | To | Purpose |
|------|----|---------|
| Every solution page | Related industry pages (1-3) | Prove industry-specific relevance |
| Every industry page | Relevant solution pages (3-4) | Connect visitor to product options |
| Every case study | Parent solution page + parent industry page | Provide context and conversion path |
| Every product detail | Parent catalogue page (breadcrumb) | Navigation |
| Every catalogue page | Parent solution page (breadcrumb) | Navigation |
| Homepage | All 6 solution pages | Product range visibility |
| Homepage | 1-2 featured case studies | Social proof at entry |

---

## 9. Navigation and Hierarchy Rules

### 9.1 Maximum Depth

| Rule | Value |
|------|-------|
| Maximum depth from homepage | 4 levels |
| Practical maximum for content-heavy pages | 3 levels (beyond this, visitors lose context) |
| Wizard is an exception | Single URL with client-side routing (no breadcrumb needed) |

### 9.2 When to Create a Child Page

A child page is justified when ALL of the following are true:

1. **The parent page cannot adequately serve the content** — the child page serves a distinct conversion role or audience intent that the parent cannot accommodate without becoming bloated.
2. **The child page has its own CTA hierarchy** — it drives a specific conversion action that differs from or advances the parent's CTA.
3. **The child page is reachable from the parent via a clear, intuitive link** — no visitor should struggle to find it.

Examples of justified child pages:
- `/solutions/led-mirrors` → `/solutions/led-mirrors/catalogue` (different role: evaluation → comparison)
- `/solutions/led-mirrors/catalogue` → `/solutions/led-mirrors/catalogue/fleuve-one` (different role: comparison → conversion-ready detail)

### 9.3 When to Merge Content into a Parent Page

Content should be merged into the parent when ANY of the following are true:

1. **The content is too thin to justify its own page** — it would fail the Section I.0.2 depth insufficiency tests as a standalone page.
2. **The content naturally belongs as a section of the parent** — it is a subsection of the parent's topic, not a distinct topic.
3. **The content exists primarily to support the parent** — it has no independent conversion value.

Examples of content that should NOT be separate pages:
- Individual FAQ answers (belong in /faq)
- Individual warranty terms (belong in /warranty)
- Shipping timelines by region (belong in /shipping)

### 9.4 When NOT to Create a Page

A page should NOT be created when:

1. **The content serves no conversion role** — "nice to have" without buyer journey value.
2. **The page would have fewer than 2 navigation paths to it** — it would be an orphan.
3. **The content could be a section on an existing page** — no justification for a new URL.
4. **The page would only serve SEO purposes** — content marketing pages should be deferred to post-launch.
5. **No case study, proof, or product data exists to support it** — the page would be placeholder content.

### 9.5 Naming and Slug Rules

| Rule | Standard |
|------|----------|
| **Homepage** | `/` |
| **Solution pages** | `/solutions/[kebab-case-slug]` — e.g., `/solutions/led-mirrors` |
| **Catalogue pages** | `/solutions/[slug]/catalogue` — note: "catalogue" (British spelling, matching existing convention and Master Section H.3) |
| **Product detail** | `/solutions/[slug]/catalogue/[product-slug]` — e.g., `/solutions/led-mirrors/catalogue/fleuve-one` |
| **Industry pages** | `/industries/[kebab-case-slug]` — e.g., `/industries/hotels` |
| **Case studies** | `/case-studies/[kebab-case-slug]` — e.g., `/case-studies/hotel-chain-rollup` |
| **Support pages** | `/[kebab-case-slug]` — e.g., `/about`, `/contact`, `/faq`, `/warranty`, `/shipping`, `/returns` |
| **Wizard** | `/estimate` |
| **Case** | Always lowercase, kebab-case, no underscores, no numbers at start |
| **Word separators** | Hyphens only (`-`). No underscores. |

---

## 10. Production Order Recommendation

### 10.1 Gate 3 — Page Models (What to Model First)

Page models define the content structure, block order, and specification for each page type. The order below prioritizes the highest-impact, highest-dependency pages first.

| Sequence | Page Type | Count | Rationale |
|----------|-----------|-------|-----------|
| **3.1** | Solution page model (template) | 1 model | 6 solution pages share the same structure. Modeling one produces the template for all 6. This is the highest-value model because solution pages are the evaluation workhorse. |
| **3.2** | Industry page model (template) | 1 model | 3 industry pages share the same structure. Must be modeled after solution model because industries link to solutions. |
| **3.3** | Case study model (template) | 1 model | 5 case studies share the same structure. Cross-links to solutions and industries. |
| **3.4** | Catalogue listing page model (template) | 1 model | 6 catalogue pages share the same structure. Depends on product data being defined. |
| **3.5** | Product detail page model (template) | 1 model | All product detail pages share the same structure. Depends on catalogue model. |
| **3.6** | Homepage model | 1 model | Homepage aggregates content from all other models. Must be modeled last. |
| **3.7** | Support page models (templates) | 4 models | About, FAQ, Warranty, Contact. Shipping and Returns follow simplified variants of FAQ/Warranty. |
| **3.8** | Wizard model | 1 model | Already extensively specified in file 23. Needs validation and cleanup, not creation. |

### 10.2 Gate 4 — Content Production (What to Write First)

Content production follows the page model sequence, with each family batch-produced after its model is approved.

| Phase | Page Family | Pages | Dependencies | Estimated Turns |
|-------|-------------|-------|-------------|-----------------|
| **P1** | Solution pages (LED, Smart, Cabinets, Shower, Arch Glass, Standard) | 6 | Solution page model approved | 6 turns |
| **P2** | Industry pages (Hotels, Real Estate, Senior Living) | 3 | Industry page model + solution pages approved | 3 turns |
| **P3** | Case studies (all 5) | 5 | Case study model + solution/industry pages approved | 2-3 turns |
| **P4** | Catalogue listing pages (all 6) | 6 | Catalogue model + product data defined | 2-3 turns |
| **P5** | Product detail pages (LED, Smart, Cabinets) | ~48 | Product detail model + catalogue pages approved | 6-8 turns (batch by category) |
| **P6** | Product detail pages (Shower, Arch Glass, Standard) | TBD | Owner must define product catalogs for these 3 categories | TBD |
| **P7** | Homepage | 1 | All other pages approved | 1 turn |
| **P8** | Support pages (About, Contact, FAQ, Warranty, Shipping, Returns) | 6 | Support models approved | 2-3 turns |
| **P9** | Wizard cleanup | 1 | All content approved | 1 turn |
| **P10** | Final QA pass | — | All content approved | 1-2 turns |

### 10.3 Dependency Chain

```
SOLUTION MODEL → Solution Pages → Industry Pages → Case Studies
                                ↓
                        CATALOGUE MODEL → Catalogue Pages → Product Detail Pages
                                                             ↓
                                                         HOMEPAGE
                                                             ↓
                                                        SUPPORT PAGES
                                                             ↓
                                                        WIZARD CLEANUP
                                                             ↓
                                                          FINAL QA
```

### 10.4 Parallelization Opportunities

Within a phase, pages within the same family CAN be produced in parallel (e.g., all 6 solution pages can be written simultaneously once the model is approved). Pages across families should NOT be parallelized because later families depend on earlier families for cross-linking.

---

## 11. Open Architecture Decisions Requiring Owner Validation

| # | Decision | Context | Options | Recommendation | Impact if Deferred |
|---|----------|---------|---------|----------------|-------------------|
| **A1** | Product naming: Which product names are canonical? | Existing catalog files use inconsistent names. Content says "FLEUVE" for LED, "INTELLI/GENIUS" for Smart, "ESSENTIAL/DELUXE" for Cabinets. Filenames reference "ILLUMA", "NEXA", "RITUAL". | (a) Content names are canonical, filenames are legacy. (b) Filename names are canonical, content needs rewriting. (c) Owner provides definitive product catalog. | **Option C — Owner provides definitive product catalog with canonical names, slugs, and specs.** | Blocks all catalogue and product detail page production (P4-P6). |
| **A2** | Navigation: Accept 5-item nav + CTA button, or keep Master's 7-item nav? | This document recommends 5 nav links + persistent CTA button (Sections 4.1). Master Section H.2 specifies 7 items including Estimate and FAQ. | (a) Approve 5-item nav + CTA button. (b) Keep 7-item nav as specified in Master. | **Option A** — Fewer nav items focus the buyer's attention and elevate the CTA. FAQ is accessible from footer and support pages. | Master Section H.2 would need amendment if Option A. |
| **A3** | Returns page: Merge claims into Warranty, or keep separate? | This document recommends consolidating claims process into Warranty page (Section 6.5). | (a) Consolidate claims into Warranty. Returns focuses on return eligibility/process only. (b) Keep both pages as-is with duplicated claims content. | **Option A** — Reduces content duplication, simplifies maintenance, clarifies user journey. | Content production for Returns page. |
| **A4** | Product catalog for Shower Glass, Architectural Glass, Standard Mirrors | No product names, specs, or slugs exist for these 3 categories. Solution pages exist but have no product content to link to. | (a) Owner provides product definitions. (b) Remove catalogue links from these 3 solution pages — make them estimate-only. (c) Defer these categories to post-launch. | **Option A** — All 6 categories should have complete product funnels. | Blocks P4-P6 for 3 categories. If deferred, 3 solution pages become dead-ends at catalogue level. |
| **A5** | Mixed-use and commercial office industry pages | Referenced in existing content but no dedicated pages exist. | (a) Create both. (b) Create mixed-use only (has case study). (c) Defer both. | **Option C — Defer both.** No case studies or industry-specific proof exists for commercial office. Mixed-use can be reconsidered if demand warrants it. | Minimal impact — these are not in the Master's sitemap. |
| **A6** | Legacy file: Archive or delete 00_MASTER-GUIDELINES.md? | Superseded by docs/00_MASTER_SYSTEM.md. Still in repository root. | (a) Move to docs/archive/. (b) Delete entirely. | **Option A** — Archive preserves history while removing confusion. | None — but clutters the repo. |
| **A7** | Pricing data for catalog and product pages | Multiple pages contain "$XXX" placeholders. | (a) Owner provides real pricing now. (b) Defer pricing to post-launch. (c) Use "Request a Quote" model (no prices shown). | **Owner decision** — impacts all catalogue and product detail pages. Real pricing dramatically improves conversion. Quote-only model shifts more traffic to wizard. | All catalogue and product detail pages. |

---

*This document defines the structural blueprint for the HILO website. It is subordinate to the Master System Document (docs/00_MASTER_SYSTEM.md) in all matters of strategic, editorial, and conversion doctrine. It will be referenced by Gate 3 (Page Models) and Gate 4 (Content Production).*
