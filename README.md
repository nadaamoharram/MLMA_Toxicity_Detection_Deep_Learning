# MLMA_Toxicity_Detection_Deep_Learning

Detecting harmful content is critical for user safety and moderation on social media platforms. Online hate speech can spiral into real violence, as when unmoderated hate-speech on Facebook precipitated genocide in Myanmar. A robust hate speech detection model would be able to help analyze social behavior—for example, do women in fitness on instagram receive more hate comments than men? Most systems are optimized for English, (as Facebook’s was in Myanmar,) leaving other low resource or morphological complex languages like Arabic less protected. We propose a Multilingual Sentiment (Toxicity) Detection system to classify hostility sentiment, directness, and hate-targeted groups in social media comments across multiple languages (English, Arabic and French). The goal is to fine-tune existing NLP models to improve upon the performance achieved by existing efforts. Current hate speech detection models using BERT variants like mBERT and XLM-RoBERTa are only fine-tuned for modeling binary hate speech detection, or hate speech topics with limited classes. We extend this research to fine-tune a multilingual model to predict many classes and labels. Our multi-class, multi-label classification task includes a mix of multi-class outputs where each row has exactly one label (hate speech, directness, target, group), and multi-label outputs where each row has one or more labels (sentiment). Addressing a larger multi-class hate-speech classification problem is a step towards building more inclusive, global NLP systems.

Group Members: Bella Davies, Nadaa Moharram, Ishani Cheshire

## Folder Structure:
- /Data contains Raw Data files and combined dataset splits.
- /EDA contains code to combine datasets, clean datasets, and conduct exploratory data analysis on the training dataset.
- /Modeling contains code for the baseline and fine-tuned deep learning models.

## Contributions:
( To be Updated )