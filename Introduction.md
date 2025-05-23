---
layout: page
title: Introduction
tags: [AI Biases, Introduction]

---

In 2018, Amazon abandoned an experimental Artificial Intelligence (AI) hiring tool after discovering it systematically showed bias against women by downgrading CVs containing the word “women’s” and penalized graduates from all-women’s universities (Dastin, 2018). Trained on historical hiring data of the company, the system had inadvertently learned to prefer masculine career paths and language, thus embedding past discrimination into its scoring model. This controversy became illustrative of a larger concern: as AI becomes integrated in HR and management practices, it risks reproducing or amplifying existing inequalities under the guise of objectivity (Raghavan et al., 2020).  

Algorithmic tools can be employed across every stage of the hiring process, from sourcing candidates, screening, to interviewing and even final selection (Raghavan et al., 2020, p. 470). Resume matching algorithms generally operate at the screening stage, determining which candidates from the sourced pool are suitable to proceed to human review. These systems typically use natural language processing and machine learning (Sharma et al., 2021) to compare candidates CVs against job descriptions, screening applicants based on experience, inferred relevance and compatibility. Despite being presented as neutral evaluators that save time and costs (Kuncel, 2014), algorithms are not impartial: they reflect the biases embedded in their training data and design (Chander, 2016;‌ Köchling & Wehner, 2020). Concerns have emerged around how such automated systems approach resumes that reflect variations in gender, ethnicity or ideological expression, attributes that are often implicitly embedded in resume content through names, universities or extracurriculars (Bertrand & Mullainathan, 2004; Rivera, 2011).  

While much of the academic debate around algorithmic bias has focused on conceptual and normative critiques, addressing ethical risks, legal accountability and design principles, a relatively limited number of studies have empirically examined how such biases manifest in practice (Kordzadeh & Ghasemaghaei, 2021). This trend is shifting with the increasingly widespread availability of LLMs like ChatGPT, Gemini and Mistral, prompting a rise in empirical research on AI behavior (Wen et al., 2025; Iso et al., 2025). However, due to their proprietary nature, few studies directly assess actual hiring algorithms, instead researchers often resort to proxy models to simulate their effects. This project follows that strategy, using an open-source resume matching algorithm to investigate how identity-linked attributes influence candidate’s job compatibility. 

Therefore, this study aims to decode the implicit biases of one representative hiring model in depth, revealing how it responds to indicators of gender, ethnicity and ideology across different work industries. Specifically, we aim to address the following question: ***To what extent do resume matching algorithms exhibit bias–based on gender, ethnicity, and ideological expressions–across different professional sectors?***

By simulating application scenarios with controlled variations in resume content, this research contributes to the growing field of empirical AI ethics. It offers both theoretical insights into how bias manifests in automated hiring processes, and practical implications for those designing and regulating AI tools used in HR. As algorithmic decision-making increasingly dictates access to job and economic opportunities, understanding the mechanics of bias is essential to shaping just and accountable hiring practices.

This study is structured as follows: the literature review and theoretical framework provide a theoretical foundation, discussing the existing documentation of biases in hiring processes and algorithms, as well as key concepts like algorithmic fairness and bias formation. The methodology then outlines the performed experimental correspondence testing design. The results section subsequently presents evidence of significant gender and ethnicity biases but limited ideological bias with important sectorial variations. Finally, the discussion and conclusion contextualize these findings and highlight the societal and research implications, emphasizing the need for ongoing scrutiny of AI hiring tools. 


<section style="display: flex; justify-content: center; margin: 40px 0;">
    <div style="margin-top: 20px; text-align: center;">
      <a href="https://pouvoirdasha.github.io/Decoding_Biases_in_Resume_Matcher/literature_review/" 
         style="
           display: inline-block;
           padding: 12px 24px;
           background-color: #2b2a2a;
           color: white;
           text-decoration: none;
           border-radius: 25px;
           font-size: 16px;
           font-weight: bold;
           transition: background-color 0.3s ease;
         "
         onmouseover="this.style.backgroundColor='#404040';"
         onmouseout="this.style.backgroundColor='#2b2a2a';">
        Read the rest of the paper →
      </a>
    </div>
</section>

