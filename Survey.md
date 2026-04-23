# F — Survey

*Sondage complémentaire développé en parallèle de la Phase A terrain. Site déployé et accessible publiquement, résultats à la date du rendu insuffisants pour publication statistique. Méthodologie, architecture et accès documentés pour traçabilité et audit.*

---

## Accès direct

**URL publique du sondage** : [marketresearch.orangepeel.fr](https://marketresearch.orangepeel.fr/)

Durée d'un test : environ 3 minutes · Score personnalisé /10 affiché immédiatement · Résultats agrégés de l'étude envoyés par email à publication (si email renseigné).

![Page d'accueil du sondage](assets/survey_landing.png)

---

## Objectif

Triangulation **terrain × self-declaration** : mesurer le niveau de maturité Bitcoin auto-déclaré des professionnels financiers sur 5 segments cibles, en complément des 8 entretiens qualitatifs de la Phase A, pour :

- Valider ou nuancer les signaux qualitatifs terrain sur un volume plus large
- Capter des signaux d'urgence réglementaire auto-déclarés (MiCA · DAC8 · ANC 2026-01)
- Établir un baseline de maturité par segment exploitable en Phases B et C

---

## Structure

- Cinq segments couverts : **Notaire · CGP / CGPI · Expert-comptable · Banque / Établissement de crédit · PSAN / CASP**. Sélection en une étape avant démarrage automatique. 
- 8 à 10 questions spécifiques par segment + 2 questions communes

![Sélection du segment](assets/survey_segment_selection.png)

---

## Architecture technique

- **Frontend** : Next.js (App Router) · déploiement sous-domaine `marketresearch.orangepeel.fr`
- **Backend données** : Airtable (base `Survey-DB`, table `responses`)
- **Email** : Brevo (envoi conditionnel à publication du rapport)
- **Scoring** : logique `src/lib/scoring.ts` — fonction `calculateScore(answers, segment)` → score /10
- **Signaux kill criteria** : dérivés via `src/lib/airtable.ts::computeLofSignals()` (KC-1 · KC-2 · KC-5) — *nom historique de la fonction conservé dans le code ; le référentiel documentaire de l'étude = kill criteria*

Le code source (Next.js · logique de scoring · schéma Airtable · configuration Brevo) est **privé**, disponible en revue sur demande.

---

## Méthodologie

### Criterion types couverts (9 catégories)

`questions_recues` · `experience_crypto` · `a_laise` · `formation` · `mica_adapte` · `reaction_client` · `dossier_traite` · `pret_payer` · `lof_info`

### Règle de scoring

Le score mesure la **maturité du répondant** (0 à 10), pas un signal GTM direct. Deux axes coexistent et sont stockés séparément :

- **Score maturité** : somme des points attribués par question, normalisé sur 10 à l'affichage (`SCORE_MAX = 26`).
- **Signaux GTM** (KC-1 à KC-5) : chaque question est taggée avec un kill criterion. Les réponses sont post-traitées par `computeLofSignals()` pour produire un profil GTM du répondant (besoin formation · financement · urgence MiCA · Bitcoin-only · Qualiopi) indépendant du score maturité.

### Exemple concret — segment Notaire

Trois questions du questionnaire Notaire (8 au total), choisies pour illustrer les deux axes :

| ID | Question | Réponses possibles | Pts maturité | Kill criterion |
|:-:|---|---|:-:|:-:|
| `not_q1` | Combien de clients ont mentionné du Bitcoin dans un dossier cette année ? | Aucun · 1 à 5 · Plus de 5 | 0 · 1 · 3 | KC-1 |
| `not_q5` | Quand un client mentionne du Bitcoin dans un dossier, vous… | Gérez seul · Avec un confrère · Déclinez | 3 · 1,5 · 0 | KC-1 |
| `not_q6` | MiCA a-t-il changé votre façon d'aborder les actifs numériques ? | Oui · Non · Je ne connais pas MiCA | 5 · 0 · 0 | KC-3 |

**Ce que ces trois questions illustrent :**

- **`not_q1`** — scoring par paliers classique : l'exposition client mesure la maturité structurelle du répondant.
- **`not_q5`** — *« Déclinez »* rapporte 0 point de maturité mais déclenche un signal KC-1 fort (ce notaire a un besoin de formation explicite — prospect haute priorité pour Découvre Bitcoin). **Le 0 point ne neutralise pas le signal GTM.**
- **`not_q6`** — deux réponses à 0 point (*« Non »* et *« Je ne connais pas MiCA »*) ne disent pas la même chose côté GTM : l'une signale une non-adaptation volontaire, l'autre une ignorance réglementaire. Ces nuances sont exploitables en segmentation post-sondage.

Cette séparation maturité / signal GTM évite le biais d'un score agrégé unique qui écraserait les signaux d'opportunité commerciale.

### Contrôle qualité appliqué

- Question sur l'expérience crypto (achat · vente · transfert · théorique), et pas sur la pratique/possession personnelle ou professionnelle actuelles
- Réordonnancement des questions par segment pour éviter l'effet d'anchor (logique G5 dans `src/app/survey/page.tsx`)

---

## Résultats à la date du rendu

**Volume insuffisant pour publication statistique** au moment de la remise du rapport (avril 2026).

![Base Airtable — réponses collectées](assets/survey_airtable.png)

### État agrégé observé

- 25+ réponses collectées sur le segment CGP (majoritaire)
- Autres segments : volumes très faibles
- Distribution limitée au réseau personnel MP + cercle LinkedIn → biais d'échantillon fort
- Taux de complétion variable selon segment

### Pourquoi le rapport ne s'appuie pas dessus

Les conclusions du rapport reposent exclusivement sur :

- Les 8 entretiens qualitatifs Phase A (signaux convergents de praticiens identifiés)
- Le desk research sourcé (réglementation, statistiques officielles, cartographie concurrentielle)

Le sondage reste ouvert et actif post-remise. Une exploitation statistique pourra être envisagée une fois un volume suffisant atteint par segment.

---

## Accès lecteurs et auditeurs

| Accès | Lien |
|---|---|
| Tester le sondage (reproduction du parcours utilisateur) | [marketresearch.orangepeel.fr](https://marketresearch.orangepeel.fr/) |
| Revue du code source (privé — Next.js · scoring · schéma Airtable) | Sur demande [LinkedIn](https://www.linkedin.com/in/manuelproquin/) |
| Vue Airtable en lecture (réponses anonymisées) | Sur demande à [LinkedIn](https://www.linkedin.com/in/manuelproquin/) |

---

*Retour au [Rapport](./Report.md) · [Sources & Interview Index](./Appendix_2_Sources_Index.md)*
