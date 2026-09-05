---
name: audit-rapport-vs-avis-ct
description: "Évaluer l'exactitude et la qualité d'un rapport d'analyse critique et d'interprétation d'un essai clinique destiné à la pratique médicale, en le comparant à l'avis de la Commission de Transparence (HAS) portant sur le même essai, pris comme référence. Utiliser cette compétence quand l'utilisateur demande d'« auditer / évaluer / vérifier / noter la qualité d'un rapport d'analyse critique », de « comparer un rapport à l'avis de la CT/HAS », de vérifier que « toutes les réserves méthodologiques de l'avis ont bien été identifiées », ou la « cohérence de la conclusion pour la pratique médicale » avec celle de la Commission de transparence, et téléverse à la fois un rapport d'analyse critique et le PDF d'un avis de la Commission de Transparence portant sur le même essai."
---

# Audit d'un rapport d'analyse critique par rapport à l'avis de la Commission de Transparence

## Objectif

Deux documents en entrée :
1. le **rapport à évaluer** — une analyse critique et interprétation d'un essai clinique, destinée à orienter la pratique médicale ;
2. l'**avis de la Commission de Transparence (CT)** de la HAS portant sur le même essai (PDF), pris comme **référence externe (benchmark)**.

Produire un audit qui répond à deux questions, et seulement ces deux questions :

- **Q1 — Exhaustivité** : le rapport a-t-il identifié toutes les réserves méthodologiques que la Commission de Transparence a relevées sur cet essai ?
- **Q2 — Cohérence** : la conclusion du rapport pour la pratique médicale est-elle cohérente avec celle de la Commission de Transparence ?

## Principes

- L'avis CT sert de **référentiel**, pas d'arbitre absolu de la vérité méthodologique : il matérialise le niveau minimal de vigilance qu'un rapport de qualité doit couvrir. Un rapport ne peut pas ignorer une réserve que la CT a jugée assez importante pour la mentionner.
- **La substance prime sur la formulation.** Peu importe que le rapport utilise d'autres mots : ce qui compte est que le fond de chaque réserve CT soit retrouvé et exploité (c'est-à-dire qu'une conséquence en soit tirée sur le niveau de preuve ou la conclusion), pas seulement évoqué en passant.
- **Cohérence ≠ identité mot pour mot.** Il s'agit d'une convergence sur : le niveau de preuve retenu, la population/place dans la stratégie thérapeutique concernée, et le degré de prudence exprimé. Un rapport peut légitimement être plus sévère que la CT s'il le justifie. En revanche, **un rapport plus optimiste que l'avis CT sans justification explicite des réserves non levées est le cas le plus problématique** pour la sécurité de la pratique médicale, et doit être signalé sans ambiguïté.
- Cet audit **ne refait pas** une analyse critique indépendante de l'essai : il compare exclusivement le rapport au contenu de l'avis CT.

## Prérequis

- Vérifier en premier lieu que les deux documents portent bien sur **le même essai clinique** (même nom d'essai / même NCT / même publication pivot). Si ce n'est pas le cas, avertir l'utilisateur et ne pas poursuivre l'audit sans confirmation.
- Si l'avis CT couvre un programme d'études (essai pivot + essais de support), circonscrire l'extraction à ce qui concerne l'essai objet du rapport, en signalant à part les réserves qui portent sur le programme dans son ensemble.
- Si l'un des deux documents manque ou n'est pas exploitable (PDF scanné non océrisé, etc.), le signaler et le demander avant de poursuivre.

## Workflow

### Étape 1 — Lire intégralement les deux documents

Lire le rapport à évaluer et le PDF de l'avis CT (s'appuyer sur la compétence `pdf` pour l'extraction si nécessaire, y compris OCR si le PDF est scanné). Identifier au passage : traitement évalué, indication, essai(s) concerné(s) (nom, NCT), date et référence de l'avis CT, SMR et ASMR attribués.

### Étape 2 — Construire le référentiel des réserves méthodologiques à partir de l'avis CT

Repérer dans l'avis CT — typiquement les sections « Données/résultats disponibles », « Analyse des données disponibles » (efficacité, tolérance, discussion), « Programme d'études », et les paragraphes qui précèdent la conclusion SMR/ASMR — toute réserve, limite, incertitude ou critique méthodologique formulée par la Commission à propos de l'essai concerné.

Découper chaque réserve en un **item atomique et distinct** (une réserve = un item), reformulé de façon neutre, avec la citation ou la référence de page/section permettant de la retrouver. Catégoriser chaque item, par exemple selon :

- Population / critères d'inclusion-exclusion / transposabilité
- Comparateur (pertinence, dose, conformité au standard de soins)
- Critère de jugement principal ou secondaire (pertinence clinique, hiérarchisation, contrôle de la multiplicité)
- Randomisation / aveugle / risque de biais de suivi ou de mesure
- Durée de suivi / maturité des données
- Analyse statistique (méthode, données manquantes, analyses de sensibilité, sous-groupes non pré-spécifiés)
- Ampleur et pertinence clinique de l'effet (différence absolue, IC95 %, seuil cliniquement pertinent)
- Sécurité / tolérance
- Qualité de vie / critères rapportés par les patients
- Autre (préciser)

Construire un **tableau numéroté « Référentiel des réserves CT »** (R1, R2, …) qui sert de base à toute la comparaison.

Extraire séparément la **conclusion de la CT pour la pratique** : SMR, ASMR, population retenue, place dans la stratégie thérapeutique, et toute restriction ou nuance formulée (ex. « chez les patients en échec de… », « l'apport thérapeutique ne peut être établi que… »).

### Étape 3 — Relever ce que couvre le rapport à évaluer

Parcourir le rapport (sections risque de biais, limites, discussion, conclusion) et relever, pour **chaque réserve du référentiel CT**, si et où elle est traitée, en notant si le rapport en tire réellement une conséquence sur le niveau de preuve ou la conclusion.

Relever aussi les éventuelles réserves supplémentaires soulevées par le rapport et absentes de l'avis CT — à noter comme valeur ajoutée, jamais comme défaut.

Extraire la **conclusion du rapport pour la pratique médicale** : le traitement doit-il être intégré ou non dans la stratégie thérapeutique, pour quelle population, à quelle place, avec quelles précautions.

### Étape 4 — Apparier réserve par réserve

Pour chaque item du référentiel CT, statuer :

| Statut | Signification |
|---|---|
| ✅ Identifiée | La substance de la réserve est retrouvée dans le rapport, même reformulée, et une conséquence en est tirée |
| ⚠️ Partiellement identifiée | La réserve est évoquée mais affaiblie, incomplète, noyée, ou mentionnée sans que sa portée sur le niveau de preuve soit exploitée |
| ❌ Non identifiée | Absente du rapport |

Justifier chaque statut par une citation ou un renvoi précis au passage du rapport (ou constater explicitement l'absence). Ne jamais combler par une supposition : si le rapport n'aborde pas un point, l'écrire tel quel.

### Étape 5 — Évaluer la cohérence de la conclusion pour la pratique

Comparer explicitement, côte à côte, la conclusion de la CT et celle du rapport selon : niveau de preuve retenu, population concernée, place dans la stratégie thérapeutique, degré de prudence exprimé. Classer :

- **Cohérente** — même sens, même degré de prudence (formulation différente admise)
- **Partiellement cohérente** — sens globalement compatible mais nuances importantes non reprises (population plus large, précaution non mentionnée…)
- **Discordante** — conclusions contradictoires, ou rapport significativement plus optimiste/pessimiste sans justification

Signaler explicitement et en priorité tout cas où **le rapport est plus optimiste que l'avis CT sans justifier les réserves non levées**.

### Étape 6 — Synthèse et verdict global

Calculer un taux de couverture (✅ = 1, ⚠️ = 0,5, ❌ = 0, rapporté au nombre total d'items du référentiel). Identifier les **réserves critiques manquées** : celles qui, si elles avaient été prises en compte, auraient pu changer le niveau de preuve retenu ou la conclusion pour la pratique.

Attribuer un verdict global :

- **Rapport fidèle et cohérent** — couverture élevée, aucune réserve critique manquée, conclusion cohérente
- **Rapport globalement satisfaisant mais incomplet** — omissions non critiques et/ou partielles, conclusion néanmoins cohérente
- **Rapport insuffisant** — réserve(s) critique(s) manquée(s) et/ou conclusion discordante de celle de la CT

Formuler des recommandations concrètes pour améliorer le rapport (réserves à ajouter, nuances à apporter à la conclusion).

### Étape 7 — Produire le rapport d'audit en markdown

Structure cible :

1. **En-tête** — traitement, indication, essai concerné, référence du rapport évalué, référence et date de l'avis CT.
2. **Référentiel des réserves CT et appariement** — tableau : n°, catégorie, réserve CT (résumé + citation/page), statut (✅/⚠️/❌), justification (citation ou constat d'absence dans le rapport).
3. **Taux de couverture** — chiffre global + détail par catégorie, réserves critiques manquées mises en évidence.
4. **Analyse de cohérence de la conclusion** — citation de la conclusion CT, citation de la conclusion du rapport, verdict (Cohérente / Partiellement cohérente / Discordante) et justification.
5. **Réserves additionnelles du rapport** (le cas échéant) — valeur ajoutée par rapport à l'avis CT.
6. **Verdict global.**
7. **Recommandations d'amélioration du rapport.**

## Règles non négociables

- Ne juger le rapport que sur ce que dit effectivement l'avis CT : ne pas ajouter de réserves méthodologiques personnelles au référentiel (ce n'est pas l'objet de cet audit).
- Une réserve n'est « ✅ Identifiée » que si le rapport en tire une conséquence sur le niveau de preuve ou la conclusion — une simple mention sans exploitation reste « ⚠️ Partiellement identifiée ».
- Toujours citer précisément (page, section, phrase) chaque réserve CT extraite et chaque correspondance ou absence relevée dans le rapport.
- Toujours vérifier en premier lieu que les deux documents portent sur le même essai ; sinon avertir et ne pas poursuivre sans confirmation de l'utilisateur.
- Ne jamais combler un manque par une supposition ; écrire « non traité dans le rapport » plutôt que d'inventer un contenu.
- Signaler en priorité toute divergence où le rapport est plus optimiste que l'avis CT sans justification — cas le plus critique pour la sécurité de la pratique médicale.

## Ressources de référence

- Pour la grille de catégorisation des domaines méthodologiques d'un ECR, s'appuyer si besoin sur la même terminologie que la compétence `analyse-critique-ecr`.
- Pour l'extraction de texte depuis le PDF de l'avis CT, s'appuyer sur la compétence `pdf`.