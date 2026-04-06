# LIVRABLE 3.3 — Solution Pages: Architectural Glass + Standard Mirrors

**Projet**: HILO Website Optimization
**Auteur**: Senior Conversion Architect
**Date**: Avril 2026
**Statut**: En attente de validation

---

## Table des Matières

1. [Architecture CTA (Rappel)](#architecture-cta-rappel)
2. [Solution Page: Architectural Glass](#solution-page-architectural-glass)
3. [Solution Page: Standard Mirrors](#solution-page-standard-mirrors)
4. [Catalogue Structures](#catalogue-structures)
5. [Product Detail Pages](#product-detail-pages)

---

## Architecture CTA (Rappel)

### Niveaux de CTA

```
┌─────────────────────────────────────────────────────────────────┐
│  NIVEAU 1: SOLUTION PAGE                                        │
│  ────────────────────────                                       │
│  CTA PRINCIPAL: "See Our Products" → Catalogue                  │
│  CTA SECONDAIRE: "Get AI Estimate" → Outil d'estimation         │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│  NIVEAU 2: CATALOGUE (E-commerce Style)                         │
│  ────────────────────────────────────                           │
│  Grille de produits avec filtres                                │
│  Chaque produit → Product Detail Page                           │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│  NIVEAU 3: PRODUCT DETAIL PAGE                                  │
│  ─────────────────────────────                                  │
│  CTA PRINCIPAL: "Get AI Instant Quote" → AI Quote Flow          │
│  CTA SECONDAIRE: "Book a Call"                                  │
└─────────────────────────────────────────────────────────────────┘
```

---

## Solution Page: Architectural Glass

### URL Structure
```
/architectural-glass
```

### Hero Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  [IMAGE HERO: Partition en verre dans lobby hôtelier moderne]       │
│                                                                      │
│  ──────────────────────────────────────────────────────────────────  │
│                                                                      │
│  ARCHITECTURAL GLASS                                                │
│  ──────────────────                                                 │
│                                                                      │
│  Custom Glass Solutions for Commercial Spaces                       │
│  Engineered to Perform. Built to Last 5+ Years.                     │
│                                                                      │
│  ──────────────────────────────────────────────────────────────────  │
│                                                                      │
│  [See Our Products]  [Get AI Estimate]                              │
│                                                                      │
│  ──────────────────────────────────────────────────────────────────  │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

**Copy exact:**

**Headline:**
> Architectural Glass
> Custom Glass Solutions for Commercial Spaces

**Subheadline:**
> Engineered to Perform. Built to Last 5+ Years.

**Trust Line:**
> 🏆 180+ Projects | 🛡️ 5-Year Warranty | 🇨🇦 Designed in Canada. Distributed across North America.

**CTAs:**
- **PRINCIPAL**: `See Our Products` → `/architectural-glass/catalogue`
- **SECONDAIRE**: `Get AI Estimate` → `/ai-estimate`

---

### Section 1: When Glass Failure Is Not an Option

**Titre:**
> Architectural Glass That Performs Under Pressure

**Copy:**

Architectural glass isn't just a design element—it's a structural component that must perform reliably for decades. Conference room partitions that shatter during installation. Balcony railings that fail safety inspections. Glass facades that develop stress cracks after the first winter. These aren't hypothetical scenarios—they're real failures that cost developers millions in replacements, legal exposure, and reputational damage.

The architectural glass industry is fragmented between fabricators who understand glass but not commercial construction, and general contractors who understand construction but not glass. This knowledge gap creates projects where specifications are wrong, installations are compromised, and warranties are voided before the building opens.

HILO bridges that gap. We combine deep expertise in glass fabrication with practical understanding of commercial construction requirements. Our architectural glass systems are engineered for real-world conditions: thermal cycling, wind loads, impact resistance, and the daily wear of high-traffic environments.

**Common Architectural Glass Failures (That HILO Prevents):**

| Failure Mode | Root Cause | HILO Prevention |
|--------------|------------|-----------------|
| Spontaneous breakage | Nickel sulfide inclusions | Heat-soak testing on all tempered glass |
| Edge cracking | Improper edge finishing | Polished edges, verified quality |
| Stress fractures | Thermal expansion mismatch | Engineered systems with proper clearances |
| Hardware failure | Underspecified components | Load-rated hardware with safety factors |
| Seal failure (IGUs) | Low-quality spacers | Commercial-grade warm-edge spacers |
| Safety non-compliance | Wrong glass type | Laminated safety glass where required |

---

### Section 2: 5-Year Structural Warranty

**Titre:**
> 5-Year Warranty. No Fine Print.

**Copy:**

Architectural glass warranties typically read like legal defense documents—pages of exclusions, pro-rated values, and requirements that shift responsibility to installers or building owners. HILO's warranty is different by design.

**What's Covered:**

| Component | Coverage | Exclusions |
|-----------|----------|------------|
| Glass panels | 5 years | Vandalism, intentional impact |
| Hardware | 5 years | None |
| Seals (IGUs) | 5 years | None |
| Coatings | 5 years | Abrasive cleaning |
| Installation workmanship | 5 years | When HILO partners install |

**No Pro-Rating:**

If a panel fails in year 4, you don't receive 20% of its value. You receive a replacement panel at no cost. Period.

**Claims Process:**

1. **Report Issue** — Photo documentation via email or portal
2. **Assessment** — HILO team reviews within 48 hours
3. **Resolution** — Replacement shipped within 2 weeks for stock items
4. **No Paperwork Chase** — We handle logistics, you get results

**Why We Can Offer This:**

Our failure rate across 180+ architectural glass projects is less than 0.5%. When you engineer products correctly and control quality throughout production, warranty claims become rare exceptions rather than expected costs. We price our products to include realistic warranty reserves—not inflated margins to cover anticipated failures.

---

### Section 3: Competitive Pricing for Commercial Projects

**Titre:**
> Commercial-Grade Glass at Competitive Prices

**Copy:**

Architectural glass pricing varies dramatically across the market. The same specification can vary by 40-60% between vendors, often for identical products from the same glass manufacturers. The difference? Markups, inefficiencies, and supply chain complexity.

HILO's pricing reflects actual costs plus reasonable margins. We source directly from glass manufacturers, fabricate in our own facilities, and sell directly to commercial buyers. No distributor markups. No unnecessary intermediaries.

**Price Transparency:**

Unlike many architectural glass suppliers who require project-specific quotes for basic pricing, HILO provides transparent base pricing for common configurations:

| Product Category | Base Pricing |
|------------------|--------------|
| Partitions (clear) | From $XX/sq ft |
| Partitions (frosted) | From $XX/sq ft |
| Railings (tempered) | From $XX/linear ft |
| Railings (laminated) | From $XX/linear ft |
| Canopies | From $XX/sq ft |
| Facade systems | Custom quote |

**What's Included in Our Pricing:**

- Glass fabrication to your specifications
- Edge finishing (flat polish standard)
- Hardware (where applicable)
- Engineering documentation
- Delivery to your location

**What's Not Hidden:**

- No "processing fees"
- No "rush charges" for standard lead times
- No "minimum order fees" for project quantities
- No "documentation fees" for engineering stamps

**Pricing Callout:**

```
┌────────────────────────────────────────────────────────────────┐
│  💰 TRANSPARENT ARCHITECTURAL GLASS PRICING                    │
│  ────────────────────────────────────                          │
│                                                                │
│  • Standard partitions: From $XX/sq ft                         │
│  • Laminated safety glass: From $XX/sq ft                      │
│  • Railing systems: From $XX/linear ft                         │
│  • Custom configurations: AI estimate in 60 seconds            │
│  • Volume projects: Custom pricing for 1,000+ sq ft            │
│                                                                │
│  [Get AI Estimate →]                                           │
└────────────────────────────────────────────────────────────────┘
```

---

### Section 4: Product Categories

**Titre:**
> Architectural Glass Solutions for Every Application

**Copy:**

HILO offers a comprehensive range of architectural glass products designed for commercial and hospitality environments.

---

#### Category 1: Glass Partitions

**Description:**

Glass partitions transform open spaces into functional areas while maintaining visual connection and natural light flow. From conference rooms to hotel lobbies, glass walls create modern, professional environments.

**Options:**

| Type | Description | Best For |
|------|-------------|----------|
| Frameless partitions | Minimalist, all-glass appearance | Lobbies, conference rooms |
| Framed partitions | Metal frame structure with glass infill | High-traffic areas |
| Switchable glass | Privacy on demand (smart glass) | Executive offices, healthcare |
| Acoustic partitions | Enhanced sound isolation | Conference rooms, meeting spaces |
| Fire-rated glass | 60-120 minute ratings | Code-required applications |

**Specs:**

- Glass thickness: 3/8" to 3/4" depending on height
- Tempered or laminated options
- Clear, frosted, or custom patterns
- Hardware: Clamps, hinges, door hardware

---

#### Category 2: Glass Railings & Balustrades

**Description:**

Glass railings provide safety without obstructing views. Ideal for balconies, staircases, mezzanines, and pool surrounds where visual openness matters.

**Options:**

| Type | Description | Best For |
|------|-------------|----------|
| Base shoe mounted | Glass anchored at floor level | Balconies, terraces |
| Post mounted | Glass panels between metal posts | Staircases, walkways |
| Standoff mounted | Glass secured with decorative standoffs | Modern interiors |
| Channel mounted | Glass inserted into floor/wall channel | Seamless aesthetic |
| Frameless cantilever | No visible hardware | Premium applications |

**Specs:**

- Glass: 1/2" to 3/4" tempered or laminated
- Load capacity: Engineered to IBC/ local codes
- Top cap options: None, metal, or handrail
- Compliance: ADA, IBC, local building codes

---

#### Category 3: Glass Canopies & Overhead Glazing

**Description:**

Glass canopies provide weather protection while maintaining transparency. Entrance canopies, walkway covers, and overhead glazing systems that combine function with architectural impact.

**Options:**

| Type | Description | Best For |
|------|-------------|----------|
| Laminated glass canopies | Safety glass for overhead applications | Entrances, walkways |
| Point-supported canopies | Minimalist connection points | Contemporary architecture |
| Framed canopies | Structured support system | Traditional applications |
| Back-painted canopies | Opaque glass with custom colors | Design statements |

**Specs:**

- Glass: Laminated (required for overhead)
- Load design: Snow, wind, and live loads
- Drainage: Integrated water management
- Attachment: Wall-mounted, post-mounted, or suspended

---

#### Category 4: Glass Facades & Curtain Walls

**Description:**

Glass facades define building identity. HILO supplies glass and components for curtain wall systems, storefronts, and custom facade applications.

**Options:**

| Type | Description | Best For |
|------|-------------|----------|
| Insulated glass units (IGUs) | Double or triple glazed | Energy-efficient facades |
| Spandrel glass | Opaque panels for floor lines | Multi-story buildings |
| Low-E coatings | Energy performance | Climate-responsive design |
| Decorative glass | Patterned, colored, or textured | Design differentiation |

**Specs:**

- Standard sizes and custom dimensions
- Multiple coating options
- Warm-edge spacer technology
- Argon or air fill options

---

### Section 5: Door-to-Door Logistics

**Titre:**
> Specialized Handling for Architectural Glass

**Copy:**

Architectural glass presents unique logistics challenges. Large panel sizes, significant weight, and zero tolerance for damage require specialized equipment and expertise.

**Our Shipping Process:**

| Step | Description |
|------|-------------|
| **1. Production** | Glass cut, tempered, and finished to spec |
| **2. Inspection** | Quality verification before packaging |
| **3. Packaging** | Custom A-frames or crates for each order |
| **4. Protection** | Edge protectors, corner guards, surface film |
| **5. Documentation** | Packing list, inspection photos, handling instructions |
| **6. Transport** | Climate-controlled carriers with air-ride suspension |
| **7. Delivery** | Scheduled delivery with lift-gate or crane as needed |

**Large Panel Capabilities:**

| Panel Size | Shipping Method |
|------------|-----------------|
| Up to 60 sq ft | Standard lift-gate delivery |
| 60-120 sq ft | Specialized flatbed |
| 120+ sq ft | Dedicated truck or crane delivery |

**Damage-Free Guarantee:**

Panels arrive in perfect condition or we ship replacements at no cost. Our damage rate is under 0.5%—and when damage occurs, we don't waste your time with freight claims. We ship replacement glass immediately.

**Multi-Site Projects:**

Coordinated delivery across multiple buildings or job sites. Staged shipments that match your construction schedule. One logistics partner for complex distribution requirements.

---

### Section 6: Catalogue vs Custom

**Titre:**
> Standard Solutions and Custom Engineering

**Copy:**

Architectural glass projects span a spectrum from standard applications to complex custom designs. HILO supports both.

**Standard Configurations:**

For common applications—conference room partitions, standard railing heights, typical canopy spans—we offer pre-engineered solutions with documented specifications:

- Pre-calculated structural ratings
- Standard hardware packages
- Known lead times and pricing
- Code compliance documentation

**Custom Engineering:**

For unique applications—unusual spans, complex geometries, special load requirements—our engineering team develops custom solutions:

- Structural analysis and calculations
- Custom hardware design
- PE-stamped drawings (where required)
- Coordination with project engineers

**Decision Guide:**

| Project Type | Choose Standard | Choose Custom |
|--------------|-----------------|---------------|
| Standard partition heights (<10') | ✓ | |
| Typical railing runs | ✓ | |
| Standard canopy spans | ✓ | |
| Heights over 12' | | ✓ |
| Curved or angled glass | | ✓ |
| Special wind/snow loads | | ✓ |
| Unique attachment conditions | | ✓ |

**CTA Decision Box:**

```
┌─────────────────────────────────────────────────────────────────┐
│  HOW WOULD YOU LIKE TO PROCEED?                                 │
│                                                                 │
│  [Browse Standard Solutions]   [Request Custom Engineering]     │
│  Pre-engineered systems        Custom solutions designed        │
│  Instant pricing               AI estimate in 60 seconds        │
│  Faster delivery              Full engineering support          │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

### Section 7: AI-Powered Estimation

**Titre:**
> Complex Quotes. Simple Process.

**Copy:**

Architectural glass quotes have traditionally required site visits, engineering review, and extended back-and-forth. HILO's AI estimation tool delivers accurate preliminary quotes in under 60 seconds—even for custom configurations.

**How It Works:**

1. **Select product category** — Partition, railing, canopy, or custom
2. **Enter dimensions** — Height, width, panel count
3. **Choose glass type** — Tempered, laminated, insulated
4. **Specify options** — Hardware, finishes, features
5. **Get instant quote** — Itemized pricing with lead time

**AI Estimate Capabilities:**

| Capability | Description |
|------------|-------------|
| ⚡ | **60-Second Results** — No waiting for callbacks |
| 📐 | **Structural Guidance** — Identifies potential engineering needs |
| 🔄 | **Option Comparison** — Multiple configurations instantly |
| 📊 | **Itemized Breakdown** — Glass, hardware, shipping separated |
| 📧 | **Professional PDF** — Shareable with stakeholders |

**From Quote to Delivery:**

Our AI estimates are accurate enough for budgeting and often identical to final quotes. When engineering review is needed, we flag it automatically and provide a quote range with clear next steps.

**CTA:**

```
┌────────────────────────────────────────────────────────────────┐
│                                                                │
│  START YOUR ARCHITECTURAL GLASS QUOTE                          │
│                                                                │
│  [Get AI Estimate →]          [Book a Call]                    │
│                                                                │
└────────────────────────────────────────────────────────────────┘
```

---

### Section 8: Complete Glass Portfolio

**Titre:**
> One Partner for All Glass and Mirror Products

**Copy:**

HILO offers a complete range of glass and mirror products for hospitality, multi-family, and commercial projects.

**Full Product Line:**

| Category | Products | Application |
|----------|----------|-------------|
| LED Mirrors | 200+ designs | Guest rooms, bathrooms |
| Smart Mirrors | 50+ configurations | Premium rooms, lobbies |
| Medicine Cabinets | 100+ options | Guest room bathrooms |
| Shower Glass | Frameless & semi-frameless | Guest bathrooms |
| Architectural Glass | Partitions, railings, facades | Common areas |
| Standard Mirrors | All sizes | Gyms, common areas |

**Bundle Benefits:**

- **Single procurement** for your entire project
- **Coordinated logistics** across product types
- **Consolidated warranty** management
- **Volume pricing** across categories

**CTA:**
```
[See All Products →]
```

---

### Section 9: Installation & Technical Support

**Titre:**
> Expert Installation and Technical Support

**Copy:**

Architectural glass installation requires specialized skills, proper equipment, and attention to safety. Poor installation compromises performance and creates liability.

**Installation Partner Network:**

HILO partners with certified glazing contractors across North America who specialize in commercial architectural glass:

| Service | Description |
|---------|-------------|
| 📐 | **Site Measurement** — Verification before fabrication |
| 🔧 | **Professional Installation** — Code-compliant mounting |
| 🏗️ | **Structural Coordination** — Interface with building structure |
| ✅ | **Final Inspection** — Safety and performance verification |
| 📋 | **Documentation** — Installation records for warranty |

**Technical Support:**

| Support Type | Description |
|--------------|-------------|
| 📞 | **Phone Consultation** — Technical questions answered |
| 📄 | **Engineering Documentation** — Drawings and specifications |
| 🏗️ | **Contractor Coordination** — Interface with project teams |
| 📊 | **Shop Drawings** — Detailed installation plans |

**How to Add Installation:**

Request installation services during the quote process. We'll connect you with certified partners in your area and coordinate scheduling with your project timeline.

---

### Final CTA Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  START YOUR ARCHITECTURAL GLASS PROJECT                              │
│                                                                      │
│  Custom solutions • 5-year warranty • Engineering support            │
│                                                                      │
│  [See Our Products]              [Get AI Estimate]                   │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

---

## Solution Page: Standard Mirrors

### URL Structure
```
/standard-mirrors
```

### Hero Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  [IMAGE HERO: Grands miroirs muraux dans espace commun hôtelier]    │
│                                                                      │
│  ──────────────────────────────────────────────────────────────────  │
│                                                                      │
│  STANDARD MIRRORS                                                   │
│  ────────────────                                                   │
│                                                                      │
│  Quality Mirrors for Every Space                                    │
│  5-Year Warranty Against Defects and Degradation                    │
│                                                                      │
│  ──────────────────────────────────────────────────────────────────  │
│                                                                      │
│  [See Our Products]  [Get AI Estimate]                              │
│                                                                      │
│  ──────────────────────────────────────────────────────────────────  │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

**Copy exact:**

**Headline:**
> Standard Mirrors
> Quality Mirrors for Every Space

**Subheadline:**
> 5-Year Warranty Against Defects and Degradation

**Trust Line:**
> 🏆 180+ Projects | 🛡️ 5-Year Warranty | 🇨🇦 Designed in Canada. Distributed across North America.

**CTAs:**
- **PRINCIPAL**: `See Our Products` → `/standard-mirrors/catalogue`
- **SECONDAIRE**: `Get AI Estimate` → `/ai-estimate`

---

### Section 1: Not All Mirrors Are Created Equal

**Titre:**
> The Mirror Quality Problem

**Copy:**

A mirror is just glass with a reflective coating—until it isn't. Low-quality mirrors develop problems that become visible within months: black edge corrosion where moisture attacks the silvering, distortion from uneven glass, scratches from inadequate surface hardness, and warping from thin substrates that can't maintain flatness.

In commercial settings, these defects don't just look bad—they reflect poorly on your property. A gym mirror that develops black edges sends a message about facility maintenance. A lobby mirror with visible distortion undermines the professional image you've invested in. A hallway mirror that arrives scratched becomes an immediate maintenance ticket.

HILO standard mirrors are built for commercial reality. We use copper-free silvering that resists corrosion, glass substrates with proven flatness, and surface treatments that stand up to daily cleaning. The result: mirrors that maintain their appearance for 5+ years in demanding environments.

**Quality Comparison:**

| Quality Factor | Budget Mirrors | HILO Mirrors |
|----------------|----------------|--------------|
| Silvering type | Copper-based (corrodes) | Copper-free (resists corrosion) |
| Glass thickness | 2-3mm (warps) | 4-6mm (stays flat) |
| Edge sealing | None or minimal | Full perimeter seal |
| Surface hardness | Standard | Enhanced scratch resistance |
| Edge finishing | Raw or simple grind | Polished edges standard |
| Warranty | 1 year (if any) | 5 years |

---

### Section 2: 5-Year Quality Warranty

**Titre:**
> 5 Years. No Black Edges. No Distortion. No Excuses.

**Copy:**

HILO's 5-year warranty covers the defects that other mirror warranties exclude:

**What's Covered:**

| Issue | Coverage |
|-------|----------|
| Black edge corrosion | 100% replacement |
| Surface distortion | 100% replacement |
| Coating degradation | 100% replacement |
| Edge chips (from normal use) | 100% replacement |
| Scratches from normal cleaning | 100% replacement |

**What's Not Covered:**

- Intentional damage or vandalism
- Impact damage from objects
- Damage from abrasive cleaners (steel wool, etc.)
- Improper installation (if not HILO-partner installed)

**The HILO Difference:**

Most mirror warranties are 1-2 years because manufacturers know their products will degrade. Our 5-year warranty exists because we've engineered out the common failure modes. We use copper-free silvering that won't corrode, substrate glass that won't warp, and edge sealing that prevents moisture infiltration.

**Claims Process:**

Report an issue with photos. We'll ship a replacement within 2 weeks for standard sizes. No complicated claim forms. No debates about whether damage is "covered." We stand behind our products.

---

### Section 3: Competitive Pricing

**Titre:**
> Commercial Quality at Competitive Prices

**Copy:**

Commercial-grade mirrors don't require premium pricing. HILO's direct manufacturing model delivers quality that exceeds big-box alternatives at prices that respect project budgets.

**Price Comparison (Typical 36x48 Wall Mirror):**

| Source | Typical Price | Quality Level |
|--------|---------------|---------------|
| Big Box Retail | $80-150 | Consumer grade, 1-year warranty |
| Commercial Supplier | $150-250 | Variable quality |
| Glass Shop | $200-400 | Good quality, higher markup |
| **HILO** | **Competitive** | **Commercial-grade, 5-year warranty** |

**Volume Pricing:**

| Quantity | Discount |
|----------|----------|
| 10-24 units | 10% off |
| 25-49 units | 15% off |
| 50+ units | 20% off |

**Pricing Callout:**

```
┌────────────────────────────────────────────────────────────────┐
│  💰 TRANSPARENT STANDARD MIRROR PRICING                        │
│  ────────────────────────────────────                          │
│                                                                │
│  • Wall mirrors: From $XX/sq ft                                │
│  • Vanity mirrors: From $XX                                    │
│  • Gym mirrors: From $XX/sq ft                                 │
│  • Custom sizes: AI estimate in 60 seconds                     │
│  • Volume discounts: Up to 20% off for 50+ units               │
│                                                                │
│  [Get AI Estimate →]                                           │
└────────────────────────────────────────────────────────────────┘
```

---

### Section 4: Product Categories

**Titre:**
> Standard Mirrors for Every Application

**Copy:**

HILO offers a complete range of standard mirrors for commercial, hospitality, and multi-family applications.

---

#### Category 1: Wall Mirrors

**Description:**

Large-format mirrors for common areas, hallways, and feature walls. Available in standard sizes or custom dimensions to fit any space.

**Options:**

| Type | Sizes | Features |
|------|-------|----------|
| Standard rectangular | 24"x36" to 60"x96" | Polished edges, safety backing |
| Custom dimensions | Any size up to 96"x144" | Made to your specifications |
| Beveled edge | All sizes | Decorative beveled edges |
| Safety backed | All sizes | Film backing prevents shatter |
| Framed | Standard sizes | Metal or wood frame options |

**Applications:**
- Hotel hallways and lobbies
- Common areas in multi-family buildings
- Retail spaces
- Office environments

---

#### Category 2: Vanity Mirrors

**Description:**

Mirrors sized for bathroom vanities and grooming areas. Coordinate with our LED mirrors and medicine cabinets for complete bathroom solutions.

**Options:**

| Type | Sizes | Features |
|------|-------|----------|
| Standard vanity | 24" to 48" widths | Polished edges standard |
| Beveled vanity | All sizes | Beveled edge options |
| Oversized vanity | 60" to 96" widths | Large format for double vanities |
| Custom shapes | Any dimension | Fit your specific opening |

**Applications:**
- Guest room bathrooms
- Public restrooms
- Locker rooms
- Grooming stations

---

#### Category 3: Gym Mirrors

**Description:**

Large-format mirrors designed for fitness facilities, yoga studios, and athletic spaces. Built to withstand the demands of active environments.

**Options:**

| Type | Sizes | Features |
|------|-------|----------|
| Standard gym panels | 4'x6', 4'x8', 6'x8' | Safety backing required |
| Full wall coverage | Custom | Seamless appearance |
| Impact resistant | All sizes | Enhanced durability |
| Dance studio panels | Custom | Professional grade |

**Applications:**
- Hotel fitness centers
- Apartment complex gyms
- Corporate wellness rooms
- Yoga and pilates studios

---

#### Category 4: Safety Mirrors

**Description:**

Mirrors with safety features required for specific applications—tempered glass, laminated construction, or film backing.

**Options:**

| Type | Description | Application |
|------|-------------|-------------|
| Tempered mirrors | Breaks into small pieces | Code-required applications |
| Laminated mirrors | Glass stays in place | Overhead or high-risk locations |
| Film-backed mirrors | Prevents shatter | Sports facilities, gyms |
| Fire-rated mirrors | Rating up to 60 minutes | Fire-rated assemblies |

**Applications:**
- Athletic facilities
- Overhead mounting
- Code-required installations
- High-traffic public areas

---

### Section 5: Door-to-Door Delivery

**Titre:**
> Safe Delivery. Every Time.

**Copy:**

Large mirrors require specialized handling during shipping. HILO's packaging and delivery process protects your investment.

**Packaging Standards:**

| Protection | Description |
|------------|-------------|
| Corner guards | Protect vulnerable edges |
| Surface protection | Film or paper prevents scratches |
| Edge padding | Foam protection on all edges |
| Sturdy packaging | Custom crates for large mirrors |

**Delivery Options:**

| Option | Timeline | Best For |
|--------|----------|----------|
| Standard | 2-3 weeks | Regular schedules |
| Expedited | 1-2 weeks | Tight timelines |
| Staged delivery | Custom | Multi-phase projects |

**Damage-Free Guarantee:**

If a mirror arrives damaged, we ship a replacement immediately. No freight claims to file. No waiting for carrier investigations. We handle the hassle.

---

### Section 6: Catalogue vs Custom

**Titre:**
> Standard Sizes or Custom Dimensions

**Copy:**

HILO offers both catalogue products for quick ordering and custom fabrication for non-standard requirements.

**Catalogue Mirrors:**

Standard sizes available for immediate order:

| Category | Standard Sizes |
|----------|----------------|
| Wall mirrors | 24x36, 30x40, 36x48, 36x60, 48x72, 48x96 |
| Vanity mirrors | 24x30, 30x36, 36x48, 48x36, 48x60 |
| Gym mirrors | 48x72, 48x96, 72x96 |

**Custom Mirrors:**

When standard sizes don't fit:

- Any dimension up to 96" x 144"
- Custom shapes (arches, circles, cutouts)
- Special edge treatments
- Non-standard thicknesses

**Decision Guide:**

| Situation | Choose Catalogue | Choose Custom |
|-----------|-----------------|---------------|
| Standard opening sizes | ✓ | |
| Quick delivery needed | ✓ | |
| Budget constraints | ✓ | |
| Non-standard dimensions | | ✓ |
| Custom shapes required | | ✓ |
| Architectural feature | | ✓ |

**CTA Decision Box:**

```
┌─────────────────────────────────────────────────────────────────┐
│  HOW WOULD YOU LIKE TO PROCEED?                                 │
│                                                                 │
│  [Browse Catalogue]           [Request Custom Quote]            │
│  Standard sizes               Any dimension up to 96x144        │
│  Instant pricing              AI estimate in 60 seconds         │
│  2-3 week delivery            Custom lead time provided         │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

### Section 7: AI-Powered Estimation

**Titre:**
> Instant Quotes. No Waiting.

**Copy:**

Mirror quotes shouldn't require phone calls and email chains. HILO's AI estimation tool delivers accurate quotes in under 60 seconds.

**How It Works:**

1. **Select mirror type** — Wall, vanity, gym, or safety
2. **Enter dimensions** — Width and height
3. **Choose options** — Edge type, safety features, quantity
4. **Get instant quote** — Pricing with delivery timeline

**AI Estimate Benefits:**

| Benefit | Description |
|---------|-------------|
| ⚡ | **60-Second Results** — No callbacks needed |
| 🔄 | **Compare Options** — Multiple sizes instantly |
| 📊 | **Itemized Breakdown** — Mirror, options, shipping |
| 📧 | **PDF Export** — Professional quote document |
| 📞 | **Expert Available** — Book a call if needed |

**CTA:**

```
┌────────────────────────────────────────────────────────────────┐
│                                                                │
│  GET YOUR MIRROR QUOTE NOW                                     │
│                                                                │
│  [Get AI Estimate →]          [Book a Call]                    │
│                                                                │
└────────────────────────────────────────────────────────────────┘
```

---

### Section 8: Complete Product Range

**Titre:**
> More Than Standard Mirrors

**Copy:**

HILO offers a complete portfolio of glass and mirror products. One partner for your entire project.

**Full Product Line:**

| Category | Products | Starting From |
|----------|----------|---------------|
| LED Mirrors | 200+ designs | $XXX |
| Smart Mirrors | 50+ configurations | $XXX |
| Medicine Cabinets | 100+ options | $XXX |
| Shower Glass | Frameless & semi-frameless | $XXX/sq ft |
| Architectural Glass | Partitions, railings, facades | Custom |
| Standard Mirrors | All sizes | $XXX/sq ft |

**CTA:**
```
[See All Products →]
```

---

### Section 9: Installation Services

**Titre:**
> Professional Installation Available

**Copy:**

Large mirror installation requires proper anchoring, safety considerations, and attention to finish. HILO partners with certified installers across North America.

**Installation Services:**

| Service | Description |
|---------|-------------|
| 📐 | **Site Measurement** — Verify dimensions before fabrication |
| 🔧 | **Professional Mounting** — Secure installation to walls |
| 🛡️ | **Safety Compliance** — Proper mounting for overhead or large mirrors |
| ✅ | **Final Inspection** — Quality check and adjustment |
| 🧹 | **Site Cleanup** — Complete debris removal |

**How to Add Installation:**

Select "Include Installation" during the quote process. We'll connect you with certified partners in your area.

---

### Final CTA Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  EXPLORE OUR STANDARD MIRROR COLLECTION                              │
│                                                                      │
│  All sizes • 5-year warranty • Commercial quality                    │
│                                                                      │
│  [See Our Products]              [Get AI Estimate]                   │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

---

## Catalogue Structures

### Architectural Glass Catalogue

**URL:** `/architectural-glass/catalogue`

**Filter Categories:**

| Filter | Options |
|--------|---------|
| **Product Type** | Partitions, Railings, Canopies, Facades |
| **Glass Type** | Clear, Frosted, Laminated, IGU |
| **Glass Thickness** | 1/4", 3/8", 1/2", 3/4" |
| **Application** | Interior, Exterior, Overhead |
| **Safety Rating** | Tempered, Laminated, Fire-Rated |
| **Price Range** | $XX-$XX per sq ft |

### Standard Mirrors Catalogue

**URL:** `/standard-mirrors/catalogue`

**Filter Categories:**

| Filter | Options |
|--------|---------|
| **Category** | Wall Mirrors, Vanity Mirrors, Gym Mirrors, Safety Mirrors |
| **Size** | Small (<24"), Medium (24-48"), Large (48-72"), Extra Large (72"+) |
| **Shape** | Rectangle, Square, Round, Arch, Custom |
| **Edge Type** | Flat Polish, Beveled, Pencil Polish |
| **Safety Features** | None, Film-Backed, Tempered, Laminated |
| **Price Range** | $XX-$XX per sq ft |

---

## Product Detail Pages

### Architectural Glass Product Detail

**URL:** `/architectural-glass/catalogue/[product-slug]`

**Key Elements:**

| Element | Description |
|---------|-------------|
| **Configuration Selector** | Partition type, railing style, etc. |
| **Dimension Inputs** | Height, width, panel count |
| **Glass Options** | Type, thickness, coating |
| **Hardware Options** | Finish, style |
| **Engineering Notes** | Structural requirements flagged |
| **Primary CTA** | `Get AI Instant Quote` |
| **Secondary CTA** | `Book a Call` |

### Standard Mirror Product Detail

**URL:** `/standard-mirrors/catalogue/[product-slug]`

**Key Elements:**

| Element | Description |
|---------|-------------|
| **Size Selector** | Standard sizes or custom input |
| **Edge Type** | Flat, beveled, pencil |
| **Safety Options** | Film-backed, tempered, laminated |
| **Quantity Selector** | Per size |
| **Primary CTA** | `Get AI Instant Quote` |
| **Secondary CTA** | `Book a Call` |

---

## Résumé des Éléments Clés

### CTA Architecture (LIVRABLE 3.3)

| Niveau | Page | CTA Principal | CTA Secondaire |
|--------|------|---------------|----------------|
| 1 | Solution Page | See Our Products → Catalogue | Get AI Estimate |
| 2 | Catalogue | View Details → Product Page | — |
| 3 | Product Detail | Get AI Instant Quote | Book a Call |

### 7 Critères HILO Appliqués

| # | Critère | Application Architectural Glass | Application Standard Mirrors |
|---|---------|--------------------------------|------------------------------|
| **1** | Fiabilité 5 ans | Hero + Warranty section | Hero + Quality warranty |
| **2** | Prix compétitif | Per sq ft pricing | Per sq ft pricing |
| **3** | Delivery porte-à-porte | Specialized logistics | Safe delivery guarantee |
| **4** | Catalogue/sur mesure | Standard vs Custom engineering | Standard sizes vs Custom |
| **5** | AI estimation | Complex quotes simplified | Instant quotes |
| **6** | Grand choix | 4 categories detailed | 4 categories detailed |
| **7** | Installation | Certified glazing partners | Professional mounting |

### Trust Line (Consistent)

```
🏆 180+ Projects | 🛡️ 5-Year Warranty | 🇨🇦 Designed in Canada. Distributed across North America.
```

---

## LIVRABLE 3 — RÉSUMÉ COMPLET

### Progression LIVRABLE 3

| Sous-Livrable | Produits | Statut |
|---------------|----------|--------|
| **3.1** | LED Mirrors + Smart Mirrors | ✅ Complété |
| **3.2** | Medicine Cabinets + Shower Glass | ✅ Complété |
| **3.3** | Architectural Glass + Standard Mirrors | ✅ Complété |

### Architecture Globale LIVRABLE 3

**Total Solution Pages Créées:** 6
- `/led-mirrors`
- `/smart-mirrors`
- `/medicine-cabinets`
- `/shower-glass`
- `/architectural-glass`
- `/standard-mirrors`

**Total Catalogues Créés:** 6
- `/led-mirrors/catalogue`
- `/smart-mirrors/catalogue`
- `/medicine-cabinets/catalogue`
- `/shower-glass/catalogue`
- `/architectural-glass/catalogue`
- `/standard-mirrors/catalogue`

**CTA Architecture Unifiée:**

| Niveau | CTA Principal | CTA Secondaire |
|--------|---------------|----------------|
| Solution Page | See Our Products | Get AI Estimate |
| Catalogue | View Details | — |
| Product Detail | Get AI Instant Quote | Book a Call |

---

**Document préparé pour validation client.**

**Prochaine étape**: LIVRABLE 4 — Case Study Pages (en attente de validation)
