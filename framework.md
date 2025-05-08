---
layout: page
title: Theoretical Framework
tags:
  - AI
  - Biases
  - framework
  - bias_definition
  - fairness
---
# **Theoretical framework**

  

## *What is bias?*

Bias occurs when personal opinions compromise impartiality, leading to unfair support for or opposition against a particular person or thing. In AI, bias can have many different origins, and three of them, most commonly present in computing science, will be described in the following sections. 

  

**Data bias** occurs when the training data used to develop an algorithm is unrepresentative, incomplete, or prejudiced. This can happen if certain groups are underrepresented or overrepresented, or if historical prejudices are embedded within the data. This is typically true for most unmodified datasets, as they tend to reflect and perpetuate the biases embedded in the societies from which they derive..

  
**Model bias** refers to biases that arise from the assumptions and limitations inherent in the model's structure or the way it is designed. Even with unbiased data, a model may have a tendency to oversimplify complex relationships, leading to systematic errors. For example, a linear model may not capture nonlinear patterns, resulting in biased predictions.

  
**Algorithmic bias** encompasses biases introduced during the actual process of algorithm design, implementation, or operation. This can involve choices made in feature selection, parameter tuning or the use of fairness constraints, which can unintentionally favor certain outcomes or groups. For instance, an algorithm designed without considering fairness metrics might produce biased outcomes even if it was trained on unbiased data and has a flexible structure.

  

Depending on the situation, one or several of those forms of bias can be observed. In this study’s case, since the data are synthetic and under control, we want to focus on the algorithmic biases to explore the consequences of using those algorithms in the hiring process.

  
  

## *Defining fairness*

  

Ideally, the algorithms should treat information, CVs in this context, in a fair manner to accomplish their intended mission–and if the manner is deemed unfair then the algorithm is considered to be biased. However, the idea of fairness itself is complex and difficult to conceptualize under one single definition. This section aims to provide a brief overview of the most prominent perspectives on algorithmic fairness within the academic discourse. 

  

Evidence shows that commonly used fairness methods can actually harm individuals, particularly those from marginalized communities (Chohlas-Wood et al. 2023), hence the approach has to be carefully evaluated. The simplest definition would be the one of the Oxford Dictionary defining fairness as *the [quality](https://dictionary.cambridge.org/dictionary/english/quality) of [treating](https://dictionary.cambridge.org/dictionary/english/treat) [people](https://dictionary.cambridge.org/dictionary/english/people) [equally](https://dictionary.cambridge.org/dictionary/english/equal) or in a way that is [right](https://dictionary.cambridge.org/dictionary/english/right) or [reasonable](https://dictionary.cambridge.org/dictionary/english/reasonable)*. However, the notions of “right” or “reasonable” are socially, culturally and politically constructed, and have evolved through time. It is commonly admitted that public policies and, namely, laws are a good indicator of local morality. Indeed, it often reflects the way of thinking of one population as it has been underlined: the consensus perspective gives a central role to public opinion and “suggests that… law is essentially a codification of the values of a people” (Thomas et al. 1976, p. 110). However, algorithms are not yet regulated in most countries, which itself necessitates further consideration. Since algorithms are nowadays essentially developed by Western and East-Asian companies, it is relevant to present a brief comparison of how the notion is understood in both contexts. 

  

An ancestral definition of fairness seems to be the Golden-Rule Fairness. Simply explained, it is the incarnation of the popular sayings “Treat others as you would like others to treat you” (positive or directive form), or “Do not treat others in ways that you would not like to be treated” (negative or prohibitive form). However, as a social group gets bigger, it is more difficult to apply this rule, creating a need for finding other definitions.

Questioning generations of thinkers, the current western American understanding of what fair means seems to have been largely influenced by the philosopher John Rawls and current discussions of fairness underlay his book, *A Theory of Justice*. Rawls says that a “well-ordered” political society is “a fair system of cooperation over time from one generation to the next, where those engaged in cooperation are viewed as free and equal citizens and normal cooperating members of society over a complete life”. To achieve this, the concept of “veil of ignorance” is developed: to make fair decisions, one has to act without knowing the characteristics of the object the decision will be taken for. The limit of this logic lies in the implementation of this “veil”, as algorithms that initially inspired such optimism have rapidly revealed their constraints. 

  

This previous conception of fairness involves the notions of freedom and equality. Japan will be chosen here to give an alternative perspective on how the notion of fairness can be understood. The choice of Japan comes from the large economic and technological exchanges with multiple countries including the US. In Japanese, a unique word translating the word fairness does not exist (Kidder, 1986) and can be translated into two different words. 公正 (Kousei) focuses on the principle of being right and just according to established rules and moral standards, closer to *justice*. 公平 (Kouhei) focuses on the practice of treating everyone equally and without bias, or *equity*. The influences of Confucianism, Buddhism, and collectivism, as well as other societal factors, have brought a different perception of those notions, influencing the way people act in certain given situations. A concrete example could be that factors considered important for US employees, such as participatory decision-making, may not resonate with Japanese workers, who often believe that top management should retain decision-making authority (Kidder et al. 1991).

  

However, those definitions are difficult to generalize. Indeed, even among the western or among Asian countries, because of the large variety of historical, religious and philosophical backgrounds, it has been proven that the notion of fairness is understood very differently (Abramson & Inglehart, 1995; Scarborough, 1998). However, parallely to this limit, the unprecedented globalization faced today, like with the internet, brings new challenges. Indeed, an AI system created in the US can be used all across the world, even in countries with different philosophical and social norms, unless the country itself puts restrictions in place, like in China or North Korea. The question of how to define fairness in a global context becomes necessary. For Edgar Porter, substantive agreement on the practical application of fair behavior remains unattainable, but it is possible for different cultures to converge on the conceptualization of fairness as a universal construct within the context of globalization (Dator et al 2006). However, not reproducing the colonial pattern of the western world trying to impose its “definition” of fairness is an essential issue. In general, it seems to be important to thwart any form of philosophical hegemony which would have very concrete consequences, raising numerous ethical issues.

  

Finally, in the computer science literature, the three following definitions of fairness seem to be used often (Saxena et al. 2020). It is interesting to note that certain cultures are dominating the research ecosystem (above all American and Chinese), and therefore, can bring a form of normative domination of the computing science ethic.

- **Treating similar individuals similarly** (Dwork et al., 2012): Fairness, in this formulation, necessitates the equitable treatment of observationally similar individuals with respect to favorable decision outcomes. Similarity is quantified via a task-dependent metric that is intended to approximate a veridical representation of the relevant decision context. Algorithmic fairness is then operationalized through the satisfaction of the Lipschitz condition, a mathematical constraint guaranteeing decision continuity and stability with respect to the designated similarity metric.
    
- **Never favor a worse individual over a better one** (Joseph et al., 2016): in a setting where a single individual is to be selected for a favorable decision introduce a meritocratic fairness criterion for single-selection problems, positing that the probability of selecting a superior individual (characterized by a greater expected value of an intrinsic quality metric) must be at least equivalent to the probability of selecting an inferior individual. For example within the domain of loan allocation, this principle translates to ensuring that applicants with superior repayment histories are afforded at least equivalent access to funding as their less creditworthy counterparts.
    
- **Calibrated fairness** (Liu et al., 2017): in the setting of sequential decision-making, calibrated fairness selects individuals in proportion to their merit. It is a sequential decision-making paradigm characterized by proportional selection based on individual merit. Calibrated fairness is shown to subsume Joseph et al.'s meritocratic formulation under conditions of complete information and imply Dwork et al.'s fairness for appropriately specified similarity metrics.
    

  

Once an agreement on what fair means for an algorithm is achieved, an essential question arises on how to technically process it to render it fair. This discussion has increased in the academic discourse of the past few years. Depending on the field of application (here, the hiring process), as well as the support (the algorithms), the way to apprehend the question might be different. In *Designing equitable algorithms* (Chohlas-Wood et al. 2023), the three following fairness principles for algorithms are explored, to avoid biases as much as possible. 

- **Blinding**: involving minimizing or eliminating the influence of demographic characteristics, like race, on decision-making processes
    
- **Equalizing decision rates across demographic groups**: equal outcomes across groups
    
- **Equalizing error rates across demographic groups**: equal error rates across groups
    

None of those principles are “perfect” and are often mutually incompatible, meaning achieving one can violate another, and some trade-off has to be made. This compromise is, again, the result of a choice which can always be evaluated critically. 

In the case of this study, biases are measured based on the compatibility score. Biases are considered to be present if certain demographics achieve a better score despite having the same qualifications.

We will be basing the analysis of the result on the definition of fairness as the fact of *treating similar individuals similarly* (Dwork et al., 2012), that is for instance, people with the same competences should obtain the same score, independently of their ethnicity, gender or ideological expression. Based on Rawls' idea that the algorithm should play the role of the veil of ignorance, we will follow the methodology explained below to answer our question.

## *Hypothesis*

Taking into account the fairness framework and existing literature on the topic, this study tests **the following hypotheses**: 

- **H1.** The resumes with traditionally masculine names will receive higher compatibility scores than those with traditionally feminine names
    
- **H2.** The resumes with traditionally British-sounding names will receive higher compatibility scores than those with non-British sounding names
    
- **H3.** The resumes featuring religious or political engagements will receive lower compatibility scores. The effect will also be more pronounced in different professional sectors.
    
- **H4.** Certain professional sectors exhibit greater sensitivity to gender, ethnicity and ideological indicators in resumes.