# Emotion-Cause Pair Extraction in Conversations

## Project Overview

This repository contains the final report and code for the project **"A Comparison Analysis of Emotion-Cause Pair Extraction in Conversations"** conducted as part of the CS685 course at UMass Amherst. The project aims to develop and analyze methods for extracting emotion-cause pairs (ECPE) in conversations, which involves identifying emotions in textual data and uncovering their underlying causes.

## Problem Statement

Emotion-Cause Pair Extraction (ECPE) is a crucial task in Natural Language Processing (NLP), particularly for understanding and analyzing conversational data. The project focuses on Subtask 1: Textual Emotion-Cause Pair Extraction in Conversations from SemEval-2024 Task 3. The goal is to identify both emotions and their causes from text-based conversations, providing deeper insights into emotional dynamics within dialogues.

## Motivations

- **Enhanced Emotional Intelligence in AI**: Improving AI's ability to understand and respond to human emotions.
- **Applications in Various Domains**: From social media analysis to mental health services and customer service.
- **Challenges of Conversational Data**: Addressing the complexities of conversational dynamics and implicit causes.
- **Advancing NLP Understanding and Learning**: Pushing the boundaries of emotion analysis in NLP tasks.

## Objectives

- Develop advanced models for ECPE using state-of-the-art NLP models (BERT, RoBERTa, DeBERTa, OPT 350M).
- Conduct a comprehensive evaluation using metrics like accuracy, precision, recall, and F1-score.
- Perform a comparative study of different approaches to ECPE.
- Explore an end-to-end solution using BiLSTM networks.

## Dataset

The project uses the Emotion-Cause-in-Friends (ECF) dataset, which contains rich emotional content and diverse conversational contexts from the sitcom "Friends." The dataset includes annotated conversations, utterances with emotions, and emotion-cause pairs.

## Approaches

### 1. End-to-End Architecture (E2E PExtE)

- **Components**: Word-Level Encoder (BiLSTM + Attention), Clause-Level Encoder (BiLSTM), Auxiliary Tasks (Emotion and Cause Detection), Pair Predictor (Fully Connected Network).
- **Motivation**: Leveraging hierarchical structure to enhance learning suitable clause representations.

### 2. EmoBERTa-Based Approach

- **Components**: EmoBERTa model for emotion recognition, Transformer Encoder for cause identification, Mapping logic for emotion-cause pairs, DeBERTa model for enhanced pair extraction.
- **Motivation**: Using advanced transformer architecture for accurate emotion classification and cause identification.

### 3. Prompt Tuning-Based Approach

- **Components**: Pre-trained language model (facebook/opt-350m), Formatting prompts for conversational context, Fine-tuning with custom prompts.
- **Motivation**: Leveraging pre-trained models for specific sequence classification tasks.

## Results and Comparison

The performance of different approaches was evaluated using precision, recall, and F1-score for emotion-cause pair extraction, emotion identification, and cause identification.

## Contributions

- **Prudhvi Nikku**: Data collection, preprocessing, and implementation of DeBERTa-EmoBERTa based architecture.
- **Mani Kishan Ghantasala**: E2E PExtE model development and prompt tuning.
- **Srimathi Mahalingam**: Prompt-based tuning and report compilation.
- **Muskan Dhar**: Model analysis, refinement, and baseline models.
- **Satya Sriram Potluri**: Prompt tuning and model experimentation.

## Future Work

- Explore multimodal data (text, video, audio) for a more comprehensive understanding of conversational context.
- Leverage advanced language models (GPT-3.5, Mistral, LLama) with techniques like Flash Attention and DeepSpeed to improve ECPE performance.

## Conclusion

This project demonstrates the potential of advanced NLP models for Emotion-Cause Pair Extraction in conversations, contributing to the development of AI systems with enhanced emotional intelligence.

## References

- [Busso et al., 2008]
- [Chen et al., 2022]
- [Ding et al., 2019]
- [Gao et al., 2015]
- [Ghazi et al., 2015]
- [Gui et al., 2017]
- [Inoue et al., 2023]
- [Khunteta and Singh, 2021]
- [Lee et al., 2010]
- [Li and Xu, 2014]
- [Li et al., 2018]

## Contact

For any queries, please contact:

- Prudhvi Nikku - snikku@umass.edu
- Srimathi Mahalingam - srimathimaha@umass.edu
- Mani Kishan Ghantasala - mghantasala@umass.edu
- Satya Sriram Potluri - spotluri@umass.edu
- Muskan Dhar - mdhar@umass.edu
