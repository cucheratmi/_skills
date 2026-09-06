---
name: analyse-critique-maic
description: "Réaliser une analyse critique méthodologique d'une comparaison indirecte ajustée sur les caractéristiques individuelles des patients de type MAIC (Matching-Adjusted Indirect Comparison), ancrée ou non ancrée. Utiliser cette compétence quand l'utilisateur demande d'« analyser / évaluer / critiquer une MAIC », une « comparaison ajustée par appariement », un « matching-adjusted indirect comparison », de juger le « niveau de preuve » ou l'« acceptabilité » d'une MAIC en vue d'une décision (HTA, remboursement, avis de la Commission de la Transparence), ou téléverse la publication ou le rapport technique d'une étude MAIC."
metadata:
  author: "Michel Cucherat"
  version: "1.0.0"
  url: "https://github.com/cucheratmi/_skills"
---

# Analyse critique d'une comparaison indirecte ajustée de type MAIC

## Objectif

Produire un rapport structuré qui répond point par point aux critères méthodologiques déterminant la fiabilité d'une **MAIC (Matching-Adjusted Indirect Comparison)**, qu'elle soit **ancrée** ou **non ancrée**, en vue d'une décision d'accès au marché, de remboursement ou de positionnement thérapeutique. Cette compétence ne remplace pas une analyse critique complète de chacun des essais impliqués (rôle de `analyse-critique-ecr`) : elle se concentre sur ce qui est **spécifique à la comparaison ajustée elle-même** — son ancrage, sa planification, la recherche des déterminants du critère de jugement, le choix et la justification des covariables d'ajustement, la qualité de la pondération obtenue et la taille d'échantillon effective.

## Principe axiomatique

Une MAIC n'est qu'une tentative de **reconstituer, à partir de données agrégées et de données individuelles pondérées, un essai randomisé fictif** comparant directement les deux traitements. Sa validité repose entièrement sur une hypothèse qui n'est **jamais vérifiable de façon directe** :

- en situation **ancrée** (comparateur commun aux deux essais), l'hypothèse de **constance conditionnelle des effets relatifs** : tous les modificateurs d'effet en déséquilibre entre les deux essais ont été identifiés et inclus dans la pondération ;
- en situation **non ancrée** (pas de comparateur commun), l'hypothèse, beaucoup plus forte, de **constance conditionnelle des effets absolus** : tous les facteurs pronostiques **et** tous les modificateurs d'effet en déséquilibre ont été identifiés et inclus.

Cette hypothèse ne peut être rendue plausible que par une **démarche prospective, systématique et transparente** de recherche des déterminants pertinents, **avant** toute analyse. À défaut, la liste des covariables d'ajustement est suspecte de sélection guidée par les résultats, et aucun ajustement statistique — aussi bien exécuté soit-il — ne peut compenser l'omission d'un déterminant pertinent non mesuré. Le doute sur la validité de cette hypothèse profite au statu quo (à l'absence de conclusion), jamais au traitement évalué.

## Prérequis

Rassembler avant de commencer : la publication ou le rapport technique de la MAIC ; la publication de l'essai index (traitement évalué, données individuelles) ; la publication de l'essai comparateur (données agrégées) ; si disponibles, le protocole et le plan d'analyse statistique (SAP) spécifiques à la MAIC, dont la date doit être comparée à la date de disponibilité des résultats de l'essai index. Si ces documents ne sont pas tous fournis, le signaler et poursuivre avec ce qui est disponible, en écrivant explicitement « non disponible » pour ce qui manque plutôt que de l'inférer.

## Workflow

### Étape 1 — Identifier les traitements et les études

Identifier le **traitement index** (celui évalué) et son **comparateur**, ainsi que les études correspondantes : nom/acronyme de l'essai, numéro d'enregistrement (NCT ou équivalent), référence bibliographique complète, phase, indication et population étudiée dans chacun des deux essais. Noter explicitement l'origine des données de chaque essai : **données individuelles (IPD)** — en principe celles de l'essai index, sponsorisé par le demandeur — versus **données agrégées (AgD)** — en principe celles de l'essai comparateur, extraites de sa publication.

### Étape 2 — MAIC ancrée ou non ancrée ?

Déterminer s'il existe un **comparateur commun connectant les deux essais** (le plus souvent un bras placebo ou un traitement de référence partagé) :

- **MAIC ancrée** : un comparateur commun existe ; la comparaison porte sur les effets relatifs de chaque essai par rapport à ce comparateur commun, puis sur la différence de ces effets relatifs. Seule l'hypothèse de constance conditionnelle des **effets relatifs** est requise.
- **MAIC non ancrée** : aucun comparateur commun (réseau déconnecté), ou comparaison directe des bras de traitement actif des deux essais sans passer par un comparateur commun. L'hypothèse de constance conditionnelle des **effets absolus** est requise, ce qui suppose qu'**aucun facteur pronostique ni modificateur d'effet** en déséquilibre n'a été omis — hypothèse nettement plus forte et, en pratique, rarement démontrable de façon convaincante.

Conclure explicitement sur le statut retenu et rappeler que les méthodes d'ajustement sur données agrégées sans comparateur commun sont considérées par les guides méthodologiques de référence comme fournissant des estimations **peu fiables**, à n'envisager qu'en l'absence de réseau connecté d'essais randomisés ou en présence d'études à bras unique.

### Étape 3 — La comparaison était-elle prévue a priori ou envisagée post hoc ?

Rechercher si le protocole ou le SAP de la MAIC a été **rédigé et daté avant** la disponibilité des résultats de l'essai index (ou de l'essai comparateur, si celui-ci est le plus récent des deux), ou si la comparaison n'apparaît qu'après coup, comme analyse complémentaire construite une fois les résultats connus. Rechercher la trace d'un enregistrement (protocole publié, PROSPERO ou équivalent si comparaison assimilable à une synthèse de preuves, plan de développement clinique mentionnant la MAIC en amont).

Une comparaison ajustée envisagée après la divulgation des résultats de l'essai index expose à un choix de comparateur, de population cible, de covariables d'ajustement ou de méthode d'analyse **orienté par le résultat souhaité**, à l'image du risque bien documenté pour les comparaisons externes post hoc dans les essais à bras unique. Écrire explicitement le statut retenu (planifiée a priori / post hoc / indéterminable à partir des documents disponibles) : c'est un facteur de confiance transversal à tous les critères suivants, jamais un simple détail administratif.

### Étape 4 — Pour les MAIC non ancrées : recherche formalisée des facteurs pronostiques ?

Uniquement pour les MAIC non ancrées (l'ajustement sur les seuls facteurs pronostiques ne se justifie pas pour une MAIC ancrée). Rechercher si les auteurs rapportent une démarche **formalisée et prospective** d'identification des facteurs pronostiques du ou des critères de jugement dans la pathologie concernée : revue de la littérature (systématique ou a minima structurée), construction d'un DAG (diagramme acyclique dirigé), consultation de cliniciens experts du domaine, ou appui sur des modèles pronostiques validés déjà publiés. L'absence de toute démarche de ce type, ou une liste de facteurs pronostiques reprise sans justification explicite (par exemple simplement recopiée de la liste des caractéristiques à l'inclusion de l'essai index), est une limite méthodologique majeure à signaler sans ambiguïté, dans la mesure où la sélection de covariables sur la seule base de leur significativité statistique ou de l'amélioration de l'ajustement du modèle n'est pas une méthode valide (les échantillons de ce type d'analyse sont structurellement sous-dimensionnés pour ce genre de sélection).

### Étape 5 — Recherche formalisée des modificateurs d'effet (ancrées et non ancrées)

Pour les deux types de MAIC, rechercher si une démarche **formalisée et prospective** d'identification des modificateurs d'effet des deux traitements a été réalisée, mobilisant typiquement : l'analyse des résultats en sous-groupes rapportés dans l'essai index et dans l'essai comparateur ; l'examen des tests d'interaction traitement × covariable lorsqu'ils sont disponibles ; une discussion argumentée des mécanismes d'action des deux traitements et de leur plausibilité biologique/pharmacologique en tant que source de modification d'effet ; toute autre donnée pertinente (méta-analyses de sous-groupes, avis d'experts cliniques, guides de pratique). Vérifier que cette recherche a été menée **indépendamment du résultat de la MAIC elle-même**, et non construite après coup pour justifier une liste de covariables déjà arrêtée. À défaut de toute démarche rapportée, l'écrire explicitement : l'hypothèse de constance conditionnelle des effets relatifs (ancrée) ou absolus (non ancrée) repose alors sur une base non documentée.

### Étape 6 — La liste des covariables d'ajustement est-elle rapportée, justifiée et complète ?

Extraire la liste effective des covariables retenues pour la pondération et vérifier sa cohérence avec le type de MAIC :

- **MAIC non ancrée** : la liste attendue comprend **les facteurs pronostiques et les modificateurs d'effet** identifiés aux étapes 4 et 5.
- **MAIC ancrée** : la liste attendue comprend **les seuls modificateurs d'effet** en déséquilibre identifiés à l'étape 5 ; l'ajout de facteurs purement pronostiques (non modificateurs d'effet) n'améliore pas la validité de l'ajustement et a pour seul effet d'augmenter inutilement la variance de l'estimateur (« sur-ajustement »/« over-matching ») — le signaler si constaté.

Pour chaque covariable retenue, vérifier qu'une **justification individuelle explicite** est rapportée (référence à une donnée de sous-groupe, à un test d'interaction, à un mécanisme d'action, à une méta-analyse ou à un consensus d'experts cité), plutôt qu'une justification générique ou l'absence totale de justification. Confronter la liste retenue à celle qui aurait dû résulter des étapes 4-5 : signaler explicitement toute covariable identifiée comme pertinente aux étapes précédentes mais **non retenue** dans l'ajustement final, sans justification de cette exclusion.

### Étape 7 — Quelles covariables nécessaires étaient indisponibles ?

Confronter la liste des covariables sur lesquelles il était nécessaire d'ajuster (étapes 4-6) aux données réellement disponibles : dans les **données individuelles de l'essai index**, d'une part, et dans le **tableau des caractéristiques à l'inclusion publié de l'essai comparateur**, d'autre part (seules les distributions marginales y sont en général rapportées, jamais la distribution jointe). Lister explicitement chaque covariable pertinente non disponible dans l'une ou l'autre source. Pour chacune, vérifier si les auteurs proposent une **quantification, même qualitative, de l'ampleur et du sens probable du biais résiduel** attendu du fait de cette omission (sur- ou sous-estimation de l'effet du traitement index, et dans quelle mesure) ; à défaut d'une telle discussion, le signaler comme une limite non traitée par les auteurs plutôt que la combler soi-même par une hypothèse non fondée sur les documents fournis.

### Étape 8 — L'ajustement réalisé peut-il être considéré comme optimal ?

Sur la base des étapes 4 à 7, porter un jugement de synthèse explicite sur l'adéquation entre l'ajustement **nécessaire** (liste théoriquement complète des déterminants pertinents) et l'ajustement **réalisé** (covariables effectivement incluses dans le modèle de pondération). Distinguer au moins trois situations et l'énoncer clairement : ajustement complet et correctement ciblé (concordance avec les étapes 4-5, aucune covariable pertinente manquante ou son absence est explicitement discutée) ; ajustement partiel (une ou plusieurs covariables pertinentes manquent sans discussion du biais résiduel attendu) ; ajustement non fiable (recherche des déterminants non formalisée et/ou liste de covariables non justifiée, rendant l'hypothèse de constance conditionnelle non plausible).

### Étape 9 — La pondération a-t-elle été efficiente ? Équilibre des covariables (SMD)

Vérifier que l'équilibre des covariables après pondération est rapporté, covariable par covariable, typiquement par la **différence de moyenne standardisée (SMD)** entre la population pondérée de l'essai index et la population de l'essai comparateur (ou, à défaut de SMD rapportée, par la comparaison directe des moyennes/proportions pondérées avant/après pondération). Le seuil de **SMD < 0,10** est un repère conventionnel largement utilisé en pratique (issu de la littérature sur les scores de propension) pour qualifier un déséquilibre résiduel de négligeable, mais ce n'est **pas un seuil réglementaire imposé** par les guides méthodologiques de référence (ni NICE DSU, ni les guides JCA cités ci-dessous, ne l'érigent en exigence formelle) : l'utiliser comme repère de lecture, mais ne jamais le présenter comme une norme opposable, et discuter la **pertinence clinique** d'un éventuel déséquilibre résiduel plutôt que sa seule signification statistique — les tests d'hypothèse comparant les moyennes après pondération ne sont pas une méthode recommandée pour juger de l'équilibre atteint. Rapporter explicitement, covariable par covariable ayant nécessité un ajustement, la SMD obtenue (ou son absence de disponibilité) et conclure sur l'équilibre global atteint.

### Étape 10 — Quel effective sample size (ESS) a été obtenu ? Est-il satisfaisant ?

Extraire l'**effective sample size (ESS)** de la population pondérée de l'essai index (méthode de Signorovitch et al., ESS = (Σwᵢ)² / Σwᵢ²) et la comparer à la **taille d'échantillon initiale** de cet essai. Il n'existe pas de seuil minimal officiellement prescrit, mais une réduction importante de l'ESS par rapport à l'échantillon initial est un signal d'alerte à interpréter conjointement avec la **distribution des poids** (présence de poids extrêmes, effectif de patients dont le poids devient négligeable) : ces éléments traduisent un **faible chevauchement (overlap)** entre les populations des deux essais, une **perte de puissance statistique** et une **instabilité potentielle de l'estimation**, avec des intervalles de confiance qui doivent alors être obtenus par une méthode tenant compte de l'incertitude liée à la pondération elle-même (erreurs-types robustes de type sandwich, ou bootstrap) — une absence d'une telle méthode conduit à des intervalles de confiance artificiellement trop étroits, à signaler explicitement si observée. Conclure explicitement si l'ESS obtenu, mis en regard de la distribution des poids, est satisfaisant, limite, ou franchement problématique pour la population cible réellement analysée (qui est, après pondération, la population commune aux deux essais, et non plus la population initiale de l'essai index).

### Étape 11 — Produire un rapport en markdown

Structure cible :

1. **En-tête** — traitement index et comparateur, études correspondantes (acronyme, NCT, référence), indication (étape 1).
2. **Cadre de la comparaison** — ancrée/non ancrée et hypothèse requise ; planification a priori ou post hoc (étapes 2-3).
3. **Recherche des déterminants du critère de jugement** — facteurs pronostiques (si non ancrée) et modificateurs d'effet, démarche suivie et son caractère formalisé ou non (étapes 4-5).
4. **Covariables d'ajustement** — liste rapportée, justification covariable par covariable, complétude au regard des étapes 4-5, covariables nécessaires indisponibles et discussion du biais résiduel associé (étapes 6-7).
5. **Qualité de l'ajustement** — jugement de synthèse sur l'optimalité de l'ajustement (étape 8), équilibre des covariables après pondération (SMD, étape 9), ESS et distribution des poids (étape 10), avec pour chacun un **tableau récapitulatif** (covariable, statut pronostique/modificateur d'effet, disponibilité, SMD post-pondération).
6. **Conclusion orientée décision** — synthèse explicite du niveau de confiance à accorder au résultat de la MAIC (fiable / à interpréter avec réserve / non fiable), direction probable d'un biais résiduel le cas échéant, et implication pour son utilisation dans la décision (positionnement thérapeutique, avis HTA).

## Règles non négociables

- **Ne jamais confondre** une méthode d'ajustement correctement mise en œuvre avec un ajustement qui atteint effectivement son but : une MAIC techniquement bien exécutée sur une liste de covariables incomplète reste une comparaison biaisée. Toujours distinguer l'ajustement *nécessaire* (théorique) de l'ajustement *réalisé*.
- **MAIC non ancrée = vigilance maximale.** Rappeler explicitement, chaque fois qu'une MAIC non ancrée est analysée, qu'elle repose sur l'hypothèse la plus forte et la moins vérifiable (constance conditionnelle des effets absolus) et qu'elle n'est en principe défendable qu'en l'absence de réseau connecté d'essais randomisés.
- **Sélection de covariables non guidée par la significativité statistique ou l'ajustement du modèle** : la considérer comme une méthode non valide et le signaler si c'est le cas rapporté, quel que soit le type de MAIC.
- **Ne jamais inventer** une justification de covariable, un DAG, une donnée de sous-groupe ou un mécanisme d'action qui ne serait pas rapporté dans les documents fournis : écrire explicitement « non rapporté » ou « non justifié dans les documents disponibles ».
- **Toujours discuter la pertinence clinique**, et pas seulement statistique, de tout déséquilibre résiduel après pondération et de toute covariable nécessaire mais indisponible.
- **Toujours interpréter l'ESS conjointement avec la distribution des poids** (poids extrêmes), jamais l'ESS isolément comme unique indicateur de qualité de la pondération.
- **Toujours vérifier la méthode d'estimation de l'incertitude** (erreurs-types robustes ou bootstrap) : son absence invalide la précision affichée de l'intervalle de confiance, indépendamment de la qualité de l'ajustement lui-même.
- **Toujours citer la source** (tableau, section méthodes, protocole/SAP) de chaque élément factuel rapporté dans le rapport.
- **Ne jamais se baser** sur la discussion ou la conclusion des auteurs ou sur des commentaires ou analyses externes
- **Toujours mentionner que le rapport a été élaboré par une IA**.

## Ressources de référence

- Vanier A, Fernandez J, Kelley S, *et al.* Rapid access to innovative medicinal products while ensuring relevant health technology assessment. Position of the French National Authority for Health. *BMJ Evid Based Med* 2023. [PMC10850619](https://pmc.ncbi.nlm.nih.gov/articles/PMC10850619/)
- Methodological Guideline for Quantitative Evidence Synthesis: Direct and Indirect Comparisons (Joint Clinical Assessment, Commission européenne). [PDF](https://health.ec.europa.eu/document/download/4ec8288e-6d15-49c5-a490-d8ad7748578f_en?filename=hta_methodological-guideline_direct-indirect-comparisons_en.pdf)
- Practical Guideline for Quantitative Evidence Synthesis: Direct and Indirect Comparisons (Joint Clinical Assessment, Commission européenne). [PDF](https://health.ec.europa.eu/document/download/1f6b8a70-5ce0-404e-9066-120dc9a8df75_en?filename=hta_practical-guideline_direct-and-indirect-comparisons_en.pdf)
- NICE DSU Technical Support Document 18 — Methods for population-adjusted indirect comparisons in submissions to NICE (Phillippo *et al.*, 2016). [PDF](https://sheffield.ac.uk/media/34216/download)
- Signorovitch JE *et al.* Comparative effectiveness without head-to-head trials: a method for matching-adjusted indirect comparisons applied to psoriasis treatment. *Pharmacoeconomics* 2010 (méthode originale de la MAIC et du calcul de l'ESS).
