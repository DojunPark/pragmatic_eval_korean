# Pragmatic Competence Evaluation of Large Language Models for the Korean Language

This repository contains resources from our study, [Pragmatic Competence Evaluation of Large Language Models for the Korean Language](https://arxiv.org/abs/2403.12675), which details the assessment of context-dependent expressions using Gricean conversational maxims.

## Dataset Description
The dataset is composed of 120 test units designed to assess the ability of LLMs to interpret conversational implicature based on Grice's maxims:

* **Quantity** – Provide as much information as required, no more.
* **Quality** – Only provide information that is true.
* **Relation** – Be relevant to the conversation.
* **Manner** – Be clear, brief, and orderly.

Each test unit involves a contextual scenario and a statement where the LLM must infer the implied meaning from a choice of answers or provide an open-ended response.

## Data Structure
Each data point in `korean_pragmatics_testset.csv` is structured as follows:

* **ID**: A unique identifier for each test case.
* **Type of Maxim**: The conversational maxim being tested (quantity, quality, relation, manner).
* **Context**: The scenario or dialogue in which the key utterance occurs.
* **Statement**: The key utterance whose meaning must be inferred.
* **MCQ**: A multiple-choice question asking for the most appropriate interpretation of the statement.
* **OEQ**: An open-ended question asking for a narrative interpretation of the statement.
* **MCQ Answer**: The correct answer option for the multiple-choice question.
* **MCQ Details**: Additional details about the multiple-choice answers, including wrong and literal interpretations.
* **OEQ Answer**: The correct narrative answer for the open-ended question.

## Usage
This dataset is intended for researchers and practitioners interested in evaluating and improving the pragmatic inference abilities of language models, particularly those focused on Korean. It is suitable for both automated evaluation (through MCQs) and human assessment (through OEQs).


## How to Use
1. **Multiple-Choice Evaluation**: Use the MCQ column to assess how well models select the correct pragmatic interpretation from a set of options.
2. **Open-Ended Evaluation**: Use the OEQ column for a more in-depth analysis of the model's generative capabilities, requiring human experts to rate the quality of the generated answers.


## Citation

If you utilize the dataset in your research, please cite our paper:

```bibtex
@article{park2024korean_pragmatic,
  title={Pragmatic Competence Evaluation of Large Language Models for the Korean Language,
  author={Park, Dojun and Lee, Jiwoo and Jeong, Hyeyun and Park, Seohyun and Lee, Sungeun},
  journal={arXiv preprint arXiv:2403.12675},
  year={2024},
  url={https://arxiv.org/abs/2403.12675}
}
