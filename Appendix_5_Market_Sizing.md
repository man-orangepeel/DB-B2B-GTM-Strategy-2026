# Appendix 5 — Market Sizing & Segment Scoring

*Ce fichier présente la taille du marché adressable (TAM/SAM/SOM) par segment professionnel. Méthodologie complète : [Appendix_1_Methodology.md](Appendix_1_Methodology.md).*

---

## 0. Cadrage méthodologique

### 0.1 Objet A4

Quantifier en € HT la valeur économique de trois niveaux de marché pour Découvre Bitcoin :

- **TAM** — marché total théorique (toute la population pro payant au pricing marché de référence)
- **SAM** — marché adressable par DB (après filtres d'accessibilité segment × zone × maturité)
- **SOM 12M / 24M** — marché effectivement capté par DB sur 12 et 24 mois (plan C3 nominal)

### 0.2 Scope

Périmètre restreint aux **2 segments prioritaires post-révision terrain** :

| Segment | Population | Source |
|---|:---:|:---:|
| **Notaires en exercice** | 17 000 | CSN 2024 |
| **Experts-comptables libéraux inscrits** | 22 685 | CSOEC 2024 |
| **Salariés cabinets EC branche IDCC 787** | 138 400 | campusAtlas (OPCO ATLAS) |

*Segments desk sortis post-révision terrain (Banques · PSAN · Family Offices · CGP · Avocats) : hors scope A4 — mentionnés pour rappel en §7 limites.*

### 0.3 Définitions TAM / SAM / SOM

| Niveau | Définition retenue | Unité | Formule |
|---|---|---|---|
| **TAM** | Marché total théorique si 100 % des pros suivaient ~1-2 j formation crypto/an au pricing moyen marché de référence | € HT / an | Population × pricing moyen marché |
| **SAM** | Marché réellement adressable par DB après filtres (adressabilité 24 mois × zones non saturées × maturité client) | € HT / an | TAM × coefficient filtres SAM |
| **SOM 12M** | Marché effectivement capté par DB à T+12 — scénario nominal C3 (proba 40-50 %) | € HT cumul T+12 | Volume cible B4 × CA net DB moyen participant |
| **SOM 24M** | Extrapolation Year 2 scénario nominal (scale chambres + CROEC + campusAtlas si accepté) | € HT cumul Y2 | SOM 12M × facteur scale 2,5-3 |

### 0.4 Hypothèses structurantes (8)

Hypothèses explicites et contestables (principe : défendable > optimiste sans source). Ajustables si données terrain contradictoires.

| # | Hypothèse | Valeur retenue | Source / Justification |
|:---:|---|---|---|
| **H1** | Pricing marché référence TAM Notaires | **1 000 €/pro/an** (bas) · **1 500 €/pro/an** (haut) | INAFON 2 000 €/j · AUREP 1 075 €/j · 1-1,5 j formation crypto / pro / an moyenne |
| **H2** | Pricing marché référence TAM EC libéraux | **500 €/pro/an** (bas) · **1 500 €/pro/an** (haut) | FP × Expert Crypto 1 475 € HT/3j distance · demande variable selon cabinet |
| **H3** | Pricing marché référence TAM EC salariés | **200 €/pro/an** (bas) · **500 €/pro/an** (haut) | Tarification branche plus compressée · OPCO ATLAS finance employeur (prix négocié collectivement) |
| **H4** | Filtre SAM Notaires | **15 % TAM** | Adressabilité 24 mois ~20 % (curieux + touchés client Bitcoin + bull cycle) × hors zones E&C saturées ~75 % ≈ 15 %. Aligné flow E&C observé (~12 % TAM/an S1 2026) |
| **H5** | Filtre SAM EC libéraux | **7 % TAM** | Adressabilité 24 mois ~10 % (anticipateurs ANC 2026-01 + cabinets clients crypto + JO-type curieux) × hors zones FP × Expert Crypto ~70 % ≈ 7 %. Double de la prévalence JO "~2 % entreprises avec crypto" |
| **H6** | Filtre SAM EC salariés | **5 % TAM** | Cabinets engagés DPC crypto volontaire 24 mois ~7 % × branche IDCC 787 (100 %) × ajustement -2 pts pour filtre géographique/organisation ≈ 5 %. Cohérent taux pénétration modules "exotiques" catalogues OPCO |
| **H7** | Pricing DB net moyen participant (pour SOM) | **200-400 €/pro net DB** (milieu 250-300 €) | C2 §9.3 pricing mix : session chambre (200-400 €/pers) · pack 2 modules (150-200 €/pers) · cabinet one-shot (200-500 €/pers selon taille). Net après rétrocession 70-85 % via 4NK (pour sessions OF hôte) ou 100 % marge (pour session chambre ou cabinet direct) |
| **H8** | Facteur scale Year 2 (SOM 24M) | **× 2,5 à × 3** | Scénario nominal C3 : +2-3 chambres N actives (×2 N) · +2 CROEC actifs (×2 EC) · campusAtlas catalogue 2027 mis en ligne si accepté (×2-3 EC salariés) · consolidation modules N#2 et EC#2 · publications déjà publiées (crédibilité) |

### 0.5 Principes de lecture

- **Unité** : € HT · "professionnel-année" pour TAM/SAM (flow annualisé) · **cumul T+12 ou T+24** pour SOM
- **Fourchettes** : pas de précision fausse. Préférer "2,5-3,8 M€" à "3,14 M€"
- **DB revenue = net** : SOM chiffré après rétrocession OF hôte (benchmark 70-85 % DB via 4NK) — pas revenu brut session
- **Pricing cible DB ≠ pricing marché** : DB se positionne 50-100 €/j/pers (grille b C1 §6.4) = 30-50 % en dessous FP · SAM et TAM utilisent pricing marché, SOM utilise pricing DB réel

---

## 1. Données de base consolidées

### 1.1 Populations

| Segment | Population | Commentaire |
|---|:---:|---|
| Notaires en exercice | **17 000** | CSN 2024 (valeur stricte 17 527) |
| Collaborateurs offices notariaux | ~55 000 | Hors scope A4 (cible DB = notaires décideurs uniquement) |
| EC libéraux inscrits | **22 685** | CSOEC 2024 |
| Cabinets EC | ~21 000 | Référence structure (pas directement A4) |
| Collaborateurs cabinets EC | ~190 000 | Dont 138 400 branche IDCC 787 adressables via campusAtlas |
| **Salariés branche IDCC 787** | **138 400** | campusAtlas — bassin OPCO ATLAS |

### 1.2 Pricing marché référence (benchmarks consolidés)

| Acteur / pricing | Valeur | Équivalent normalisé | Usage A4 |
|---|---|:---:|:---:|
| INFN (intervenant N) | 1 000 €/j intervenant | N/A (facturation OF, pas participant) | Référence bas N |
| INAFON (intervenant N) | 2 000 €/j intervenant | N/A | Référence haut N |
| **AUREP CCP Notaires RS6827** | 6 450 € / 6 j | **1 075 €/j/pers** | Référence N |
| Parcours Office EDHEC-INAFON | 4 200 € HT / 8 j | 525 €/j/pers | Référence N basse |
| **FP × Expert Crypto certificat EC** | 1 475 € HT / 3 j distance | **~490 €/j/pers** | Référence EC |
| Pricing cible DB grille (b) | 50-100 €/j/pers (session 20) | Positionnement | Usage SOM (net rétrocession) |
| Pricing session chambre N | 5 000-10 000 €/session (15-25 N) | 200-400 €/pers | Référence session chambre |
| Pricing cabinet one-shot EC | 3 000-10 000 €/cabinet | 200-500 €/pers selon taille | Référence one-shot |

---

## 2. TAM — marché total théorique

### 2.1 TAM par segment (flow annualisé)

| Segment | Population | Pricing bas €/pro/an | Pricing haut €/pro/an | **TAM bas (M€/an)** | **TAM haut (M€/an)** |
|---|:---:|:---:|:---:|:---:|:---:|
| **Notaires** | 17 000 | 1 000 | 1 500 | **17,0 M€** | **25,5 M€** |
| **EC libéraux** | 22 685 | 500 | 1 500 | **11,3 M€** | **34,0 M€** |
| **EC salariés** (IDCC 787) | 138 400 | 200 | 500 | **27,7 M€** | **69,2 M€** |
| **Total cross** | 178 085 | — | — | **~56 M€/an** | **~128 M€/an** |

### 2.2 Lecture TAM

**TAM total cross-segment Notaires + EC = 56-128 M€/an** en pricing marché de référence.

Lecture : si 100 % des notaires + EC libéraux + EC salariés branche IDCC 787 suivaient 1-2 j formation crypto/an au pricing moyen marché (INFN/INAFON/AUREP/FP), le marché formation crypto B2B pour ces 2 segments représenterait ~56 à 128 M€ annuels. Aucun acteur ne capture cette totalité — la concurrence (E&C · FP × Expert Crypto · LD · RF · AUREP · 4NK) fragmente ce TAM.

---

## 3. SAM — marché adressable par DB

### 3.1 Filtres SAM détaillés

| Segment | Filtre 1 : adressabilité 24 mois | Filtre 2 : zones non saturées | **SAM en % TAM** | Justification terrain |
|---|:---:|:---:|:---:|---|
| **Notaires** | ~20 % (curieux + touchés client Bitcoin + bull cycle 2026-2027) | × ~75 % (hors zones E&C Toulouse/Lyon + 2-3 chambres absorbées d'ici 24 mois) | **~15 %** | Flow réel E&C ~12 % TAM/an observé S1 2026 (700 N formés 4 mois) · SAM 15 % cohérent (+ marge hors zones) |
| **EC libéraux** | ~10 % (anticipateurs ANC 2026-01 + cabinets clients crypto + JO-type curieux) | × ~70 % (hors zones saturées FP × Expert Crypto) | **~7 %** | JO "~2 % entreprises avec crypto" · SAM 7 % prudent-optimiste (demande latente + ANC 2026-01 pousse adoption) |
| **EC salariés** (IDCC 787) | ~7 % (cabinets engagés DPC crypto volontaire 24 mois) | × filtre organisation cabinet | **~5 %** | Cohérent taux pénétration modules "exotiques" catalogues OPCO · campusAtlas blockchain transversal existe mais volume faible |

### 3.2 SAM par segment

| Segment | TAM annualisé | Coefficient SAM | **SAM bas (M€/an)** | **SAM haut (M€/an)** |
|---|:---:|:---:|:---:|:---:|
| **Notaires** | 17,0-25,5 M€ | 15 % | **2,5 M€** | **3,8 M€** |
| **EC libéraux** | 11,3-34,0 M€ | 7 % | **0,8 M€** | **2,4 M€** |
| **EC salariés** (IDCC 787) | 27,7-69,2 M€ | 5 % | **1,4 M€** | **3,5 M€** |
| **Total cross** | 56-128 M€ | 8,5 % pondéré | **~4,7 M€/an** | **~9,7 M€/an** |

### 3.3 Lecture SAM

**SAM total cross-segment = 4,7-9,7 M€/an**.

Lecture : le marché **réellement adressable par un acteur Bitcoin-only bien positionné** (stack partenariats + Qualiopi partenaire + publications signature) s'élève à 4,7-9,7 M€ annuels. E&C seul capture déjà ~2 M€/an en zones Toulouse/Lyon (extrapolation 2 000 N formés × 1 000 €/pro). DB peut viser une part de ce SAM à horizon 12-24 mois, pas l'intégralité (fragmentation + maturité segment).

---

## 4. SOM — marché effectivement capté par DB

### 4.1 Hypothèses SOM

- Volumes cibles **scénario nominal C3** (probabilité 40-50 %)
- Pricing DB **net rétrocession 70-85 % via 4NK** (pour sessions OF hôte) ou **100 % marge** (pour sessions chambre N directes ou cabinet one-shot EC direct) · **moyenne pondérée ~250 €/pro net DB** (pack 2 modules)
- T+12 = Avril 2027 · T+24 = Avril 2028

### 4.2 SOM 12M (scénario nominal)

| Segment | Volume cible T+12 | CA net DB moyen/pro | **SOM 12M bas (k€)** | **SOM 12M haut (k€)** |
|---|:---:|:---:|:---:|:---:|
| **Notaires** | 100-200 N | 200-400 €/pro | **20 k€** | **80 k€** |
| **EC libéraux** | 30-90 EC (hypothèse split 60 % des 50-150 EC cible T+12 sont libéraux) | 200-400 €/pro | **6 k€** | **36 k€** |
| **EC salariés** (IDCC 787) | 0-60 EC (0 si campusAtlas non accepté · max 60 si pilote cabinet EC salariés T+9-T+12) | 100-200 €/pro (pricing branche compressé) | **0 k€** | **12 k€** |
| **Total cross** | 130-350 pros | ~200-350 € moyen | **~26 k€** | **~128 k€** |

### 4.3 SOM 24M (extrapolation Year 2 scénario nominal · facteur × 2,5-3)

| Segment | Scale drivers Y2 | SOM 12M base | Facteur scale | **SOM 24M bas (k€)** | **SOM 24M haut (k€)** |
|---|---|:---:|:---:|:---:|:---:|
| **Notaires** | +2-3 chambres actives · scale INFN/INAFON via GT+Pezzetti | 20-80 k€ | × 2,5 | **50 k€** | **200 k€** |
| **EC libéraux** | +2-3 CROEC actifs · cabinets EC crypto one-shot réguliers | 6-36 k€ | × 3 | **18 k€** | **108 k€** |
| **EC salariés** (IDCC 787) | campusAtlas catalogue 2027 mis en ligne si G6 accepté · scale massif possible | 0-12 k€ | × 5-10 (effet catalogue institutionnel) | **0 k€** | **120 k€** |
| **Total cross** | — | 26-128 k€ | × 2,5-3,4 | **~70 k€** | **~430 k€** |

### 4.4 Lecture SOM

**SOM cumul T+12 = 26-128 k€** (scénario nominal · pricing DB net moyen)
**SOM cumul T+24 (Year 2 scénario nominal) = 70-430 k€**

Lecture : le chiffre d'affaires net DB cumulé est **modeste année 1** (26-128 k€), conforme à la stratégie de pilote T+3 + scale T+6 à T+12 (scellage P0 partenariats avant volume). **Year 2** permet une montée en puissance significative (×2,5 à ×10 selon acceptation campusAtlas · +2-3 chambres + CROEC).

---

## 5. Synthèse récapitulative

### 5.1 Tableau cross-segment

| Indicateur | Notaires | EC libéraux | EC salariés IDCC 787 | **Total cross** |
|---|:---:|:---:|:---:|:---:|
| **Population** | 17 000 | 22 685 | 138 400 | 178 085 |
| **TAM (€/an)** | 17-25 M€ | 11-34 M€ | 28-69 M€ | **56-128 M€** |
| **SAM (€/an)** | 2,5-3,8 M€ | 0,8-2,4 M€ | 1,4-3,5 M€ | **4,7-9,7 M€** |
| **SOM 12M (€ cumul)** | 20-80 k€ | 6-36 k€ | 0-12 k€ | **26-128 k€** |
| **SOM 24M (€ cumul)** | 50-200 k€ | 18-108 k€ | 0-120 k€ | **70-430 k€** |
| **Part SOM 12M / SAM** | ~1-2 % | ~1-2 % | 0-0,3 % | **~1 %** |
| **Part SOM 24M / SAM** | ~2-5 % | ~2-5 % | 0-3 % | **~2-4 %** |

### 5.2 Verdict market sizing

**TAM cross = 56-128 M€/an** · **SAM cross = 4,7-9,7 M€/an** · **SOM cumul T+12 = 26-128 k€** · **SOM cumul T+24 = 70-430 k€**.

DB capture **1-2 % du SAM Year 1** et monte à **2-5 % du SAM Year 2** en scénario nominal. L'opportunité existe en absolu (SAM adressable 4,7-9,7 M€/an) mais nécessite une exécution rigoureuse du plan C3 : scellage P0 T+3 · pilote N T+3 · chambre N#1 T+5 · module EC T+6 · candidature campusAtlas T+3 (G6) · scale Year 2.

---

## 6. Share of wallet — part de DB dans budget formation annuel moyen du pro cible

### 6.1 Budget formation annuel moyen par segment

| Segment | Budget formation crypto moyen / pro / an | Source |
|---|:---:|:---:|
| **Notaires en exercice** | 200-600 €/an (1 j crypto dans 20 h formation continue obligatoire) | Décret 2011-1230 (20 h/an) · A3 §4.3 · pricing INAFON/INFN |
| **EC libéraux** | 100-400 €/an (DPC obligatoire · 1 j crypto optionnelle dans formation technique) | DPC OEC · JO §6 "500-700 €/j seuil sensibilité OPCO" · A3 §7.3 |
| **EC salariés** (IDCC 787) | 50-200 €/an (branche · actions collectives OPCO ATLAS) | Branche IDCC 787 · campusAtlas tarifs généraux |

### 6.2 Part DB dans budget formation crypto

| Segment | Pricing DB pack 2 modules | Budget formation crypto annuel pro | **Share of wallet DB** |
|---|:---:|:---:|:---:|
| **Notaires** | 300-400 €/pro (pack complet) | 200-600 €/an | **50-100 %** (pack DB ≈ budget annuel crypto complet — positionnement "formation unique crypto de l'année") |
| **EC libéraux** | 300-400 €/pro | 100-400 €/an | **75-100 %+** (pack DB ≈ ou > budget annuel crypto — justifie positionnement "formation essentielle ANC 2026-01 + DAC8") |
| **EC salariés** (IDCC 787) | 150-300 €/pro (via OPCO ATLAS) | 50-200 €/an | **75-100 %** (DB = la formation crypto de l'année pour salarié cabinet · financée OPCO ATLAS) |

### 6.3 Lecture share of wallet

DB capte **50-100 % du budget formation crypto annuel** du pro cible — positionnement cohérent avec stratégie "formation crypto essentielle de l'année" (pas formation récurrente multi-sessions).

Implication GTM : DB doit **justifier sa valeur sur 1 an de budget formation crypto** du pro cible — d'où l'importance du packaging 2 modules (fondamentaux + DAC8/ANC 2026-01) + couplage Le Coffre (valeur additionnelle post-formation).

---

## 7. Limites & contestabilité

### 7.1 Limites structurelles de la modélisation A4

| Limite | Impact sur TAM/SAM/SOM | Mitigation |
|---|---|---|
| **Pricing marché référence composite** | TAM varie ±30 % selon pricing moyen retenu | Fourchette bas/haut explicite (H1/H2/H3) |
| **Adressabilité 24 mois estimée** | SAM varie ±50 % selon filtres | Justifications terrain explicites (H4/H5/H6) contestables |
| **Scénario SOM = nominal C3** (40-50 % proba) | Scénarios dégradés (20-25 % proba) divisent volume par 1,3-2 | Cf C3 §14.7 matrice scénarios pour SOM dégradé |
| **EC salariés campusAtlas conditionnel** | Si G6 KO, SOM 24M EC salariés = 0 | Plan B FIFPL + direct cabinets limite la perte mais ne compense pas volume campusAtlas |
| **Facteur scale Year 2 ×2,5-3** | Contestable — dépend réussite G1-G8 Year 1 | Fourchette ×2,5-×3 avec justification C3 §4-§6 |

### 7.2 Segments hors scope A4 (justification de l'exclusion)

| Segment exclu | Raison exclusion | Order de grandeur TAM potentiel |
|---|---|---|
| Banques (salariés) | Score terrain 23/40 (dégradé 28→23 post-révision AS+MD) · cycle DRH très long · hors Top 5 | TAM > 100 M€/an mais SAM quasi-nul court terme |
| PSAN / CASP | Score terrain 17/40 (dégradé 29→17 post-révision AG+AS) · segment en contraction | TAM ~5 M€/an · SAM < 200 k€/an (10 PSAN actifs × pricing Art.81) |
| Family Offices | Score 25/40 · desk research seul · 300-500 structures FR | TAM ~2 M€/an · SAM niche |
| CGP / CGPI | Score 25/40 · LAF "cible la plus dure qui existe" · frein structurel commission | TAM ~15 M€/an · SAM < 1 M€/an |
| Avocats | Score 26/40 · desk research seul · 0 interview | Hors A4 (pas données qualifiées) |

---

## 8. Sources & cohérence cross-fichiers

### Sources primaires

| Source | Section utilisée | Usage A4 |
|---|---|---|
| `A_Market_Mapping/A3_Paysage_Financier.md` | §4.1 + §7.1 | Populations N + EC |
| `C_GTM_Strategy/C1_Positionnement_Messaging.md` §6.4 | Pricing dual | H7 pricing DB · SOM calcul |
| `C_GTM_Strategy/C2_Stack_Partenariats.md` §9 | Pricing + packaging | H7 pricing · rétrocession OF hôte |
| `B_Benchmark/B4_Synthese_Cross_Segment.md` §8.1 | Volumes cibles 12 mois | SOM 12M volumes |
| `C_GTM_Strategy/C3_Sequencement_Operationnel_12mois.md` §14.7 | Scénarios 12 mois | SOM nominal · H8 scale Y2 |

### Sources externes

- [CSN — Chiffres clés 2024](https://www.notaires.fr) — 17 000 notaires
- [CSOEC — Chiffres clés 2024](https://www.experts-comptables.fr) — 22 685 EC
- campusAtlas (OPCO ATLAS) — 138 400 salariés branche IDCC 787
- [AUREP CCP Notaires RS6827 tarifs 2025-2026](https://www.aurep.com/)
- FP × Expert Crypto site MAJ 23/03/2026 — 1 475 € HT / 3 j
- ADAN/KPMG 2024 — 12 % Français détiennent crypto

### Cohérence vérifiée

- ✅ TAM populations alignées A3 + CLAUDE.md (écart négligeable 17 000 vs 17 527 notaires)
- ✅ SAM filtres **défendables terrain** post-challenge MP (recalibrage H4/H5/H6 à 15%/7%/5% pour aligner avec flow E&C observé + prévalence JO)
- ✅ SOM volumes alignés B4 §8.1 + C3 §14.7 scénario nominal
- ✅ Pricing DB net aligné C1 §6.4 grille + C2 §9 rétrocession OF hôte
- ✅ Facteur scale Year 2 aligné C3 §5-§6 scale chambres + CROEC + campusAtlas

---

## Historique & MAJ

Version finalisée au 22/04/2026. Le fichier intègre les filtres SAM recalibrés post-challenge terrain (15%/7%/5% vs initial 40%/35%/25%), confirmés cohérents avec flow E&C observé (700 notaires formés en 4 mois = ~12 % TAM/an S1 2026). Méthodologie détaillée : [METHODOLOGY.md](Appendix_1_Methodology.md).

---

*Retour au [glossaire](./Appendix_3_Glossary.md) · [méthodologie](./Appendix_1_Methodology.md) · [index rapport](./README.md)*
