# Structure du rapport MarkDown d'analyse critique

Format cible : `.md`. Style sobre, orienté décideur HTA.

## Page de garde

- Titre : « Analyse critique de l'essai [NOM_ESSAI] »
- Sous-titre : référence bibliographique complète (auteurs, journal, année, DOI)
- Date de l'analyse
- Mention : « Document généré par IA »

## 1. Synthèse exécutive (1 page max)

À mettre en premier après la page de garde — c'est ce que liront les décideurs pressés.

- **Question évaluée** : 1 phrase
- **Réponse synthétique** : le traitement doit-il être inclus dans la stratégie thérapeutique ? Pour qui, à quelle place ?
- **Principaux résultats démontrés**
- **Principales limites / incertitudes résiduelles**
- **Recommandation** (3-5 lignes)

## 2. Description de l'étude

### 2.1 Contexte et rationnel
- Pathologie, besoin médical non couvert, mécanisme d'action
- Place attendue du traitement dans la stratégie thérapeutique

### 2.2 Méthodologie (PICOT-S)
- Population (critères I/E, n randomisés, n analysés)
- Intervention (molécule, dose, schéma, durée)
- Comparateur (nature, justification, dose, durée)
- Critères de jugement (principal, secondaires hiérarchisés, exploratoires, sécurité)
- Timing (suivi, dates)
- Setting (pays, centres, contexte)

### 2.3 Analyse statistique
- Hypothèses (taille d'effet attendue, puissance, alpha)
- Gestion de la multiplicité, liste des critères avec gestion de la multiplicité (mention que les autres critères ne permettant pas d'inférer l'effet du traitement)
- Population d'analyse principale (ITT, mITT), gestion des événéments intercurrents
- Gestion des données manquantes

### 2.4 Caractéristiques de base
- Tableau comparatif des deux groupes
- Signaler tout déséquilibre sur variable pronostique majeure

## 3. Évaluation du risque de biais 

- Justification 1-2 phrases par domaine
- Jugement global

## 4. Résultats par catégorie

Présenter les résultats par catégorie selon `classification-resultats.md`.

Pour chaque catégorie, tableau standardisé :

|  Critère de jugement | Résultat | Signification statistique | Risque de biais | Pertinence clinique |
|---|---|---|---|---|
| … | … | … | … | … |


## 5. Sécurité et balance bénéfice/risque

- Effets indésirables suceotible de contrebalancer le bénéfice quantitativement ou qualitativement
- Effets indésirables d'intérêt particulier
- Décès liés au traitement
- Calcul explicite de la balance B/R sur les principaux critères

## 6. Limites et points de vigilance

- Validité externe (généralisation à la population française)
- Comparateur (loyal vs dépassé)
- Conflits d'intérêt et rôle du sponsor
- Cohérence protocole / SAP / publication
- Données manquantes
- Suivi insuffisant pour des outcomes à long terme

## 8. Conclusion orientée décision

Réponse explicite à :
1. Quels résultats sont **suffisamment probants** pour démontrer l'interet clinique du traitement étudié ?
2. Le traitement doit-il être **inclus** dans la stratégie thérapeutique ? Pour quelle population ? À quelle place (1ʳᵉ ligne, 2ᵈᵉ ligne, recours) ?
3. Quelles **incertitudes résiduelles** justifient des données complémentaires (étude post-AMM, registre, vie réelle, étude tête-à-tête vs comparateur actuel) ?


---

## Style éditorial

- Phrases courtes, vocabulaire précis
- Pas de marketing, pas d'emphase superflue
- Chaque chiffre cité doit pointer vers une table/figure de l'article
- Les résultats NS sont présentés comme « non démontrés », **pas** comme « équivalents »
- Quand une donnée manque, l'écrire : « Non rapporté dans l'article »
