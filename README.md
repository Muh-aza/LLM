# Evaluation of Large Language Models in Studying Genes and Pathways
   This is the official repository for our comprehensive study on leveraging 21 large language models (LLMs) for extracting gene regulatory relations and pathway knowledge from biomedical literature, detailed in our publication (doi: https://doi.org/10.1101/2024.01.21.576542 ).This repository shares insights on model selection and prompt design by highlighting the distinct performances of API-based versus open-source LLMs, with GPT-4 and Claude-Pro standing out for their effectiveness. These findings are pivotal for gene network analysis and pathway mapping, pushing forward the understanding of disease mechanisms and drug development.
# Quick Overview
![alt Fig-3](https://raw.githubusercontent.com/Muh-aza/LLM/main/image/Fig-3.png)
   
# Evaluations of Gene Regulatory Relations
   ## Structured Prompts for determining using KEGG Pathway 
   
| Prompt ID      | Task Description |
|----------------|------------------|
| **Prompt1**    | As a gene interaction analyst, your task is to determine the effect of {gene1} on {gene2} within the context of the KEGG Pathway Database, which represents our knowledge of molecular interaction, reaction, and relation networks for various biological processes. Provide a concise and definitive answer using one of the following terms: activation (gene1 activates gene2), inhibition (gene1 inhibits gene2), phosphorylation (gene1 phosphorylates gene2), or no information (no known relationship). Make sure your answer is definitive, composed of 'activation', 'inhibition', 'phosphorylation' or 'no information without further details or explanation.'. |
| **Prompt2**    | As a gene interaction specialist, your task is to determine the effect of {gene1} on {gene2} using the KEGG Pathway Database, a comprehensive resource for understanding molecular interaction and relation networks in cellular processes. Provide a clear and unambiguous answer using one of the following terms: 'activation' (gene1 activates gene2), 'inhibition' (gene1 inhibits gene2), 'phosphorylation' (gene1 phosphorylates gene2), or 'no information' if there is no known relationship. Ensure your answer is definitive and based on the current knowledge in the KEGG Pathway Database, composed of 'activation', 'inhibition’,’ phosphorylation', or 'no information' without further details or explanation. |
| **Prompt3**    |As a gene interaction analyst, you are tasked with determining the effect of {gene1} on {gene2} using the KEGG Pathway Database, a valuable resource for understanding molecular interaction networks in biological processes. Your answer should only include one of the following terms: 'activation' (gene1 activates gene2), 'inhibition' (gene1 inhibits gene2), or 'phosphorylation' (gene1 phosphorylates gene2). Make sure your answer is definitive, composed of 'activation', 'inhibition', 'phosphorylation' or 'no information without further details or explanation. |
| **Prompt4**    | As a gene interaction analyst, your task is to determine the effect of {gene1} on {gene2} using the KEGG Pathway Database, a comprehensive resource for understanding molecular interaction networks involved in cellular processes. Provide a clear and unambiguous answer using one of the following terms: 'activation' (gene1 activates gene2), 'inhibition' (gene1 inhibits gene2), or 'phosphorylation' (gene1 phosphorylates gene2). Ensure your answer is definitive and composed of 'activation', 'inhibition', 'phosphorylation', or 'no information without further details or explanation. |
| **Prompt5**    | As a gene interaction specialist, your task is to determine the effect of {gene1} on {gene2} using the KEGG Pathway Database, a comprehensive resource for understanding molecular interaction networks in various biological processes. Provide a clear and unambiguous answer using one of the following terms: 'activation' (gene1 activates gene2), 'inhibition' (gene1 inhibits gene2), or 'phosphorylation' (gene1 phosphorylates gene2). Ensure your answer is based on the current knowledge in the KEGG Pathway Database and composed of 'activation', 'inhibition', or 'phosphorylation' without further details or explanation. Make sure your answer is definitive, composed of 'activation', 'inhibition', 'phosphorylation' or 'no information without further details or explanation. |
| **Prompt6**    | As a gene interaction specialist, your task is to determine the effect of {gene1} on {gene2} using the KEGG Pathway Database, a comprehensive resource for understanding molecular interaction and relation networks in cellular processes. Provide a clear and unambiguous answer using one of the following terms: 'activation' (gene1 activates gene2), 'inhibition' (gene1 inhibits gene2), 'phosphorylation' (gene1 phosphorylates gene2), or 'no information' if there is no known relationship. Ensure your answer is definitive and composed of 'activation', 'inhibition', 'phosphorylation', or 'no information without further details or explanation. |
| **Final Prompt** | As a computational biologist, determine what is the relation between {gene1} and {gene2} in KEGG Pathway Database. KEGG pathways are collections of pathway maps that represent our knowledge of the molecular interaction, reaction, and relation networks for various biological processes. To determine the relation between {gene1} and {gene2}, please provide a definitive answer without further thought. Describe the relation in one or two of the following words: activation, inhibition, phosphorylation. If you are replying with two relations, separate two relations using '...'. Please note that the directionality of the relationship is important. Make sure your answer is definitive, answer with relations only, without further details or explanations. Make sure your answer is definitive, composed of 'activation', 'inhibition', 'phosphorylation' or 'no information without further details or explanation. |



   # Evaluations of KEGG Pathway Recognition 
     ### Which genes are involved in "Adherens junction"?

  ![alt Fig-3](https://raw.githubusercontent.com/Muh-aza/LLM/main/image/Fig2-A.png)
   
 ## References

- Park, Gilchan, Yoon, Byung-Jun, Luo, Xihaier, López-Marrero, Vanessa, Johnstone, Patrick, Yoo, Shinjae, Alexander, Francis J. "Comparative Performance Evaluation of Large Language Models for Extracting Molecular Interactions and Pathway Knowledge." arXiv:2307.08813v1 [cs.CL] (2023).

- Xu, Dong. "ChatGPT opens a new door for bioinformatics." Quantitative Biology 11.2 (2023): 204-206. [https://doi.org/10.15302/J-QB-023-0328](https://doi.org/10.15302/J-QB-023-0328).

# Citation
If you find our work useful in your research, please consider citing:

```bibtex
@misc{azam2024comprehensive,
  title={A Comprehensive Evaluation of Large Language Models in Mining Gene Relations and Pathway Knowledge}, 
  author={Muhammad Azam and Yibo Chen and Micheal Olaolu Arowolo and Haowang Liu and Mihail Popescu and Dong Xu},
  year={2024},
  eprint={2024.01.21.576542},
  archivePrefix={bioRxiv},
  primaryClass={cs.LG}
}




