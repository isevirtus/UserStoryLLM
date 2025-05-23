# Towards Automating User Story Classification with LLMs Using a Reuse-Oriented Taxonomy

<p align="center">
  <b>Evaluating the Capability of Prompted LLMs Classify User Stories with a Taxonomy</b><br/>
  <i>Companion Artifact for SBES 2025 Submission</i><br/>
</p>

---

## About

This repository contains the dataset, results, and prompting instructions related to the article submitted to SBES 2025, titled:

> **Towards Automating User Story Classification with LLMs Using a Reuse-Oriented Taxonomy**

---

 ## 🎯 Goals

This repository aims to:

- Provide open access to the **dataset** used in the study.
- Share the **LLM classification results** and comparative metrics.
- Enable **reproducibility** of the prompt engineering process used to classify user stories.
- Support further research in **software reuse**, **user story analysis**, and **LLM evaluation**.

---

## 🗂️ Project Structure

| Folder/File     | Description                                                                                                 |
| ----------------| ----------------------------------------------------------------------------------------------------------- |
| 📁 <b>data/</b> | Contains the dataset with processed user stories and annotations.<br/>File: <code>dados_dos_projetos.xlsx</code> |
| 📁 <b>prompts/</b> | Contains the Jupyter notebook used for LLM inference via OpenAI API.<br/>File: <code>prompt_classificador.md</code><br/>File:<code>prompt_validador.md</code> |
| 📁 <b>results/</b> | Summary Report: statistical overview including agreement rate, coverage, and divergence examples.<br/>Main file: <code>classificacao_base_inicial.csv</code> |
| 📄 <b>README.md</b> | This file. Provides description, usage instructions, and credits. |

---

## 🚀 How to Use

To reproduce the LLM-based classification:

1. Open [ChatGPT](https://chat.openai.com) with access to **GPT-4o**.
2. Navigate to the `prompts/` directory and manually paste the prompt content into the chat interface.
   - Follow the two-step prompting protocol as described in the folder.
3. Input the user story text (from `data/`) in the appropriate step.
4. Save or compare the model's output with the labels found in `results/`.

> ⚠️ **Note**: The prompts were designed for use with **ChatGPT 4o**, and manual intervention is required to execute each step.
