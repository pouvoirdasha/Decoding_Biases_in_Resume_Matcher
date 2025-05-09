---
layout: page
title: Literature review
tags: [AI Biases, literature]

---
# **What did we learn from the literature ?**

## *Bias in Hiring*

Bias in hiring practices is a long-standing concern. Decades of audit studies have demonstrated that applicants are evaluated not only on qualifications but also on socially constructed traits such as gender, ethnicity and perceived cultural fit. As a result, applicants from marginalized groups, including but not limited to women, ethnic minorities and people with disabilities, often face discrimination during recruitment processes. In their seminal study on racial discrimination in the labor market, Bertrand and Mullainathan (2004) found that applicants with names perceived as Black received significantly fewer callbacks than identical resumes with White sounding names–this discrimination persisted through sectors and industries. Building on this evidence, Quillian & Midtbøen’s (2021) cross-national study reveals that such racial and ethnic discrimination is not confined to the US, but represents a widespread international issue. Similarly, gender bias in hiring has been observed across countries (Petit, 2007; Baert et al., 2016; Kübler et al., 2018). Gender discrimination is particularly significant in male-dominated jobs (Fabris et al., 2024, p. 7) and for mothers (González et al., 2019). These findings underscore how implicit and explicit human biases influence hiring outcomes, often in seamless but systematic ways. 

## *Bias in Algorithmic Hiring*

In response to these issues, many organizations have turned to algorithmic hiring systems to minimize bias by standardizing evaluations and offering a more objective alternative to human judgement, particularly in the screen phase of hiring, where application volumes make consistency and speed crucial. However, this techno-solutionist view (Houser, 2019) is increasingly challenged by empirical findings revealing that algorithmic systems are not bias-free. Instead, they often may reproduce or exacerbate biases and historical inequalities (Raghavan et al., 2020; Drage & Mackereth, 2022). 

Indeed, a growing body of empirical research demonstrates that bias persists in algorithmic hiring tools, including resume matchers, interview video analysis tools and LLM-based CV screeners. These models, even when stripped of explicit attributes like gender or race, frequently encode and operationalize proxy variables, such as university attended, word choice, zip code or extracurricular activity, that correlate with those attributes (Barocas & Selbst, 2016). 

These biases usually arise from their training data and are reinforced through learned association in large language models. Garg et al. (2018), for instance, quantified how word embeddings–statistical models that capture semantic relationships between words–have encoded gender and ethnic stereotypes over the past century, demonstrating that women continue to be linguistically associated with family and domestic roles. Similarly, they showed that racial minorities were consistently connected to stereotypical professions and negative affective descriptions. These embeddings are foundational to many natural language processing (NLP) systems used in resume screening. 

Moreover, in hiring contexts these biases affect how candidate resumes are interpreted. Köchling and Wehner (2020) have conducted a systematic literature review of studies on algorithmic decision making in HR particularly in recruitment and development. Their meta-analysis has clearly revealed consistent discrimination across a range of AI-based recruitment tools on the different stages of the recruitment process. De-Arteage et al. (2019) showed that implicit gender indicators in text led to lower fit scores for female-coded resumes in algorithmic occupation prediction. They analyzed the textual bios of real-world candidates and found that bios inferred to belong to women were scored lower for technical roles, despite identical qualifications. These differences arise from biased semantic representations and can result in systemically lower ranking or exclusion from consideration pools. Indeed, Drage and Mackereth (2022) argue that AI recruitment does not eliminate disparities, but reclassifies and reinforces them, promoting candidates who match historically dominant patterns while marginalizing those who deviate from algorithmically encoded norms. 

Even LLMs specifically designed for fairness often exhibit implicit biases, particularly based on race (Amin et al., 2024) or gender (Kumar et al., 2024), when tested in hiring contexts (Wen et al., 2025; Iso et al., 2025). Veldanda et al. (2023) replicated Bertrand and Mullainathan (2004) design in a digital context, testing whether racialized names still influence candidate outcomes. Their findings demonstrate that algorithmic systems continue to display discriminatory behavior towards different demographic groups, with varying degrees of bias depending on input and context. Their study therefore highlights the persistence of racial bias in modern AI systems built on LLMs. 

## *Ideological Bias*

A less explored but increasingly relevant dimension of bias in algorithmic hiring relates to ideological and cultural expressions. Applicants often include indicators of their beliefs, affiliations or values in their resumes, such as participation in religious, activist or political organizations. Rivera (2012) investigated the impact of cultural matching between the candidate and employer on outcomes in traditional hiring practices. Her findings showed that employers overwhelmingly preferred candidates who resembled them and shared similar experiences and interests. This can lead to bias and discrimination by systematically putting at a disadvantage candidates from different cultural, socioeconomic or educational backgrounds, regardless of their qualifications. Applied to the digital context, these cues can then affect algorithmic evaluations, especially when NLP models lean latent associations between particular ideologies and perceived fit or risk. 

  

Furthermore, certain professional sectors, such as education or governmental institutions, may be more sensitive to perceived ideological alignment. Despite the potential for discriminatory selection, there remains a shortage of empirical studies that systematically investigate algorithmic bias toward ideological content in resumes, especially across sectors.

  
  

## *Sectorial and Intersectional Variations*

Sectoral differences in hiring practices influence how bias manifests in algorithmic models. For instance, the language valued in a resume for a tech role may diverge from that for a healthcare position. Few studies have conducted sector-specific audits, but those that do (e.g. Kim et al., 2020; Veldanda et al., 2023) reveal that certain sectors tolerate greater algorithmic opacity, are more prone to embedding proxies for identity attributes and subsequently exhibit greater bias. 

  

Moreover, current literature presents a shortage of intersectional analyses. Most studies isolate one demographic variable despite the fact that real-world identities intersect in complex ways. For instance, a Black woman who signals progressive political views, through her work or volunteering experience, may be doubly disadvantaged by algorithmic filters than white, male, apolitical candidates. The theoretical implications of intersectionality, as articulated by Crenshaw (1991), have yet to be thoroughly incorporated into algorithmic auditing practices.

Back to [Previous Page](Introduction.md)
Go to [Next Page](framework.md)
