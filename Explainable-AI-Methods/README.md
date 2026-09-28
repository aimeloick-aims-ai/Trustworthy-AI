# Explainable AI Methods

A practical collection of notebooks exploring **how machine learning models make predictions**.

The repository covers explainability for **tabular data, images, and transformers**, from local feature attribution to concept-based explanations.

## Methods

| Method | Focus | Notebook |
| --- | --- | --- |
| **Surrogate Models** | Approximate black-box models with interpretable models and study fidelity. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/interpretations.ipynb) |
| **Counterfactuals** | Find minimal changes that would alter a model prediction. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/Counterfactuals/Counterfactuals_multiobj.ipynb) |
| **LIME — Tabular** | Explain individual predictions with a simple local model. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/LIME/titanic_LIME.ipynb) |
| **LIME — Images** | Highlight image regions supporting or opposing a prediction. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/LIME/image_LIME.ipynb) |
| **Shapley Values** | Build intuition for attribution through marginal contributions. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/Shapley_SHAP/Shapley.ipynb) |
| **SHAP** | Explain local and global feature contributions. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/Shapley_SHAP/SHAP.ipynb) |
| **PDP** | Study average prediction changes when features vary. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/PDP_ALE/partial_dependence_plot.ipynb) |
| **ALE** | Measure local feature effects across the observed distribution. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/PDP_ALE/accumulated_local_effects.ipynb) |
| **LOFO** | Measure performance loss after removing a feature. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/LOFO_SAGE/LOFO.ipynb) |
| **SAGE** | Estimate global feature importance through predictive loss reduction. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/LOFO_SAGE/SAGE.ipynb) |
| **CAV & TCAV** | Test model sensitivity to human-defined concepts. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/CAV/TCAV-resnet.ipynb) |
| **CNN Attributions** | Compare gradients, CAM, Grad-CAM, and Integrated Gradients. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/CNN/cnn_attributions.ipynb) |
| **Transformer Explanations** | Explore attention, Grad-SAM, SHAP, and TCAV for transformers. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/Transformers/Transformers.ipynb) |

## Suggested path

**Surrogates → LIME → SHAP → PDP/ALE → LOFO/SAGE → CNN Attribution → TCAV → Transformers**

## Why this repository?

Different XAI methods answer different questions:

- **What features contributed?** → SHAP, LIME
- **What would change the decision?** → Counterfactuals
- **How does a feature affect predictions?** → PDP, ALE
- **What is globally important?** → LOFO, SAGE
- **Where does a CNN look?** → Grad-CAM
- **Does the model rely on a concept?** → TCAV

The goal is to understand not just **how to generate explanations**, but **what those explanations actually mean**.
