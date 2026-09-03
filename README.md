# INSIGHT skills

**Apporter à l'IA l'expertise méthodologique et statistique nécessaire pour interpréter les études cliniques évaluant les interventions de santé**

Les skills mise à disposition ici permettent de doter les IA généralistes des compétences nécessaires pour analyser de manière critique et interpréter les résultats des études cliniques comme les essais randomisés de supériorité ou d'infériorité, les études observationnelles inférentielles (type étude de Real World Evidence), les méta-analyses, etc.

Ces skills permettent à votre IA de produire un rapport évaluant une étude à partir du pdf de l'article (et éventuellement du supplément, du protocole ou du SAP) en se basant sur une expertise validée. 

>_Attention il convient de vérifier que l'IA que vous utiliser peut recevoir des pdf d'articles sans que cela enfreigne les disposition légale en vigueur (ce qui pourrait avoir lieu si cette IA utilise les documents des documents pour leur apprentissage). Il y a souvent une option à cocher/décocher sur ce point._

## Skills disponibles

Les skills actuellement proposées (d'autres sont en développement) sont les suivantes.

| Nom | Description et référence |
| --- | --- |
| analyse-critique-ecr | Interprétation et analyse critique d'un essai randomisé de supériorité. Base sur le document de la Société Française de Pharmacologie sur la [lecture critique des essais thérapeutique](https://sfpt-fr.org/livreblancmethodo/part4/file_0.htm) |
| analyse-critique-observationnelle-inferentielle | Interprétation et analyse critique d'une étude observationnelle inférentielle (type RWE). Basée sur le travail de la table ronde des atelier de Giens 2024 [Attentes méthodologiques pour la démonstration de l’efficacité des produits de santé par les études observationnelles](https://hal.science/hal-04812328v1/document) |
| rob2-0 | Evaluation du risque de biais d'un essai clinique randomisés à l'aide de l'outil [ROB 2.0](https://www.bmj.com/content/366/bmj.l4898)|
| audit-rapport-vs-avis-ct | Évalue la qualité de l'évaluation d'une étude faite par l'une de ces skills en utilisant comme benchmark l'avis de transparence portant sur la même étude. Nécessite de fournir le rapport d'analyse produit par la skill et le pdf de l'avis de transparence correspondant | 


## Généralités sur les skills (compétences)

Les skills permettent d'apporter des compétences spécifiques aux agents et plateformes d'IA (comme Vibe de Mistral, chatGPT, Claude, antigravity, etc.). Il permettent de compléter les capacités de ces outils généraliste avec des expertises de haut niveau spécifiques à une taches.
Il s'agit d'un [standard ouvert](https://agentskills.io/home) disponible maintenant sur presque toutes les IA.


## Comment utiliser ces skills

Une fois installées les skills se déclenche automatiquement lorsqu'un prompt demande une tache qui est couverte par les skills. Par exemple après avoir télécharger le pdf d'un article d'essais clinique et demander d'analyse ou d'interpréter cette étude, l'AI détectera que cette demande correspond à la skill 'analyse-critique-ecr' et l'utilisera pour répondre à la demande de l'utilisateur.

Vous pouvez aussi demander explicitement l'execution d'une skill pour votre prompt à l'aide de la commande '''/''' suivi du nom de la skill, comme par exemple :
```
/analyse-critique-ecr analyse cet essai clinique
```


## Installation

Pour installer ces skills sur votre outil habituel (Vibe de Mistral, chatGPT, Claude, antigravity, etc.) poser lui la question dans un prompt.

```
Comment installer les skills disponibles dans le GitHub cucheratmi/_skills 
```

ou plus directement 

```
Installe les skills disponible dans le Github cucheratmi/_skills (https://github.com/cucheratmi/_skills)
```

Si vous ne souhaitez installer qu'une skill particulière le préciser dans le prompt d'installation.

>_Il est important d'analyser le contenu des skills avant de les installer pour écarter la possibilité de skill malveillante (par injection de prompt). Les IA font une analyse avant de faire l'installation mais rien ne vaut une inspection visuelle du contenu de la skill._


## Interest de l'approche  

L'expertise apportée par ces skills court-circuite l'approche naive que pourrait avoir une IA généraliste sur cette tache. Cette approche basée sur une compétence parfaitement explicitée dans les skills garantie une évaluation parfaitement transparente (explicable), contrairement aux productions standards des IA. De même les skills demande à l'IA de ne se baser que sur la publication et de ne pas tenir compte d'analyses ou de commentaires externes sur cette étude qu'elle pourrait avoir ingurgité leur de son apprentissage. Cela permet d'éviter, par exemple, que la communication promotionnelle concernant le traitement évalué interfère avec l'analyse de l'étude.   
Il est aussi demandé que l'interprétation ne tiennent pas compte de la conclusion et de la discussion des auteurs afin d'éviter les intoxications par les spins de conclusion qui pourraient être présents dans les publication.


## Validation 

D'une manière générale l'évaluation de ces outils est difficile car la qualité du résultat produit dépend entre autres du model utilisé, de sa version, mais aussi de la boucle agentique de l'IA utilisée. les évolution technologique sur ces éléments étant tellement rapide qu'un évaluation a un moment donné ne préjugera pas de la performances des ces skills ultérieurement ou avec un nouveaux modèle ou une nouvelle IA ou boucle agentique.





## Auteurs



