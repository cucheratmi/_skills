---
name: robins-i
description: Conduct a risk of bias assessment of a Non-randomized Studies of Interventions, using the ROBINS-I tool (v2)
---

## Instructions

- Base your assessment **exclusively on the information reported in the publication** (methods and results sections). Do not make assumptions beyond what is explicitly stated. Do not rely on external RoB assessments of this trial.
- For each domain, answer the signalling questions, then formulate a judgment: **Low / Some concerns / High**.
- Justify each judgment concisely (1–2 sentences).


---

 Variant A (the analysis is estimating the intention-to-treat effect so only baseline confounding needs to be addressed)

# Domain 1. Bias due to confounding

The questions in this domain focus on the confounding factors (see Guidance note 10) that were identified as important in the preliminary evaluation in section E.
We use the term uncontrolled confounding to refer to confounding that was not controlled by the design or analysis of the study – and is therefore likely to bias the estimated effect of intervention. This may arise because (i) confounding factors were not (or could not) be measured; (ii) variables used to measure confounding factors were insufficient to characterize the confounding factor; or (iii) variables that characterize the confounding factor were measured but not included in the analysis. 
The answers to the signalling questions are based on contents of the completed table ‘Evaluation of confounding factors’.
There are two variants of this domain. 
Variant A is used when the analysis is estimating the intention-to-treat effect, when only baseline confounding needs to be addressed. Baseline confounding occurs when one or more prognostic factors, present before the start of follow-up, predict whether participants start the intervention or comparator strategy. Appropriate methods to control for baseline confounding include stratification, regression, matching, standardization, and inverse probability weighting. The analysis may control for individual variables or for estimated propensity scores. Inverse probability weighting is based on a function of the propensity score.
Variant B is used when the analysis is estimating the per-protocol effect, that is, the effect of receiving a specified intervention strategy versus a comparator strategy over time. This is the case when the analysis accounted for protocol deviations (switches during follow-up between the intervention strategies being compared, or other protocol deviations during follow-up). Such an analysis might be performed, for example, by partitioning follow-up for individual participants according to the intervention received, or by censoring follow-up when participants deviated from their initial intervention. When estimating the per protocol effect, both baseline confounding and time-varying confounding need to be addressed. It is usually not appropriate to attempt to control for time-varying confounding by including the time-varying confounders in regression models. Special methods (‘g methods’) that avoid ‘conditioning on’ time-varying confounders should be used. For example, in analyses that censor follow-up when participants deviate from their initial intervention strategy, one appropriate approach to analysis is to model the probability of such deviations over time, based on the baseline- and time—varying confounding factors, and then to adjusted for the censoring using inverse probability of censoring weights.

## Signalling questions 1.1 - Did the authors control for all the important confounding factors for which this was necessary?
The important confounding factors are those specified in the Preliminary consideration of confounding factors. The preliminary assessment will have determined whether there were important confounding factors that were not controlled for and should have been (because there was no evidence that controlling for the variable was unnecessary). Failure to control for all important confounding factors may lead to bias. The analysis should attempt to control for these confounding factors using an appropriate method, for example using stratification, regression, matching, standardization or inverse probability weighting (control may be for individual variables or for estimated propensity scores).
Answer ‘Y’ or ‘PY’ if all the important confounding factors for which it is was deemed necessary to control (under Preliminary consideration of confounding factors) were indeed controlled for appropriately. Also answer ‘Y’ or ‘PY’ in the (very rare) situation that there are no confounding factors and an unadjusted analysis is presented.
Answer ‘WN’ if most of the important confounding factors for which it was deemed necessary to control (under Preliminary consideration of confounding factors) were controlled for using appropriate methods, and any uncontrolled confounding (because not all important confounding factors were controlled for) was not likely to be substantial. This would be the case, for example, if the factors that were not controlled for were likely to be highly correlated with factors that were controlled for.
Answer ‘SN’ if there is at least one important confounding factor that should have been controlled for but was not, and the failure to control for this factor is likely to have a material impact on the estimated effect of intervention.

## Signalling questions 1.2 - If Y/PY/WN to 1.1: Were confounding factors that were controlled for (and for which control was necessary) measured validly and reliably by the variables available in this study?
Appropriate control of confounding requires that the variables adjusted for are valid and reliable measures of the confounding factors. For some topics, a list of valid and reliable measures of confounding factors will be specified in the review protocol but for others such a list may not be available. Study authors may cite references to support the use of a particular measure. If authors control for confounding variables with no indication of their validity or reliability, then subjectivity of the measure should be evaluated.
In the (very rare) situation that there are no confounding factors and an unadjusted analysis is presented, answer ‘Y’ or ‘PY’.

## Signalling questions 1.3 If Y/PY/WN to 1.1: Did the authors control for any post-intervention variables that could have been affected by the intervention?
Controlling for post-intervention variables that are affected by intervention is not appropriate (this is sometimes called ‘over-adjustment’). Controlling for mediating variables estimates the direct effect of intervention and may introduce bias. Controlling for common effects of intervention and outcome (sometimes referred to as ‘colliders’) introduces bias.

## Signalling questions 1.4. Did the use of negative controls, quantitative bias analysis, or other considerations, suggest serious uncontrolled confounding?
Use of a “negative control” – exploration of an alternative analysis in which no association should be observed – can sometimes suggest that the result is subject to uncontrolled confounding, if similar associations are identified for the result being assessed and the negative control. 
If the study did not use negative controls and no other considerations suggest uncontrolled confounding, answer ‘N’.
Answer ‘Y’ or ‘PY’ if negative controls indicate that the result being assessed suffers from material bias due to confounding.

## Optional: What is the predicted direction of bias due to confounding?
If the likely direction of bias can be predicted, it is helpful to state this. A judgement about the predicted direction of bias should take into account all uncontrolled confounding from omitted important confounders and may therefore require judgements about the relative impact of confounding factors operating in different directions.
The effect of confounding is to bias the estimated effect upwards or downwards – to overestimate or to underestimate the intervention effect. If the true intervention effect is above 0 (above 1 for a ratio measure) then an upward bias will also represent a bias away from the null; if the true intervention effect is below 0 (below 1 for a ratio measure) then a downward bias will also represent a bias away from the null. The situation is not always so clear. For example, if the true effect is above 0 then a downward bias may bring the estimate towards the null or beyond it (to a value less than 0). 


# Domain 2. Bias in classification of interventions

This domain addresses bias arising from misclassification of the intervention strategies being compared. The first three questions in the domain address a type of misclassification bias arising from immortal time, time during which outcome events are prevented from happening by the way the analysis was done. Such analytical problems generally occur when the intervention and comparator strategies cannot be distinguished at the time when follow-up would have started in the target trial, making it difficult or impossible to know which intervention strategy participant were following. This is the first of two types of bias arising from immortal time that are addressed in ROBINS-I V2 (the second type, which is usually less serious, is addressed in Domain 3, Bias in selection of participants into the study). 
Misclassification is generally considered to be differential if it is related to subsequent outcomes; or non differential if it is unrelated to subsequent outcomes. The fourth and fifth signalling questions in the domain address differential misclassification and non-differential misclassification, respectively. Differential misclassification, which is generally considered to be more serious than non-differential misclassification, may occur when classification of intervention status is influenced by knowledge of the outcome or risk of the outcome.

## 2.1 Were the intervention strategies distinguishable at the time when follow-up would have started in the target trial?
In the target trial, follow-up starts when participants meet eligibility criteria and are assigned to a strategy. In most non-randomized studies, there is no formal assignment and so participants are classified according to information on interventions that were prescribed or received. However, some strategies cannot be distinguished at the start of follow-up. For example, for the strategies “Surgery within 6 months of diagnosis” and “Delay surgery until clinical progression of disease”, then follow-up starts at the time of diagnosis and patients who do not undergo surgery and do not experience disease progression have adhered to both strategies until 6 months after diagnosis. 
Assigning participants to intervention strategies based on information after the start of follow-up may lead to participants in one of the groups having a period of ‘immortal time’ during which the outcome cannot occur. In the example above, participants who are assigned to the intervention group because they have surgery within 6 months of diagnosis cannot experience the outcome during the period between diagnosis and surgery.

## 2.2 If N/PN/NI to 2.1: Did all or nearly all outcome events occur after the intervention and comparator strategies could be distinguished?
If the period during which the intervention and control strategies cannot be distinguished is short in relation to the total follow-up, then the proportion of outcome events occurring during that period may be low. This limits the risk of bias due to misclassification of participants into intervention groups based on events that occurred after the start of follow-up.

## 2.3 If N/PN/NI to 2.2: Did the analysis avoid problems arising from intervention strategies that are not distinguishable at the start of follow-up?
Analyses using, for example, the ‘clone-censor-weighting method’ (https://www.bmj.com/content/360/bmj.k182.long) or the g-formula can overcome problems associated with intervention strategies that are not distinguishable at the start of follow-up. For analyses using these approaches, answer ‘SY’ if predictors of treatment during follow-up were measured and used appropriately to derive inverse-probability weights. Answer ‘WY’ if the analysis used these methods or another appropriate method but is unlikely to have fully adjusted for prognostic factors that predict treatment after the start of follow-up.
Answer ‘SY’ if the study used a ‘landmark’ analysis, which avoids these problems by starting follow-up after the intervention strategies can be distinguished. However, note that a ‘landmark’ analysis will be at risk of selection bias, which is addressed in the domain ‘Bias in selection of participants into the study’.

## 2.4 Was classification of intervention status influenced by knowledge of the outcome or risk of the outcome?
Differential misclassification arises if the outcome, or the factors influencing the outcome (other then the interventions), influence the classification. If intervention classification is based on information that was collected after follow-up started, this information may be influenced by the outcome or the risk of the outcome, for example if participants were asked to recall past interventions. Differential misclassification is less likely if all the information used to classify the intervention and comparator groups came from sources that were recorded at or before the time that interventions were assigned and follow-up started.
It is possible for outcome events to affect the availability of information used to classify interventions in a non-randomized study. For example, if records of receipt of an intervention are destroyed if a participant dies (leading to misclassification of that participant into the comparator group) then analyses investigating the effect of the intervention on mortality will be biased due to differential misclassification depending on the outcome.
Response options ‘WY’ and ‘SY’ are used to distinguish between different risk-of-bias judgements.  Answer ‘SY’ if the impact of knowledge of the outcome or risk of bias outcome was likely to be substantial.

## 2.5 Were further classification errors (not influenced by knowledge of the outcome or risk of the outcome) likely?
This question relates to non-differential misclassification (that is, unrelated to the subsequent outcome) of intervention status. For example, intervention status may be misclassified for some participants if receipt of (or assignment to) the intervention is not recorded in the information source used to classify intervention status. Similarly, some participants may receive (or be assigned to) the intervention without it being recorded. Misclassification errors of this nature usually bias the result towards the null.
Criteria for considering individuals to have received each intervention should be clear and explicit, covering issues such as type, setting, dose, frequency, intensity and timing of intervention. A pre-requisite for correct classification of interventions is that the interventions are well defined. Ambiguity in the definition may lead to misclassification of participants, and so is likely to lead to a response of ‘N’ or ‘PN’ to this question.
It may be helpful to think separately about (i) whether all people who were assigned to (or who received) the intervention were correctly classified, and (ii) whether all people who were assigned to (or who received) the comparator were correctly classified.
“Nearly all” should be interpreted as “enough to be confident of the findings”, and a suitable proportion will depend on the context. In many situations, correct classification for 95% of the participants may be sufficient

## Optional: What is the predicted direction of bias in classification of interventions?
If the likely direction of bias can be predicted, it is helpful to state this. The direction might be characterized as being in favour of the intervention, as being in favour of the comparator, or as towards (or away from) the null. Non-differential misclassification will often bias results towards the null.












