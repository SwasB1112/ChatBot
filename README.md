# Chatbot for Question Answering on Delegation of Power (DOP) Document

## Project Overview

This project involves the development of a chatbot using a large language model (LLM) to facilitate question answering on the Delegation of Power (DOP) Document for the North Eastern Electric Power Corporation Limited (NEEPCO). The chatbot aims to enhance information retrieval efficiency and accessibility within corporate operations.

## Table of Contents

1. [Abstract](#abstract)
2. [Introduction](#introduction)
3. [Literature Survey](#literature-survey)
4. [Methodology](#methodology)
5. [Results](#results)
6. [References](#references)
7. [Submitted By](#submitted-by)

## Abstract

This project explores the application of a chatbot using advanced natural language understanding capabilities of state-of-the-art LLMs, such as Meta-LLaMA-2, for question answering on the DOP Document. The chatbot is designed to provide accurate, contextually relevant, and timely responses, improving the efficiency and accessibility of information retrieval in corporate settings.

## Introduction

Efficient and accurate information retrieval is crucial for maintaining smooth and effective operations within large organizations like NEEPCO. The DOP document outlines various levels of authority and responsibilities, providing guidelines for decision-making and operational procedures. The chatbot leverages LLMs to interact conversationally with users and provide accurate responses, enhancing operational efficiency and decision-making.

## Literature Survey

The literature survey reviews key studies and advancements in the application of LLM-based chatbots for question answering, focusing on organizational use cases such as NEEPCO's DOP. It covers:

- Machine Learning in NLP
- Chatbots and Large Language Models
- Information Retrieval in Organizational Contexts

## Methodology

### Data Collection and Preparation

Data was extracted from the DOP, arranging it into meaningful context paragraphs and preparing questions and answers in the format of “CoQA” and “SQuAD_v2.0”.

### Model Selection and Training

Models such as “Google-BERT”, “T5”, “Google-FLAN-T5", and “Meta-LLaMA-2" were trained and evaluated. Meta-LLaMA-2 was selected for answer generation and Sentence-Transformers for encoding, making a Hybrid Model.

### Chatbot Development

A user-friendly chatbot integrated with LLM models was developed using the Rasa Framework, supporting functionalities like continuous questioning for the same context.

### User-Friendly Web GUI

A web GUI for easy interaction between the chatbot and users was developed using the Django and Flask frameworks in Python.

## Results

The models were trained on a dataset of 5 MB with a batch size of 16 and 10 epochs. The most efficient model in terms of accuracy was Meta-LLaMA-2, though its size makes it unsuitable for local hosting due to hardware constraints.

| Model          | Parameters  | Size after Training | Accuracy | Response Time (ms) |
| -------------- | ----------- | ------------------- | -------- | ------------------ |
| BERT           | 110 million | ~420 MB             | 80%      | 120                |
| T5             | 220 million | ~800 MB             | 87%      | 150                |
| FLAN-T5        | 220 million | ~950 MB             | 88%      | 160                |
| Meta-LLaMA-2   | 7 billion   | ~28 GB              | 92%      | 200                |

### Future Work

Future work includes improving the accuracy and performance of the T5 model through fine-tuning and developing algorithms to parse context more efficiently.

## References

1. S. Reddy, D. Chen, and C. D. Manning, "CoQA: A Conversational Question Answering Challenge," 2018. [arXiv:1808.07042](https://arxiv.org/abs/1808.07042)
2. P. Rajpurkar, J. Jia, and P. Liang, "Know What You Don’t Know: Unanswerable Questions for SQuAD," 2018. [arXiv:1806.03822](https://arxiv.org/abs/1806.03822)
3. J. Devlin, M. Chang, K. Lee, and K. Toutanova, "BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding," 2018. [arXiv:1810.04805](https://arxiv.org/abs/1810.04805)
4. C. Raffel et al., "Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer," 2019. [arXiv:1910.10683](https://arxiv.org/abs/1910.10683)
5. Meta AI, "LLaMA: Open and Efficient Foundation Language Models," 2023. [arXiv:2302.13971](https://arxiv.org/abs/2302.13971)
6. A. Radford et al., "Language Models are Unsupervised Multitask Learners," OpenAI, 2019. GPT-2 paper
7. T. B. Brown et al., "Language Models are Few-Shot Learners," OpenAI, 2020. GPT-3 paper
8. D. Jurafsky and J. H. Martin

## Submitted By
Swastayan Borah
Kalpojyoti Koch
Deep Baro
Theophilas Chapar
