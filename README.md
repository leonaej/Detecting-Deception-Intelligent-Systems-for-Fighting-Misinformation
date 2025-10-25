# Detecting-Deception-Intelligent-Systems-for-Fighting-Misinformation
Hybrid Fake News Detection using Feature Fusion and Ensemble Learning, integrates transformer-based models (RoBERTa) with interpretable, rule-based reasoning. The system fuses linguistic, semantic, and logical features and employs an ensemble framework for improved accuracy, robustness, and explainability on datasets like LIAR and FakeNewsNet.


## Detecting Deception: Intelligent Systems for Fighting Misinformation

This repository contains the implementation and supplementary materials for the paper **_Detecting Deception: Intelligent Systems for Fighting Misinformation_**, 

## 🔹Project Overview
The rapid spread of misinformation online threatens public trust and information integrity. This project explores **hybrid fake news detection frameworks** that combine transformer-based models with interpretable reasoning techniques.

Three complementary methodologies were developed:
1. **Hybrid Feature Fusion and Ensemble Model** — *my primary contribution*  
2. Logic-Gated ML Overrides with Contradiction Detection  
3. Retrieval-Augmented Generation (RAG) with RoBERTa  

The paper describing all three approaches (`IDAI710_Project_FinalPaper.pdf`) is included in the root folder.

## 🔹My Contribution — Feature Fusion & Ensemble Learning
I developed the **first methodology**, which integrates multiple representations of the LIAR dataset to improve fake news classification accuracy:

- **Branch 1:** Transformer-based model using the raw statement  
- **Branch 2:** Metadata transformed into natural-language sentences and processed via another transformer  
- **Branch 3:** LLM-engineered semantic features (political tone, quotes, accusatory language, etc.) trained with XGBoost  
- **Final Ensemble:** Weighted fusion of the three models optimized through validation grid search  

This approach achieved **73.4% accuracy** and demonstrated that fusing linguistic, contextual, and engineered features improves robustness and interpretability.

## 🔹How to Run

Follow the detailed instructions in code/README.md to reproduce the results step-by-step — from feature engineering to ensemble prediction.

## 🔹Keywords

Fake News Detection · Feature Fusion · Ensemble Learning · Transformer Models · Explainable AI · LIAR Dataset
