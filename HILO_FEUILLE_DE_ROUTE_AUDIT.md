# FEUILLE DE ROUTE & SYSTÈME D'AUDIT — HILO Website Optimization

**Version**: 1.0  
**Date**: Avril 2026  
**Auteur**: Senior Conversion Architect  
**Statut**: Document de référence pour exécution

---

## 📋 PHASE 1 — CORRECTIONS CRITIQUES

### Séquencement d'Exécution

| Étape | Livrable | Actions | Priorité | Dépendances |
|-------|----------|---------|----------|-------------|
| 1.1 | LIVRABLE 8.1 | Supprimer prix + Corriger CTAs | 🔴 CRITIQUE | Aucune |
| 1.2 | LIVRABLE 8.2 | Supprimer prix + Corriger CTAs | 🔴 CRITIQUE | Aucune |
| 1.3 | LIVRABLE 8.3 | Supprimer prix + Corriger CTAs | 🔴 CRITIQUE | Aucune |
| 1.4 | LIVRABLE 8.4 | Supprimer prix + Corriger CTAs | 🔴 CRITIQUE | Aucune |
| 1.5 | LIVRABLE 9.1 | Supprimer prix + Corriger CTAs | 🔴 CRITIQUE | Aucune |

### Actions Obligatoires par Livrable

#### A. Suppression des Prix

| Élément à supprimer | Exemple | Remplacement |
|---------------------|---------|--------------|
| Ligne "From $X,XXX" | `From $1,299` | **SUPPRIMER** |
| Colonne "Price From" | Tableau des tailles | **SUPPRIMER LA COLONNE** |
| Colonne "Price Add" | Tableau Options & Upgrades | **SUPPRIMER LA COLONNE** |
| Toute mention "$" | `$1,299`, `+$299` | **SUPPRIMER** |

#### B. Correction des CTAs

| CTA Incorrect | CTA Correct | Contexte |
|---------------|-------------|----------|
| `Book a Consultation` | `Book a Call` | Hero Section |
| `Book a Consultation` | `Book a Call` | CTA Section |

### Contraintes Phase 1

```
┌─────────────────────────────────────────────────────────────────────────┐
│  ⚠️ CONTRAINTES PHASE 1                                                 │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  ✓ Ne PAS modifier le contenu textuel au-delà des corrections          │
│  ✓ Ne PAS changer la structure des documents                           │
│  ✓ Ne PAS réécrire les descriptions                                    │
│  ✓ Conserver tous les tableaux techniques                              │
│  ✓ Préserver les Video Blocks et specifications                        │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## 📋 PHASE 2 — UNIFORMISATION GLOBALE

### Séquencement d'Exécution

| Étape | Action | Livrables | Priorité | Dépendances |
|-------|--------|-----------|----------|-------------|
| 2.1 | Standardisation ton | Tous | 🟠 HAUTE | Phase 1 complète |
| 2.2 | Standardisation structure sections | Tous | 🟠 HAUTE | 2.1 |
| 2.3 | Standardisation format titres | Tous | 🟠 HAUTE | 2.2 |
| 2.4 | Standardisation style CTAs | Tous | 🟠 HAUTE | 2.3 |
| 2.5 | Standardisation hiérarchie visuelle | Tous | 🟡 MOYENNE | 2.4 |

### Standards à Appliquer

#### A. Ton et Niveau de Langage

| Caractéristique | Standard HILO |
|-----------------|---------------|
| **Ton** | Professionnel, direct, orienté bénéfices |
| **Vocabulaire** | Pas de slang, pas d'emojis excessifs |
| **Phrases** | Simples, claires, sans jargon |
| **Données** | Vérifiables, pas d'hyperboles |

#### B. Structure des Sections Produit

```
1. URL Structure
2. Product Identity (tableau)
3. Hero Section (diagramme ASCII)
4. Product Description (Short + Long)
5. Key Features (tableau)
6. Video Block (diagramme + contenu)
7. Technical Specifications (tableau)
8. Available Sizes (tableau SANS prix)
9. Options & Upgrades (tableau SANS prix)
10. CTA Section (diagramme ASCII)
```

#### C. Format des Titres

| Élément | Format |
|---------|--------|
| **Titre produit** | `[NOM]™ Smart Mirror` |
| **Tagline** | `[Phrase courte]. [Phrase courte].` |
| **URL** | `/smart-mirrors/catalogue/[slug]` |

#### D. Style des CTAs

| Position | CTA Principal | CTA Secondaire |
|----------|---------------|----------------|
| Hero | `[Get AI Instant Quote]` | `[Book a Call]` |
| CTA Section | `[Get AI Instant Quote]` | `[Book a Call]` |

#### E. Trust Line (Obligatoire)

```
🏆 180+ Projects | 🛡️ 5-Year Warranty | 🇨🇦 Designed in Canada. Distributed across North America.
```

### Contraintes Phase 2

```
┌─────────────────────────────────────────────────────────────────────────┐
│  ⚠️ CONTRAINTES PHASE 2                                                 │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  ✓ AUCUNE réécriture du contenu (seulement harmonisation)              │
│  ✓ Respect total de l'intention initiale de chaque section             │
│  ✓ Ne PAS ajouter de nouveau contenu                                   │
│  ✓ Ne PAS supprimer de sections existantes                             │
│  ✓ Conserver les différences légitimes entre produits                  │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## 🔍 SYSTÈME D'AUDIT

### Checklist de Validation — Page Produit

```
□ TRUST LINE présente et exacte
□ AUCUN prix visible (règle absolue)
□ CTA Principal: "Get AI Instant Quote"
□ CTA Secondaire: "Book a Call" (pas "Consultation")
□ Structure sections respectée
□ Tableau Available Sizes SANS colonne prix
□ Tableau Options SANS colonne prix
□ Video Block présent avec titre/sous-titre uniques
□ Technical Specifications complètes
□ Ton professionnel maintenu
□ Minimum 150 mots par section principale
□ Paragraphes de 3-5 phrases minimum
```

### Checklist de Validation — Conformité 7 Critères HILO

```
□ Critère #1: Fiabilité long terme (5 ans, <0.5% failure rate)
□ Critère #2: Prix compétitif (mention "competitive pricing")
□ Critère #3: Delivery porte-à-porte
□ Critère #4: Flexibilité (catalogue + sur mesure)
□ Critère #5: Minimum interaction (CTA AI Quote visible)
□ Critère #6: Grand choix (cross-sell présent)
□ Critère #7: Installation (partenaires certifiés)
```

### Critères de Conformité B2B Premium

| Critère | Standard | Validation |
|---------|----------|------------|
| **Ton** | Professionnel, sans familiarité | Relecture humaine |
| **Vocabulaire** | "Reliable", "Proven" vs "Amazing" | Recherche mots interdits |
| **Structure** | Cohérente entre pages | Comparaison automatisée |
| **CTAs** | Action-oriented, cohérents | Recherche patterns |
| **Données** | Spécifiques, vérifiables | Validation manuelle |

### Système de Détection des Écarts

| Type d'écart | Détection | Action |
|--------------|-----------|--------|
| Prix visible | Recherche regex `\$[0-9]` | Suppression immédiate |
| CTA incorrect | Recherche `Consultation` | Remplacement par `Call` |
| Trust Line manquante | Recherche pattern | Ajout |
| Section manquante | Comparaison structure | Ajout si critique |
| Ton inapproprié | Liste mots interdits | Flag pour révision |

---

## ✅ PROCESS DE VALIDATION FINALE

### Étape 1: Validation Automatisée

```bash
# Checks automatisés
1. Aucun prix visible (regex \$[0-9,]+)
2. CTAs corrects (pas "Consultation")
3. Trust Line présente sur toutes les pages
4. Structure sections complète
```

### Étape 2: Validation Humaine

```
1. Cohérence ton et style
2. Intention conversion préservée
3. Lisibilité et clarté
4. Alignement B2B premium
```

### Étape 3: Validation Cross-Collection

```
1. Comparaison FLEUVE™ vs Smart Mirrors vs Medicine Cabinets
2. Uniformité des patterns
3. Cohérence globale du catalogue
```

### Étape 4: Sign-Off Final

```
□ Toutes corrections Phase 1 appliquées
□ Toutes uniformisations Phase 2 appliquées
□ Tous checks automatisés passés
□ Validation humaine complétée
□ Validation cross-collection complétée
□ Document mis à jour
```

---

## 📊 TABLEAU DE SUIVI

### Phase 1 — Corrections Critiques

| Livrable | Prix Supprimés | CTAs Corrigés | Trust Line | Statut |
|----------|----------------|---------------|------------|--------|
| 8.1 | ⬜ | ⬜ | ⬜ | ⏳ En attente |
| 8.2 | ⬜ | ⬜ | ⬜ | ⏳ En attente |
| 8.3 | ⬜ | ⬜ | ⬜ | ⏳ En attente |
| 8.4 | ⬜ | ⬜ | ⬜ | ⏳ En attente |
| 9.1 | ⬜ | ⬜ | ⬜ | ⏳ En attente |

### Phase 2 — Uniformisation

| Élément | FLEUVE™ (7.x) | Smart (8.x) | Med Cab (9.x) | Statut |
|---------|---------------|-------------|---------------|--------|
| Ton | ✅ | ⏳ | ⏳ | En attente |
| Structure | ✅ | ⏳ | ⏳ | En attente |
| Titres | ✅ | ⏳ | ⏳ | En attente |
| CTAs | ✅ | ⏳ | ⏳ | En attente |
| Hiérarchie | ✅ | ⏳ | ⏳ | En attente |

---

## 📝 RÈGLES D'EXÉCUTION

### Règles Absolues

```
┌─────────────────────────────────────────────────────────────────────────┐
│  ⚠️ RÈGLES NON-NÉGOCIABLES                                              │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  1. AUCUN PRIX visible sur le site — RÈGLE ABSOLUE                     │
│  2. CTA Secondaire = "Book a Call" — JAMAIS "Consultation"             │
│  3. Trust Line exacte sur toutes les pages                             │
│  4. Respecter l'intention de conversion B2B premium                    │
│  5. Ne pas altérer le contenu au-delà des corrections requises         │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

### Ordre d'Exécution Obligatoire

```
1. Phase 1 complète → Validation
2. Phase 2 → Validation  
3. Phase 3 (ce document) → Validation finale
```

---

**Document préparé pour exécution immédiate**  
**HILO® Website Optimization Project**
