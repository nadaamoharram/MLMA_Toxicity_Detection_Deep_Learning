# Multi-Output Hate Speech Modeling: Fine-Tuning Multilingual Transformer Architectures with Multi-Task Hierarchical Models and LIME Explainable AI

Detecting harmful content is critical for user safety and moderation on social media platforms. Online hate speech can spiral into real violence, as when unmoderated hate-speech on Facebook precipitated genocide in Myanmar in 2022. A robust hate speech detection model would be able to help analyze social behavior—for example, do women in fitness on instagram receive more hate comments than men? Most systems are optimized for English, (as Facebook’s was in Myanmar,) leaving other low resource or morphological complex languages like Arabic less protected. We propose a Multilingual Sentiment (Toxicity) Detection system to classify hostility sentiment, directness, and hate-targeted groups in social media comments across multiple languages (English, Arabic and French). The goal is to fine-tune existing NLP models to improve upon the performance achieved by existing efforts. 

Current hate speech detection models using BERT variants like mBERT and XLM-RoBERTa are mostly fine-tuned for modeling binary hate speech detection, or hate speech topics with limited classes. We extend this research for a multi-class, multi-label classification task, which includes a mix of multi-class outputs where each observation has exactly one label (hate speech, directness, target, group), and multi-label outputs where each observation has one or more labels (sentiment). Our multi-class, multi-label classification model achieves test prediiction with an 85% F1 score, and includes a mix of multi-class outputs where each row has exactly one label (hate speech, directness, target, group), and multi-label outputs where each row has one or more labels (sentiment). For comparison the single label hate speech classification task in English achieved a 99.5 F1 score. Employing LIME explanations on test predictions enables increased transparency for model decision making for each label and language. Addressing a larger multi-class hate-speech classification problem is a step towards building more inclusive, global NLP systems.

**Group Members:** Bella Davies, Nadaa Moharram, Ishani Cheshire

Presentation Link: https://docs.google.com/presentation/d/1EcGKn1onkD6ttvpIeHXXl_ECrRhO9o4W5S_gfpIDWvE/edit?usp=sharing 

## Folder Structure:
- **/Data** contains Raw Data files and combined dataset splits (train, validation, test).
- **/EDA** contains code to combine datasets, clean datasets, and conduct exploratory data analysis on the training dataset.
- **/Modeling** contains code for the baseline, fine-tuned, and hierarchical deep learning models.
- **/Test_Predictions_and_LIME_Explanations** contains code for generating predictions on the test dataset, visualization confusion matrices and metrics overall and per language, and LIME explanations of the test predictions of each language.

## Contributions:
**Bella**
- Background: Siddiqui et al. (2024), Wong et al. (2024) 
- Data Collection: Ousidhoum et al. (2019) multilingual hate speech dataset (MLMA), English datasets Davidson et al. (2017), Sachdeva et al. (2022), Mandl et al. (2019) 
- Data Cleaning: Encode labels, clean text, combine datasets, drop duplicates, train/validation/test split 
- EDA on combined training dataset: Distributions of classes, text lengths, correlation & co-occurrence matrices, language differences
- Modeling: Modeling/Baseline_mBERT.ipynb, Modeling/FineTuning_mBERT.ipynb, Modeling/Hierarchical_mBERT_with_LIME_Explanations.ipynb
- Test Predictions and Metrics per Language, English/French/Arabic LIME Visualizations

**Nadaa**
- Introduction
- Background: Srikissoon and Marivate. (2023), Tonneau et al. (2024)
- Data Collection: Zaghouani et al. (2024) Arabic dataset, Tonneau et al. (2024) French dataset 
- Data Cleaning: Combine datasets, shuffle combined dataset
- Modeling: Baseline classification model, XLM-RoBERTa baseline and fine-tuning, hierarchical XLM-RoBERTa
- Lime Analysis: French/Arabic LIME Explanations

**Ishani**
- Background:  Jahan and Oussalah. (2023), Chung et al. (2020)
- EDA on MLMA dataset: Distributions of classes
- Modeling: RemBERT baseline and fine-tuning, RemBERT hierarchical model
- Methods (part of modeling), Results (~half)
- Conclusion (entire)
- Introduction
