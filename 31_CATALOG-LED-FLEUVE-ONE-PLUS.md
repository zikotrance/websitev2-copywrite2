# LIVRABLE 7.1 — LED Mirrors: FLEUVE™ Collection

**Projet**: HILO Website Optimization  
**Auteur**: Senior Conversion Architect  
**Date**: Avril 2026  
**Statut**: En attente de validation  
**Collection**: FLEUVE™

---

## Table des Matières

1. [Style Guide HILO](#style-guide-hilo)
2. [Video Block Component](#video-block-component)
3. [Product 1: FLEUVE™ One](#product-1-fleuve-one)
4. [Product 2: FLEUVE™ Plus](#product-2-fleuve-plus)
5. [Product 3: FLEUVE™ Pro](#product-3-fleuve-pro)
6. [Product 4: FLEUVE™ Ultra](#product-4-fleuve-ultra)
7. [Product 5: FLEUVE™ Round](#product-5-fleuve-round)

---

## Style Guide HILO

### Structure des Titres
```
FLEUVE™ [Model] | HILO® Hospitality
```

### Structure des Descriptions
```
FLEUVE™ [Model] by HILO® delivers [bénéfice principal] — ideal for [application].
```

### Trust Line (sur toutes les pages produit)
```
🏆 180+ Projects | 🛡️ 5-Year Warranty | 🇨🇦 Designed in Canada. Distributed across North America.
```

### Les 7 Critères HILO (à intégrer sur chaque page)

| # | Critère | Application Produit |
|---|---------|---------------------|
| 1 | **Fiabilité long terme** | "5-year warranty, <0.5% failure rate" |
| 2 | **Prix compétitif** | "Get AI Instant Quote for project pricing" |
| 3 | **Delivery porte-à-porte** | "Door-to-door delivery, damage-free guarantee" |
| 4 | **Flexibilité** | "Catalogue sizes + custom options available" |
| 5 | **Minimum interaction** | CTA "Get AI Instant Quote" → Wizard 60s |
| 6 | **Grand choix** | Cross-sell vers autres collections |
| 7 | **Installation** | "Installation via certified partners" |

### Éléments Obligatoires par Produit

| Élément | Description |
|---------|-------------|
| **Hero Section** | Image produit in-situ + titre + CTA |
| **Product Description** | Short + Long description |
| **Key Features** | 4-6 bullet points avec icônes |
| **Video Block** | Vidéo interactive avec overlay |
| **Technical Specifications** | Specs détaillées |
| **Product Variations** | Options de configuration |
| **Technical Documents** | Liens fiches techniques + manuels |
| **CTA Section** | Principal + Secondaire |
| **Related Products** | Cross-sell |

---

## Video Block Component

### Comportement Interactif

```
┌────────────────────────────────────────────────────────────────────────┐
│                     VIDEO BLOCK - SPECIFICATIONS                        │
├────────────────────────────────────────────────────────────────────────┤
│                                                                        │
│  ÉTAT INITIAL (avant clic):                                            │
│  ────────────────────────────                                          │
│  • Vidéo visible avec opacité réduite (40-50%)                         │
│  • Overlay sombre semi-transparent                                     │
│  • Bouton PLAY centré (icône cercle + triangle)                        │
│  • Titre + Sous-titre en bas du bloc                                   │
│                                                                        │
│  ÉTAT APRÈS CLIC:                                                      │
│  ────────────────────                                                  │
│  • Vidéo démarre automatiquement                                       │
│  • Opacité passe à 100%                                                │
│  • Overlay disparaît                                                   │
│  • Texte (titre + sous-titre) disparaît                                │
│  • Bouton play disparaît ou devient pause                              │
│                                                                        │
│  CONTRÔLES VIDÉO:                                                      │
│  ─────────────────                                                     │
│  • Barre de progression en bas                                         │
│  • Bouton mute/unmute                                                  │
│  • Bouton fullscreen                                                   │
│  • Clic sur vidéo = pause                                              │
│                                                                        │
└────────────────────────────────────────────────────────────────────────┘
```

### Template HTML/CSS

```html
<!-- VIDEO BLOCK COMPONENT -->
<div class="video-block">
  
  <!-- Video Container -->
  <div class="video-container" id="video-container-[PRODUCT-ID]">
    
    <!-- Video Element -->
    <video 
      class="product-video" 
      id="product-video-[PRODUCT-ID]"
      poster="/assets/videos/[PRODUCT-SLUG]-poster.jpg"
      preload="metadata"
    >
      <source src="/assets/videos/[PRODUCT-SLUG].mp4" type="video/mp4">
      <source src="/assets/videos/[PRODUCT-SLUG].webm" type="video/webm">
    </video>
    
    <!-- Overlay (initial state) -->
    <div class="video-overlay" id="video-overlay-[PRODUCT-ID]">
      
      <!-- Play Button -->
      <button class="play-button" id="play-btn-[PRODUCT-ID]" aria-label="Play video">
        <svg class="play-icon" viewBox="0 0 100 100">
          <circle cx="50" cy="50" r="48" fill="rgba(255,255,255,0.9)" stroke="none"/>
          <polygon points="40,30 40,70 75,50" fill="#1a1a1a"/>
        </svg>
      </button>
      
      <!-- Text Overlay (bottom) -->
      <div class="video-text-overlay">
        <h3 class="video-title">[VIDEO TITLE - Unique per product]</h3>
        <p class="video-subtitle">[VIDEO SUBTITLE - Unique per product]</p>
      </div>
      
    </div>
    
  </div>
  
</div>
```

### Position dans la Page Produit

```
┌──────────────────────────────────────────────────────────────────────┐
│  PAGE PRODUIT - STRUCTURE                                            │
├──────────────────────────────────────────────────────────────────────┤
│                                                                      │
│  1. HERO SECTION (image + titre + CTA)                               │
│  2. PRODUCT DESCRIPTION (short + long)                               │
│  3. KEY FEATURES TABLE                                               │
│  ★ 4. VIDEO BLOCK ◄─── POSITION ICI                                 │
│  5. TECHNICAL SPECIFICATIONS                                         │
│  6. PRODUCT VARIATIONS                                               │
│  7. TECHNICAL DOCUMENTS (fiches + manuels)                           │
│  8. CTA SECTION                                                      │
│  9. RELATED PRODUCTS                                                 │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

---

## Product 1: FLEUVE™ One

### URL Structure
```
/led-mirrors/catalogue/fleuve-one
```

### Product Identity

| Field | Value |
|-------|-------|
| **Collection** | FLEUVE™ |
| **Product Name** | FLEUVE™ One LED Mirror |
| **Tagline** | Essential Illumination. Proven Reliability. |
| **Category** | LED Mirrors - Essential |
| **Application** | Hospitality, Multi-Family, Senior Living |
| **Positionnement** | Entrée de gamme, fonctionnalités essentielles |

### Hero Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  [HERO IMAGE: FLEUVE One LED Mirror in hotel bathroom]              │
│                                                                      │
│  ──────────────────────────────────────────────────────────────────  │
│                                                                      │
│  FLEUVE™ ONE LED MIRROR                                             │
│  ───────────────────────                                            │
│                                                                      │
│  Essential Illumination. Proven Reliability.                        │
│  The Foundation of Every Premium Bathroom Project                   │
│                                                                      │
│  ★★★★★ (127 reviews)                                                │
│                                                                      │
│  [Get AI Instant Quote]  [Book a Call]                              │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

### Product Description

**Short Description:**
> FLEUVE™ One LED Mirror by HILO® delivers reliable, even illumination across the entire mirror surface — ideal for hospitality and multi-family projects seeking essential functionality with proven durability.

**Long Description:**

The FLEUVE™ One represents the foundation of HILO's LED mirror lineup, combining essential functionality with proven durability. Engineered specifically for high-traffic commercial environments, this mirror features edge-to-edge LED illumination that eliminates shadows and provides consistent, flattering light for guests and residents throughout the property.

The slim profile design mounts seamlessly to any wall surface, while the tempered safety glass construction ensures years of trouble-free operation. With over 180 successful installations across North America, the FLEUVE™ One has earned its reputation as the go-to choice for developers and facility managers who prioritize reliability and value without compromising on quality.

Every FLEUVE™ One mirror is backed by HILO's comprehensive 5-year warranty, covering both the LED system and glass components. Our industry-leading failure rate of less than 0.5% means you can specify with confidence, knowing your project will deliver lasting satisfaction for property owners and guests alike.

### Key Features

| Feature | Description |
|---------|-------------|
| 💡 **Edge-to-Edge LED** | 360° uniform illumination, no hot spots or shadows |
| 🛡️ **Tempered Safety Glass** | 5x stronger than standard glass, exceeds ANSI Z97.1 |
| ⏱️ **50,000+ Hour Lifespan** | 17+ years of operation at 8 hours daily use |
| 🎨 **Multiple Finishes** | Available in Chrome, Brushed Nickel, Matte Black, Gold |
| 📐 **Standard & Custom Sizing** | Catalogue sizes + custom dimensions available |
| 🔧 **Easy Installation** | Surface mount or recessed options |

### Video Block

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  ┌────────────────────────────────────────────────────────────────┐  │
│  │                                                                │  │
│  │                    [VIDEO FLEUVE ONE]                          │  │
│  │                    ═════════════════                           │  │
│  │                                                                │  │
│  │                           ▶                                    │  │
│  │                      [PLAY BUTTON]                             │  │
│  │                                                                │  │
│  │  ─────────────────────────────────────────────────────────────│  │
│  │  FLEUVE™ One: Essential Brilliance                            │  │
│  │  See how reliable LED illumination transforms ordinary        │  │
│  │  bathrooms into premium guest experiences.                    │  │
│  └────────────────────────────────────────────────────────────────┘  │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

**Video Content:**
| Field | Value |
|-------|-------|
| **Video File** | `/assets/videos/fleuve-one.mp4` |
| **Poster Image** | `/assets/videos/fleuve-one-poster.jpg` |
| **Video Title** | FLEUVE™ One: Essential Brilliance |
| **Video Subtitle** | See how reliable LED illumination transforms ordinary bathrooms into premium guest experiences. |
| **Duration** | ~45 seconds |

**Video Script Outline:**
1. Opening shot: Dark bathroom, lights turn on revealing FLEUVE One mirror
2. Close-up: Edge-to-edge illumination spreading across mirror surface
3. Application shots: Hotel bathroom, multi-family unit, senior living facility
4. Detail shots: Tempered glass, mounting system, LED components
5. Closing: Guest interaction with mirror, fade to CTA

### Technical Specifications

| Specification | Details |
|---------------|---------|
| **LED Type** | High-efficiency SMD LEDs |
| **Color Temperature** | 3000K (Warm), 4000K (Neutral), 5000K (Cool) |
| **CRI** | >90 (Color Rendering Index) |
| **Wattage** | 18W - 36W (depending on size) |
| **Input Voltage** | 120V AC / 277V AC (commercial) |
| **Mounting** | Surface mount or recessed |
| **Glass Thickness** | 5mm tempered safety glass |
| **Frame Options** | Frameless, Metal Frame (1" profile) |
| **Certifications** | cETLus, CE, IP44 rated |

### Product Variations

#### Available Sizes

| Model | Dimensions | Application |
|-------|------------|-------------|
| FLEUVE-ONE-2430 | 24" x 30" | Standard vanity |
| FLEUVE-ONE-2436 | 24" x 36" | Standard vanity |
| FLEUVE-ONE-3036 | 30" x 36" | Double vanity |
| FLEUVE-ONE-3648 | 36" x 48" | Large bathroom |
| FLEUVE-ONE-4860 | 48" x 60" | Suite bathroom |
| FLEUVE-ONE-4872 | 48" x 72" | Full-length / gym |

#### Configuration Options

| Option | Description | Availability |
|--------|-------------|--------------|
| **Anti-Fog Demister** | Heated pad prevents condensation | Optional |
| **Touch Dimmer** | Adjustable brightness with memory | Optional |
| **Motion Sensor** | Auto on/off activation | Optional |
| **ADA Compliant Mounting** | Pre-configured for accessible installations | Optional |

#### Frame Finishes

| Finish | Code | Application |
|--------|------|-------------|
| Chrome | CR | Classic hospitality |
| Brushed Nickel | BN | Modern residential |
| Matte Black | MB | Contemporary design |
| Brushed Gold | BG | Luxury hospitality |
| Frameless | FL | Minimalist aesthetic |

### Technical Documents

| Document | Description | Link |
|----------|-------------|------|
| **Technical Spec Sheet** | Complete specifications, dimensions, electrical requirements | `/docs/fleuve-one-specs.pdf` |
| **Installation Manual** | Step-by-step installation guide, mounting options | `/docs/fleuve-one-installation.pdf` |
| **Care & Maintenance** | Cleaning instructions, warranty terms | `/docs/fleuve-one-care.pdf` |
| **CAD Drawing** | DWG file for architects and designers | `/docs/fleuve-one-cad.dwg` |
| **Revit Family** | BIM model for project integration | `/docs/fleuve-one.rfa` |
| **LEED Documentation** | Environmental certifications and compliance | `/docs/fleuve-one-leed.pdf` |

### CTA Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  READY TO SPECIFY FLEUVE™ ONE FOR YOUR PROJECT?                     │
│                                                                      │
│  Get an instant AI-powered estimate in 60 seconds.                  │
│  No sales calls. No waiting. Just accurate project pricing.         │
│                                                                      │
│  [Get AI Instant Quote]              [Book a Call]                   │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

### Related Products

| Product | Collection | Note |
|---------|------------|------|
| FLEUVE™ Plus | FLEUVE™ | Anti-fog included |
| FLEUVE™ Pro | FLEUVE™ | Tunable LED, premium features |
| RITUAL™ One | RITUAL™ | Matching medicine cabinet |

---

## Product 2: FLEUVE™ Plus

### URL Structure
```
/led-mirrors/catalogue/fleuve-plus
```

### Product Identity

| Field | Value |
|-------|-------|
| **Collection** | FLEUVE™ |
| **Product Name** | FLEUVE™ Plus LED Mirror |
| **Tagline** | Enhanced Clarity. Built-In Comfort. |
| **Category** | LED Mirrors - Standard |
| **Application** | Hospitality, Multi-Family, Senior Living, Spas |
| **Positionnement** | Standard, anti-fog intégré |

### Hero Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  [HERO IMAGE: FLEUVE Plus LED Mirror in spa bathroom]               │
│                                                                      │
│  ──────────────────────────────────────────────────────────────────  │
│                                                                      │
│  FLEUVE™ PLUS LED MIRROR                                            │
│  ─────────────────────────                                          │
│                                                                      │
│  Enhanced Clarity. Built-In Comfort.                                │
│  Anti-Fog Technology for Clear Reflections Every Time               │
│                                                                      │
│  ★★★★★ (89 reviews)                                                 │
│                                                                      │
│  [Get AI Instant Quote]  [Book a Call]                              │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

### Product Description

**Short Description:**
> FLEUVE™ Plus LED Mirror by HILO® combines edge-to-edge illumination with integrated anti-fog technology — ideal for hospitality projects, spas, and environments where clear reflections are essential after every shower.

**Long Description:**

The FLEUVE™ Plus elevates the essential FLEUVE™ One design with integrated anti-fog technology, ensuring crystal-clear reflections even in the steamiest bathroom environments. A heated demister pad, invisible behind the mirror surface, activates automatically to prevent condensation buildup, eliminating the frustration of foggy mirrors for your guests and residents.

This integrated approach simplifies specification and installation—no separate heating elements to coordinate or additional wiring to manage. The anti-fog system operates quietly and efficiently, consuming minimal power while delivering maximum convenience. For spa environments, luxury hotels, and any property where guest experience matters, the FLEUVE™ Plus represents thoughtful design that anticipates real-world needs.

Like all FLEUVE™ collection mirrors, the Plus model features commercial-grade LED components rated for 50,000+ hours of operation, tempered safety glass, and HILO's comprehensive 5-year warranty that covers the entire system including the anti-fog functionality.

### Key Features

| Feature | Description |
|---------|-------------|
| 💡 **Edge-to-Edge LED** | 360° uniform illumination, no hot spots |
| 🌫️ **Integrated Anti-Fog** | Built-in demister pad, always ready |
| 🛡️ **Tempered Safety Glass** | Commercial-grade, 5x stronger than standard |
| ⏱️ **50,000+ Hour Lifespan** | 17+ years of reliable operation |
| 🎚️ **Touch Dimmer Ready** | Compatible with dimmer upgrade |
| 📐 **Standard & Custom Sizing** | Full range of catalogue and custom sizes |

### Video Block

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  ┌────────────────────────────────────────────────────────────────┐  │
│  │                                                                │  │
│  │                    [VIDEO FLEUVE PLUS]                         │  │
│  │                    ══════════════════                          │  │
│  │                                                                │  │
│  │                           ▶                                    │  │
│  │                      [PLAY BUTTON]                             │  │
│  │                                                                │  │
│  │  ─────────────────────────────────────────────────────────────│  │
│  │  FLEUVE™ Plus: Clarity Without Compromise                     │  │
│  │  Watch how integrated anti-fog technology keeps mirrors      │  │
│  │  crystal clear in any environment.                           │  │
│  └────────────────────────────────────────────────────────────────┘  │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

**Video Content:**
| Field | Value |
|-------|-------|
| **Video File** | `/assets/videos/fleuve-plus.mp4` |
| **Poster Image** | `/assets/videos/fleuve-plus-poster.jpg` |
| **Video Title** | FLEUVE™ Plus: Clarity Without Compromise |
| **Video Subtitle** | Watch how integrated anti-fog technology keeps mirrors crystal clear in any environment. |
| **Duration** | ~50 seconds |

**Video Script Outline:**
1. Opening shot: Steamy bathroom after hot shower
2. Comparison: Standard mirror foggy vs FLEUVE Plus crystal clear
3. Technology demonstration: Anti-fog pad activation visualized
4. Application shots: Spa, hotel suite, residential bathroom
5. Closing: Guest enjoying clear reflection, fade to CTA

### Technical Specifications

| Specification | Details |
|---------------|---------|
| **LED Type** | High-efficiency SMD LEDs |
| **Color Temperature** | 3000K, 4000K, 5000K |
| **CRI** | >90 |
| **Anti-Fog Power** | 15W - 25W (depending on size) |
| **Total Wattage** | 33W - 61W (LED + anti-fog) |
| **Input Voltage** | 120V AC / 277V AC |
| **Mounting** | Surface mount or recessed |
| **Glass Thickness** | 5mm tempered safety glass |
| **Certifications** | cETLus, CE, IP44 rated |

### Product Variations

#### Available Sizes

| Model | Dimensions | Application |
|-------|------------|-------------|
| FLEUVE-PLUS-2430 | 24" x 30" | Standard vanity |
| FLEUVE-PLUS-2436 | 24" x 36" | Standard vanity |
| FLEUVE-PLUS-3036 | 30" x 36" | Double vanity |
| FLEUVE-PLUS-3648 | 36" x 48" | Large bathroom |
| FLEUVE-PLUS-4860 | 48" x 60" | Suite bathroom |

#### Configuration Options

| Option | Description | Availability |
|--------|-------------|--------------|
| **Touch Dimmer** | Adjustable brightness with memory | Optional |
| **Motion Sensor** | Auto on/off activation | Optional |
| **Tunable LED** | Adjustable color temperature 2700K-5000K | Optional |

#### Frame Finishes

| Finish | Code | Application |
|--------|------|-------------|
| Chrome | CR | Classic hospitality |
| Brushed Nickel | BN | Modern residential |
| Matte Black | MB | Contemporary design |
| Brushed Gold | BG | Luxury hospitality |
| Frameless | FL | Minimalist aesthetic |

### Technical Documents

| Document | Description | Link |
|----------|-------------|------|
| **Technical Spec Sheet** | Complete specifications, dimensions, electrical requirements | `/docs/fleuve-plus-specs.pdf` |
| **Installation Manual** | Step-by-step installation guide, mounting options | `/docs/fleuve-plus-installation.pdf` |
| **Care & Maintenance** | Cleaning instructions, warranty terms | `/docs/fleuve-plus-care.pdf` |
| **CAD Drawing** | DWG file for architects and designers | `/docs/fleuve-plus-cad.dwg` |
| **Revit Family** | BIM model for project integration | `/docs/fleuve-plus.rfa` |

### CTA Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  ELEVATE YOUR PROJECT WITH FLEUVE™ PLUS                             │
│                                                                      │
│  Anti-fog LED mirrors for crystal-clear reflections.                │
│  Get an instant AI-powered estimate in 60 seconds.                  │
│                                                                      │
│  [Get AI Instant Quote]              [Book a Call]                   │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

### Related Products

| Product | Collection | Note |
|---------|------------|------|
| FLEUVE™ One | FLEUVE™ | Essential version |
| FLEUVE™ Pro | FLEUVE™ | Premium with tunable LED |
| RITUAL™ Plus | RITUAL™ | Matching medicine cabinet |

---

## Product 3: FLEUVE™ Pro

### URL Structure
```
/led-mirrors/catalogue/fleuve-pro
```

### Product Identity

| Field | Value |
|-------|-------|
| **Collection** | FLEUVE™ |
| **Product Name** | FLEUVE™ Pro LED Mirror |
| **Tagline** | Professional Performance. Premium Features. |
| **Category** | LED Mirrors - Premium |
| **Application** | Premium Hospitality, Luxury Multi-Family, Boutique Hotels |
| **Positionnement** | Premium, tunable LED, toutes fonctionnalités |

### Hero Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  [HERO IMAGE: FLEUVE Pro LED Mirror in boutique hotel suite]        │
│                                                                      │
│  ──────────────────────────────────────────────────────────────────  │
│                                                                      │
│  FLEUVE™ PRO LED MIRROR                                             │
│  ───────────────────────                                            │
│                                                                      │
│  Professional Performance. Premium Features.                        │
│  Tunable LED + Anti-Fog + Dimmer for Complete Control               │
│                                                                      │
│  ★★★★★ (73 reviews)                                                 │
│                                                                      │
│  [Get AI Instant Quote]  [Book a Call]                              │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

### Product Description

**Short Description:**
> FLEUVE™ Pro LED Mirror by HILO® delivers professional-grade performance with tunable LED technology, integrated anti-fog, and touch dimmer — ideal for premium hospitality and luxury developments where complete lighting control is essential.

**Long Description:**

The FLEUVE™ Pro represents the pinnacle of the FLEUVE™ collection, combining every premium feature into a single, sophisticated package. The tunable LED system allows adjustment of color temperature from warm 2700K to cool 5000K, enabling guests and residents to customize their lighting environment for any activity—from relaxing evening ambiance to bright, energizing morning preparation.

Integrated anti-fog technology ensures clear reflections in any humidity condition, while the touch-sensitive dimmer provides smooth brightness control from 10% to 100% with automatic memory of the last setting. Every interaction feels premium, from the responsive touch controls to the gradual fade-in when the mirror activates.

For property developers and hospitality brands seeking to differentiate their offerings, the FLEUVE™ Pro provides tangible luxury features that guests notice and appreciate. The combination of advanced technology with HILO's proven reliability and comprehensive 5-year warranty makes this mirror a specification choice that delivers lasting value and guest satisfaction.

### Key Features

| Feature | Description |
|---------|-------------|
| 🌡️ **Tunable LED** | Adjustable color temperature 2700K-5000K |
| 🌫️ **Integrated Anti-Fog** | Built-in demister, always ready |
| 🎚️ **Touch Dimmer** | Smooth 10-100% brightness control with memory |
| 💡 **High CRI >92** | Superior color rendering for accurate reflection |
| 🛡️ **Premium Tempered Glass** | 6mm commercial-grade safety glass |
| 🔧 **Smart Integration Ready** | Compatible with building automation systems |

### Video Block

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  ┌────────────────────────────────────────────────────────────────┐  │
│  │                                                                │  │
│  │                    [VIDEO FLEUVE PRO]                          │  │
│  │                    ═════════════════                           │  │
│  │                                                                │  │
│  │                           ▶                                    │  │
│  │                      [PLAY BUTTON]                             │  │
│  │                                                                │  │
│  │  ─────────────────────────────────────────────────────────────│  │
│  │  FLEUVE™ Pro: Complete Control                                │  │
│  │  Discover how tunable LED and premium features create        │  │
│  │  the ultimate bathroom lighting experience.                   │  │
│  └────────────────────────────────────────────────────────────────┘  │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

**Video Content:**
| Field | Value |
|-------|-------|
| **Video File** | `/assets/videos/fleuve-pro.mp4` |
| **Poster Image** | `/assets/videos/fleuve-pro-poster.jpg` |
| **Video Title** | FLEUVE™ Pro: Complete Control |
| **Video Subtitle** | Discover how tunable LED and premium features create the ultimate bathroom lighting experience. |
| **Duration** | ~55 seconds |

**Video Script Outline:**
1. Opening shot: Luxury boutique hotel suite
2. Color temperature demonstration: Warm to cool transition
3. Touch dimmer interaction: Brightness adjustment
4. Anti-fog demonstration: Steam clearing instantly
5. Application shots: Presidential suite, luxury condo, spa
6. Closing: Guest customizing their lighting, fade to CTA

### Technical Specifications

| Specification | Details |
|---------------|---------|
| **LED Type** | Premium tunable SMD LEDs |
| **Color Temperature Range** | 2700K - 5000K (adjustable) |
| **CRI** | >92 |
| **Dimming Range** | 10% - 100% |
| **Anti-Fog Power** | 15W - 25W |
| **Total Wattage** | 39W - 73W (depending on size) |
| **Input Voltage** | 120V AC / 277V AC |
| **Mounting** | Surface mount or recessed |
| **Glass Thickness** | 6mm tempered safety glass |
| **Certifications** | cETLus, CE, IP44 rated |

### Product Variations

#### Available Sizes

| Model | Dimensions | Application |
|-------|------------|-------------|
| FLEUVE-PRO-2436 | 24" x 36" | Standard vanity |
| FLEUVE-PRO-3036 | 30" x 36" | Double vanity |
| FLEUVE-PRO-3648 | 36" x 48" | Large bathroom |
| FLEUVE-PRO-4860 | 48" x 60" | Suite bathroom |
| FLEUVE-PRO-4872 | 48" x 72" | Full-length / luxury suite |

#### Configuration Options

| Option | Description | Availability |
|--------|-------------|--------------|
| **Motion Sensor** | Auto on/off activation | Optional |
| **Smart Home Integration** | App control via Zigbee/WiFi | Optional |
| **Extended Warranty** | 7-year comprehensive coverage | Optional |

#### Frame Finishes

| Finish | Code | Application |
|--------|------|-------------|
| Chrome | CR | Classic hospitality |
| Brushed Nickel | BN | Modern residential |
| Matte Black | MB | Contemporary design |
| Brushed Gold | BG | Luxury hospitality |
| Frameless | FL | Minimalist aesthetic |

### Technical Documents

| Document | Description | Link |
|----------|-------------|------|
| **Technical Spec Sheet** | Complete specifications, dimensions, electrical requirements | `/docs/fleuve-pro-specs.pdf` |
| **Installation Manual** | Step-by-step installation guide, mounting options | `/docs/fleuve-pro-installation.pdf` |
| **Tunable LED Guide** | Color temperature adjustment instructions | `/docs/fleuve-pro-tunable-guide.pdf` |
| **Care & Maintenance** | Cleaning instructions, warranty terms | `/docs/fleuve-pro-care.pdf` |
| **CAD Drawing** | DWG file for architects and designers | `/docs/fleuve-pro-cad.dwg` |
| **Revit Family** | BIM model for project integration | `/docs/fleuve-pro.rfa` |
| **Smart Integration API** | Technical documentation for automation integration | `/docs/fleuve-pro-api.pdf` |

### CTA Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  SPECIFY PREMIUM WITH FLEUVE™ PRO                                   │
│                                                                      │
│  Professional LED mirrors with complete control features.           │
│  Get an instant AI-powered estimate in 60 seconds.                  │
│                                                                      │
│  [Get AI Instant Quote]              [Book a Call]                   │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

### Related Products

| Product | Collection | Note |
|---------|------------|------|
| FLEUVE™ Ultra | FLEUVE™ | Backlit + edge-lit combined |
| NEXA™ Pro | NEXA™ | Smart mirror upgrade |
| RITUAL™ Pro | RITUAL™ | Matching medicine cabinet |

---

## Product 4: FLEUVE™ Ultra

### URL Structure
```
/led-mirrors/catalogue/fleuve-ultra
```

### Product Identity

| Field | Value |
|-------|-------|
| **Collection** | FLEUVE™ |
| **Product Name** | FLEUVE™ Ultra LED Mirror |
| **Tagline** | Dual Illumination. Maximum Impact. |
| **Category** | LED Mirrors - Luxury |
| **Application** | Luxury Hotels, Premium Multi-Family, Signature Spaces |
| **Positionnement** | Luxe, backlit + edge-lit combinés |

### Hero Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  [HERO IMAGE: FLEUVE Ultra LED Mirror with dual lighting effect]    │
│                                                                      │
│  ──────────────────────────────────────────────────────────────────  │
│                                                                      │
│  FLEUVE™ ULTRA LED MIRROR                                           │
│  ──────────────────────────                                         │
│                                                                      │
│  Dual Illumination. Maximum Impact.                                 │
│  Backlit + Edge-Lit for Dramatic Floating Effect                    │
│                                                                      │
│  ★★★★★ (54 reviews)                                                 │
│                                                                      │
│  [Get AI Instant Quote]  [Book a Call]                              │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

### Product Description

**Short Description:**
> FLEUVE™ Ultra LED Mirror by HILO® combines backlit halo effect with edge-lit illumination for a dramatic floating appearance — ideal for luxury hospitality and premium developments seeking maximum visual impact.

**Long Description:**

The FLEUVE™ Ultra represents the ultimate expression of LED mirror design, combining two distinct lighting systems into one stunning installation. The backlit LED array creates a soft, ambient halo effect that makes the mirror appear to float elegantly off the wall, while the edge-lit perimeter provides brilliant, even illumination for task lighting and daily grooming activities.

This dual-system approach offers unparalleled flexibility in creating ambiance. The backlight can operate independently for subtle nighttime glow, while the edge lighting provides functional illumination when needed. Both systems feature independent dimming and can be controlled separately, allowing guests and residents to create their perfect lighting environment for any time of day or activity.

The floating design conceals all mounting hardware and electrical connections behind the mirror, delivering a clean, minimalist aesthetic that complements the most sophisticated interior design schemes. Every FLEUVE™ Ultra installation becomes a signature element, transforming ordinary bathrooms into spa-like retreats that leave lasting impressions on guests and residents.

### Key Features

| Feature | Description |
|---------|-------------|
| ✨ **Dual LED System** | Backlit + edge-lit for complete lighting flexibility |
| 🌟 **Floating Effect** | Halo glow creates stunning visual depth |
| 🌫️ **Integrated Anti-Fog** | Built-in demister technology |
| 🎚️ **Independent Dimming** | Separate control for back and edge lighting |
| 🛡️ **Premium Glass** | 6mm low-iron tempered safety glass |
| 📱 **Smart Ready** | Compatible with automation systems |

### Video Block

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  ┌────────────────────────────────────────────────────────────────┐  │
│  │                                                                │  │
│  │                    [VIDEO FLEUVE ULTRA]                        │  │
│  │                    ═══════════════════                         │  │
│  │                                                                │  │
│  │                           ▶                                    │  │
│  │                      [PLAY BUTTON]                             │  │
│  │                                                                │  │
│  │  ─────────────────────────────────────────────────────────────│  │
│  │  FLEUVE™ Ultra: Light Redefined                               │  │
│  │  Experience the dramatic combination of backlit and           │  │
│  │  edge-lit illumination in perfect harmony.                    │  │
│  └────────────────────────────────────────────────────────────────┘  │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

**Video Content:**
| Field | Value |
|-------|-------|
| **Video File** | `/assets/videos/fleuve-ultra.mp4` |
| **Poster Image** | `/assets/videos/fleuve-ultra-poster.jpg` |
| **Video Title** | FLEUVE™ Ultra: Light Redefined |
| **Video Subtitle** | Experience the dramatic combination of backlit and edge-lit illumination in perfect harmony. |
| **Duration** | ~55 seconds |

**Video Script Outline:**
1. Opening shot: Luxury hotel suite at twilight
2. Backlight activation: Soft halo effect emerging
3. Edge light activation: Brilliant illumination
4. Dual lighting demonstration: Both systems in harmony
5. Application shots: Presidential suite, luxury condo, spa
6. Independent dimming: Custom lighting scenes
7. Closing: Dramatic floating effect, fade to CTA

### Technical Specifications

| Specification | Details |
|---------------|---------|
| **Edge LED Type** | High-output SMD LEDs |
| **Backlight Type** | Diffused LED array |
| **Color Temperature** | 2700K-5000K tunable |
| **CRI** | >92 |
| **Backlight Wattage** | 18W - 36W |
| **Edge Light Wattage** | 24W - 48W |
| **Anti-Fog Power** | 15W - 25W |
| **Total Wattage** | 57W - 109W (depending on size) |
| **Projection** | 2" from wall (including backlight gap) |
| **Glass Thickness** | 6mm low-iron tempered glass |
| **Certifications** | cETLus, CE, IP44 rated |

### Product Variations

#### Available Sizes

| Model | Dimensions | Application |
|-------|------------|-------------|
| FLEUVE-ULTRA-2436 | 24" x 36" | Standard vanity |
| FLEUVE-ULTRA-3036 | 30" x 36" | Double vanity |
| FLEUVE-ULTRA-3648 | 36" x 48" | Large bathroom |
| FLEUVE-ULTRA-4860 | 48" x 60" | Suite bathroom |
| FLEUVE-ULTRA-4872 | 48" x 72" | Full-length / luxury suite |

#### Configuration Options

| Option | Description | Availability |
|--------|-------------|--------------|
| **Motion Sensor** | Auto on/off activation | Optional |
| **Smart Home Integration** | App control via Zigbee/WiFi | Optional |
| **RGBW Backlight** | Color-changing backlight option | Optional |
| **Extended Warranty** | 7-year comprehensive coverage | Optional |

#### Frame Finishes

| Finish | Code | Application |
|--------|------|-------------|
| Chrome | CR | Classic hospitality |
| Brushed Nickel | BN | Modern residential |
| Matte Black | MB | Contemporary design |
| Brushed Gold | BG | Luxury hospitality |
| Frameless | FL | Minimalist aesthetic |

### Technical Documents

| Document | Description | Link |
|----------|-------------|------|
| **Technical Spec Sheet** | Complete specifications, dimensions, electrical requirements | `/docs/fleuve-ultra-specs.pdf` |
| **Installation Manual** | Step-by-step installation guide, mounting options | `/docs/fleuve-ultra-installation.pdf` |
| **Dual System Guide** | Backlight and edge light operation instructions | `/docs/fleuve-ultra-dual-guide.pdf` |
| **Care & Maintenance** | Cleaning instructions, warranty terms | `/docs/fleuve-ultra-care.pdf` |
| **CAD Drawing** | DWG file for architects and designers | `/docs/fleuve-ultra-cad.dwg` |
| **Revit Family** | BIM model for project integration | `/docs/fleuve-ultra.rfa` |

### CTA Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  CREATE DRAMATIC IMPACT WITH FLEUVE™ ULTRA                          │
│                                                                      │
│  Dual illumination LED mirrors for signature spaces.                │
│  Get an instant AI-powered estimate in 60 seconds.                  │
│                                                                      │
│  [Get AI Instant Quote]              [Book a Call]                   │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

### Related Products

| Product | Collection | Note |
|---------|------------|------|
| FLEUVE™ Pro | FLEUVE™ | Single system premium option |
| NEXA™ Ultra | NEXA™ | Smart mirror upgrade |
| RITUAL™ Pro | RITUAL™ | Matching medicine cabinet |

---

## Product 5: FLEUVE™ Round

### URL Structure
```
/led-mirrors/catalogue/fleuve-round
```

### Product Identity

| Field | Value |
|-------|-------|
| **Collection** | FLEUVE™ |
| **Product Name** | FLEUVE™ Round LED Mirror |
| **Tagline** | Organic Curves. Elegant Illumination. |
| **Category** | LED Mirrors - Round/Oval |
| **Application** | Boutique Hotels, Spas, Wellness Centers, Design-Forward Spaces |
| **Positionnement** | Formes organiques, design signature |

### Hero Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  [HERO IMAGE: FLEUVE Round LED Mirror in spa bathroom]              │
│                                                                      │
│  ──────────────────────────────────────────────────────────────────  │
│                                                                      │
│  FLEUVE™ ROUND LED MIRROR                                           │
│  ──────────────────────────                                         │
│                                                                      │
│  Organic Curves. Elegant Illumination.                              │
│  Round and Oval Designs for Distinctive Spaces                      │
│                                                                      │
│  ★★★★★ (67 reviews)                                                 │
│                                                                      │
│  [Get AI Instant Quote]  [Book a Call]                              │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

### Product Description

**Short Description:**
> FLEUVE™ Round LED Mirror by HILO® combines soft, rounded silhouettes with brilliant edge lighting — ideal for boutique hotels, spas, and design-forward spaces seeking distinctive bathroom elements.

**Long Description:**

The FLEUVE™ Round collection breaks from traditional rectangular designs with a stunning range of round and oval LED mirrors that bring organic elegance to any bathroom environment. These curved silhouettes soften architectural lines and create visual interest, making them perfect for boutique properties seeking differentiation in a competitive market where every design element matters.

Each FLEUVE™ Round mirror features precision-engineered edge lighting that follows the curved contour, delivering uniform illumination without the hot spots or inconsistencies common in curved LED applications. The result is a flawless, flattering light that enhances the guest experience while meeting the practical demands of daily use in commercial environments.

Available in multiple sizes and proportions, FLEUVE™ Round mirrors can be specified as statement pieces above vanities or grouped in creative arrangements for dramatic effect. Every mirror undergoes HILO's rigorous quality testing and is backed by our comprehensive 5-year warranty, ensuring lasting performance in demanding commercial environments.

### Key Features

| Feature | Description |
|---------|-------------|
| ⭕ **Curved Silhouettes** | Round and oval designs in multiple proportions |
| 💡 **Contoured Edge Lighting** | Uniform illumination following curved profile |
| 🌫️ **Anti-Fog Option** | Integrated demister for spa environments |
| 🔲 **Frameless Design** | Clean, uninterrupted reflection surface |
| 🛡️ **Curved Tempered Glass** | Specialized tempering for curved safety glass |
| 📐 **Custom Shapes** | Arch, capsule, and custom radius available |

### Video Block

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  ┌────────────────────────────────────────────────────────────────┐  │
│  │                                                                │  │
│  │                    [VIDEO FLEUVE ROUND]                        │  │
│  │                    ════════════════════                        │  │
│  │                                                                │  │
│  │                           ▶                                    │  │
│  │                      [PLAY BUTTON]                             │  │
│  │                                                                │  │
│  │  ─────────────────────────────────────────────────────────────│  │
│  │  FLEUVE™ Round: Curves That Captivate                         │  │
│  │  Experience how organic silhouettes and precision lighting    │  │
│  │  create spa-like tranquility in any space.                    │  │
│  └────────────────────────────────────────────────────────────────┘  │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

**Video Content:**
| Field | Value |
|-------|-------|
| **Video File** | `/assets/videos/fleuve-round.mp4` |
| **Poster Image** | `/assets/videos/fleuve-round-poster.jpg` |
| **Video Title** | FLEUVE™ Round: Curves That Captivate |
| **Video Subtitle** | Experience how organic silhouettes and precision lighting create spa-like tranquility in any space. |
| **Duration** | ~55 seconds |

**Video Script Outline:**
1. Opening shot: Spa bathroom with soft natural light
2. Hero shot: Round FLEUVE mirror with edge lighting illuminating
3. Shape montage: Round, oval, and arch variants in sequence
4. Application shots: Boutique hotel, wellness center, luxury residence
5. Detail: Contoured edge lighting following curved profile
6. Closing: Peaceful guest reflection, soft fade to CTA

### Technical Specifications

| Specification | Details |
|---------------|---------|
| **LED Type** | Flexible LED strip with optical diffuser |
| **Color Temperature** | 3000K, 4000K, 5000K, or tunable |
| **CRI** | >90 |
| **Wattage** | 15W - 32W (depending on size) |
| **Input Voltage** | 120V AC / 277V AC |
| **Mounting** | Surface mount with concealed bracket |
| **Glass Thickness** | 5mm curved tempered safety glass |
| **Certifications** | cETLus, CE, IP44 rated |

### Product Variations

#### Available Shapes & Sizes

| Model | Shape | Dimensions | Application |
|-------|-------|------------|-------------|
| FLEUVE-RD-24 | Round | 24" diameter | Standard vanity |
| FLEUVE-RD-30 | Round | 30" diameter | Double vanity |
| FLEUVE-RD-36 | Round | 36" diameter | Statement piece |
| FLEUVE-OV-2436 | Oval | 24" x 36" | Standard vanity |
| FLEUVE-OV-3048 | Oval | 30" x 48" | Large bathroom |
| FLEUVE-AR-3648 | Arch | 36" x 48" | Signature design |

#### Configuration Options

| Option | Description | Availability |
|--------|-------------|--------------|
| **Anti-Fog Demister** | Heated pad for spa/humid environments | Optional |
| **Touch Dimmer** | On-mirror touch control with memory | Optional |
| **Tunable LED** | Adjustable color temperature | Optional |
| **Pivoting Mount** | Adjustable angle mounting system | Optional |

### Technical Documents

| Document | Description | Link |
|----------|-------------|------|
| **Technical Spec Sheet** | Complete specifications, dimensions, electrical requirements | `/docs/fleuve-round-specs.pdf` |
| **Installation Manual** | Step-by-step installation guide, mounting options | `/docs/fleuve-round-installation.pdf` |
| **Shape Options Guide** | Overview of round, oval, and arch configurations | `/docs/fleuve-round-shapes.pdf` |
| **Care & Maintenance** | Cleaning instructions, warranty terms | `/docs/fleuve-round-care.pdf` |
| **CAD Drawing** | DWG file for architects and designers | `/docs/fleuve-round-cad.dwg` |
| **Revit Family** | BIM model for project integration | `/docs/fleuve-round.rfa` |

### CTA Section

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  ADD ELEGANT CURVES TO YOUR DESIGN WITH FLEUVE™ ROUND               │
│                                                                      │
│  Round and oval LED mirrors for distinctive spaces.                 │
│  Custom shapes available for unique architectural requirements.      │
│                                                                      │
│  [Get AI Instant Quote]              [Book a Call]                   │
│                                                                      │
│  🏆 180+ Projects | 🛡️ 5-Year Warranty |                            │
│  🇨🇦 Designed in Canada. Distributed across North America.           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

### Related Products

| Product | Collection | Note |
|---------|------------|------|
| FLEUVE™ Plus | FLEUVE™ | Rectangular with anti-fog |
| FLEUVE™ Pro | FLEUVE™ | Premium features |
| RITUAL™ Pro | RITUAL™ | Matching medicine cabinet |

---

## Récapitulatif Collection FLEUVE™

| Model | Positionnement | Fonctionnalités Clés |
|-------|----------------|---------------------|
| **FLEUVE™ One** | Entrée de gamme | LED edge-lit, essential features |
| **FLEUVE™ Plus** | Standard | LED + Anti-fog intégré |
| **FLEUVE™ Pro** | Premium | LED + Anti-fog + Tunable + Dimmer |
| **FLEUVE™ Ultra** | Luxe | Backlit + Edge-lit dual system |
| **FLEUVE™ Round** | Design | Round/Oval/Arch shapes |

---

## Prochaines Étapes

- **LIVRABLE 7.2**: Continuer LED Mirrors avec modèles additionnels si requis
- **LIVRABLE 8.x**: Collection NEXA™ (Smart Mirrors)
- **LIVRABLE 9.x**: Collection RITUAL™ (Medicine Cabinets)
- **LIVRABLE 10.x**: Collection CASCADE™ (Shower Glass)
- **LIVRABLE 11.x**: Collection MONOLITH™ (Architectural Glass)
- **LIVRABLE 12.x**: Collection LUMINA™ (Standard Mirrors)

---

**LIVRABLE 7.1 — Complet**

*En attente de validation avant de continuer avec le prochain livrable.*
