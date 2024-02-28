# Evaluation of Large Language Models in Studying Genes and Pathways
   This is the official repository for our comprehensive study on leveraging 21 large language models (LLMs) for extracting gene regulatory relations and pathway knowledge from biomedical literature, detailed in our publication (doi: https://doi.org/10.1101/2024.01.21.576542 ).This repository shares insights on model selection and prompt design by highlighting the distinct performances of API-based versus open-source LLMs, with GPT-4 and Claude-Pro standing out for their effectiveness. These findings are pivotal for gene network analysis and pathway mapping, pushing forward the understanding of disease mechanisms and drug development.
# Quick Overview
    ![Fig-3](https://github.com/Muh-aza/LLM/blob/0ddfca9b03b9066559250c592690d34b7c432d32/image/Fig-3.png)
# Structured Prompts for determining using KEGG Pathway 
   
   ## Prompt 1: As a gene interaction analyst, your task is to determine the effect of {gene1} on {gene2} within the context of the KEGG Pathway Database, which represents our knowledge of molecular interaction, reaction, and relation networks for various biological processes. Provide a concise and definitive answer using one of the following terms: activation (gene1 activates gene2), inhibition (gene1 inhibits gene2), phosphorylation (gene1 phosphorylates gene2), or no information (no known relationship). Make sure your answer is definitive, composed of 'activation', 'inhibition', 'phosphorylation' or 'no information without further details or explanation.
## Prompt2: 
As a gene interaction specialist, your task is to determine the effect of {gene1} on {gene2} using the KEGG Pathway Database, a comprehensive resource for understanding molecular interaction and relation networks in cellular processes. Provide a clear and unambiguous answer using one of the following terms: 'activation' (gene1 activates gene2), 'inhibition' (gene1 inhibits gene2), 'phosphorylation' (gene1 phosphorylates gene2), or 'no information' if there is no known relationship. Ensure your answer is definitive and based on the current knowledge in the KEGG Pathway Database, composed of 'activation', 'inhibition’,’ phosphorylation', or 'no information' without further details or explanation.
## Prompt 3:
As a gene interaction analyst, you are tasked with determining the effect of {gene1} on {gene2} using the KEGG Pathway Database, a valuable resource for understanding molecular interaction networks in biological processes. Your answer should only include one of the following terms: 'activation' (gene1 activates gene2), 'inhibition' (gene1 inhibits gene2), or 'phosphorylation' (gene1 phosphorylates gene2). Make sure your answer is definitive, composed of 'activation', 'inhibition', 'phosphorylation' or 'no information without further details or explanation.
##Prompt4:
As a gene interaction analyst, your task is to determine the effect of {gene1} on {gene2} using the KEGG Pathway Database, a comprehensive resource for understanding molecular interaction networks involved in cellular processes. Provide a clear and unambiguous answer using one of the following terms: 'activation' (gene1 activates gene2), 'inhibition' (gene1 inhibits gene2), or 'phosphorylation' (gene1 phosphorylates gene2). Ensure your answer is definitive and composed of 'activation', 'inhibition', 'phosphorylation', or 'no information without further details or explanation.
## Prompt5: As a gene interaction specialist, your task is to determine the effect of {gene1} on {gene2} using the KEGG Pathway Database, a comprehensive resource for understanding molecular interaction networks in various biological processes. Provide a clear and unambiguous answer using one of the following terms: 'activation' (gene1 activates gene2), 'inhibition' (gene1 inhibits gene2), or 'phosphorylation' (gene1 phosphorylates gene2). Ensure your answer is based on the current knowledge in the KEGG Pathway Database and composed of 'activation', 'inhibition', or 'phosphorylation' without further details or explanation. Make sure your answer is definitive, composed of 'activation', 'inhibition', 'phosphorylation' or 'no information without further details or explanation
## Prompt6:
As a gene interaction specialist, your task is to determine the effect of {gene1} on {gene2} using the KEGG Pathway Database, a comprehensive resource for understanding molecular interaction and relation networks in cellular processes. Provide a clear and unambiguous answer using one of the following terms: 'activation' (gene1 activates gene2), 'inhibition' (gene1 inhibits gene2), 'phosphorylation' (gene1 phosphorylates gene2), or 'no information' if there is no known relationship. Ensure your answer is definitive and composed of 'activation', 'inhibition', 'phosphorylation', or 'no information without further details or explanation.
## Prompt7:Final Prompt :  As a computational biologist, determine what is the relation between {gene1} and {gene2} in KEGG Pathway Database. KEGG pathways are collections of pathway maps that represent our knowledge of the molecular interaction, reaction, and relation networks for various biological processes. To determine the relation between {gene1} and {gene2}, please provide a definitive answer without further thought. Describe the relation in one or two of the following words: activation, inhibition, phosphorylation. If you are replying with two relations, separate two relations using '...'. Please note that the directionality of the relationship is important. Make sure your answer is definitive, answer with relations only, without further details or explanations. Make sure your answer is definitive, composed of 'activation', 'inhibition', 'phosphorylation' or 'no information without further details or explanation. 


# Evaluations of Gene Regulatory Relations
# Evaluations of KEGG Pathway Recognition 
Adherens Junction complex
   false positive predictions and their performance in the Adherens junction
Tight junction 
      Predicted genes not present in Tight junction by the 21 LLMs.
Gap junction
 Predicted genes not present in the gap junction by the 21 LLMs.
Cellular Senescence Function
 Predicted genes not present in cellular senescence by the 21 LLMs.
Phagosome Function
Predicted genes not present in phagosome by the 21 LLMs
Proteoglycans in Cancer
Predicted genes not present in proteoglycans in cancer by the 21 LLMs.
Autoimmune Thyroid Disease
