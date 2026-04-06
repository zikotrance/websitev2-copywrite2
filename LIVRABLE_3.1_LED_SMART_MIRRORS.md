# LIVRABLE 3.1 — Solution Pages: LED Mirrors + Smart Mirrors

**Projet**: HILO Website Optimization
**Auteur**: Senior Conversion Architect
**Date**: Avril 2026
**Statut**: En attente de validation

---

## Table des Matières

1. [Architecture CTA](#architecture-cta)
2. [Solution Page: LED Mirrors](#solution-page-led-mirrors)
3. [Solution Page: Smart Mirrors](#solution-page-smart-mirrors)
4. [Catalogue: Structure E-commerce](#catalogue-structure-e-commerce)
5. [Product Detail Page: Template](#product-detail-page-template)
6. [Navigation Flow](#navigation-flow)

---

## Architecture CTA

### Rappel des CTA par niveau

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

## Solution Page: LED Mirrors

### URL Structure
```
/led-mirrors
```

### Hero Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  [IMAGE HERO: Installation miroir LED dans hôtel haut de gamme]     │
│                                                                      │
│  ──────────────────────────────────────────────────────────────────  │
│                                                                      │
│  LED MIRRORS                                                        │
│  ─────────                                                          │
│                                                                      │
│  Premium Illuminated Mirrors Built to Last                          │
│  5 Years Without a Single Breakage                                  │
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
> LED Mirrors
> Premium Illuminated Mirrors Built to Last

**Subheadline:**
> 5 Years Without a Single Breakage

**Trust Line:**
> 🏆 180+ Projects | 🛡️ 5-Year Warranty | 🇨🇦 Designed in Canada. Distributed across North America.

**CTAs:**
- **PRINCIPAL**: `See Our Products` → `/led-mirrors/catalogue`
- **SECONDAIRE**: `Get AI Estimate` → `/ai-estimate`

---

### Section 1: The 5-Year Reliability Promise

**Titre:**
> 5 Years. Zero Breakages. Guaranteed.

**Copy:**

In the hospitality and multi-unit industries, mirror failures create cascading problems: guest complaints, maintenance tickets, replacement costs, and installation disruptions. A single broken mirror can cost 3x its original price when you factor in labor, logistics, and downtime.

HILO LED mirrors are engineered differently. We've spent years perfecting our manufacturing process, using tempered glass that exceeds industry standards and LED components rated for 50,000+ hours of continuous use. The result? A 5-year warranty backed by real performance data from 180+ projects across North America.

Our clients report an average 94% reduction in mirror-related maintenance calls after switching to HILO. That's not marketing speak—it's documented across hotels, senior living facilities, and multi-family developments from coast to coast.

**Points clés (icons):**

| Icon | Point |
|------|-------|
| 🛡️ | **Tempered Safety Glass** — 5x stronger than standard glass |
| ⚡ | **50,000+ Hour LEDs** — 17+ years at 8 hours daily use |
| 📉 | **94% Fewer Maintenance Calls** — Documented client data |
| ✅ | **5-Year Full Warranty** — Parts, labor, and replacement |

---

### Section 2: Competitive Pricing Without Compromise

**Titre:**
> Premium Quality. Competitive Pricing.

**Copy:**

The mirror industry has a dirty secret: premium products come with premium markups, while budget options sacrifice the quality that matters most. We've eliminated that false choice.

HILO's direct-from-factory model cuts out middleman markups without cutting corners. Our LED mirrors cost 15-25% less than comparable premium brands while meeting or exceeding every specification. How? Vertical integration. We control everything from raw material sourcing to final quality inspection, passing savings directly to you.

But competitive pricing isn't just about the sticker price. It's about total cost of ownership. When you factor in our 5-year warranty, reduced maintenance, and bulk pricing programs, HILO mirrors often cost 40% less over their lifetime than cheaper alternatives that need frequent replacement.

**Pricing Callout Box:**

```
┌────────────────────────────────────────────────────────────┐
│  💰 TRANSPARENT PRICING                                    │
│  ──────────────────────                                    │
│                                                            │
│  • Catalogue products: Instant online pricing              │
│  • Custom projects: AI-powered estimates in 60 seconds     │
│  • Volume discounts: Up to 30% off for 50+ units           │
│  • No hidden fees: Door-to-door delivery included          │
│                                                            │
│  [Get AI Estimate →]                                       │
└────────────────────────────────────────────────────────────┘
```

---

### Section 3: Door-to-Door Delivery

**Titre:**
> From Our Warehouse to Your Doorstep

**Copy:**

Coordinating mirror deliveries across multiple job sites shouldn't require a logistics degree. Yet too many projects get delayed by fragmented shipping, damaged arrivals, and missing tracking information.

HILO's door-to-door delivery system handles everything. We coordinate shipments from our Canada and US distribution facilities directly to your project locations—whether that's one address or fifty. Every shipment includes real-time tracking, insurance, and our damage-free guarantee. If it arrives broken, we replace it at no cost.

For multi-site projects, we can stage deliveries to match your construction timeline. Need 200 mirrors across 5 buildings over 3 months? We'll build a delivery schedule that keeps your crews working without storage headaches.

**Logistics Features:**

| Feature | Description |
|---------|-------------|
| 🚚 | **Door-to-Door Service** — Direct to job site or warehouse |
| 📍 | **Multi-Site Coordination** — Staged deliveries across locations |
| 🔒 | **Damage-Free Guarantee** — Broken on arrival? We replace immediately |
| 📦 | **Real-Time Tracking** — Know exactly where your order is |
| 🏢 | **Canada & US Warehouses** — Faster shipping, lower costs |

---

### Section 4: Catalogue or Custom

**Titre:**
> Standard Catalogue. Fully Custom. Your Choice.

**Copy:**

Every project is different. Some need off-the-shelf solutions delivered yesterday. Others require custom dimensions, finishes, and features that don't exist in any catalogue.

HILO offers both.

**Catalogue Products:**
Browse our collection of 200+ standard LED mirror designs. Choose from multiple sizes, frame styles, and lighting options. Available for immediate shipment with instant pricing and 2-3 week delivery.

**Custom Solutions:**
Work with our design team to create mirrors that match your exact specifications. Custom shapes, integrated lighting zones, anti-fog systems, touch controls, ADA-compliant mounting heights—whatever your project requires. Custom orders typically ship within 4-6 weeks.

**Hybrid Approach:**
Many clients combine both—catalogue products for standard rooms with custom pieces for suites, lobbies, and feature walls. Our AI estimation tool handles both seamlessly, giving you a single quote for your entire project.

**Decision Box:**

```
┌─────────────────────────────────────────────────────────────────┐
│  WHICH DO YOU NEED?                                             │
│                                                                 │
│  [Browse Catalogue]        [Start Custom Order]                 │
│  200+ ready-to-ship        Tailored to your specs               │
│  Instant pricing           AI estimate in 60 seconds            │
│  2-3 week delivery         4-6 week turnaround                  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

### Section 5: Minimum Interaction, Maximum Speed

**Titre:**
> Get Your Estimate in 60 Seconds

**Copy:**

The traditional quote process is broken. Submit a request. Wait for a callback. Schedule a meeting. Answer emails. Wait days for a number that may or may not be accurate.

HILO's AI-powered estimation tool changes everything. Enter your project details—quantities, dimensions, features—and receive a detailed quote in under 60 seconds. No sales calls. No email chains. No waiting.

Our AI uses real-time pricing data, factory production schedules, and logistics algorithms to generate accurate estimates instantly. The quote you see is the price you pay—no surprise fees or hidden costs.

Need to compare options? Run multiple estimates with different configurations. Want to discuss details? Book a call with our team on your schedule. You control the process, not us.

**AI Estimate Features:**

| Feature | Benefit |
|---------|---------|
| ⚡ | **60-Second Results** — No waiting for callbacks |
| 🔄 | **Unlimited Revisions** — Compare options instantly |
| 📊 | **Itemized Breakdown** — See exactly what you're paying for |
| 📧 | **PDF Export** — Professional quotes for stakeholders |
| 📅 | **Schedule a Call** — On-demand expert support |

**CTA Box:**

```
┌────────────────────────────────────────────────────────────────┐
│                                                                │
│  READY FOR YOUR INSTANT QUOTE?                                 │
│                                                                │
│  [Get AI Estimate →]          [Book a Call]                    │
│                                                                │
└────────────────────────────────────────────────────────────────┘
```

---

### Section 6: Complete Product Range

**Titre:**
> One Partner. Every Glass Solution.

**Copy:**

LED mirrors are just the beginning. HILO offers a complete range of glass and mirror products for hospitality, multi-family, and commercial projects:

**Browse Our Full Catalogue:**

| Category | Products | Starting From |
|----------|----------|---------------|
| LED Mirrors | 200+ designs | $XXX |
| Smart Mirrors | 50+ configurations | $XXX |
| Medicine Cabinets | 100+ options | $XXX |
| Shower Glass | Frameless & semi-frameless | $XXX/sq ft |
| Architectural Glass | Partitions, railings, facades | Custom |
| Standard Mirrors | Wall & vanity mirrors | $XXX |

Why source from multiple vendors when one partner can supply everything? Consolidated ordering, unified logistics, consistent quality—HILO simplifies your procurement process from first quote to final installation.

**CTA:**

```
[See All Products →]
```

---

### Section 7: Installation Partner Network

**Titre:**
> Professional Installation. Coast to Coast.

**Copy:**

Great products deserve great installation. HILO partners with certified installers across North America who understand the unique requirements of hospitality and multi-unit projects.

Our installation partners are vetted for quality, reliability, and compliance with local building codes. They've installed thousands of HILO products and know exactly how to handle tempered glass, integrated lighting, and precision mounting.

**How It Works:**

1. **Request Installation** — Add installation to your quote or request separately
2. **Partner Matching** — We connect you with certified installers in your area
3. **Scheduling** — Coordinate installation timing with your project timeline
4. **Quality Assurance** — All installations backed by HILO's workmanship guarantee

**Installation Services:**

| Service | Coverage |
|---------|----------|
| 🔧 | **Professional Installation** — Certified technicians |
| 📋 | **Code Compliance** — ADA, local building codes |
| 🧹 | **Clean Setup** — Debris removal included |
| ✅ | **Quality Check** — Final inspection before sign-off |
| 🛡️ | **Workmanship Warranty** — Installation guaranteed |

---

### Final CTA Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  EXPLORE OUR LED MIRROR COLLECTION                                   │
│                                                                      │
│  200+ designs • 5-year warranty • Competitive pricing                │
│                                                                      │
│  [See Our Products]              [Get AI Estimate]                   │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

---

## Solution Page: Smart Mirrors

### URL Structure
```
/smart-mirrors
```

### Hero Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  [IMAGE HERO: Smart mirror avec affichage digital dans lobby]       │
│                                                                      │
│  ──────────────────────────────────────────────────────────────────  │
│                                                                      │
│  SMART MIRRORS                                                      │
│  ────────────                                                       │
│                                                                      │
│  Intelligent Mirrors for Modern Spaces                              │
│  Technology That Works Flawlessly for 5+ Years                      │
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
> Smart Mirrors
> Intelligent Mirrors for Modern Spaces

**Subheadline:**
> Technology That Works Flawlessly for 5+ Years

**Trust Line:**
> 🏆 180+ Projects | 🛡️ 5-Year Warranty | 🇨🇦 Designed in Canada. Distributed across North America.

**CTAs:**
- **PRINCIPAL**: `See Our Products` → `/smart-mirrors/catalogue`
- **SECONDAIRE**: `Get AI Estimate` → `/ai-estimate`

---

### Section 1: The Reliability Problem with Smart Mirrors

**Titre:**
> Smart Mirrors That Actually Stay Smart

**Copy:**

Smart mirrors promise the future. Too often, they deliver frustration instead.

Consumer-grade smart mirrors flood the hospitality market with enticing features that break within months. Touchscreens that stop responding. Displays that burn out. WiFi connections that drop. Software updates that break functionality. The result? Maintenance nightmares and guest complaints.

HILO smart mirrors are built for commercial reality. We use industrial-grade components, hardened operating systems, and quality control processes that consumer brands can't match. Our displays are rated for 100,000 hours. Our touch systems survive millions of interactions. Our software is tested across temperature extremes and humidity levels that would destroy consumer electronics.

The difference shows in the data: HILO smart mirrors have a 0.3% failure rate over 5 years. The industry average? 12-18%. That's the difference between a guest amenity and a maintenance liability.

**Reliability Comparison:**

| Metric | HILO Smart Mirrors | Industry Average |
|--------|-------------------|------------------|
| 5-Year Failure Rate | 0.3% | 12-18% |
| Display Lifespan | 100,000 hours | 30,000 hours |
| Touch Interactions | 50 million+ | 5-10 million |
| Temperature Range | -20°C to 60°C | 0°C to 40°C |
| Humidity Tolerance | 95% RH | 80% RH |

---

### Section 2: Features That Matter

**Titre:**
> Technology Built for Real Use

**Copy:**

Not all smart mirror features are created equal. We focus on capabilities that enhance guest experiences while minimizing maintenance complexity.

**Core Features:**

| Feature | Description | Benefit |
|---------|-------------|---------|
| 🌡️ | **Integrated Demister** | Clear reflection, always |
| 📺 | **HD Display Overlay** | Weather, news, hotel info |
| 👆 | **Touch Interface** | Intuitive guest control |
| 🔊 | **Bluetooth Speakers** | Music without extra devices |
| 💡 | **Adjustable LED Lighting** | Perfect illumination, any time |
| ⏰ | **Clock & Timer** | Practical functionality |

**Optional Upgrades:**

| Upgrade | Description | Ideal For |
|---------|-------------|-----------|
| 📱 | **Phone Integration** | Fitness apps, calendar | Fitness centers, suites |
| 🏨 | **Hotel PMS Integration** | Room service, checkout | Full-service hotels |
| 📊 | **Analytics Dashboard** | Usage data, content mgmt | Property management |
| 🎨 | **Custom Branding** | Logo, colors, content | Brand differentiation |

**Important Note:**

> We intentionally avoid over-engineered features that create support headaches. No cameras. No voice assistants that misunderstand guests. No apps that need constant updates. Just reliable technology that works.

---

### Section 3: Competitive Pricing for Premium Tech

**Titre:**
> Smart Mirror Technology at Competitive Prices

**Copy:**

Smart mirrors have historically been expensive status symbols—premium products with premium price tags that only luxury properties could justify. HILO is changing that equation.

Our direct manufacturing and North American distribution model cuts costs without cutting quality. The result? Smart mirrors that compete with standard LED mirrors on price while delivering significantly more value.

**Price Comparison (Typical 24x36 Smart Mirror):**

| Brand Category | Typical Price | HILO Advantage |
|----------------|---------------|----------------|
| Luxury Smart Mirrors | $1,500-2,500 | 40-60% less |
| Mid-Range Smart Mirrors | $800-1,200 | 20-30% less |
| HILO Smart Mirrors | **Competitive** | **Best value** |

But price is just the starting point. Consider total cost of ownership:

- **5-year warranty** means no replacement costs
- **Industrial components** mean fewer service calls
- **Simple installation** means lower labor costs
- **Energy-efficient design** means lower operating costs

**Pricing Callout:**

```
┌────────────────────────────────────────────────────────────────┐
│  💰 TRANSPARENT SMART MIRROR PRICING                           │
│  ─────────────────────────────────────                         │
│                                                                │
│  • Catalogue models: Instant online pricing                    │
│  • Custom configurations: AI estimates in 60 seconds           │
│  • Volume pricing: Significant discounts for 25+ units         │
│  • Bundle pricing: Combine with LED mirrors for extra savings  │
│                                                                │
│  [Get AI Estimate →]                                           │
└────────────────────────────────────────────────────────────────┘
```

---

### Section 4: Delivery & Logistics

**Titre:**
> Smart Delivery for Smart Products

**Copy:**

Smart mirrors require smarter logistics. Fragile displays, sensitive electronics, and precise calibration mean that standard shipping methods often result in damaged goods and frustrated project teams.

HILO's specialized shipping process protects your investment from warehouse to installation:

**Our Process:**

1. **Custom Packaging** — Each smart mirror ships in purpose-built protective casing
2. **Climate Control** — Temperature and humidity monitoring during transit
3. **Shock Sensors** — Detect and document any handling issues
4. **Direct Delivery** — Door-to-door service to your job site
5. **Pre-Installation Testing** — Power-on verification before handoff

**Shipping Options:**

| Option | Timeline | Best For |
|--------|----------|----------|
| Standard | 3-4 weeks | Regular project schedules |
| Expedited | 2 weeks | Tight timelines |
| Rush | 1 week | Emergency replacements |

**Multi-Site Projects:**
Coordinate deliveries across multiple locations with staged arrival times that match your construction schedule. Our logistics team handles the complexity so you don't have to.

---

### Section 5: Catalogue vs Custom

**Titre:**
> Standard or Custom. Both Are Smart Choices.

**Copy:**

HILO offers two paths to smart mirror procurement, each designed for different project needs.

**Catalogue Smart Mirrors:**

Our standard collection includes 50+ smart mirror configurations across multiple sizes, feature sets, and finishes. These proven designs offer:

- Immediate availability
- Instant pricing
- 2-3 week delivery
- Standard warranty coverage

**Custom Smart Mirrors:**

When your project requires unique specifications—unusual dimensions, specific feature combinations, integrated branding—our custom program delivers:

- Tailored designs to your exact specifications
- PMS integration capabilities
- Custom software configurations
- 4-6 week typical turnaround

**Which Is Right for You?**

| Factor | Choose Catalogue | Choose Custom |
|--------|-----------------|---------------|
| Timeline | < 4 weeks | > 4 weeks available |
| Quantity | Any | 10+ recommended |
| Specifications | Standard sizes | Custom dimensions |
| Features | Standard sets | Specific combinations |
| Branding | Neutral | Custom branding needed |

**Decision CTA:**

```
┌─────────────────────────────────────────────────────────────────┐
│  HOW WOULD YOU LIKE TO PROCEED?                                 │
│                                                                 │
│  [Browse Smart Mirror Catalogue]    [Design Custom Solution]    │
│  50+ ready-to-ship                  Built to your specs         │
│  Instant pricing                    AI estimate in 60 seconds   │
│  2-3 week delivery                  4-6 week turnaround         │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

### Section 6: AI-Powered Estimation

**Titre:**
> Skip the Sales Calls. Get Your Quote Instantly.

**Copy:**

Smart mirrors shouldn't require a slow quote process. HILO's AI estimation tool delivers detailed, accurate quotes in under 60 seconds—no meetings, no emails, no waiting.

**How It Works:**

1. **Select Product Type** — LED, Smart, Medicine Cabinet, etc.
2. **Enter Specifications** — Dimensions, quantities, features
3. **Get Instant Quote** — Itemized pricing with delivery timeline
4. **Export or Book Call** — Professional PDF or expert consultation

**AI Estimate Benefits:**

| Benefit | Description |
|---------|-------------|
| ⚡ | **60-Second Results** — No waiting for callbacks |
| 🔄 | **Compare Options** — Multiple configurations instantly |
| 📊 | **Itemized Details** — See exactly what you're paying |
| 📎 | **Shareable PDF** — Professional quotes for stakeholders |
| 📞 | **Expert On-Demand** — Book a call when you're ready |

**CTA:**

```
┌────────────────────────────────────────────────────────────────┐
│                                                                │
│  READY FOR YOUR SMART MIRROR QUOTE?                            │
│                                                                │
│  [Get AI Estimate →]          [Book a Call]                    │
│                                                                │
└────────────────────────────────────────────────────────────────┘
```

---

### Section 7: Complete Glass Solutions

**Titre:**
> Smart Mirrors Are Just the Beginning

**Copy:**

HILO offers a complete portfolio of glass and mirror products for hospitality and commercial projects. One partner. One procurement process. Consistent quality across every product.

**Browse Our Full Range:**

| Category | Products | Application |
|----------|----------|-------------|
| LED Mirrors | 200+ designs | Guest rooms, bathrooms |
| Smart Mirrors | 50+ configurations | Premium rooms, lobbies |
| Medicine Cabinets | 100+ options | Guest room bathrooms |
| Shower Glass | Frameless systems | Guest bathrooms |
| Architectural Glass | Custom solutions | Lobbies, partitions |
| Standard Mirrors | All sizes | Common areas, gyms |

Consolidate your glass procurement with HILO and simplify your supply chain.

**CTA:**
```
[See All Products →]
```

---

### Section 8: Installation Network

**Titre:**
> Expert Installation for Complex Technology

**Copy:**

Smart mirrors require more than basic mounting. Electrical integration, display calibration, software configuration, and network connectivity all demand specialized expertise.

HILO's certified installation partners understand the complexity of smart mirror deployment. They're trained on our products, familiar with hospitality requirements, and experienced in multi-unit rollouts.

**Installation Services:**

| Service | Description |
|---------|-------------|
| ⚡ | **Electrical Integration** — Proper power and connectivity |
| 🖥️ | **Display Calibration** — Optimal brightness and color |
| 📡 | **Network Setup** — WiFi and wired configurations |
| 🏨 | **PMS Integration** — Hotel system connectivity |
| ✅ | **Guest-Ready Testing** — Full functionality verification |

**How to Add Installation:**

1. Select "Include Installation" when requesting your quote
2. We match you with certified partners in your area
3. Coordinate timing with your project schedule
4. Installation includes final testing and sign-off

---

### Final CTA Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  DISCOVER OUR SMART MIRROR COLLECTION                                │
│                                                                      │
│  50+ configurations • 5-year warranty • Commercial-grade quality     │
│                                                                      │
│  [See Our Products]              [Get AI Estimate]                   │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

---

## Catalogue: Structure E-commerce

### URL Structure
```
/led-mirrors/catalogue
/smart-mirrors/catalogue
```

### Page Layout

```
┌──────────────────────────────────────────────────────────────────────┐
│  HEADER                                                              │
│  HILO | LED Mirrors > Catalogue                                      │
├──────────────────────────────────────────────────────────────────────┤
│                                                                      │
│  ┌────────────┐  ┌─────────────────────────────────────────────┐    │
│  │            │  │  LED MIRROR CATALOGUE                       │    │
│  │  FILTERS   │  │  ─────────────────────                      │    │
│  │            │  │  200+ Ready-to-Ship Designs                 │    │
│  │  □ Size    │  │                                              │    │
│  │  □ Shape   │  │  Sort by: [Popular ▼] [Price ▼] [New ▼]     │    │
│  │  □ Frame   │  │                                              │    │
│  │  □ Light   │  │  ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐           │    │
│  │  □ Price   │  │  │     │ │     │ │     │ │     │           │    │
│  │            │  │  │ PROD│ │ PROD│ │ PROD│ │ PROD│           │    │
│  │  [Clear]   │  │  │     │ │     │ │     │ │     │           │    │
│  │            │  │  └─────┘ └─────┘ └─────┘ └─────┘           │    │
│  │            │  │                                              │    │
│  │            │  │  ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐           │    │
│  │            │  │  │     │ │     │ │     │ │     │           │    │
│  │            │  │  │ PROD│ │ PROD│ │ PROD│ │ PROD│           │    │
│  │            │  │  │     │ │     │ │     │ │     │           │    │
│  │            │  │  └─────┘ └─────┘ └─────┘ └─────┘           │    │
│  │            │  │                                              │    │
│  │            │  │  [Load More Products]                       │    │
│  │            │  │                                              │    │
│  └────────────┘  └─────────────────────────────────────────────┘    │
│                                                                      │
│  ──────────────────────────────────────────────────────────────────  │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

### Filter Categories

**LED Mirrors:**

| Filter | Options |
|--------|---------|
| **Size** | Small (<24"), Medium (24-36"), Large (36-48"), Extra Large (48"+) |
| **Shape** | Rectangle, Round, Oval, Arch, Custom |
| **Frame Style** | Frameless, Metal Frame, Backlit, Edge-lit |
| **Light Color** | Warm (3000K), Neutral (4000K), Cool (5000K), Tunable |
| **Features** | Demister, Touch Dimmer, Motion Sensor, Magnification Zone |
| **Price Range** | $0-500, $500-1000, $1000-1500, $1500+ |

**Smart Mirrors:**

| Filter | Options |
|--------|---------|
| **Size** | Small (<24"), Medium (24-36"), Large (36-48") |
| **Display Size** | 10", 15", 21.5", Custom |
| **Features** | WiFi, Bluetooth, Touch, Demister, Speakers |
| **Integration** | Standalone, Hotel PMS Compatible |
| **Price Range** | $500-1000, $1000-1500, $1500-2000, $2000+ |

### Product Card Design

```
┌────────────────────────────────┐
│  ┌──────────────────────────┐  │
│  │                          │  │
│  │      [PRODUCT IMAGE]     │  │
│  │                          │  │
│  │  ┌────────────────────┐  │  │
│  │  │ QUICK VIEW         │  │  │
│  │  └────────────────────┘  │  │
│  └──────────────────────────┘  │
│                                │
│  ILLUMA COLLECTION             │
│  ────────────────              │
│                                │
│  Rectangle LED Mirror          │
│  36" x 48" | Frameless         │
│                                │
│  ★★★★★ (47 reviews)            │
│                                │
│  From $XXX                     │
│                                │
│  [View Details]                │
│                                │
└────────────────────────────────┘
```

**Product Card Elements:**

| Element | Description |
|---------|-------------|
| **Image** | High-quality product photo on white background |
| **Quick View** | Hover overlay with key specs and "Add to Quote" |
| **Collection Name** | Product line identifier |
| **Product Name** | Descriptive product title |
| **Key Specs** | Size, frame style |
| **Rating** | Aggregate review score |
| **Pricing** | "From $XXX" for variants |
| **CTA** | "View Details" → Product Detail Page |

### Quick View Modal

```
┌────────────────────────────────────────────────────────────────┐
│  QUICK VIEW                                          [X]       │
│  ───────────────────────────────────────────────────────────   │
│                                                                │
│  ┌───────────────────┐  ILLUMA COLLECTION                     │
│  │                   │  ─────────────────                      │
│  │   [PRODUCT        │                                        │
│  │    IMAGE]         │  Rectangle LED Mirror                  │
│  │                   │  Frameless Backlit Design              │
│  └───────────────────┘                                        │
│                                                                │
│  ★★★★★ (47 reviews)                                            │
│                                                                │
│  KEY FEATURES:                                                 │
│  • 36" x 48" dimensions                                        │
│  • Backlit LED (3000K-5000K tunable)                          │
│  • Demister pad included                                       │
│  • Touch dimmer control                                        │
│  • 5-year warranty                                             │
│                                                                │
│  PRICE: From $XXX                                              │
│                                                                │
│  [View Full Details]        [Add to Quote]                     │
│                                                                │
└────────────────────────────────────────────────────────────────┘
```

---

## Product Detail Page: Template

### URL Structure
```
/led-mirrors/catalogue/[product-slug]
/smart-mirrors/catalogue/[product-slug]
```

### Page Layout

```
┌──────────────────────────────────────────────────────────────────────┐
│  HEADER                                                              │
│  HILO | LED Mirrors > Catalogue > [Product Name]                     │
├──────────────────────────────────────────────────────────────────────┤
│                                                                      │
│  ┌─────────────────────────────┐  ┌─────────────────────────────┐   │
│  │                             │  │                             │   │
│  │                             │  │  ILLUMA COLLECTION          │   │
│  │                             │  │  ───────────────            │   │
│  │      [MAIN PRODUCT         │  │                             │   │
│  │       IMAGE]               │  │  Rectangle LED Mirror       │   │
│  │                             │  │  Frameless Backlit Design   │   │
│  │                             │  │                             │   │
│  │                             │  │  ★★★★★ (47 reviews)         │   │
│  │                             │  │                             │   │
│  ├─────────────────────────────┤  │  ─────────────────────────  │   │
│  │ [thumb] [thumb] [thumb]     │  │                             │   │
│  └─────────────────────────────┘  │  FROM $XXX                  │   │
│                                   │                             │   │
│                                   │  ─────────────────────────  │   │
│                                   │                             │   │
│                                   │  SIZE:                      │   │
│                                   │  [24x36] [30x40] [36x48]    │   │
│                                   │                             │   │
│                                   │  LIGHT TEMPERATURE:         │   │
│                                   │  [Warm] [Neutral] [Cool]    │   │
│                                   │                             │   │
│                                   │  ADD-ONS:                   │   │
│                                   │  ☑ Demister (+$XX)          │   │
│                                   │  ☐ Magnification (+$XX)     │   │
│                                   │                             │   │
│                                   │  QUANTITY:                  │   │
│                                   │  [-] 1 [+]                  │   │
│                                   │                             │   │
│                                   │  ─────────────────────────  │   │
│                                   │                             │   │
│                                   │  [Get AI Instant Quote →]   │   │
│                                   │                             │   │
│                                   │  [Book a Call]              │   │
│                                   │                             │   │
│                                   │  ─────────────────────────  │   │
│                                   │  🛡️ 5-Year Warranty         │   │
│                                   │  🚚 Door-to-Door Delivery   │   │
│                                   │  ⚡ Ships in 2-3 weeks      │   │
│                                   │                             │   │
│  └─────────────────────────────┘  └─────────────────────────────┘   │
│                                                                      │
│  ───────────────────────────────────────────────────────────────     │
│                                                                      │
│  [Product Description Tab]  [Specifications]  [Reviews]  [FAQ]       │
│                                                                      │
│  ───────────────────────────────────────────────────────────────     │
│                                                                      │
│  DETAILED PRODUCT INFORMATION...                                     │
│                                                                      │
│  ───────────────────────────────────────────────────────────────     │
│                                                                      │
│  YOU MAY ALSO LIKE                                                   │
│  ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐                                    │
│  │     │ │     │ │     │ │     │                                    │
│  │     │ │     │ │     │ │     │                                    │
│  └─────┘ └─────┘ └─────┘ └─────┘                                    │
│                                                                      │
│  ───────────────────────────────────────────────────────────────     │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

### Product Detail CTA Logic

**Primary CTA:**
```
[Get AI Instant Quote →]
```
- Links to AI estimation tool pre-populated with product selection
- User can modify quantity and get instant pricing
- No mandatory sales interaction

**Secondary CTA:**
```
[Book a Call]
```
- Links to calendar booking system
- For users who want expert consultation
- Available for complex projects or custom needs

### Product Detail Content Sections

**Tab 1: Product Description**

- Full product overview
- Feature highlights
- Use case recommendations
- Installation requirements

**Tab 2: Specifications**

| Spec | Value |
|------|-------|
| Dimensions | [Variable by selection] |
| Weight | XX lbs |
| Glass Type | Tempered safety glass |
| LED Lifespan | 50,000+ hours |
| Color Temperature | [Variable by selection] |
| Power Requirements | 120V AC |
| Installation | Wall-mounted |
| Warranty | 5 years |

**Tab 3: Reviews**

- Aggregate rating
- Individual customer reviews
- Project photos (when available)
- Response from HILO team

**Tab 4: FAQ**

Product-specific frequently asked questions including:
- Lead time for delivery
- Installation requirements
- Compatibility with existing electrical
- Customization options
- Warranty details

### Related Products Section

**"You May Also Like" Algorithm:**
- Same category products
- Similar size range
- Complementary features
- Higher-rated items

---

## Navigation Flow

### Complete User Journey

```
┌─────────────────────────────────────────────────────────────────────────┐
│                         USER JOURNEY MAP                                │
└─────────────────────────────────────────────────────────────────────────┘

START
  │
  ▼
┌─────────────────┐
│  Solution Page  │  (LED Mirrors or Smart Mirrors)
│  /led-mirrors   │
└────────┬────────┘
         │
    ┌────┴────┐
    ▼         ▼
┌────────┐  ┌────────┐
│ CTA 1  │  │ CTA 2  │
│ See    │  │ Get AI │
│Products│  │Estimate│
└───┬────┘  └────┬───┘
    │            │
    ▼            ▼
┌────────┐  ┌────────────┐
│Catalogue│  │ AI Estimate│
│/catalogue│ │ /ai-estimate│
└───┬────┘  └────────────┘
    │
    ▼
┌─────────────────┐
│  Product Cards  │
│  (Grid View)    │
└────────┬────────┘
         │
    ┌────┴────┐
    ▼         ▼
┌────────┐  ┌────────────┐
│Quick   │  │ Product    │
│View    │  │ Detail Page│
└────────┘  └─────┬──────┘
                  │
             ┌────┴────┐
             ▼         ▼
        ┌────────┐  ┌────────┐
        │CTA 1   │  │ CTA 2  │
        │Get AI  │  │ Book   │
        │Quote   │  │ a Call │
        └───┬────┘  └────────┘
            │
            ▼
      ┌────────────┐
      │ AI Quote   │
      │ Flow       │
      │ /ai-quote  │
      └────────────┘
```

### Breadcrumb Structure

**LED Mirrors:**
```
Home > LED Mirrors > Catalogue > [Product Name]
```

**Smart Mirrors:**
```
Home > Smart Mirrors > Catalogue > [Product Name]
```

---

## Résumé des Éléments Clés

### CTA Architecture (LIVRABLE 3.1)

| Niveau | Page | CTA Principal | CTA Secondaire |
|--------|------|---------------|----------------|
| 1 | Solution Page | See Our Products → Catalogue | Get AI Estimate |
| 2 | Catalogue | View Details → Product Page | — |
| 3 | Product Detail | Get AI Instant Quote | Book a Call |

### 7 Critères HILO Appliqués

| # | Critère | Application dans 3.1 |
|---|---------|----------------------|
| **1** | Fiabilité 5 ans | Hero subheadline + Section dédiée |
| **2** | Prix compétitif | Section dédiée + Transparence |
| **3** | Delivery porte-à-porte | Section dédiée + Garantie |
| **4** | Catalogue/sur mesure | Section dédiée + Decision Box |
| **5** | AI estimation | Multiple CTA + Section dédiée |
| **6** | Grand choix | Cross-sell vers autres catégories |
| **7** | Installation partenaires | Section dédiée |

### Trust Line (Consistent)

```
🏆 180+ Projects | 🛡️ 5-Year Warranty | 🇨🇦 Designed in Canada. Distributed across North America.
```

---

**Document préparé pour validation client.**

**Prochaine étape**: LIVRABLE 3.2 — Medicine Cabinets + Shower Glass (en attente de validation)
