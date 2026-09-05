---
name: analyse-marge-non-inferiorite
description: "Évaluer les aspects méthodologiques de la limite (marge) de non-infériorité utilisée dans un essai clinique randomisé de non-infériorité. Utiliser cette compétence quand l'utilisateur demande d'« analyser / évaluer / interpréter la marge de non-infériorité », « la limite de non-infériorité », « le seuil de non-infériorité » d'un essai, ou téléverse un essai de non-infériorité et veut en juger l'acceptabilité méthodologique et clinique."
---

# Analyse de la limite (marge) de non-infériorité d'un essai clinique randomisé

## Objectif

Évaluer, dans un essai clinique randomisé de non-infériorité, tout ce qui touche à la **limite de non-infériorité (marge, delta, seuil)** : sa valeur, sa signification concrète, sa justification statistique, et son acceptabilité clinique compte tenu des avantages par ailleurs du nouveau traitement. Cette compétence ne refait pas une analyse critique complète de l'essai (rôle de `analyse-critique-ecr`) : elle **approfondit spécifiquement la question de la marge**, qui est le point méthodologique le plus souvent mal posé ou mal justifié dans ce type d'essai.

## Principe axiomatique

Un essai de non-infériorité ne peut jamais démontrer l'absence de différence : il démontre seulement que, si une perte d'efficacité existe, elle est **inférieure à une limite fixée a priori**. Cette limite n'est scientifiquement défendable que si elle est **ancrée sur l'efficacité historique démontrée du comparateur** par rapport à son propre contrôle (le plus souvent le placebo). Et elle n'est **cliniquement acceptable** que si la perte d'efficacité qu'elle autorise est compensée par un **avantage tangible** du nouveau traitement (tolérance, sécurité, simplicité, coût, accessibilité). En l'absence de l'un ou l'autre de ces deux piliers — ancrage statistique et avantage clinique compensateur — une conclusion de non-infériorité ne permet pas d'affirmer que le nouveau traitement constitue une option acceptable en pratique, même si le test statistique est formellement positif.

## Prérequis

- Vérifier que l'essai relève bien d'une hypothèse de **non-infériorité** (formulation explicite dans la section méthodes/analyse statistique, ou dans le protocole/SAP si fourni), et non de supériorité ou d'un design séquentiel supériorité-puis-non-infériorité (à signaler comme tel).
- Si le protocole ou le plan d'analyse statistique (SAP) est disponible en plus de la publication, les utiliser en priorité pour la justification de la marge : elle y est souvent plus détaillée que dans l'article.
- Si l'essai n'est pas un essai de non-infériorité, informer l'utilisateur et ne pas poursuivre cette compétence (rediriger vers `analyse-critique-ecr`).

## Workflow

### Étape 1 — Identifier le cadre du test de non-infériorité

Extraire : le comparateur (traitement de référence actif — jamais un placebo dans un essai de NI), le critère de jugement principal, le risque alpha utilisé et son caractère uni- ou bilatéral (le standard est un test unilatéral à 2,5 %, équivalent le plus souvent à la borne d'un IC bilatéral à 95 %, parfois un IC à 90 % ou 97,5 % selon le nombre de comparaisons), et la règle de décision exacte telle que rapportée (« NI conclue si la borne supérieure/inférieure de l'IC de l'effet est meilleure que la marge »).

### Étape 2 — Extraire la valeur de la limite de non-infériorité et la mesure de taille d'effet concernée

Rapporter avec précision :
- La **valeur numérique** de la marge, telle que rapportée dans le protocole/méthodes.
- La **mesure de taille d'effet** sur laquelle elle porte : effet relatif (risque relatif, hazard ratio, odds ratio — ex. « HR seuil = 1,25 ») ou effet absolu (différence de risque, différence de moyennes — ex. « marge = -10 points sur l'échelle X »).
- L'échelle de calcul (linéaire ou logarithmique) et le sens de la marge (quelle valeur signe une perte d'efficacité selon le codage utilisé).
- Si la marge n'est disponible nulle part de façon explicite et chiffrée, l'écrire explicitement (« non rapportée ») plutôt que de l'inférer.

### Étape 3 — Expliciter ce que signifie concrètement cette limite

Traduire la marge en langage clinique compréhensible, par exemple : « on accepte que le nouveau traitement soit jusqu'à X % moins efficace que le comparateur » ou « on accepte jusqu'à Y événements de plus pour 100 patients traités, tout en concluant à la non-infériorité ». Si la marge est exprimée en effet relatif, la traduire aussi en équivalent absolu en utilisant le risque de base observé dans le bras comparateur **de l'essai lui-même**, en précisant explicitement que cette traduction est spécifique à la population et au risque de base de cet essai et n'est pas généralisable telle quelle.

### Étape 4 — Un seul critère de jugement ou plusieurs sont-ils concernés par la non-infériorité ?

Identifier si l'hypothèse de non-infériorité porte sur un critère de jugement unique, ou sur plusieurs critères (co-critères principaux, critères hiérarchisés, critère composite). Si le critère est composite, vérifier l'homogénéité clinique de ses composantes : un composite mêlant des événements qui ne sont pas des équivalents cliniques les uns des autres (ex. un événement thromboembolique et un saignement majeur) est intrinsèquement problématique en logique de non-infériorité, car une marge unique appliquée au composite masque des arbitrages différents selon la composante réellement affectée.

### Étape 5 — Si plusieurs critères : une marge unique ou des marges différentes ont-elles été utilisées ?

Vérifier si chaque critère de jugement dispose de sa **propre marge, justifiée par ses propres données historiques**, ou si une marge unique a été reprise indistinctement pour plusieurs critères sans justification spécifique à chacun. Une marge « générique » transposée d'un critère à l'autre sans ancrage propre est un défaut méthodologique à signaler explicitement. Vérifier aussi si un contrôle du risque alpha global a été prévu lorsque plusieurs tests de non-infériorité sont réalisés.

### Étape 6 — La marge a-t-elle été calculée à partir de la perte maximale d'efficacité possible (logique dite « M1 ») ?

Rechercher si les auteurs justifient la marge par le raisonnement suivant, classique dans la littérature méthodologique (SFPT, EMA) :

1. Estimer l'**efficacité historique** du comparateur par rapport à son propre contrôle (le plus souvent placebo), à partir d'un essai pivot antérieur ou d'une méta-analyse.
2. Retenir la **borne la plus conservatrice** (péjorative) de l'intervalle de confiance de cette efficacité historique — c'est l'« efficacité minimale garantie » du comparateur.
3. Choisir un **pourcentage de préservation** de cette efficacité minimale (par exemple 50 %, 75 %) : la marge autorise alors de perdre au maximum (1 − pourcentage de préservation) de cette efficacité minimale garantie.

Formule générale : **marge maximale défendable = efficacité minimale garantie du comparateur × (1 − pourcentage de préservation retenu)**.

Exemple numérique type : si une méta-analyse historique montre une réduction de risque du comparateur vs placebo de −25 % [IC95 % : −30 % à −20 %], l'efficacité minimale garantie est de 20 %. Avec une préservation cible de 75 %, la perte acceptable est de 25 % de ces 20 %, soit une marge maximale défendable de +5 % en différence absolue de risque.

Si ce raisonnement est bien retrouvé dans l'essai analysé :
- Reconstituer ou vérifier le calcul à partir des données historiques citées par les auteurs.
- Exprimer la perte d'efficacité qu'autorise la marge choisie **en pourcentage de l'efficacité historique démontrée du comparateur** (ex. « la marge utilisée correspond à une perte consentie de 40 % de l'efficacité du comparateur vs placebo »).
- Vérifier en particulier que cette perte reste **strictement inférieure à 100 %** de l'efficacité historique du comparateur : une marge autorisant une perte ≥ 100 % signifie que l'essai pourrait conclure à la « non-infériorité » d'un traitement en réalité moins efficace que le placebo — défaut majeur à signaler sans ambiguïté.
- Produire un **schéma** représentant la marge par rapport à l'efficacité du comparateur, sous la forme d'un axe de l'effet (ex. réduction de risque ou risque relatif) portant, de gauche à droite ou de bas en haut selon le sens de l'effet, les repères suivants : (a) l'effet du placebo / absence d'effet (référence 0 ou RR = 1), (b) l'estimation ponctuelle de l'efficacité historique du comparateur vs placebo, (c) la borne conservatrice de son IC (« efficacité minimale garantie »), (d) la limite de non-infériorité retenue dans l'essai, et (e) le résultat observé (estimation ponctuelle + IC) du nouveau traitement vs comparateur dans l'essai analysé. Si l'environnement de sortie permet un diagramme graphique (artifact, mermaid, image), le produire sous cette forme ; sinon, produire un schéma textuel clair (axe numéroté avec repères alignés, ou tableau ordonné des valeurs) directement dans le rapport markdown.

Si ce raisonnement n'est **pas** retrouvé : passer à l'étape 7.

### Étape 7 — Si la marge n'est pas basée sur la perte maximale d'efficacité : comment est-elle justifiée ?

Rechercher une justification alternative explicite : jugement d'experts, consensus clinique, reprise d'une marge conventionnelle générique (ex. « 10 % » ou « HR < 1,25 ») sans ancrage propre à la pathologie et au comparateur étudiés, recommandation réglementaire (FDA/EMA) antérieure, ou reprise de la marge d'un essai antérieur sur le même comparateur (avec le risque de « chaîne » de non-infériorités successives : chaque nouvel essai se compare à un comparateur déjà positionné par rapport à un placebo de plus en plus ancien, ce qui peut conduire à une dérive cumulative de l'efficacité réelle au fil des essais — à signaler si l'essai s'inscrit dans une telle filiation).

Si aucune justification statistique ou clinique explicite n'est fournie pour la valeur choisie, l'écrire clairement comme une limite méthodologique majeure du rapport (« la marge de X n'est justifiée par aucune donnée historique rapportée »), sans en inventer une a posteriori.

### Étape 8 — Identifier l'avantage par ailleurs du nouveau traitement

Rechercher si les auteurs mettent en avant, explicitement ou implicitement (rationnel de l'introduction, discussion), un avantage du nouveau traitement autre que l'efficacité sur le critère de jugement principal, par exemple : meilleure tolérance ou sécurité, voie d'administration plus simple (orale vs intraveineuse), prise unique ou moins fréquente, absence de surveillance biologique ou d'ajustement de dose, procédure moins invasive ou moins délabrante, coût plus faible, meilleure accessibilité/praticabilité. Si aucun avantage n'est identifié ni revendiqué par les auteurs, le signaler explicitement : une approche de non-infériorité sans aucun avantage par ailleurs perd sa justification rationnelle, puisqu'elle ne peut alors qu'aboutir, au mieux, à un traitement équivalent, au pire à un traitement moins efficace sans aucune contrepartie.

### Étape 9 — La limite de non-infériorité est-elle cliniquement acceptable compte tenu de cet avantage ?

Mettre en balance, par un jugement clinique explicite et argumenté : la perte d'efficacité **maximale possible** selon la marge (étapes 6-7) est-elle proportionnée à la nature et à l'ampleur de l'avantage identifié (étape 8) ? Tenir compte de la gravité de la pathologie et des conséquences cliniques d'une perte d'efficacité de cette ampleur (une marge large peut être plus difficilement acceptable dans une pathologie à pronostic vital engagé à court terme que dans une pathologie chronique de confort). Conclure explicitement : acceptable / discutable / non acceptable, avec justification.

### Étape 10 — La perte d'efficacité réellement consentie par les résultats est-elle cliniquement acceptable ?

Distinguer la perte **maximale possible** selon le protocole (la marge, un plafond a priori) de la perte **réellement observée** dans les résultats de l'essai (borne de l'IC de l'effet observé, qui peut être bien en-deçà de la marge). Conclure explicitement si, compte tenu du résultat observé (pas seulement de la marge théorique) et de l'avantage par ailleurs, le nouveau traitement représente une option acceptable en pratique clinique, et pour quelle population.

### Étape 11 — Produire un rapport en markdown

Structure cible :

1. **En-tête** — essai, référence bibliographique, comparateur, indication.
2. **Cadre du test de non-infériorité** (étape 1).
3. **La limite utilisée** — valeur, mesure d'effet, signification concrète (étapes 2-3).
4. **Critère(s) de jugement concerné(s) et marge(s) associée(s)** (étapes 4-5).
5. **Justification statistique de la marge** — calcul M1 reconstitué et schéma, ou justification alternative le cas échéant, avec verdict sur son ancrage (étapes 6-7).
6. **Avantage par ailleurs du nouveau traitement** (étape 8).
7. **Acceptabilité clinique de la marge et du résultat observé** (étapes 9-10), avec conclusion explicite orientée décision : le raisonnement en non-infériorité de cet essai est-il fondé, et le traitement peut-il être considéré comme une option acceptable, pour quelle population et avec quelles réserves ?

## Règles non négociables

- **Ne jamais confondre** « différence non significative » et « non-infériorité démontrée » : la non-infériorité ne peut être conclue que par la comparaison explicite de la borne de l'IC de l'effet observé à la marge prédéfinie, jamais par la seule absence de significativité d'un test de supériorité.
- **Toujours vérifier la concordance** entre l'analyse en intention de traiter et l'analyse per-protocole : contrairement aux essais de supériorité, une non-observance ou des données manquantes non différentielles tendent à biaiser un essai de non-infériorité vers une fausse conclusion de non-infériorité ; une discordance entre les deux populations d'analyse est un signal d'alerte à toujours mentionner.
- **Ne jamais inventer** une valeur de marge, un calcul M1, ou une justification qui ne serait pas rapportée dans les documents fournis (article, protocole, SAP) : écrire explicitement « non rapporté » ou « non justifié dans les documents disponibles ».
- **Toujours quantifier** la perte d'efficacité en deux temps distincts : perte maximale autorisée par la marge (théorique) et perte réellement compatible avec les résultats observés (bornes de l'IC observé), sans les confondre.
- **Toujours citer la source** (page, section méthodes/protocole/SAP) de chaque valeur numérique rapportée.
- **Signaler sans ambiguïté** toute marge autorisant une perte ≥ 100 % de l'efficacité historique démontrée du comparateur, et toute absence d'avantage par ailleurs du nouveau traitement : ce sont les deux défauts les plus critiques pour la validité du raisonnement de non-infériorité.

## Ressources de référence

- [Livre blanc SFPT — Essai de non-infériorité](https://sfpt-fr.org/livreblancmethodo/source/dossier%206%20-%20essai%20de%20non-inf%C3%A9riorit%C3%A9.pdf)
- Pour une analyse critique complète de l'essai au-delà de la seule question de la marge, s'appuyer sur la compétence `analyse-critique-ecr`.