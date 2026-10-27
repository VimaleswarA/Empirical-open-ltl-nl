# A Systematic Empirical Study of Open-Source Large Language Models for Linear Temporal Logic to Natural Language Translation

This repository contains the appendix and codes for the paper: "A Systematic Empirical Study of Open-Source Large Language Models for Linear Temporal Logic to Natural Language Translation".

**Authors:** Vimaleswar A (IISER Bhopal), Dr. Arpit Sharma (IISER Bhopal)

**Abstract:**
Linear Temporal Logic (LTL) is widely used to formalize software requirements in a mathematically precise form, enabling the verification of system properties. However, interpreting LTL formulas requires familiarity with formal notation, which can hinder understanding and validation of formal specifications, particularly among stakeholders without expertise in formal methods. Large language models (LLMs) offer a way to make formal specifications more accessible by translating them into natural language (NL). Existing studies provide limited empirical evidence on the performance of open-source LLMs in generating NL descriptions from LTL specifications. To address this gap, we conduct an empirical study comprising two stages. First, 40 open-source models are examined to determine whether they can produce meaningful descriptions of LTL formulas. Subsequently, 16 models are subjected to a detailed evaluation using 7 prompting techniques and 80 LTL formulas collected from four datasets. Five evaluation metrics are employed to examine lexical similarity, syntactic correspondence, and semantic preservation. The results show that model rankings vary across evaluation metrics and that prompting techniques influence translation quality. Moreover, several Small and Medium models achieve competitive results, suggesting that LTL to NL translation performance depends on factors beyond model size. We further assess 400 generated NL descriptions through independent judgments from three domain experts, obtaining an overall correctness rate of 88.5\%. Inter-annotator agreement is assessed using Cohen's kappa and Fleiss' kappa, and incorrect translations are analyzed to identify four major error categories. This study combines quantitative evaluation with expert assessment to compare models and identify challenges in preserving LTL semantics during translation across diverse specifications.

The repository contains the details of the models, prompts, datasets, and code used in the paper.

---
## Repository Structure

- In this repository, you'll find:

  - `Appendix.pdf` → Supplementary material containing the list of evaluated open-source LLMs, Phase-1 screening results, all 80 LTL formulas used in Phase-2 from the four datasets, prompt templates (P1-P7), and additional experimental details.
  - `Automatic_Explanation_Evaluation.ipynb` → Jupyter notebook containing evaluation script for explanation evaluation (BARTScore).
  - `Reference_Explanations.pdf` → Contains the explanations generated using ChatGPT that serve as the reference explanations.
  - `Automatic_Natural_Language_Evaluation.ipynb` → Jupyter notebook containing evaluation scripts for natural language evaluation (BLEU, ROUGE, METEOR, SBERT).
