---
name: analyse-critique-ecr
description: Réaliser une analyse critique complète d'un essai clinique randomisé (ECR) en français, orientée HTA et décision réglementaire. Utilise cette compétence quand l'utilisateur demande une "analyse critique", une "lecture critique d'article (LCA)", une "évaluation méthodologique", "analyser cet essai", "appréciation critique", "review d'un RCT", ou téléverse un PDF d'essai clinique randomisé. Produit un rapport markdown structuré avec classification des résultats, évaluation du risque de biais, pertinence clinique et conclusion orientée décision (inclure / ne pas inclure le traitement dans la stratégie thérapeutique).
---

# Analyse critique d'un essai clinique randomisé

## Objectif

Produire un rapport d'analyse critique d'un ECR destiné à un comité HTA
ou à un décideur réglementaire, qui répond à la question : **cet essai
apporte-t-il les preuves nécessaires pour intégrer le traitement dans la
stratégie thérapeutique ?**

## Principe axiomatique

Il faut des **preuves au-delà de tout doute raisonnable d'un bénéfice
clinique pertinent** pour intégrer un nouveau traitement dans la
stratégie thérapeutique. Le doute profite au statu quo, pas au
traitement évalué.

## Workflow

### Étape 1 — Lire intégralement l'article

Lire le PDF de l'essai (et le supplément si fourni). Si l'article n'est
pas téléversé, demander à l'utilisateur de le fournir avant de
continuer.

Identifier en passant : nom de l'essai, sponsor, registre (NCT…), revue,
année, phase.

### Étape 2 — Décrire l'étude (PICOT-S)

Extraire de manière concise : - **P** Population : critères d'inclusion
/ exclusion, n randomisés, caractéristiques de base - **I** Intervention
: molécule, dose, schéma, durée - **C** Comparateur : nature (placebo,
traitement actif, soins standards), pertinence - **O** Outcomes :
critère principal, critères secondaires avec controles de la
multiplicité, critères exploratoires, sécurité - **T** Timing : durée de
suivi, dates de l'essai - **S** Setting : pays, type de centres,
contexte de soin - **Méthodologie** : design (parallèle, cross-over,
factoriel, adaptatif), randomisation, aveugle, plan de contrôle du
risque alpha, analyses intermédiaires, population d'analyse principale
(ITT, mITT, per-protocole) ou méthode de gestion des événements
intercurrents, gestion des données manquantes

### Étape 3 — Classer chaque résultat

Pour chaque résultat de l'essai, appliquer la grille de classification
(voir `references/classification-resultats.md`). Les catégories sont :

1.  **Suffisamment probant** — démontré, pertinent, balance B/R
    favorable → peut justifier un changement de stratégie
2.  **Démontré mais balance B/R défavorable** — bénéfice statistiquement
    démontré mais contrebalancé par des effets indésirables
3.  **Insuffisamment probant** — suggéré mais non formellement démontré
4.  **Non concluant (NS)** — non statistiquement significatif
5.  **Effet délétère susceptible de contrebalancer le bénéfice** —
    invalide la possibilité d'introduction
6.  **Effet délétère certain mais ne contrebalançant par le bénéfice** —
    à signaler en sécurité

Pour chaque résultat, détailler : - **Critère de jugement** (et
population concernée si sous-groupe) - **Taille de l'effet** (effet
relatif + effet absolu + IC95 %) - **Contrôle du risque alpha global**
(signification statistique en terme de risque alpha global) - **Risque
de biais** (voir `references/risque-de-biais.md`) - **Pertinence
clinique** (cliniquement signifiant ? MCID franchi ? critère pertinent
pour patient/régulateur ?)

### Étape 4 — Conclusion orientée décision

Rédiger une conclusion synthétique qui répond explicitement : - Quels
résultats sont **suffisamment probants** pour garantir l'intéret du
traitement évalué ? - Quels effets indésirables menacent la balance B/R
? - Le traitement doit-il être **inclus** dans la stratégie
thérapeutique ? Pour quelle population, à quelle place (1ʳᵉ ligne, 2ᵈᵉ
ligne, recours), avec quelles précautions ? - Quelles **incertitudes
résiduelles** justifient de ne pas inclure le traitement évélué dans la
stratégie thérapeutique ?

### Étape 6 — Produire un rapport en markdown

Suivre la structure définie dans `references/structure-rapport.md`.

## Règles non négociables

- **ne pas tenir compte** de la discussion et de la conclusion des
  auteurs, ni de commentaires externes. N'utiliser que les informations
  disponibles dans les documents fournis.
- **Ne jamais surestimer un résultat** : un résultat post-hoc, sans
  controle de la multiplicité, ou de sous-groupe non pré-spécifié reste
  « insuffisamment probant », même si p \< 0,05.
- **Toujours quantifier** : taille d'effet absolue (différence de
  risque, NNT), pas seulement relative (RR, HR, OR).
- **Toujours examiner la sécurité** : un essai sans analyse approfondie
  des effets indésirables est incomplet. Une décision d'inclusion exige
  une balance B/R explicite.
- **Citer les sources** : pour chaque chiffre, indiquer la table ou
  figure de l'article.
- **Ne pas combler les manques** : si une donnée n'est pas dans
  l'article, l'écrire explicitement (« non rapporté ») plutôt que
  d'inventer ou d'extrapoler.

## Ressources de référence

- [Guide SFPT de lecture critique des essais
  thérapeutiques](https://sfpt-fr.org/livreblancmethodo/source/lecturecritique.pdf)
