# PAGE MODELS AND PRIORITIZATION — HILO Website Project

**Gate**: 3 — Page Models and Prioritization
**Status**: APPROVED — Gate 3 locked for Gate 4 execution
**Created**: 2026-04-08
**Last Updated**: 2026-04-08
**Created by**: Senior Conversion Architect (GLM)
**Governing Document**: docs/00_MASTER_SYSTEM.md (v1.2)
**Depends On**: docs/02_CONVERSION_ARCHITECTURE.md (FINAL — locked)
**Companion**: docs/01_WORKPROGRESS.md

---

## A. Executive Summary

### A.1 What Gate 3 Solves

Gate 1 established the rules. Gate 2 built the structural blueprint — the sitemap, navigation, page family map, and CTA flow architecture. Gate 3 converts that blueprint into **executable page specifications**. This document defines exactly what every page on the HILO website must contain, in what order, with what proof, with what conversion mechanics, and with what AI discoverability structures. It is the production manual that content writers will follow during Gate 4.

Without Gate 3, Gate 4 content production would be inconsistent — each writer (or AI turn) would interpret the Master's rules differently, producing pages that don't share a common structure, don't link to each other properly, and don't serve the conversion architecture's intent. Gate 3 eliminates that risk by defining 14 page models that serve as templates for all 154 pages on the site. Each model specifies the exact block order, mandatory content, proof requirements, CTA hierarchy, internal linking obligations, and AI discoverability structures that every instance of that page type must follow.

### A.2 What Becomes Possible After Approval

Once the owner validates this document, the following becomes actionable:

1. **Gate 4 content production can begin** — writers (human or AI) can produce page content by following the applicable page model as a template, filling in category-specific or product-specific details while adhering to the standardized block structure.
2. **Batch production becomes possible** — because every page within a family shares the same model, all 6 solution pages can be produced simultaneously, all 120 product detail pages can be batch-produced by category, and quality can be validated against a consistent standard rather than subjective judgment.
3. **Cross-linking can be executed with precision** — every page model specifies exactly which other pages it must link to and where, eliminating the orphan-page risk identified in the Gate 2 audit.
4. **AI discoverability structures can be embedded at creation time** — rather than retrofitting FAQ blocks, comparison tables, and definition blocks after content is written, they are specified as mandatory content blocks within each model, ensuring they are produced alongside the page content.
5. **QA at Gate 6 becomes objective** — the Definition of Done for each page type gives G6 reviewers a checklist, not an opinion.

### A.3 What Remains Blocked

- **Final page copy** — this document defines structure and requirements, not copy. No page content may be written until the owner approves these models.
- **Code, build, deployment** — not actionable until Gate 5.
- **Pricing data** — placeholder values ("$XXX") require owner input. Pricing model decisions (A7) must be resolved before catalogue and product detail pages can be finalized.
- **Product naming** — canonical product names, slugs, and specifications for Shower Glass, Architectural Glass, and Standard Mirrors (A4) must be provided by the owner before P6 production can begin.
- **Schema.org markup** — specified in this document as intent; implementation occurs at Gate 5 (build).

### A.4 Relationship to Governing Documents

This document is subordinate to the Master System Document (docs/00_MASTER_SYSTEM.md) in all matters of strategic doctrine, conversion rules, terminology, and brand standards. It is the operational extension of the Conversion Architecture (docs/02_CONVERSION_ARCHITECTURE.md), converting architectural decisions into executable page specifications. In case of conflict, the Master prevails, then the Conversion Architecture, then this document.

---

## B. Full Page-Model System

This section defines 14 page models that serve as templates for all 154 pages on the HILO website at launch. Each model specifies the complete content specification for that page type. Content writers during Gate 4 must follow the applicable model exactly — the block order, mandatory elements, proof requirements, and linking obligations are not suggestions.

### B.1 Homepage Model

**Route Pattern**: `/`

**Conversion Role**: The homepage is the primary entry point and brand statement. Its job is to capture attention, communicate the full value proposition across all three buyer personas, and route visitors to their most relevant next step — either a solution category, an industry page, or directly to the estimation wizard. The homepage must work for a first-time visitor who has never heard of HILO and for a returning visitor who is ready to convert. It must simultaneously serve the Developer/Project Manager evaluating vendors, the Architect/Designer seeking specification-grade products, and the Facility Manager/GM experiencing recurring product failures.

**Audience and Awareness Level**: All three buyer personas. Primarily Level 3 (Solution Aware) visitors who know they need glass/mirror solutions but are evaluating suppliers. Also serves Level 4 (Product Aware) return visitors and Level 2 (Problem Aware) visitors arriving from search or referrals. The homepage must not assume any prior knowledge of HILO.

**Primary CTA**: "Get Instant AI Estimate →" linking to `/estimate`. Placed in the hero section above the fold and repeated in the final CTA section at the bottom of the page. This CTA must be visually dominant — the highest-contrast element in the viewport.

**Secondary CTA**: "Book a Call" linking to `/contact`. Placed adjacent to the primary CTA in the hero section and in the final CTA section. Visually subordinate to the primary CTA but clearly clickable.

**Mandatory Content Blocks in Exact Order**:

| # | Block | Content Requirements | Depth Guidance |
|---|-------|---------------------|---------------|
| 1 | **Hero Section** | H1 headline communicating the core value proposition (engineered for commercial reliability). Subheadline incorporating the Trust Line or key metric (180+ projects, &lt;0.5% failure rate). Primary CTA button. Secondary CTA button. Hero image showing commercial installation context. | Focused — above the fold, scannable in 5 seconds. |
| 2 | **Trust Bar** | The mandatory Trust Line verbatim: 🏆 180+ Projects \| 🛡️ 5-Year Warranty \| 🇨🇦 Designed in Canada. Distributed across North America. Must appear immediately below the hero CTA. | Single line, persistent. |
| 3 | **Value Proposition Section** | "Why HILO?" block communicating the 7 HILO criteria as benefits, not features. Each criterion should be a short heading with 2-3 sentences of benefit-oriented explanation. Must use the Master's approved terminology. | Medium — 7 brief subsections. |
| 4 | **Solution Category Cards** | 6 cards, one per solution category (LED Mirrors, Smart Mirrors, Medicine Cabinets, Shower Glass, Architectural Glass, Standard Mirrors). Each card shows: product name, 1-line description, thumbnail image, and "Explore →" link to `/solutions/[slug]`. Cards should be in a 2×3 or 3×2 grid. | Medium — scannable grid with brief per-card copy. |
| 5 | **Industry Segmentation Section** | 3 industry cards (Hotels, Real Estate, Senior Living). Each shows: industry name, 1-line relevance statement, and "See How HILO Serves [Industry] →" link to `/industries/[slug]`. This block connects visitors to their specific vertical. | Short — 3 cards, brief copy. |
| 6 | **Process / How It Works Section** | 3-4 step visual process: (1) Get your estimate in 60 seconds, (2) Review your customized proposal, (3) Receive door-to-door delivery, (4) Install and enjoy. Each step must have a short heading and 1-2 sentences of explanatory copy. This block reduces anxiety about the buying process. | Medium — process visualization. |
| 7 | **Featured Case Study Teaser** | 1-2 featured case studies with: property name, industry, key metric (units, timeline, result), hero image, and "Read Full Case Study →" link. This provides social proof at the entry point without requiring the visitor to navigate to the case studies section. | Short — 1-2 teasers with metric callouts. |
| 8 | **FAQ Block** | 3 frequently asked questions relevant to top-of-funnel visitors. Each FAQ must use H3 markup with the question as the heading, followed by a self-contained answer of 3-5 sentences containing specific data points. Topics should address the most common first-visit objections: warranty coverage, delivery timelines, and custom vs. catalog options. | Short — 3 Q&A pairs. |
| 9 | **Final CTA Section** | Reinforced conversion section with primary CTA ("Get Instant AI Estimate →") and secondary CTA ("Book a Call"). Optional supporting headline. Trust Line repeated. | Short — focused conversion block. |
| 10 | **Footer** | Full footer navigation per Conversion Architecture Section 4.4 (3 columns: Solutions, Industries, Support + Case Studies, Estimate + Trust Line). Must include the mandatory Trust Line. | Standard footer. |

**Required Proof Elements**: Trust Line (mandatory in hero, trust bar, and footer). 180+ projects metric. &lt;0.5% failure rate. 5-year warranty mention. At least one case study metric. "Designed in Canada" origin signal.

**Required HILO Criteria Coverage**: All 7 criteria must be represented. Criteria #1 (Fiabilité) and #5 (AI Estimate) are mandatory and appear in the hero and value proposition sections. The remaining 5 criteria appear in the Value Proposition block. This is the only page type outside of solution pages where all 7 criteria are expected, because the homepage must communicate the full HILO offering.

**Required Internal Links**: All 6 solution category pages (via solution cards in Block 4). All 3 industry pages (via industry cards in Block 5). The estimation wizard (via primary CTA). The contact page (via secondary CTA). 1-2 featured case studies (via Block 7). FAQ page (via Block 8 — "View All FAQs" link). Footer links to all support pages.

**Required AI-Discoverability Blocks**: The homepage serves as the Brand Entity hub for AI systems. It must include: (1) a clear definition of HILO as a company in the hero or value proposition ("HILO is a North American manufacturer of premium glass and mirror solutions, designed in Canada and distributed across the continent"), (2) the FAQ block with self-contained, data-rich answers, (3) the Trust Line as a structured entity reference, (4) the solution category cards as entity references to the 6 primary entity hubs. Internal links from the homepage carry the highest AI authority weight — they signal to AI systems what HILO's core topics are.

**Structured Data / Schema Intent**: `Organization` schema (company name, logo, URL, contact info, sameAs). `WebSite` schema (site name, URL, potential search action for the wizard). `BreadcrumbList` is not needed (homepage is L0).

**Common Mistakes to Avoid**:
1. Using the document metadata as the H1 (found in existing 01_HOMEPAGE.md — the H1 was "HILO — Website Content" instead of a page headline).
2. Including French sections or strategy/analysis content that is not page copy (the existing file contained internal collaboration artifacts).
3. Failing to link to industry pages — the current homepage only links to solutions, creating a silo between the two major page families.
4. Making the hero too generic ("Quality glass solutions for your business") instead of specific and benefit-oriented ("Premium glass and mirror solutions engineered for commercial reliability").
5. Burying the CTA below the fold — the primary CTA must be visible without scrolling.
6. Omitting the Trust Line from the hero section — it must appear in the hero AND the footer.

**Definition of Done for Homepage**:
- [ ] H1 is a page headline (not document metadata) containing the primary value proposition
- [ ] All 7 HILO criteria are communicated
- [ ] Primary and secondary CTAs are present, correct, and link to valid destinations
- [ ] Trust Line appears in hero/CTA area and footer
- [ ] All 6 solution categories are linked via cards
- [ ] All 3 industry pages are linked via cards
- [ ] At least 1 case study teaser is present with a metric
- [ ] FAQ block has 3 self-contained, data-rich Q&A items
- [ ] Process/How It Works section has 3-4 steps
- [ ] No French metadata or collaboration artifacts
- [ ] No placeholder text (TBD, XXX, Lorem ipsum)
- [ ] All internal links use descriptive anchor text
- [ ] Content depth is appropriate to the homepage's breadth-of-value role (per Master I.0)
- [ ] Terminology is consistent with Master Section E.6 ("Designed in Canada" not "Canadian Made", etc.)


### B.2 Industry Page Model

**Route Pattern**: `/industries/[slug]` where slug is one of: `hotels`, `real-estate`, `senior-living`

**Conversion Role**: Industry pages serve as audience segmentation tools — they prove that HILO understands the visitor's specific vertical and has relevant experience. A hotel developer landing on the Hotels page should immediately see HILO's hospitality-specific expertise, not generic glass company messaging. The page drives to the estimation wizard as the primary conversion action, with secondary navigation to relevant solution categories and case studies. Industry pages are the primary tool for capturing Level 3 (Solution Aware) visitors who are searching by vertical rather than by product category.

**Audience and Awareness Level**: Industry-specific personas. Hotels page targets Hotel GMs and VP Development. Real Estate page targets multi-family developers and property managers. Senior Living page targets senior living operators and facility directors. All visitors are primarily Level 3 (Solution Aware) — they know they need glass/mirror solutions but are evaluating whether HILO understands their specific industry.

**Primary CTA**: "Get Instant AI Estimate →" linking to `/estimate`. Placed in the hero section and repeated in the final CTA section at the bottom.

**Secondary CTA**: "Book a Call" linking to `/contact`. Placed adjacent to the primary CTA in both the hero and final CTA sections.

**Mandatory Content Blocks in Exact Order**:

| # | Block | Content Requirements | Depth Guidance |
|---|-------|---------------------|---------------|
| 1 | **Industry Hero** | Industry-specific H1 (e.g., "Glass and Mirror Solutions Engineered for Hotels"). Subheadline referencing industry-specific pain points or requirements. Primary and secondary CTAs. Industry-relevant hero image. Trust Line below CTAs. | Focused — above the fold. |
| 2 | **Industry Challenge Section** | 2-3 paragraphs describing the specific challenges this industry faces with glass and mirror products. Must be specific enough to demonstrate genuine understanding — not generic "mirrors are important" content. Examples: guest complaint cycles for hotels, maintenance burden for multi-family, safety compliance for senior living. | Medium — establishes relevance. |
| 3 | **7 HILO Advantages (Industry-Customized)** | The 7 HILO criteria adapted to the specific industry. Each advantage should have a heading and 2-3 sentences explaining how the criterion applies to this vertical. For example, "Fiabilité long terme" for hotels should reference guest experience continuity and brand standard compliance, not just the warranty terms. | Medium-deep — 7 subsections. |
| 4 | **Recommended Solutions** | 3-4 solution categories most relevant to this industry, presented as cards with links to `/solutions/[slug]`. Each card should explain WHY this solution matters for this industry (1-2 sentences). The Hotels page should prioritize LED Mirrors and Smart Mirrors. The Senior Living page should emphasize safety-rated products. | Medium — 3-4 solution cards. |
| 5 | **Industry Case Study** | One featured case study relevant to this industry with: project overview (property name, location, scale), challenge, HILO solution, results with specific metrics, testimonial (if available), and "Read Full Case Study →" link. This is the primary social proof element on the page. | Medium — narrative with data. |
| 6 | **FAQ Block** | 3 industry-specific frequently asked questions. Each uses H3 markup with question as heading, followed by a self-contained answer of 3-5 sentences with specific data. Topics should address industry-specific objections: compliance requirements for senior living, brand standard integration for hotels, unit-scale pricing for multi-family. | Short — 3 Q&A pairs. |
| 7 | **Final CTA Section** | Reinforced conversion with primary CTA, secondary CTA, and Trust Line. Optional supporting headline referencing the industry. | Short — focused conversion block. |

**Required Proof Elements**: Trust Line (hero and footer). Industry-specific case study with specific metrics. At least 2 of the 7 HILO criteria must include quantitative proof points (&lt;0.5% failure rate, 94% maintenance reduction, 180+ projects, etc.). The case study must include at least one specific number (units delivered, timeline, failure rate improvement).

**Required HILO Criteria Coverage**: All 7 criteria must be represented in Block 3, customized to the industry. Criteria #1 (Fiabilité) and #5 (AI Estimate) are mandatory and must appear in the hero or early in the page. The remaining criteria must appear in the advantages section with industry-specific framing.

**Required Internal Links**: 3-4 relevant solution category pages (via Block 4 cards). 1 relevant case study (via Block 5, with link to full study). Estimation wizard (via primary CTA). Contact page (via secondary CTA). Other industry pages can be linked optionally but are not mandatory (industry-to-industry cross-linking is lower priority than industry-to-solution cross-linking).

**Required AI-Discoverability Blocks**: Industry pages are Contextual Hubs — they signal to AI systems that HILO has expertise within a specific vertical. Each page must include: (1) a clear industry definition in the hero (e.g., "HILO provides engineered glass and mirror solutions for the hospitality industry, serving hotel chains and boutique properties across North America"), (2) the FAQ block with industry-specific Q&A, (3) cross-links to relevant solution pages with descriptive anchor text that includes both the industry and the solution category. AI systems answering "What mirror solutions work for hotels?" will extract from the intersection of industry page content and solution page content — the cross-links help AI systems connect these entities.

**Structured Data / Schema Intent**: `BreadcrumbList` (Home > Industries > [Industry Name]). Potential `FAQPage` schema if FAQ block is substantial enough. No product schema on industry pages.

**Common Mistakes to Avoid**:
1. Writing generic content that could apply to any industry — the Hotels page must feel distinctly different from the Senior Living page.
2. Failing to include industry-specific case study data — vague "they were happy" results are worthless.
3. Not cross-linking to solution pages — the existing industry pages are completely siloed from /solutions/.
4. Being too thin — all 3 existing industry pages are under 500 words and fail the Master's depth insufficiency tests.
5. Using the wrong case study — the Senior Living page references "Château Frontenac" which is a famous hotel, not a senior living facility.
6. Listing solutions without explaining WHY they matter for this industry — the connection must be explicit.

**Definition of Done for Industry Page**:
- [ ] H1 is industry-specific and benefit-oriented
- [ ] Industry challenge section demonstrates genuine vertical understanding
- [ ] All 7 HILO criteria are present, customized to the industry
- [ ] 3-4 relevant solution categories are linked with industry-specific rationale
- [ ] Industry case study includes specific metrics and links to full study
- [ ] FAQ block has 3 industry-specific, self-contained Q&A items
- [ ] Primary and secondary CTAs are present and correct
- [ ] Trust Line appears in hero/CTA area and footer
- [ ] Cross-links to solution pages use descriptive anchor text
- [ ] Content depth is appropriate to the industry evaluation role
- [ ] No placeholder text or collaboration artifacts
- [ ] Terminology consistent with Master

### B.3 Solution Page Model

**Route Pattern**: `/solutions/[slug]` where slug is one of: `led-mirrors`, `smart-mirrors`, `medicine-cabinets`, `shower-glass`, `architectural-glass`, `standard-mirrors`

**Conversion Role**: Solution pages are the evaluation workhorses of the HILO website. This is where buyers who know what product category they want (Level 3-4 awareness) come to compare HILO against alternatives, assess proof, and decide whether to explore the catalogue or request an estimate. Solution pages must be the most content-rich pages on the site — they carry the heaviest proof burden and the most comprehensive HILO criteria coverage. Every solution page must make the case that HILO is the superior choice in this specific product category.

**Audience and Awareness Level**: Primarily Level 3 (Solution Aware) and Level 4 (Product Aware) visitors. The Developer/Project Manager evaluating suppliers and the Architect/Designer specifying products are the primary audiences. These visitors have already decided they need [LED mirrors / smart mirrors / etc.] — they are now deciding whether HILO is the right supplier.

**Primary CTA**: "See Our Products →" linking to `/solutions/[slug]/catalogue`. This drives visitors into the product comparison funnel. Placed prominently in the hero section and in the Catalog vs. Custom Decision Box.

**Secondary CTA**: "Get AI Estimate" linking to `/estimate`. Placed adjacent to the primary CTA and repeated throughout the page in strategic locations (after proof sections, in the final CTA section).

**Mandatory Content Blocks in Exact Order**:

| # | Block | Content Requirements | Depth Guidance |
|---|-------|---------------------|---------------|
| 1 | **Product Category Hero** | Category-specific H1 (e.g., "LED Mirrors Engineered for Commercial Reliability"). Subheadline with key reliability metric (&lt;0.5% failure rate or category-specific stat). Primary CTA ("See Our Products"). Secondary CTA ("Get AI Estimate"). Trust Line below CTAs. Category-relevant hero image. | Focused — above the fold. |
| 2 | **Definition Block** | Clear, concise 2-3 sentence definition of this product category for AI extraction. Example: "LED mirrors are backlit mirror products designed for commercial environments where reliability, energy efficiency, and aesthetic consistency are critical. HILO's LED mirror range includes 20 models across standard and smart configurations, engineered for hospitality, multi-family, and senior living applications." This block exists primarily for AI discoverability — it is the building block AI systems use to understand what HILO offers in this category. | Short — 2-3 sentences, clearly delineated. |
| 3 | **Criterion #1: Fiabilité Long Terme** | Dedicated section on long-term reliability. Must include: 5-year warranty details, &lt;0.5% failure rate, 180+ projects data, and category-specific reliability proof. This is the #1 HILO criterion and must always be the first content section after the hero. | Medium-deep — substantive proof section. |
| 4 | **Criterion #2: Prix Compétitif** | Competitive pricing section. Must include: direct-from-manufacturer explanation, 15-25% below premium competitors (if data supports), volume discount mention, and pricing transparency approach. May reference the wizard/estimation tool for specific pricing. | Medium — pricing rationale. |
| 5 | **Criterion #3: Delivery Porte-à-Porte** | Door-to-door delivery section. Must include: delivery timeline (2-3 weeks for catalog, 4-6 weeks for custom), multi-site coordination capability, damage-free guarantee, and geographic coverage (Canada and US). | Medium — logistics proof. |
| 6 | **Criterion #4: Flexibilité** | Catalog vs. custom decision framework. Must include: what's available in the catalog, what can be customized (dimensions, finishes, features), lead time comparison (catalog faster, custom 4-6 weeks), and a clear decision box ("Choose catalog for speed, custom for unique requirements"). This section is critical for B2B buyers who need to understand their options before committing. | Medium — decision framework. |
| 7 | **Criterion #6: Grand Choix Produits** | Full product range section. Must include: overview of the product range within this category, mention of 20 models (or however many are defined), link to the catalogue page, and cross-reference to other relevant solution categories (e.g., LED Mirrors page should mention Smart Mirrors as a premium alternative). | Medium — product breadth. |
| 8 | **Criterion #7: Installation** | Installation section. Must include: partner installation network availability, DIY-friendly design where applicable, installation support process, and geographic limitations. If installation is not available in certain regions, this must be stated clearly. | Short-medium — service description. |
| 9 | **Comparison Block** | Side-by-side comparison of HILO vs. generic alternatives. Must include: failure rate comparison, warranty comparison, pricing model comparison, and support comparison. This must be formatted as a clearly delineated table or structured block with descriptive column headers — it is the #1 AI-citable structure on solution pages. | Medium — comparison table. |
| 10 | **Specification Table** | Category-level specification summary. Must include: available sizes, materials, finish options, LED color temperatures (for LED/smart), glass thickness options (for shower/architectural), certification standards, and lead times. This table provides the technical data that architects and specifiers need. | Medium — technical reference table. |
| 11 | **Cross-Sell Section** | Links to related solution categories with brief rationale. Example: LED Mirrors page links to Smart Mirrors ("Upgrade to touchscreen and PMS integration") and Medicine Cabinets ("Complete your bathroom renovation with matching storage solutions"). 2-3 related categories, each with 1-2 sentences of cross-sell reasoning. | Short — 2-3 cross-sell cards. |
| 12 | **Industry Relevance Block** | Links to 1-3 relevant industry pages with brief explanation of why this solution matters for each industry. Example: Smart Mirrors page links to Hotels ("PMS integration for brand-standard compliance") and Senior Living ("Safety-rated smart features for resident monitoring"). | Short — 1-3 industry links. |
| 13 | **FAQ Block** | 3-5 product-category-specific frequently asked questions. Each uses H3 markup, followed by 3-5 sentences with specific data points. Topics should address the most common evaluation objections: durability, pricing, customization limits, installation, warranty specifics. | Short-medium — 3-5 Q&A pairs. |
| 14 | **Final CTA Section** | Dual CTA: "See Our Products →" (primary, to catalogue) and "Get AI Estimate" (secondary, to wizard). Trust Line. | Short — focused conversion. |

**Required Proof Elements**: Trust Line (hero and footer). &lt;0.5% failure rate with context (across 180+ projects). 5-year warranty terms. At least one category-specific metric. Comparison data (HILO vs. generic). The comparison block and specification table serve as the primary proof structures.

**Required HILO Criteria Coverage**: ALL 7 criteria are MANDATORY on solution pages (per Master Section P.1). This is the only page type where all 7 are required. Criteria #1 and #5 must appear prominently — #1 as the first content section, #5 via the CTA system and estimation references throughout.

**Required Internal Links**: Catalogue page (via primary CTA and Block 7). Estimation wizard (via secondary CTA, appearing at least 3 times). 2-3 related solution categories (via Block 11). 1-3 relevant industry pages (via Block 12). FAQ page (via Block 13 — "View All FAQs" link). Parent breadcrumb: Home > Solutions > [Category Name].

**Required AI-Discoverability Blocks**: Solution pages are PRIMARY ENTITY HUBS — they are the pages most likely to be cited by AI systems answering questions about specific product categories. Each solution page MUST include: (1) the Definition Block (Block 2) — a concise, extractable category definition, (2) the Comparison Block (Block 9) — clearly structured for AI extraction with descriptive headers, (3) the Specification Table (Block 10) — tabular data that AI systems can extract to answer technical questions, (4) the FAQ Block (Block 13) — self-contained, data-rich answers, (5) cross-links to related solution pages and industry pages with descriptive anchor text. Together, these structures make the solution page a comprehensive, AI-citable reference for its product category.

**Structured Data / Schema Intent**: `BreadcrumbList` (Home > Solutions > [Category]). `FAQPage` schema for the FAQ block. Potential `Product` or `ItemList` schema referencing the catalogue page. `Organization` reference via Trust Line context.

**Common Mistakes to Avoid**:
1. Missing any of the 7 HILO criteria — solution pages are the ONLY page type where all 7 are mandatory.
2. No cross-linking to industry pages — the existing solution pages are completely siloed from /industries/.
3. Having the "See All Products" CTA link to nowhere — the primary CTA on solution pages must point to the catalogue listing page.
4. Using generic comparison language — the comparison block must have specific numbers, not just "better quality."
5. Not including a definition block — AI systems need a clear category definition to understand the page's entity.
6. No FAQ block — the existing solution pages have no FAQ sections, which makes them less AI-citable.
7. Placeholder pricing data — "$XXX" must be resolved before final content production.

**Definition of Done for Solution Page**:
- [ ] H1 is category-specific and benefit-oriented
- [ ] All 7 HILO criteria are present as dedicated sections
- [ ] Definition block provides concise, extractable category description
- [ ] Comparison block is a clearly structured, extractable table
- [ ] Specification table includes category-level technical data
- [ ] Primary CTA "See Our Products" links to `/solutions/[slug]/catalogue`
- [ ] Secondary CTA "Get AI Estimate" links to `/estimate`
- [ ] Cross-sell section links to 2-3 related solution categories
- [ ] Industry relevance block links to 1-3 industry pages
- [ ] FAQ block has 3-5 self-contained, data-rich Q&A items
- [ ] Trust Line appears in hero/CTA area and footer
- [ ] All internal links use descriptive anchor text
- [ ] Content depth is appropriate to the evaluation role (deepest of all page types)
- [ ] No placeholder text
- [ ] Terminology consistent with Master


### B.4 Catalogue Listing Page Model

**Route Pattern**: `/solutions/[slug]/catalogue` where slug is the parent solution category

**Conversion Role**: Catalogue listing pages are product comparison hubs. They sit between the solution overview page and individual product detail pages in the conversion funnel. A visitor arriving at a catalogue page has already decided on a product category (e.g., LED Mirrors) and now needs to compare specific products within that category to find the right fit for their project. The catalogue page's job is to make that comparison fast, clear, and action-oriented — presenting all products in a scannable grid with enough detail for initial comparison and clear paths to individual product pages for deeper evaluation.

**Audience and Awareness Level**: Level 4 (Product Aware) buyers who are actively comparing products within a category. They know what they need and are now evaluating specific models. These visitors are close to converting — they may go directly from a product detail page to the estimation wizard.

**Primary CTA**: "Get AI Instant Quote →" linking to `/estimate` (ideally pre-filled with the category context). Placed at the top of the page and available as a persistent element during scrolling.

**Secondary CTA**: "Book a Call" linking to `/contact`. Placed adjacent to the primary CTA.

**Mandatory Content Blocks in Exact Order**:

| # | Block | Content Requirements | Depth Guidance |
|---|-------|---------------------|---------------|
| 1 | **Catalogue Header** | H1: "[Category Name] — Full Product Catalogue" (e.g., "LED Mirrors — Full Product Catalogue"). Brief category introduction (2-3 sentences). Primary and secondary CTAs. Breadcrumb: Home > Solutions > [Category] > Catalogue. | Short — functional header. |
| 2 | **Comparison Grid** | The PRIMARY content block. A grid/table displaying all 20 products in the category with key comparison columns: product name, image thumbnail, key specification (size range, LED type, etc.), price indicator (price, range, or "Get Quote"), and "View Details →" link to product detail page. This grid is the #1 AI-citable structure on the site — it is the structure AI systems extract to answer "Which [product] should I choose?" queries. | Medium-large — comprehensive grid. |
| 3 | **Category Overview Text** | 2-3 paragraphs providing context about the category: what distinguishes HILO's approach, what the category is best suited for, and how to choose between products. This is NOT a repeat of the solution page content — it should focus on product selection guidance, not category evaluation. | Medium — selection guidance. |
| 4 | **Filter / Sort Controls** | UI specification for filtering and sorting the product grid. Filters may include: size range, price range, features (e.g., dimmable, touch-enabled, anti-fog). Sort options: price low-high, price high-low, name A-Z, newest. This is a UI specification for G5 build, not content, but the content must account for it. | UI spec — brief. |
| 5 | **Catalog vs. Custom Decision Box** | Brief callout box: "Don't see exactly what you need? HILO offers custom solutions tailored to your specifications. Get an estimate in 60 seconds →" linking to `/estimate`. This captures visitors whose requirements don't match any catalog product. | Short — callout box. |
| 6 | **Final CTA Section** | Reinforced primary CTA and secondary CTA. Trust Line. | Short — conversion block. |

**Required Proof Elements**: Trust Line (header and footer). Product specifications in the comparison grid. Warranty mention (can be a single line: "All products backed by HILO's 5-year warranty"). Pricing indicators where available.

**Required HILO Criteria Coverage**: Minimum 3 criteria: #1 (Fiabilité — via warranty mention), #5 (AI Estimate — via CTA and decision box), #6 (Grand Choix — via the full product range in the grid). Criteria #2 (Pricing) may appear if pricing data is available in the grid. The catalogue page is a selection tool, not a persuasion tool — it does not need the full 7-criteria treatment.

**Required Internal Links**: All 20 product detail pages within this category (via comparison grid "View Details" links). Parent solution page (via breadcrumb). Estimation wizard (via primary CTA). Contact page (via secondary CTA).

**Required AI-Discoverability Blocks**: The comparison grid (Block 2) is the primary AI-citable structure. It must be structured so that AI systems can extract a meaningful product comparison: each product must have a clearly labeled name, at least 2-3 extractable specifications, and a price indicator. The category overview text (Block 3) should include a category-level definition sentence that AI systems can cite. The grid is the single most important AI-citable element on the entire website for product queries.

**Structured Data / Schema Intent**: `BreadcrumbList` (Home > Solutions > [Category] > Catalogue). `ItemList` schema referencing all 20 products. `FAQPage` only if an FAQ section is added (not mandatory on catalogue pages but recommended if space allows).

**Common Mistakes to Avoid**:
1. Making the catalogue page a narrative page — it is a comparison grid, not a story. Product information should be scannable, not paragraph-form.
2. Not linking every product to its detail page — every row in the grid must have a clickable path to the product detail page.
3. Including too much text — the catalogue page should be grid-first, text-second. Visitors come here to compare, not to read.
4. Missing the custom option callout — visitors who don't find what they need should be captured by the decision box, not lost.

**Definition of Done for Catalogue Listing Page**:
- [ ] H1 clearly identifies the category and purpose
- [ ] Comparison grid displays all 20 products with key specs
- [ ] Every product has a "View Details →" link to its detail page
- [ ] Breadcrumb navigation is present (Home > Solutions > [Category] > Catalogue)
- [ ] Primary CTA "Get AI Instant Quote →" links to `/estimate`
- [ ] Catalog vs. Custom decision box is present
- [ ] Trust Line appears in header area and footer
- [ ] Category overview text provides selection guidance
- [ ] No placeholder pricing data (or clearly marked as "Request Quote" if pricing model is quote-based)
- [ ] Terminology consistent with Master

### B.5 Product Detail Page Model

**Route Pattern**: `/solutions/[slug]/catalogue/[product-slug]`

**Conversion Role**: Product detail pages are the last content stop before conversion. A visitor on a product detail page has navigated through the full evaluation funnel — homepage, solution page, catalogue page — and is now evaluating a specific product. This page must provide complete specifications, clear pricing or quote paths, and sufficient trust reinforcement to drive the visitor into the estimation wizard. It is the most conversion-critical content page on the site because it serves the most intent-rich audience — buyers who are ready to act.

**Audience and Awareness Level**: Level 4-5 (Product Aware to Most Aware). These visitors know what they want and are evaluating whether this specific product meets their requirements. The Developer/PM checking specifications, the Architect verifying dimensions and certifications, and the Facility Manager confirming compatibility are all potential visitors.

**Primary CTA**: "Get AI Instant Quote →" linking to `/estimate` (pre-filled with this product's selection). Placed prominently in the product hero and repeated in the final CTA section. This CTA must be the most visually prominent element on the page.

**Secondary CTA**: "Book a Call" linking to `/contact`. Placed adjacent to the primary CTA.

**Mandatory Content Blocks in Exact Order**:

| # | Block | Content Requirements | Depth Guidance |
|---|-------|---------------------|---------------|
| 1 | **Product Hero** | Product name as H1 (canonical name). Product image(s) — primary image + optional alternate angles. Key callout: price (if available) or "Get Instant Quote". Primary CTA. Secondary CTA. Trust Line or warranty badge. Breadcrumb: Home > Solutions > [Category] > Catalogue > [Product Name]. | Focused — above the fold. |
| 2 | **Key Specifications Table** | Structured spec table with: dimensions, materials, glass type/thickness, LED specifications (color temperature, CRI, dimming for LED/smart), certifications, available finishes/sizes, weight, and lead time. This table must be formatted for both human scanning and AI extraction — clear column headers, no ambiguous abbreviations. This is the primary AI-citable structure on product detail pages. | Medium — technical reference. |
| 3 | **Features and Benefits** | 4-6 key features of this specific product, each with a benefit-oriented heading and 2-3 sentences of explanation. Must be specific to THIS product, not generic category features. Example: "Fleuve Pro LED Mirror — Dimmable Warm-to-Cool Lighting" rather than just "LED Lighting." | Medium — product-specific. |
| 4 | **Dimensions and Size Options** | Available sizes, custom dimension capabilities, and mounting options. If the product comes in multiple size variants, list them in a table. If custom dimensions are available, explain the process. | Short-medium — size reference. |
| 5 | **Related Products** | 3-5 related products from the same category (and potentially from related categories). Each with product name, image thumbnail, 1-line description, and "View →" link. This drives continued exploration within the catalogue rather than dead-ending the visit. | Short — 3-5 product cards. |
| 6 | **Warranty and Support Callout** | Brief warranty summary for this product: "Backed by HILO's 5-year full warranty. &lt;0.5% failure rate across 180+ commercial projects." Link to full warranty page. This reinforces trust at the decision point. | Short — trust reinforcement. |
| 7 | **Final CTA Section** | Reinforced primary CTA ("Get AI Instant Quote →" pre-filled) and secondary CTA ("Book a Call"). Trust Line. | Short — conversion block. |

**Required Proof Elements**: Trust Line (footer). Warranty callout (Block 6). Product specifications in the spec table (Block 2). Specific product features and benefits (Block 3). The spec table and warranty callout serve as the primary proof structures.

**Required HILO Criteria Coverage**: Minimum 4 criteria: #1 (Fiabilité — warranty callout), #2 (Prix — pricing/quote path), #4 (Flexibilité — custom dimensions), #5 (AI Estimate — primary CTA). Additional criteria (#3 Delivery, #6 Product Range, #7 Installation) may appear if relevant to the specific product but are not mandatory on individual product pages.

**Required Internal Links**: Parent catalogue page (via breadcrumb). Parent solution page (via breadcrumb or "Back to [Category]" link). Related products (via Block 5). Warranty page (via Block 6). Estimation wizard (via primary CTA). Contact page (via secondary CTA).

**Required AI-Discoverability Blocks**: Product detail pages are SECONDARY ENTITY HUBS — AI systems cite individual product pages when answering questions about specific models ("What are the specs of the HILO Fleuve Pro LED mirror?"). Each product detail page MUST include: (1) the Key Specifications Table (Block 2) — the most AI-citable element, must have clear headers and complete data, (2) a "Specifications" section clearly marked with a heading that AI systems can identify, (3) the product name in the H1 that matches the canonical product name used across the site, (4) descriptive internal links using the product name as anchor text. The spec table is the single most important element — it must be complete and accurate.

**Structured Data / Schema Intent**: `BreadcrumbList` (Home > Solutions > [Category] > Catalogue > [Product Name]). `Product` schema with: name, image, description, sku (if applicable), brand, offers (price/availability), aggregateRating (if reviews exist). This is the most schema-rich page type on the site.

**Common Mistakes to Avoid**:
1. Incomplete specifications — the spec table must be complete and accurate. Missing data creates trust gaps.
2. Using non-canonical product names — the H1 must match the product name used everywhere else on the site.
3. Not pre-filling the estimation wizard — the CTA should pass the product context to the wizard so the visitor doesn't have to re-select.
4. Having no path back to the catalogue — the breadcrumb and "Back to [Category]" link are essential.
5. Generic features — "High-quality LED lighting" is not useful. "3000K warm white LED with CRI 90+ and dimmable driver" is what architects need.

**Definition of Done for Product Detail Page**:
- [ ] H1 uses the canonical product name
- [ ] Key Specifications Table is complete with clear column headers
- [ ] Features and Benefits are specific to this product (not generic category features)
- [ ] Dimensions/size options are clearly listed
- [ ] 3-5 related products are linked with thumbnails
- [ ] Warranty callout is present with link to full warranty page
- [ ] Primary CTA links to `/estimate` with product context
- [ ] Secondary CTA links to `/contact`
- [ ] Breadcrumb navigation is complete: Home > Solutions > [Category] > Catalogue > [Product]
- [ ] Trust Line appears in footer
- [ ] No placeholder pricing or TBD data
- [ ] `Product` schema markup is specified for G5 build
- [ ] Terminology consistent with Master and parent solution page


### B.6 Case Study Index Page Model

**Route Pattern**: `/case-studies`

**Conversion Role**: The case study index page serves as a social proof hub — it provides a single location where visitors can browse all of HILO's project evidence. For AI systems, this page is important because it aggregates proof across all projects, making it citable for queries like "Has HILO done hotel projects?" or "What are HILO's best results?" The index must make it easy for visitors to find the case study most relevant to their industry and to quickly grasp HILO's track record.

**Audience and Awareness Level**: Level 3-5 visitors. The Developer/PM evaluating vendors, the Architect looking for comparable projects, and the Facility Manager seeking reassurance. Visitors arriving here are in the consideration phase — they need proof to support a purchasing decision.

**Primary CTA**: "Start Your Project →" linking to `/estimate`. Placed prominently in the hero section and repeated at the bottom.

**Secondary CTA**: "Book a Call" linking to `/contact`. Placed adjacent to the primary CTA.

**Mandatory Content Blocks in Exact Order**:

| # | Block | Content Requirements | Depth Guidance |
|---|-------|---------------------|---------------|
| 1 | **Case Study Hero** | H1: "Proven Results Across 180+ Commercial Projects" or similar. Subheadline emphasizing the breadth of HILO's project experience. Primary and secondary CTAs. Trust Line. | Focused — above the fold. |
| 2 | **Results Summary Table** | Aggregated results across all 5 case studies in a single table: project name, industry, units/products installed, timeline, key metric (e.g., "Zero defects after 12 months"), and "Read →" link. This table is the primary AI-citable structure — AI systems extract aggregated proof from index pages to answer comparative queries. | Medium — comprehensive summary table. |
| 3 | **Case Study Cards** | 5 cards, one per case study, in a grid layout. Each card: project name, industry label, hero image, 2-3 sentence summary, key metric callout, and "Read Full Case Study →" link to `/case-studies/[slug]`. Cards should be visually consistent. | Medium — 5 cards with summaries. |
| 4 | **Industry Filter Navigation** | Quick links to filter by industry: "View All | Hotels | Real Estate | Senior Living | Mixed-Use." These are anchor links or simple UI filters (G5 build decision). Provides rapid navigation to the most relevant proof. | Short — navigation links. |
| 5 | **Final CTA Section** | Primary CTA, secondary CTA, Trust Line. Supporting headline: "Ready to see what HILO can do for your project?" | Short — conversion block. |

**Required Proof Elements**: Trust Line (hero and footer). Results summary table with specific metrics from all 5 case studies. At least one quantitative result per case study in the cards.

**Required HILO Criteria Coverage**: Minimum 2 criteria: #1 (Fiabilité — proven by project results) and #5 (AI Estimate — via CTA). Additional criteria may appear in case study summaries but are not mandatory on the index page.

**Required Internal Links**: All 5 individual case study pages (via cards and table). Estimation wizard (via primary CTA). Contact page (via secondary CTA). Industry pages (via industry filter links — optional but recommended). Breadcrumb: Home > Case Studies.

**Required AI-Discoverability Blocks**: The Results Summary Table (Block 2) is the primary AI-citable structure. AI systems answering "Which HILO projects have the best results?" or "Has HILO done hotel projects?" will extract from this table. It must be structured with clear column headers and specific, data-rich content in every cell. The case study cards (Block 3) provide additional extractable proof with project-specific context.

**Structured Data / Schema Intent**: `BreadcrumbList` (Home > Case Studies). No `FAQPage` on the index. No `Product` schema.

**Common Mistakes to Avoid**:
1. Not including a results summary table — the table is the most AI-citable element on this page.
2. Missing industry filter links — visitors need to find relevant proof quickly.
3. Vague descriptions in cards — "Great results" is not proof. "Zero defects across 120 rooms after 12 months" is proof.
4. Not linking every case study — all 5 must be accessible from this page.

**Definition of Done for Case Study Index**:
- [ ] H1 communicates HILO's proven track record
- [ ] Results summary table includes all 5 case studies with specific metrics
- [ ] 5 case study cards are present with images, summaries, and links
- [ ] Industry filter links are present
- [ ] Primary and secondary CTAs are correct
- [ ] Trust Line in hero/CTA area and footer
- [ ] All 5 case studies are linked
- [ ] No placeholder text
- [ ] Terminology consistent with Master

### B.7 Individual Case Study Page Model

**Route Pattern**: `/case-studies/[slug]` where slug is one of: `hotel-chain-rollup`, `multi-family`, `senior-living`, `mixed-use`, `boutique-hotel`

**Conversion Role**: Individual case study pages provide narrative evidence that HILO delivers on its promises. They convert by making the abstract specific — instead of "&lt;0.5% failure rate," the visitor reads "Zero mirror failures at the Radisson Montreal after 14 months." Case studies support conversion on referring pages (solution pages, industry pages, case study index) and serve as standalone proof for visitors who arrive directly from search.

**Audience and Awareness Level**: Level 4-5 (Product Aware to Most Aware). These visitors are evaluating HILO as a vendor and need specific proof to support their decision. The Developer/PM looking for comparable projects, the Architect seeking specification references, and the GM/Facility Manager seeking reassurance about post-installation performance.

**Primary CTA**: "Start Your Project →" linking to `/estimate`. Placed at the bottom of the case study narrative and in the final CTA section.

**Secondary CTA**: "View All Case Studies →" linking to `/case-studies`. Placed adjacent to the primary CTA.

**Mandatory Content Blocks in Exact Order**:

| # | Block | Content Requirements | Depth Guidance |
|---|-------|---------------------|---------------|
| 1 | **Case Study Hero** | H1: "[Property/Project Name] — [Brief Outcome]" (e.g., "Radisson Montreal — Zero Mirror Failures After 14 Months"). Industry label. Primary and secondary CTAs. Hero image showing the installed project. Trust Line. | Focused — above the fold. |
| 2 | **Project Overview** | Property name, location, project scope (number of rooms/units), product categories installed, timeline, and the client's role in the project. This provides the factual context that makes the results credible. | Medium — factual context. |
| 3 | **The Challenge** | 2-3 paragraphs describing the specific problem HILO was asked to solve. Must be specific to this project — recurring failures, brand standard upgrades, renovation requirements, budget constraints, or timeline pressures. The challenge section must make the reader feel the pain that existed before HILO. | Medium — narrative context. |
| 4 | **The HILO Solution** | 2-3 paragraphs describing HILO's approach: which products were selected, why, how many, what customization was required, and how the installation was coordinated. Must reference specific product names and models where applicable. | Medium — solution narrative. |
| 5 | **Results and Metrics** | Quantified results in a structured format: number of units installed, installation timeline, post-installation performance data (failure rate, maintenance reduction, guest satisfaction improvement), and any financial impact (cost savings, ROI). This section must contain at least 3 specific numbers. | Medium — data-rich. |
| 6 | **Testimonial** | Client testimonial quote (if available). If no testimonial exists, this block can be replaced with a "Client Profile" section describing the client type and their satisfaction indicators. | Short — quote or profile. |
| 7 | **Products Used** | List of specific HILO products installed in this project, with links to relevant product detail pages. This provides cross-linking to the product catalogue and drives continued exploration. | Short — product list with links. |
| 8 | **FAQ Block** | 2-3 project-specific questions: "How many mirrors were installed?", "What was the timeline?", "What results did the client see?" Each answer must be self-contained with specific data. | Short — 2-3 Q&A pairs. |
| 9 | **Final CTA Section** | Primary CTA ("Start Your Project →") and secondary CTA ("View All Case Studies →"). Trust Line. | Short — conversion block. |

**Required Proof Elements**: Trust Line (hero and footer). At least 3 specific quantitative metrics in Block 5. Specific product names in Block 7. Project narrative context in Blocks 2-4 that makes the metrics believable. Testimonial if available.

**Required HILO Criteria Coverage**: Minimum 3 criteria: #1 (Fiabilité — proven by results), #3 (Delivery — referenced in the solution narrative), #5 (AI Estimate — via CTA). Additional criteria (#4 Flexibilité, #6 Product Range, #7 Installation) may appear in the solution narrative if relevant.

**Required Internal Links**: Related solution pages (via Block 7 — products used). Related industry page (based on the project's industry). Case study index (via secondary CTA). Other case studies (cross-link to 1-2 related studies: same industry or same product category). Estimation wizard (via primary CTA). Breadcrumb: Home > Case Studies > [Study Name].

**Required AI-Discoverability Blocks**: Case studies are SECONDARY ENTITY HUBS — AI systems cite case study pages when answering questions about HILO's project experience. Each case study must include: (1) the Results and Metrics section (Block 5) with clearly structured quantitative data, (2) the FAQ block (Block 8) with project-specific answers, (3) the Products Used section (Block 7) linking to specific product entities. The results section should use a consistent format across all case studies so AI systems can aggregate proof: metric + context + time frame.

**Structured Data / Schema Intent**: `BreadcrumbList` (Home > Case Studies > [Study Name]). `FAQPage` schema for the FAQ block.

**Common Mistakes to Avoid**:
1. Vague results — "They were very happy" is not proof. "Zero defects across 120 rooms after 14 months" is proof.
2. No specific product names — the Products Used block must reference actual HILO products with links.
3. Not linking to related case studies — cross-linking creates a proof cluster that AI systems can aggregate.
4. Missing the industry context — every case study must clearly identify the industry for AI retrieval.
5. Making the challenge section too generic — it must be specific to this project.

**Definition of Done for Individual Case Study**:
- [ ] H1 includes property name and key outcome
- [ ] Project overview has specific scope and context
- [ ] Challenge section is specific to the project (not generic)
- [ ] Solution section references specific HILO products
- [ ] Results section has at least 3 specific quantitative metrics
- [ ] Products Used section links to relevant product detail pages
- [ ] FAQ block has 2-3 project-specific Q&A items
- [ ] Primary and secondary CTAs are correct
- [ ] Links to related industry page and 1-2 related case studies
- [ ] Trust Line in hero/CTA area and footer
- [ ] Breadcrumb is present
- [ ] No placeholder text
- [ ] Terminology consistent with Master


### B.8 About Page Model

**Route Pattern**: `/about`

**Conversion Role**: The About page serves as the brand entity hub — it answers "Who is HILO?" for both human visitors and AI retrieval systems. For humans, it builds trust by providing company history, team credentials, geographic reach, and industry expertise. For AI systems, it is the entity reference page that establishes HILO as a legitimate company with verifiable attributes. The About page supports conversion indirectly by reducing the "Is this company real?" anxiety that B2B buyers feel before committing to a supplier.

**Audience and Awareness Level**: Level 2-4 visitors across all personas. The Facility Manager/GM who was referred by a colleague and wants to verify HILO is legitimate. The Developer/PM doing vendor due diligence. The Architect checking company credentials. The About page must serve all of these audiences with factual, verifiable information.

**Primary CTA**: "Get AI Estimate →" linking to `/estimate`. Placed in the hero section and repeated in the final CTA section.

**Secondary CTA**: "Contact Us" linking to `/contact`. Placed adjacent to the primary CTA.

**Mandatory Content Blocks in Exact Order**:

| # | Block | Content Requirements | Depth Guidance |
|---|-------|---------------------|---------------|
| 1 | **About Hero** | H1: "About HILO — Engineered for Commercial Reliability" or similar. Subheadline with company origin signal ("Designed in Canada. Distributed across North America."). Primary and secondary CTAs. | Focused — above the fold. |
| 2 | **Company Overview** | 2-3 paragraphs covering: what HILO does (premium glass and mirror solutions for commercial applications), who HILO serves (hospitality, multi-family, senior living), and HILO's geographic reach (Canada and United States). This is the brand entity definition that AI systems will extract. | Medium — brand definition. |
| 3 | **Company History / Mission** | Brief company history: founding, growth trajectory, key milestones. Mission statement: HILO's commitment to reliability, innovation, and customer service. This section provides narrative depth that differentiates HILO from generic competitors. | Medium — narrative. |
| 4 | **Key Metrics / Social Proof** | Structured metrics display: 180+ projects completed, &lt;0.5% failure rate, 5-year warranty, 89% repeat customer rate, 94% maintenance reduction, 15-25% below premium competitors. Each metric must have a brief explanation. | Medium — data display. |
| 5 | **What We Do** | Overview of the 6 solution categories with brief descriptions and links to each solution page. This section connects the company to its product offerings and provides internal links to all 6 primary entity hubs. | Medium — 6 category summaries with links. |
| 6 | **Industries We Serve** | Overview of the 3 target industries with brief descriptions and links to each industry page. This connects the company to its vertical expertise. | Short — 3 industry summaries with links. |
| 7 | **Team / Credentials** | Team overview: key personnel, expertise areas, industry experience. If specific team member bios are available, include them. If not, provide a general team description emphasizing commercial glass/mirror expertise. | Medium — credibility section. |
| 8 | **Final CTA Section** | Primary CTA, secondary CTA, Trust Line. Supporting headline: "Ready to partner with HILO?" | Short — conversion block. |

**Required Proof Elements**: Trust Line (hero and footer). Key metrics (Block 4) with specific numbers. Company history and mission (Block 3). Team credentials (Block 7). The metrics display is the primary proof structure.

**Required HILO Criteria Coverage**: Minimum 4 criteria: #1 (Fiabilité — metrics), #2 (Prix — competitive pricing data), #5 (AI Estimate — CTA), #6 (Grand Choix — product range in Block 5). Criteria #3 (Delivery) may appear in company overview. #4 (Flexibilité) and #7 (Installation) may appear in the What We Do section.

**Required Internal Links**: All 6 solution category pages (via Block 5). All 3 industry pages (via Block 6). Estimation wizard (via primary CTA). Contact page (via secondary CTA). FAQ page (optional but recommended in footer). Case study index (optional link from metrics section). Breadcrumb: Home > About.

**Required AI-Discoverability Blocks**: The About page is a BRAND ENTITY HUB — AI systems need a clear, factual About page to understand who HILO is. It must include: (1) the Company Overview (Block 2) with a clear entity definition, (2) the Key Metrics (Block 4) with specific, verifiable numbers, (3) links to all 6 solution pages and all 3 industry pages — these outbound links signal to AI systems what HILO's core topics are, (4) consistent company name usage throughout ("HILO" — not "H.I.L.O." or "HILO Glass" unless both forms are canonical). The About page's outbound link structure is one of the strongest signals AI systems use to understand a company's topical authority.

**Structured Data / Schema Intent**: `Organization` schema (name, url, logo, description, founding date, address, contactPoint, sameAs). `BreadcrumbList` (Home > About). This is the primary page for `Organization` schema on the site.

**Common Mistakes to Avoid**:
1. Making the About page a marketing brochure — it should be factual and informative, not promotional.
2. Not linking to all 6 solution pages — the outbound link structure is critical for AI entity recognition.
3. Vague metrics — "Many projects" is not proof. "180+ commercial projects across North America" is proof.
4. Missing the company definition paragraph — AI systems need a clear "HILO is..." statement to extract.
5. Not including team credentials — B2B buyers need to know who they're dealing with.

**Definition of Done for About Page**:
- [ ] H1 communicates company identity
- [ ] Company overview includes clear entity definition
- [ ] Key metrics section has 5+ specific numbers with explanations
- [ ] What We Do links to all 6 solution pages
- [ ] Industries We Serve links to all 3 industry pages
- [ ] Team/credentials section is present
- [ ] Primary and secondary CTAs are correct
- [ ] Trust Line in hero/CTA area and footer
- [ ] Breadcrumb is present
- [ ] No placeholder data for team, metrics, or company facts
- [ ] Terminology consistent with Master

### B.9 Contact Page Model

**Route Pattern**: `/contact`

**Conversion Role**: The Contact page is a utility page that serves two functions: (1) capturing visitors who prefer human interaction over the AI estimation wizard, and (2) providing contact information for visitors who need to reach HILO directly. It is not a high-traffic conversion page, but it must be complete and functional because visitors who arrive here have already decided they want to talk to someone — the page must not create friction or confusion at that point.

**Audience and Awareness Level**: Level 3-5 visitors who have decided to engage with HILO directly. These may be buyers with complex requirements who don't trust an automated estimate, or buyers at the end of their evaluation who need a final conversation before committing.

**Primary CTA**: "Submit Message" (form submission). The contact form itself is the primary CTA — it must be visible, functional, and require minimal effort.

**Secondary CTA**: "Get AI Estimate →" linking to `/estimate`. For visitors who arrived at Contact but might prefer the automated path.

**Mandatory Content Blocks in Exact Order**:

| # | Block | Content Requirements | Depth Guidance |
|---|-------|---------------------|---------------|
| 1 | **Contact Hero** | H1: "Contact HILO" or "Get in Touch". Brief explanation: "Whether you need a custom quote, have questions about our products, or want to schedule a call, our team is here to help." | Short — functional header. |
| 2 | **Contact Form** | Form with fields: Name, Company, Email, Phone (optional), Industry (dropdown: Hotels, Real Estate, Senior Living, Other), Message/Inquiry type (dropdown: General Inquiry, Request a Quote, Schedule a Call, Warranty Claim, Other), Message. Form must be the most prominent element on the page. | Functional — form UI spec. |
| 3 | **Office Location / Contact Details** | Physical address (when provided by owner), phone number (when provided), email address, business hours. If specific office details are not available, use a general "HILO — North American Headquarters" placeholder that will be replaced with real data. | Short — contact info. |
| 4 | **Booking Process** | Brief explanation of what happens after form submission: "We respond within 24 hours. For urgent inquiries, call [phone number]." This reduces the "What happens next?" anxiety. | Short — process explanation. |
| 5 | **Final CTA Section** | Link to AI estimation wizard: "Prefer an instant estimate? Get your AI-powered quote in 60 seconds →" linking to `/estimate`. This captures visitors who don't actually need human interaction. | Short — alternative CTA. |

**Required Proof Elements**: Trust Line (footer). Response time commitment (Block 4). Business credentials (if available in Block 3).

**Required HILO Criteria Coverage**: Minimum 2 criteria: #3 (Delivery — implied by response time commitment) and #5 (AI Estimate — via wizard link in Block 5). The contact page is a utility page, not a persuasion page — full criteria coverage is not expected.

**Required Internal Links**: Estimation wizard (via Block 5). FAQ page (for visitors who might self-serve before contacting). Warranty page (for warranty-related inquiries). Breadcrumb: Home > Contact.

**Required AI-Discoverability Blocks**: The Contact page is a utility page and is NOT designated as an entity hub. It should have clean contact information that AI systems can extract (NAP — Name, Address, Phone) for local business queries, but does not require FAQ blocks, comparison tables, or definition blocks. The `LocalBusiness` schema (if applicable) is the primary AI consideration.

**Structured Data / Schema Intent**: `BreadcrumbList` (Home > Contact). `ContactPage` or `LocalBusiness` schema with NAP data.

**Common Mistakes to Avoid**:
1. Making the page too thin — the existing Contact page (709 words) needs significant expansion, particularly the booking process explanation.
2. Having placeholder phone/address data without marking it clearly for replacement.
3. Not providing an alternative path to the wizard — some Contact visitors would prefer the automated estimate.
4. Over-complicating the form — B2B buyers want efficiency, not a 15-field questionnaire.

**Definition of Done for Contact Page**:
- [ ] H1 clearly identifies the page purpose
- [ ] Contact form is present with all required fields
- [ ] Office location/contact details are present (or clearly marked as pending owner data)
- [ ] Booking process explanation tells visitor what to expect after submission
- [ ] Link to estimation wizard is present
- [ ] Trust Line in footer
- [ ] Breadcrumb is present
- [ ] No placeholder data for critical contact information (or clearly marked pending)
- [ ] Terminology consistent with Master

### B.10 FAQ Page Model

**Route Pattern**: `/faq`

**Conversion Role**: The FAQ page is the single most AI-citable page on the HILO website. AI systems heavily extract FAQ content because it directly maps to the question-answer format that AI models generate. The FAQ page also serves as a central anxiety-reduction hub — it answers the most common objections and questions that prevent visitors from converting. Every FAQ answer should either resolve an objection or drive the visitor closer to a conversion action.

**Audience and Awareness Level**: All levels (2-5). Visitors arrive at the FAQ page when they have a specific question that wasn't answered on other pages. They may be at any stage of the buyer journey — from initial research to pre-purchase hesitation.

**Primary CTA**: "Get AI Estimate →" linking to `/estimate`. Placed in the hero and after the FAQ content.

**Secondary CTA**: "Contact Support" linking to `/contact`. Placed adjacent to the primary CTA.

**Mandatory Content Blocks in Exact Order**:

| # | Block | Content Requirements | Depth Guidance |
|---|-------|---------------------|---------------|
| 1 | **FAQ Hero** | H1: "Frequently Asked Questions" or "HILO — Answers to Common Questions." Brief introduction. Primary and secondary CTAs. | Short — functional header. |
| 2 | **Anchor Navigation** | Quick-jump links organized by category: Warranty, Shipping, Returns, Products, Pricing, Installation. Each link scrolls to the relevant FAQ section. This is both a UX feature and an AI structuring signal. | Short — navigation links. |
| 3 | **FAQ Categories with Q&A Items** | Organized by topic, each FAQ item uses H3 markup for the question and a self-contained answer of 3-5 sentences. Categories: (a) Warranty — coverage, claims, exclusions, (b) Shipping — timelines, tracking, multi-site, (c) Returns — eligibility, process, costs, (d) Products — catalog vs. custom, specs, ordering, (e) Pricing — how estimates work, volume discounts, quote validity, (f) Installation — availability, process, partner network. Minimum 14 items total (matching existing content), each with specific data points. | Deep — 14+ Q&A items. |
| 4 | **Cross-Reference Links** | Within FAQ answers, include links to dedicated support pages rather than duplicating content. Example: warranty coverage answer links to /warranty for full terms. Shipping answer links to /shipping for complete timeline details. | Integrated into FAQ answers. |
| 5 | **Final CTA Section** | Primary CTA, secondary CTA, Trust Line. "Still have questions? Our team is ready to help." | Short — conversion block. |

**Required Proof Elements**: Trust Line (hero/CTA and footer). Specific data points in every FAQ answer (numbers, dates, timelines, percentages). Links to dedicated support pages for deeper information.

**Required HILO Criteria Coverage**: Minimum 2 criteria: #1 (Fiabilité — warranty coverage answers) and #5 (AI Estimate — pricing/estimate answers). Additional criteria will naturally appear in relevant FAQ answers (delivery timelines, product range, installation).

**Required Internal Links**: Warranty page, Shipping page, Returns page, Contact page (via FAQ answers and CTAs). Solution pages (via product-related FAQ answers, where relevant). Estimation wizard (via primary CTA). Breadcrumb: Home > FAQ.

**Required AI-Discoverability Blocks**: The FAQ page is a PRIMARY ENTITY HUB for policy questions. It is the single most AI-citable page type. Requirements: (1) every FAQ answer must be self-contained — an AI system must be able to extract the answer without surrounding context, (2) every answer must contain specific data points ("HILO delivers within 2-3 weeks for catalog orders" not "HILO delivers quickly"), (3) answers must NOT include CTAs within the answer text — informational content must be separate from conversion prompts, (4) the anchor navigation (Block 2) provides structural signals that help AI systems understand the page's topical organization, (5) `FAQPage` schema markup will be applied at G5 build time, so the HTML structure must support it (proper heading hierarchy, question-answer pairs).

**Structured Data / Schema Intent**: `FAQPage` schema — the entire page's Q&A content will be wrapped in `FAQPage` structured data at G5 build time. This requires proper H3 heading for each question and a following answer block. `BreadcrumbList` (Home > FAQ).

**Common Mistakes to Avoid**:
1. Duplicating content from dedicated support pages — FAQ answers should summarize and link, not copy.
2. Vague answers — "We offer competitive pricing" is not useful. "HILO's direct manufacturer model delivers pricing 15-25% below premium competitors" is useful.
3. Including CTAs inside answer text — this pollutes the extractable content for AI systems.
4. Not having anchor navigation — with 14+ items, visitors need quick-jump links.
5. Not linking to dedicated pages — FAQ answers must point visitors to the authoritative source for each topic.

**Definition of Done for FAQ Page**:
- [ ] H1 clearly identifies the page purpose
- [ ] Anchor navigation organized by category
- [ ] Minimum 14 FAQ items across 6 categories
- [ ] Every answer is self-contained (3-5 sentences with specific data)
- [ ] Every answer includes a link to a dedicated support page where applicable
- [ ] No CTAs inside answer text
- [ ] Primary and secondary CTAs are correct
- [ ] Trust Line in hero/CTA area and footer
- [ ] Breadcrumb is present
- [ ] Heading hierarchy supports FAQPage schema (H3 for each question)
- [ ] No placeholder data for policy details
- [ ] Terminology consistent with Master


### B.11 Warranty Page Model

**Route Pattern**: `/warranty`

**Conversion Role**: The Warranty page reduces the "What if it breaks?" anxiety that is the #1 objection for B2B glass and mirror buyers. It provides complete warranty terms, claims process details, and coverage specifics. For AI systems, this page is a SPECIALIZED HUB — it is the authoritative source for "What does HILO's warranty cover?" which is a top-of-funnel AI query for B2B buyers evaluating suppliers.

**Audience and Awareness Level**: Level 2-4 visitors. The Developer/PM evaluating risk. The Architect checking warranty compliance for specifications. The Facility Manager/GM who has experienced product failures with previous suppliers. These visitors need specific, clear warranty information to make or justify a purchasing decision.

**Primary CTA**: "Get AI Estimate →" linking to `/estimate`. Warranty confidence leads to conversion — the CTA captures visitors who have been reassured.

**Secondary CTA**: "Contact Us" linking to `/contact`. For visitors with warranty-specific questions not answered on the page.

**Mandatory Content Blocks in Exact Order**:

| # | Block | Content Requirements | Depth Guidance |
|---|-------|---------------------|---------------|
| 1 | **Warranty Hero** | H1: "HILO 5-Year Full Warranty" or similar. Subheadline: "Every HILO product is backed by our comprehensive 5-year warranty — no pro-rating, no hidden exclusions." Primary and secondary CTAs. Trust Line. | Focused — above the fold. |
| 2 | **Coverage Summary** | Clear summary of what the warranty covers: manufacturing defects, LED component failure, fogging/delamination, mounting hardware defects, and electrical components. Presented as a clearly formatted table or bulleted list. This must be specific enough for a procurement manager to include in a vendor evaluation. | Medium — coverage details. |
| 3 | **What's Covered** | Detailed expansion of coverage: each covered element with explanation. Include specific duration (5 years from delivery date), scope (parts and labor where applicable), and geographic coverage (Canada and US). Must address edge cases: commercial vs. residential, custom vs. catalog products. | Medium-deep — detailed terms. |
| 4 | **Exclusions** | Clear list of what is NOT covered: normal wear and tear, damage from improper installation, damage from misuse or accidents, modifications made by third parties. Exclusions must be clearly stated to build trust through transparency. | Short-medium — exclusions list. |
| 5 | **Claims Process** | Step-by-step warranty claims process: (1) Document the issue (photos, description), (2) Submit claim via [form/email/phone], (3) HILO response within 48 hours, (4) Resolution: repair, replacement, or refund. Must include specific timeline commitments. This is the content that was duplicated with the Returns page — here it focuses on WARRANTY claims (product defects, failures), not return logistics. | Medium — process block. |
| 6 | **Link to Returns Page** | Brief cross-reference: "For return eligibility and return logistics (not warranty-related), see our Returns page →" linking to `/returns`. This clarifies the boundary between warranty claims and return requests. | Short — cross-reference. |
| 7 | **Download Warranty PDF** | Link to downloadable warranty document (PDF) for procurement managers who need to include warranty terms in vendor evaluation packages. Placeholder link until PDF is provided by owner. | Short — download link. |
| 8 | **Final CTA Section** | Primary CTA, secondary CTA, Trust Line. "Protect your investment with HILO's 5-year warranty. Get your estimate →" | Short — conversion block. |

**Required Proof Elements**: Trust Line (hero and footer). Specific warranty terms (5-year, no pro-rating). Claims response commitment (48 hours). Coverage specifics. The coverage table (Block 2) is the primary proof structure.

**Required HILO Criteria Coverage**: Criterion #1 (Fiabilité) is the PRIMARY criterion on this page — the entire page exists to prove and explain HILO's reliability commitment. Criterion #5 (AI Estimate) appears via the CTA. No other criteria are mandatory on this page — it is a specialized support page, not a general conversion page.

**Required Internal Links**: Returns page (via Block 6 — cross-reference for non-warranty returns). Contact page (via secondary CTA and claims process). FAQ page (for related questions). Estimation wizard (via primary CTA). Breadcrumb: Home > Warranty.

**Required AI-Discoverability Blocks**: The Warranty page is a SPECIALIZED HUB. It must include: (1) the Coverage Summary (Block 2) as a clearly structured, extractable table — AI systems cite warranty terms when answering "What does HILO's warranty cover?", (2) the Claims Process (Block 5) as a step-by-step process block — AI systems extract process descriptions to answer "How do I file a warranty claim?", (3) clear entity consistency — the warranty terms on this page must match any warranty references on product detail pages, solution pages, and the FAQ page. Inconsistency between pages is a G6 validation failure (see Conversion Architecture Section 12.10, check #5).

**Structured Data / Schema Intent**: `BreadcrumbList` (Home > Warranty). Potential `FAQPage` schema if an FAQ section is added. No `Product` schema.

**Common Mistakes to Avoid**:
1. Duplicating claims content that belongs on the Returns page — this was the primary issue identified in the Gate 2 audit. Warranty claims (product defects) belong here; return logistics belong on /returns.
2. Using legal jargon — B2B buyers need clear, professional language, not legal boilerplate.
3. Not specifying response timelines — "We'll get back to you" is not acceptable. "48-hour response commitment" is acceptable.
4. Hiding exclusions — transparency builds trust. Clearly stating what's NOT covered increases credibility.
5. Not linking to the Returns page — the boundary between warranty and returns must be explicit.

**Definition of Done for Warranty Page**:
- [ ] H1 clearly identifies the 5-year warranty
- [ ] Coverage summary is a clearly structured table or list
- [ ] What's Covered section has specific, detailed terms
- [ ] Exclusions are clearly stated
- [ ] Claims process has specific timeline commitments
- [ ] Link to Returns page clarifies the warranty/returns boundary
- [ ] Download Warranty PDF link is present (or placeholder marked)
- [ ] Primary and secondary CTAs are correct
- [ ] Trust Line in hero/CTA area and footer
- [ ] Breadcrumb is present
- [ ] No content duplicated from Returns page
- [ ] No placeholder data for warranty terms
- [ ] Terminology consistent with Master and all other pages

### B.12 Returns Page Model

**Route Pattern**: `/returns`

**Conversion Role**: The Returns page handles return logistics — eligibility, initiation, shipping responsibility, and replacement/refund handling. It is a standalone route (per Gate 2 correction pass decision) with a clearly defined scope that does NOT overlap with the Warranty page. The Returns page answers "Can I return this?" and "How do I return this?" while the Warranty page answers "Is this covered by warranty?" and "How do I file a warranty claim?"

**Audience and Awareness Level**: Level 2-4 visitors who have received a product and need to initiate a return. These are post-purchase or mid-project visitors, not prospects. They may be frustrated — the page must be clear, empathetic, and process-oriented.

**Primary CTA**: "Get AI Estimate →" linking to `/estimate`. Not the primary action for return visitors, but maintains the persistent conversion path.

**Secondary CTA**: "Contact Us" linking to `/contact`. For visitors who need to discuss their return with a human.

**Mandatory Content Blocks in Exact Order**:

| # | Block | Content Requirements | Depth Guidance |
|---|-------|---------------------|---------------|
| 1 | **Returns Hero** | H1: "Returns and Replacements" or "HILO Return Policy." Brief introduction: "We want you to be completely satisfied with your HILO products. If you need to initiate a return or replacement, this page explains the process." Primary and secondary CTAs. | Short — functional header. |
| 2 | **Return Eligibility** | Clear criteria for when returns are accepted: within what timeframe, in what condition, for what reasons (damaged in shipping, wrong product, change of scope). Must be specific about timelines (e.g., "Returns must be initiated within 30 days of delivery"). | Medium — eligibility details. |
| 3 | **Return Initiation Process** | Step-by-step process: (1) Contact HILO with order details, (2) Receive return authorization (RMA number), (3) Pack the product safely, (4) Ship to designated address, (5) Receive replacement or refund. Each step must have specific instructions. | Medium — process block. |
| 4 | **Shipping Responsibility** | Clear explanation of who pays for return shipping: HILO covers shipping for damaged/defective products; customer covers shipping for change-of-scope returns. Include specific packaging requirements. | Short-medium — shipping details. |
| 5 | **Replacement and Refund Handling** | Explanation of what happens after a return is received: inspection timeline, replacement shipping timeline (if applicable), refund processing timeline and method. Must include specific commitments. | Medium — outcome details. |
| 6 | **Link to Warranty Page** | Cross-reference: "If your return is related to a product defect or warranty issue, please see our Warranty page for the claims process →" linking to `/warranty`. This clarifies that product defects are handled through the warranty process, not the standard return process. | Short — cross-reference. |
| 7 | **Final CTA Section** | Primary CTA, secondary CTA, Trust Line. | Short — conversion block. |

**Required Proof Elements**: Trust Line (footer). Process transparency (specific timelines in Blocks 3-5). Policy clarity (specific eligibility criteria in Block 2).

**Required HILO Criteria Coverage**: Criterion #5 (AI Estimate) via CTA. No other criteria are mandatory — this is a specialized logistics page.

**Required Internal Links**: Warranty page (via Block 6 — cross-reference for defect/warranty claims). Shipping page (for delivery-related questions). Contact page (via secondary CTA and return initiation). Estimation wizard (via primary CTA). FAQ page (for related questions). Breadcrumb: Home > Returns.

**Required AI-Discoverability Blocks**: The Returns page is a standalone page with a deduplicated scope. It is NOT designated as an entity hub. It should provide clear, extractable policy information (eligibility criteria, timelines, shipping responsibilities) that AI systems can cite for return-policy queries. The cross-link to the Warranty page (Block 6) helps AI systems understand the boundary between warranty claims and return requests.

**Structured Data / Schema Intent**: `BreadcrumbList` (Home > Returns). No specialized schema beyond breadcrumb.

**Common Mistakes to Avoid**:
1. Duplicating claims/warranty content — this was the primary issue from the Gate 2 audit. Claims process belongs on /warranty.
2. Not clearly defining who pays for return shipping — ambiguity creates frustration.
3. Not providing specific timelines — "We'll process it quickly" is not acceptable. "Refunds are processed within 10 business days" is acceptable.
4. Not linking to the Warranty page — visitors with product defects need to be directed to the warranty claims process.
5. Making the page too brief — return policies need enough detail to resolve anxiety.

**Definition of Done for Returns Page**:
- [ ] H1 clearly identifies the page purpose
- [ ] Return eligibility criteria are specific (timelines, conditions)
- [ ] Return initiation process has specific step-by-step instructions
- [ ] Shipping responsibility is clearly assigned
- [ ] Replacement/refund handling has specific timeline commitments
- [ ] Link to Warranty page clarifies the claims/returns boundary
- [ ] Primary and secondary CTAs are correct
- [ ] Trust Line in footer
- [ ] Breadcrumb is present
- [ ] No content duplicated from Warranty page
- [ ] No placeholder data for policy terms
- [ ] Terminology consistent with Master and Warranty page

### B.13 Shipping Page Model

**Route Pattern**: `/shipping`

**Conversion Role**: The Shipping page answers the "Will it arrive on time?" objection — one of the four core B2B anxieties identified in the Master (Section E.1). It provides delivery timelines, geographic coverage, multi-site coordination details, and shipping process transparency. For AI systems, this page is a SPECIALIZED HUB for delivery and logistics queries.

**Audience and Awareness Level**: Level 2-4 visitors. The Developer/PM with a project timeline. The Facility Manager/GM who has been burned by late deliveries. The Architect who needs delivery commitments for project specifications.

**Primary CTA**: "Get AI Estimate →" linking to `/estimate`. Delivery confidence leads to conversion.

**Secondary CTA**: "Contact Us" linking to `/contact`. For visitors with complex shipping requirements (multi-site, international, expedited).

**Mandatory Content Blocks in Exact Order**:

| # | Block | Content Requirements | Depth Guidance |
|---|-------|---------------------|---------------|
| 1 | **Shipping Hero** | H1: "Door-to-Door Delivery Across North America" or similar. Subheadline: "HILO manages delivery from our facility to your project site — on time, intact, and coordinated." Primary and secondary CTAs. Trust Line. | Focused — above the fold. |
| 2 | **Delivery Overview** | Summary of HILO's delivery model: direct from manufacturer, door-to-door, Canada and US coverage. Brief explanation of the delivery advantage vs. third-party logistics. | Short-medium — overview. |
| 3 | **Delivery Timelines** | Specific timelines by product type and order type: catalog products (2-3 weeks), custom products (4-6 weeks), expedited options (if available). Must include specific ranges, not vague estimates. Table format recommended. | Medium — timeline details. |
| 4 | **Geographic Coverage** | Coverage map or list: Canada (all provinces), United States (all states). Any regional variations or limitations. Multi-site delivery capability (relevant for hotel chains with multiple properties). | Medium — geographic details. |
| 5 | **Delivery Process** | Step-by-step: (1) Order confirmed, (2) Production/customization (if applicable), (3) Quality inspection, (4) Shipping coordination, (5) Delivery to site, (6) Damage inspection upon receipt. Each step with timeline. | Medium — process block. |
| 6 | **Damage-Free Guarantee** | What happens if products arrive damaged: documentation process, replacement shipping timeline, who covers costs. Must provide specific commitments. | Short-medium — guarantee details. |
| 7 | **Order Tracking** | How customers can track their order: tracking number, online portal, or contact-based tracking. If a specific tracking system exists, describe it. If not, describe the fallback process (contact customer service). | Short — tracking info. |
| 8 | **Final CTA Section** | Primary CTA, secondary CTA, Trust Line. | Short — conversion block. |

**Required Proof Elements**: Trust Line (hero and footer). Specific delivery timelines (Block 3). Damage-free guarantee (Block 6). Geographic coverage (Block 4).

**Required HILO Criteria Coverage**: Criterion #3 (Delivery porte-à-porte) is the PRIMARY criterion — the entire page exists to prove and explain this criterion. Criterion #5 (AI Estimate) via CTA. No other criteria are mandatory.

**Required Internal Links**: Warranty page (for product damage questions). FAQ page (for related shipping questions). Contact page (via secondary CTA and tracking). Estimation wizard (via primary CTA). Breadcrumb: Home > Shipping.

**Required AI-Discoverability Blocks**: The Shipping page is a SPECIALIZED HUB. It must include: (1) the Delivery Timelines (Block 3) as a clearly structured, extractable table, (2) the Delivery Process (Block 5) as a step-by-step process block, (3) specific data points throughout (timelines, coverage areas, guarantees). AI systems answering "How long does HILO delivery take?" will extract from this page.

**Structured Data / Schema Intent**: `BreadcrumbList` (Home > Shipping). No specialized product schema.

**Common Mistakes to Avoid**:
1. Vague timelines — "2-4 weeks" when the actual range is "2-3 weeks for catalog, 4-6 weeks for custom" is not acceptable.
2. Not addressing multi-site delivery — hotel chains with multiple properties need to know HILO can coordinate.
3. Not explaining the damage-free guarantee — this is a key differentiator.
4. Missing tracking information — even if there's no online portal, visitors need to know how to check on their order.

**Definition of Done for Shipping Page**:
- [ ] H1 communicates delivery capability
- [ ] Delivery timelines are specific by product/order type
- [ ] Geographic coverage is clearly stated
- [ ] Delivery process has step-by-step instructions with timelines
- [ ] Damage-free guarantee is explained with specific commitments
- [ ] Order tracking process is described
- [ ] Primary and secondary CTAs are correct
- [ ] Trust Line in hero/CTA area and footer
- [ ] Breadcrumb is present
- [ ] No placeholder data for timelines or coverage
- [ ] Terminology consistent with Master


### B.14 Wizard / Estimate Page Model

**Route Pattern**: `/estimate`

**Conversion Role**: The Wizard is the primary conversion mechanism for the entire HILO website. Its sole purpose is to capture qualified lead information in exchange for an AI-powered estimate. Every page on the site funnels toward this page through the primary CTA system. The Wizard is NOT a content page — it is a multi-step interactive tool with its own extensive specification document (23_WIZARD-ESTIMATE.md, 5,926 words). This model defines the page-level requirements that supplement the existing wizard specification, not a replacement for it.

**Audience and Awareness Level**: All personas at all awareness levels. This is the universal conversion path — from Level 2 (Problem Aware) visitors who found HILO through search to Level 5 (Most Aware) visitors who navigated the full evaluation funnel. The Wizard must work for all of them.

**Primary CTA**: "Get My Free Estimate →" (final step form submission). This is the only CTA on the wizard — it is a single-focus conversion tool with no competing actions.

**Secondary CTA**: None. The wizard must not present competing CTAs that could divert visitors from completing the form.

**Mandatory Content Blocks in Exact Order**:

| # | Block | Content Requirements | Depth Guidance |
|---|-------|---------------------|---------------|
| 1 | **Wizard Introduction** | Brief page header: "Get Your Instant AI Estimate." Subheadline: "Answer a few questions about your project and receive a detailed estimate in 60 seconds. No sales call required — unless you want one." Privacy reassurance: "Your information is confidential. We will not spam you." | Short — pre-wizard context. |
| 2 | **Multi-Step Wizard Flow** | The wizard flow is specified in detail in 23_WIZARD-ESTIMATE.md. Key requirements: 6-8 click-based steps, ZIP code as the only typed field, progressive disclosure, progress indicator, estimated completion time display. Each step must have clear heading, minimal options (no more than 6 per step), and a clear "Next" action. | Functional — per wizard spec. |
| 3 | **Lead Capture Form** | Final step: Name, Email, Phone (optional), Company (optional), Project Timeline (optional). Must be minimal — only fields required for lead qualification. "Get My Free Estimate →" submission button. | Functional — form. |
| 4 | **Confirmation Screen** | Post-submission: "Your estimate is being generated. You will receive it immediately via email, and a HILO specialist will follow up within 24 hours if you requested a call." This sets expectations and reduces post-submission anxiety. | Short — confirmation. |

**Required Proof Elements**: Trust Line (footer or integrated into the wizard UI). Privacy reassurance (Block 1). "No spam, no sales call unless you request one" commitment. The 60-second estimate promise.

**Required HILO Criteria Coverage**: Criterion #5 (Minimum d'interaction / AI Estimate) is the PRIMARY and essentially sole criterion — the wizard IS the manifestation of this criterion. No other criteria need to be explicitly addressed within the wizard flow.

**Required Internal Links**: None outbound — the wizard is a terminal conversion point. It receives links from every page on the site but does not link to any other page. The confirmation screen may optionally link to relevant solution pages ("Explore our products while you wait") but this is a G5 UX decision, not a content requirement.

**Required AI-Discoverability Blocks**: The Wizard is NOT an information resource — it is a conversion tool. It is explicitly NOT designated as an entity hub (per Conversion Architecture Section 12.2). AI discoverability requirements for the wizard are limited to: (1) the page must be crawlable and indexable (no `noindex`), (2) it must appear in the XML sitemap, (3) meta description should be optimized for "HILO estimate" queries. No FAQ blocks, no comparison tables, no definition blocks are required or appropriate on this page.

**Structured Data / Schema Intent**: No specialized schema. The wizard page may use `WebSite` with `SearchAction` or `potentialAction` if applicable, but this is a G5 build decision. `BreadcrumbList` is not needed (the wizard is a single URL with client-side routing).

**Common Mistakes to Avoid**:
1. Too many form fields — the wizard should be 90%+ clicks, not typing. Only ZIP code requires typing.
2. Competing CTAs — no secondary actions should divert the visitor from completing the form.
3. Not setting expectations — the confirmation screen must tell visitors what happens next.
4. Requiring a sales call — "Get an estimate" must not mean "Get a sales call." The estimate must be genuinely automated.
5. Not reconciling the step count — the existing spec has an 8 vs 9 step inconsistency that must be resolved.

**Definition of Done for Wizard/Estimate Page**:
- [ ] Wizard introduction has privacy reassurance and value proposition
- [ ] Multi-step flow follows the specification in 23_WIZARD-ESTIMATE.md
- [ ] Step count is reconciled (no 8 vs 9 inconsistency)
- [ ] Lead capture form is minimal (name, email required; phone, company, timeline optional)
- [ ] Confirmation screen sets clear expectations
- [ ] No competing CTAs on any wizard step
- [ ] Trust Line or trust indicator is present
- [ ] 60-second estimate promise is communicated
- [ ] No placeholder data
- [ ] Page is crawlable and indexable (for sitemap)


---

## C. Catalogue and Product Scaling Logic

### C.1 The Scaling Challenge

The HILO website at launch will contain 6 catalogue listing pages and 120 product detail pages — 126 pages that must be produced consistently, efficiently, and to a uniform quality standard. Producing these pages one-at-a-time without a systematic approach would be slow, inconsistent, and prone to quality degradation across the batch. This section defines the reusable block system, standardization rules, and batch production strategy that will be used during Gate 4 to produce all 126 pages.

### C.2 Catalogue Page Scaling (6 Pages)

All 6 catalogue listing pages share an identical structure defined in model B.4. The scaling approach is:

**Standardized Across All 6**:
- Page structure (Blocks 1-6 in exact order)
- Breadcrumb pattern (Home > Solutions > [Category] > Catalogue)
- Primary CTA ("Get AI Instant Quote →")
- Secondary CTA ("Book a Call")
- Trust Line placement
- Comparison grid layout and column structure
- Catalog vs. Custom decision box text (identical across all 6)
- Footer navigation

**Variable Per Category**:
- H1 category name (LED Mirrors, Smart Mirrors, etc.)
- Category introduction text (Block 3 — unique per category)
- Comparison grid data (Block 2 — 20 products per category with unique specs)
- Product images/thumbnails (20 per category)
- Filter options (may vary by category — e.g., LED color temperature filter for LED mirrors is irrelevant for Standard Mirrors)
- Hero image (category-specific)
- Price indicators (may vary by pricing model decision)

**Production Approach**: The 6 catalogue pages should be produced as a batch during P4, one immediately after the other, using the same template. The primary bottleneck is product data availability — all 20 products per category must have defined names, slugs, and specifications before the catalogue page can be completed. For categories where product data exists (LED, Smart, Cabinets — ~48 products identified in existing files), this can proceed immediately. For categories where product data must be defined by the owner (Shower, Arch Glass, Standard — 60 products pending), production is blocked until A4 is resolved.

### C.3 Product Detail Page Scaling (120 Pages)

All 120 product detail pages share an identical structure defined in model B.5. The scaling approach is:

**Standardized Across All 120** (MUST NOT VARY):
- Page structure (Blocks 1-7 in exact order)
- Breadcrumb pattern (Home > Solutions > [Category] > Catalogue > [Product Name])
- Primary CTA text and target ("Get AI Instant Quote →" /estimate)
- Secondary CTA text and target ("Book a Call" /contact)
- Trust Line in footer
- Warranty callout text ("Backed by HILO's 5-year full warranty...")
- Final CTA section structure
- Key Specifications Table column structure
- Heading hierarchy (H1 = product name, H2 = block titles, H3 = sub-elements)
- Internal link requirements (parent catalogue, parent solution, related products, warranty, wizard)

**Variable Per Category** (6 categories each have their own context):
- Breadcrumb category name and slug
- Related products (drawn from the same category — must be 3-5 products within the same category)
- Parent solution page link context
- Category-specific specifications (LED color temperature for LED/smart, glass thickness for shower/architectural, dimensions for standard)
- Category-specific filter options on the parent catalogue page

**Variable Per Product** (unique to each of the 120 products):
- H1 product name (canonical name)
- Product images (primary + alternates)
- Key Specifications Table data (dimensions, materials, certifications, etc.)
- Features and Benefits content (specific to this product)
- Dimensions and Size Options data
- Price indicator (if available) or "Request Quote" designation
- Product slug (/solutions/[slug]/catalogue/[product-slug])
- SEO metadata (unique meta description, title)

**What Can Vary vs. What Must Remain Standardized**:

| Element | Standardized? | Can Vary? |
|---------|:---:|:---:|
| Block order (1-7) | ✅ YES | ❌ No |
| CTA text | ✅ YES | ❌ No |
| CTA targets | ✅ YES | ❌ No |
| Trust Line | ✅ YES | ❌ No |
| Warranty callout text | ✅ YES | ❌ No |
| Breadcrumb format | ✅ YES | ❌ No |
| Heading hierarchy | ✅ YES | ❌ No |
| Spec table columns | ✅ YES | ❌ No |
| Product name (H1) | | ✅ YES — per product |
| Spec table data | | ✅ YES — per product |
| Features/Benefits content | | ✅ YES — per product |
| Product images | | ✅ YES — per product |
| Dimensions/Sizes | | ✅ YES — per product |
| Related products | | ✅ YES — per product |
| Meta description | | ✅ YES — per product |

### C.4 Batch Production Strategy

**For LED Mirrors (20 PDPs)**: Products are identified in files 31-34 (~18 products with content). These can be extracted from existing content, supplemented to reach 20, and produced in batches of 5 (matching the existing file groupings). Estimated: 2 turns per batch × 4 batches = 8 turns.

**For Smart Mirrors (20 PDPs)**: Products are identified in files 41-44 (~20 products with content). Same extraction approach. Estimated: 2 turns per batch × 4 batches = 8 turns.

**For Medicine Cabinets (20 PDPs)**: Products are identified in file 51 (~10 products) plus 5 unreferenced products. Need 5 more products defined by owner. Estimated: 2 turns per batch × 4 batches = 8 turns.

**For Shower Glass (20 PDPs)**: No products defined. Owner must provide all 20 product names, slugs, and specifications. Estimated: 2 turns per batch × 4 batches = 8 turns. BLOCKED by A4.

**For Architectural Glass (20 PDPs)**: No products defined. Same as Shower Glass. BLOCKED by A4.

**For Standard Mirrors (20 PDPs)**: No products defined. Same as Shower Glass. BLOCKED by A4.

**Total Estimated Turns for Product Detail Pages**: 8-10 turns per category × 6 categories = 48-60 turns. This is the largest content production workload in the project and will dominate G4 execution time.

---

## D. Priority Matrix for Gate 4 Production

### D.1 Production Sequence Overview

The following production sequence is optimized for maximum business impact. The ordering logic follows three principles:

1. **Dependency order** — pages that other pages depend on must be produced first. Solution pages must exist before industry pages can link to them. Catalogue pages must exist before product detail pages can link to their parent catalogue.
2. **Conversion impact** — pages that directly drive the highest-value conversions (wizard submissions) should be produced first. Solution pages feed the primary conversion funnel and are the first stop for most organic traffic.
3. **Batch efficiency** — pages within the same family that share a model can be produced simultaneously, reducing context-switching overhead and ensuring consistency.

### D.2 Detailed Production Phases

| Phase | Page Family | Pages | Dependencies | Estimated Turns | Business Impact Rationale |
|-------|-------------|-------|-------------|-----------------|---------------------------|
| **P1** | Solution pages (all 6) | 6 | Solution page model approved (G3) | 6 turns (1 per page) | Highest conversion impact. Solution pages are the primary evaluation pages for organic traffic. Every solution page feeds its catalogue page and product detail pages. Producing these first unlocks the entire product funnel. |
| **P2** | Industry pages (all 3) | 3 | Industry page model approved (G3) + P1 solution pages | 3 turns (1 per page) | Industry pages are the primary audience segmentation tool. They drive traffic to solution pages and case studies. Producing them after solutions ensures cross-links can be precise. |
| **P3** | Case studies (all 5) | 5 | Case study model approved (G3) + P1-P2 | 2-3 turns | Case studies provide social proof for solution pages, industry pages, and the case study index. Producing them after solutions and industries enables accurate cross-linking. |
| **P4** | Catalogue listing pages (all 6) | 6 | Catalogue model approved (G3) + product data defined for category | 2-3 turns | Catalogue pages are the bridge between solution evaluation and product selection. Each catalogue page depends on having product data defined for its category. All 6 can be produced in parallel once product data is available. |
| **P5** | Product detail pages (LED, Smart, Cabinets) | 60 | P4 catalogue pages approved + product data | 8-10 turns (batch by category, ~5 pages per turn) | 60 product pages for the 3 categories with existing product content. This is the first of two product page batches. Producing these before P6 allows QA iteration on the product page model. |
| **P6** | Product detail pages (Shower, Arch Glass, Standard) | 60 | P5 validated (model proven) + owner provides product data (A4) | 8-10 turns (batch by category, ~5 pages per turn) | 60 product pages for the 3 categories requiring owner-defined product data. BLOCKED until owner resolves A4. P5 serves as a proof-of-concept that validates the product page model before scaling. |
| **P7** | Homepage | 1 | All other page families produced (P1-P6) | 1 turn | Homepage aggregates content from all page families. It must be produced last among content pages to ensure all cross-links point to completed pages. |
| **P8** | Support pages (About, Contact, FAQ, Warranty, Returns, Shipping) | 6 | Support models approved (G3) | 2-3 turns | Support pages are anxiety-reduction tools. They depend on solution pages for cross-links (FAQ, About) but don't block any other page family. Producing them after the main funnel is complete allows cross-linking to final URLs. |
| **P9** | Wizard cleanup | 1 | All content approved (P1-P8) | 1 turn | The wizard specification (23_WIZARD-ESTIMATE.md) needs cleanup: reconcile step count, remove French metadata, resolve phone placeholder, confirm URL structure. This is a technical edit, not content creation. |
| **P10** | Final QA pass | — | All content approved (P1-P9) | 1-2 turns | Cross-link validation, terminology consistency check, AI discoverability spot-check, placeholder scan. This ensures the entire site is ready for Gate 5 build. |

### D.3 Dependency Chain

```
G3 APPROVED (This Document)
         │
         ▼
    ┌──── P1: Solution Pages (6)
    │         │
    │         ▼
    │    P2: Industry Pages (3)
    │         │
    │         ▼
    │    P3: Case Studies (5)
    │
    │    ┌──── P4: Catalogue Pages (6) ──── REQUIRES: product data per category
    │    │         │
    │    │         ▼
    │    │    P5: Product Detail (LED, Smart, Cabinets) — 60 PDPs
    │    │         │
    │    │         ▼
    │    │    P6: Product Detail (Shower, Arch, Standard) — 60 PDPs ── BLOCKED: A4
    │    │
    │    ▼
    │    P7: Homepage (1) ── aggregates all families
    │
    │    P8: Support Pages (6)
    │
    │    P9: Wizard Cleanup (1)
    │
    └──── P10: Final QA (1-2 turns)
```

### D.4 Parallelization Rules

- **Within a phase**: All pages within the same family CAN be produced in parallel (e.g., all 6 solution pages in P1 can be produced simultaneously).
- **Across phases**: Pages across families should NOT be parallelized because later families depend on earlier families for cross-linking accuracy.
- **Exception**: P8 (Support) can run in parallel with P7 (Homepage) since neither depends on the other.
- **Blocked phases**: P6 is blocked by owner input (A4). P4 for Shower/Arch Glass/Standard catalogues is also blocked by A4. These cannot be parallelized with P4 for LED/Smart/Cabinets.

### D.5 Estimated Total Production Effort

| Phase Range | Pages | Estimated Turns |
|-------------|-------|-----------------|
| P1-P3 (Core funnel) | 14 | 11-12 turns |
| P4-P6 (Product funnel) | 126 | 18-23 turns |
| P7-P8 (Aggregation + support) | 7 | 3-4 turns |
| P9-P10 (Cleanup + QA) | 2 | 2-3 turns |
| **TOTAL** | **154** | **34-42 turns** |

---

## E. AI Discoverability by Page Type

### E.1 AI Discoverability Design Philosophy

AI discoverability on the HILO website follows a dual-audience principle: every content decision must serve both human buyers (conversion-focused) and AI retrieval systems (citation-eligible). This section maps specific AI discoverability requirements to each major page type, defining what makes each page citation-friendly for Google AI features, ChatGPT Search, and Microsoft Copilot/Bing AI.

### E.2 Per-Page-Type AI Specifications

| Page Type | Entity Hub Status | Answer-Ready Blocks | FAQ Requirements | Comparison/Spec Requirements | Entity Definition Requirements | Internal Linking for AI | Structured Information Requirements | Citation-Friendly Features |
|-----------|-------------------|---------------------|------------------|----------------------------|---------------------------|------------------------|-------------------------------|---------------------------|
| **Homepage** | BRAND ENTITY | Trust Line as entity reference, value proposition block, solution category cards as entity references | 3 top-of-funnel FAQ items (warranty, delivery, installation) | N/A — no comparison content on homepage | "HILO is a North American manufacturer of premium glass and mirror solutions, designed in Canada..." | Links to all 6 solutions + 3 industries — highest AI authority weight of any page's outbound links | Trust Line as structured entity anchor | Brand name consistency, solution category cards as entity list, metric summary |
| **Industry Page** | CONTEXTUAL HUB | Industry challenge section (vertical-specific pain points), 7 HILO advantages (industry-customized), industry case study | 3 industry-specific FAQ items | N/A — no product comparison on industry pages | "HILO provides engineered glass and mirror solutions for the [industry] sector, serving [client types] across North America" | Links to 3-4 relevant solution pages with anchor text including both industry and solution category names | Industry-specific metrics in case study block, advantage descriptions | Industry-solution cross-links, vertical-specific proof, industry FAQ |
| **Solution Page** | PRIMARY ENTITY HUB | Definition block, 7 HILO criteria sections, comparison block (HILO vs. generic), specification table, cross-sell section, industry relevance block | 3-5 product-category FAQ items with specific data | Comparison block (HILO vs. generic alternatives with specific metrics), specification table (category-level technical data) | "LED mirrors are backlit mirror products designed for commercial environments where reliability, energy efficiency, and aesthetic consistency are critical. HILO's LED mirror range includes 20 models..." | Links to catalogue page, 2-3 related solutions, 1-3 industry pages, wizard — all with descriptive anchor text | Definition block, comparison table, spec table, proof blocks (metric + context + time frame) | Most AI-citable page type — definition, comparison, specs, FAQ, cross-links, proof |
| **Catalogue Page** | COMPARISON HUB | Comparison grid (primary block), category overview text, catalog vs. custom decision box | Optional (recommended if space allows) | Comparison grid (20 products with key specs and price indicators) — THE #1 AI-citable structure for "Which product should I choose?" queries | Category overview text should include category-level definition | Links to all 20 product detail pages — each with descriptive anchor text including product name | Comparison grid is the primary AI structure — must have clear headers, complete data, consistent format | Product comparison grid, category definition, product name links |
| **Product Detail Page** | SECONDARY ENTITY HUB | Key Specifications Table, Features and Benefits, Dimensions/Sizes, Warranty callout | N/A (not required — product pages are factual, not Q&A) | Key Specifications Table (the most AI-citable element — must have clear headers, complete data) | Product name in H1 must match canonical name used across site | Links to parent catalogue, parent solution, 3-5 related products, warranty page, wizard — descriptive anchor text with product names | Spec table with clear "Specifications" heading, feature list, warranty callout | Canonical product name, complete spec table, feature descriptions, related product links |
| **Case Study Index** | PROOF HUB | Results Summary Table (aggregated metrics from all 5 studies), case study cards | N/A (not required on index) | Results Summary Table — columns: project name, industry, units, timeline, key metric, link | N/A — index page aggregates proof, doesn't define entities | Links to all 5 individual case studies — descriptive anchor text | Results summary table with specific metrics per study | Aggregated proof table, project cards with metrics |
| **Individual Case Study** | SECONDARY ENTITY HUB | Results and Metrics section (structured quantitative data), Products Used section | 2-3 project-specific FAQ items | N/A (case study is narrative proof, not comparison) | N/A — case study doesn't define a product entity | Links to related solution pages, related industry page, 1-2 related case studies — descriptive anchor text | Results section with consistent format: metric + context + time frame | Specific metrics, project-specific FAQ, product entity links |
| **FAQ Page** | PRIMARY ENTITY HUB | All 14+ FAQ answers (the most AI-citable content on the site) | 14+ FAQ items across 6 categories — each self-contained with specific data | N/A — FAQ page IS the comparison/spec source for policy queries | N/A — FAQ page references entities, doesn't define them | Links to Warranty, Shipping, Returns, Contact, relevant solution pages — within FAQ answers | Every FAQ answer: 3-5 sentences, specific data points, no CTAs in answer text | Self-contained answers, category organization, anchor navigation, cross-reference links |
| **About Page** | BRAND ENTITY HUB | Company overview (entity definition), key metrics display, What We Do section | N/A (not required on About) | N/A — About page is brand-level, not product-level | "HILO is a North American manufacturer and distributor of premium glass and mirror products, designed in Canada and distributed across Canada and the United States." | Links to all 6 solution pages + all 3 industry pages — outbound links signal HILO's core topics to AI systems | Company overview as entity definition, metrics display as proof, team credentials | Brand entity definition, outbound link structure, metrics, team credentials |
| **Warranty Page** | SPECIALIZED HUB | Coverage summary table, claims process (step-by-step), exclusions list | N/A (not required — warranty is policy, not Q&A) | Coverage summary table — extractable warranty terms for "What does HILO's warranty cover?" queries | N/A | Links to Returns page (cross-reference), Contact page, FAQ page | Coverage table, claims process as numbered steps, exclusions list, specific timelines | Coverage table, process steps, response commitments |
| **Shipping Page** | SPECIALIZED HUB | Delivery timelines table, geographic coverage, delivery process, damage-free guarantee | N/A (not required) | Delivery timelines table — extractable timeline data for "How long does HILO delivery take?" queries | N/A | Links to Warranty, FAQ, Contact pages | Timeline table, process steps, geographic coverage, guarantee details | Timeline table, process block, coverage data |
| **Contact Page** | UTILITY (not hub) | NAP data (Name, Address, Phone) — extractable for local business queries | N/A | N/A | N/A | Links to wizard, FAQ, Warranty pages | Contact form, NAP data | Contact information, form, response commitment |
| **Wizard** | CONVERSION TOOL (not hub) | N/A — conversion tool, not information resource | N/A | N/A | N/A | No outbound links (terminal conversion point) | Privacy reassurance, 60-second estimate promise | Meta description optimized for "HILO estimate" queries |

---

## F. Open Dependencies

### F.1 Blocking Dependencies for Gate 4

The following owner inputs are required before Gate 4 can fully execute. Dependencies marked 🔴 P0 block specific production phases. Dependencies marked 🟡 P1 should be resolved before the affected pages are produced but do not block the overall production sequence.

| # | Dependency | Affects | Blocks | Current Status |
|---|-----------|--------|--------|---------------|
| **A1** | Canonical product names, slugs, and specifications for all 6 categories | P4 (all 6 catalogues), P5 (LED, Smart, Cabinets product pages) | P4 and P5 can proceed partially with existing product data from files 31-44, 51 (~48 products identified), but full production requires definitive canonical names from owner | 🔴 P0 — blocks full P4/P5 production |
| **A4** | Product names, slugs, and specifications for Shower Glass, Architectural Glass, Standard Mirrors | P6 (60 product detail pages), P4 (3 catalogue pages for these categories) | P6 is entirely blocked. P4 for these 3 categories is blocked. The 3 existing solution pages (08, 09, 10) are not blocked — they already exist. | 🔴 P0 — blocks P6 and partial P4 |
| **A7** | Pricing model decision: real pricing, "Request a Quote" model, or hybrid | P4, P5, P6 (catalogue and product pages need pricing data or quote-model specification) | If "Request a Quote" model is chosen, production can proceed without pricing data. If real pricing is desired, production is blocked until owner provides data. | 🟡 P1 — blocks pricing-specific content but not page structure |
| **—** | Real phone number and address | P8 (Contact page), P1-P3 (Trust Line phone reference), P9 (Wizard cleanup) | Phone/address placeholders exist in 9+ files. Cannot launch with placeholders. | 🟡 P1 — blocks final launch but not content production |
| **—** | Warranty PDF document | B.11 Warranty page (Block 7 — download link) | Placeholder link can be used during content production. PDF must be provided before launch. | 🟢 P2 — non-blocking for content production |
| **—** | Real company photos / project images | All pages with image requirements (all content pages) | Placeholder images can be used during content production. Real images must be provided before launch. | 🟢 P2 — non-blocking for content production |

### F.2 Dependency Resolution Priority

The owner should resolve dependencies in this order to maximize production parallelism:

1. **A1 (Product naming)** — resolves first because it unblocks the largest number of pages (P4 + P5 = 66 pages for LED/Smart/Cabinets, plus enables A4 resolution)
2. **A4 (3 missing categories)** — resolves after A1 because product naming conventions established in A1 can be applied to the 3 missing categories
3. **A7 (Pricing model)** — resolves independently; if "Request a Quote" is chosen, this unblocks all catalogue/product page pricing content immediately
4. **Phone/Address** — resolves independently; can be applied as a batch find-replace across all content files
5. **Warranty PDF** — resolves independently; low urgency
6. **Photos** — resolves independently; low urgency, real images can be swapped in during G5 build

---

## G. Approval Checklist

The owner should validate Gate 3 by confirming the following items:

### G.1 Page Models

- [ ] I have reviewed all 14 page models (B.1 through B.14) and approve the block structure, CTA hierarchy, and proof requirements for each.
- [ ] The Homepage model (B.1) captures the full value proposition and routes to solutions, industries, and the wizard.
- [ ] The Solution page model (B.3) includes all 7 mandatory HILO criteria and the AI discoverability blocks (definition, comparison, spec table, FAQ).
- [ ] The Product Detail page model (B.5) has a standardized block system that can scale to 120 pages consistently.
- [ ] The Warranty page (B.11) and Returns page (B.12) have distinct, non-overlapping scopes as defined.

### G.2 Production Priorities

- [ ] I approve the 10-phase production sequence (P1 through P10) as the Gate 4 execution plan.
- [ ] I understand that P6 (60 product detail pages for Shower/Arch Glass/Standard) is blocked until I provide product definitions (A4).
- [ ] I understand the estimated total effort of 34-42 turns for Gate 4.

### G.3 Dependencies

- [ ] I acknowledge that A1 (product naming) and A4 (3 missing categories) are blocking dependencies that I must resolve.
- [ ] I understand the pricing model decision (A7) and will communicate my preference before P4 production begins.
- [ ] I acknowledge that phone/address data, warranty PDF, and photos can be provided later without blocking content production.

### G.4 AI Discoverability

- [ ] I have reviewed the AI discoverability specifications per page type (Section E) and approve the approach.
- [ ] I understand that AI discoverability validation is a formal Gate 6 acceptance criterion (Conversion Architecture Section 12.10).
- [ ] I approve the entity hub designations: Solution pages (Primary), Product Detail (Secondary), FAQ (Primary), About (Brand Entity), Case Studies (Secondary), Industry (Contextual), Warranty/Shipping (Specialized).

### G.5 Scaling Logic

- [ ] I approve the product detail page scaling approach: standardized block system, 120 pages with consistent structure, variable elements clearly defined (Section C).
- [ ] I understand the distinction between what is standardized (block order, CTAs, Trust Line, breadcrumbs) and what varies per product (name, specs, features, images, pricing).

### G.6 Final Confirmation

- [ ] I approve docs/03_PAGE_MODELS_AND_PRIORITIZATION.md as the Gate 3 deliverable.
- [ ] Gate 4 content production is authorized to begin upon my approval.
- [ ] I commit to resolving blocking dependencies (A1, A4) before the affected production phases begin.

---

*This document defines the page model system and production priority framework for the HILO website. It is subordinate to the Master System Document (docs/00_MASTER_SYSTEM.md) in all matters of strategic, editorial, and conversion doctrine, and extends the structural architecture defined in docs/02_CONVERSION_ARCHITECTURE.md. It will be the primary reference for Gate 4 (Content Production).*

