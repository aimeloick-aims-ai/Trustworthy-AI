---
noteId: "df6c83b0bb4e11f1877d9711971aaae6"
tags: []

---

# Explainable AI Methods

My collection of experiments exploring how machine learning models make predictions. The notebooks cover explanations for tabular data, images, and text, with implementations, visualizations, and analysis.

## Methods and notebooks

| Method | What the notebook explores | Run notebook |
| --- | --- | --- |
| **Surrogate models** | Train interpretable decision trees and linear models to approximate an XGBoost model on California housing data, then compare fidelity and feature importance. | [Open in Colab](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/interpretations.ipynb) |
| **Counterfactual explanations** | Search for changes to a loan application that move its predicted outcome toward a desired target, balancing prediction fit, distance, sparsity, and proximity to observed data. | [Open in Colab](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/Counterfactuals/Counterfactuals_multiobj.ipynb) |
| **LIME for tabular data** | Explain individual Titanic predictions using a simple model fitted around each selected passenger; compare classification and regression explanations. | [Open in Colab](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/LIME/titanic_LIME.ipynb) |
| **LIME for images** | Perturb image regions and fit a local explanation to highlight superpixels that support or oppose a ResNet prediction. | [Open in Colab](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/LIME/image_LIME.ipynb) |
| **Shapley values** | Allocate a coalition value among its members by averaging marginal contributions; explore game examples and feature contributions using predictive fit and distance correlation. | [Open in Colab](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/Shapley_SHAP/Shapley.ipynb) |
| **SHAP** | Attribute predictions relative to a baseline using TreeExplainer for diabetes regression and DeepExplainer for an MNIST CNN; inspect individual explanations and summary plots. | [Open in Colab](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/Shapley_SHAP/SHAP.ipynb) |
| **Partial Dependence Plots (PDP)** | Average model predictions while varying selected features to show their overall relationship with the output; explore loan features, plotting ranges, and two-feature surfaces. | [Open in Colab](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/PDP_ALE/partial_dependence_plot.ipynb) |
| **Accumulated Local Effects (ALE)** | Accumulate local prediction differences within feature intervals to describe feature effects; compare linear and quantile bins with SHAP on California housing data. | [Open in Colab](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/PDP_ALE/accumulated_local_effects.ipynb) |
| **Leave-One-Feature-Out (LOFO)** | Measure the change in predictive performance after retraining without each feature; examine how correlated variables affect importance on bike demand data. | [Open in Colab](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/LOFO_SAGE/LOFO.ipynb) |
| **Shapley Additive Global Importance (SAGE)** | Estimate global feature importance through contributions to predictive loss reduction across feature subsets; compare SAGE, SHAP, and LOFO on bike demand data. | [Open in Colab](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/LOFO_SAGE/SAGE.ipynb) |
| **Concept Activation Vectors and TCAV** | Learn directions representing visual concepts in model activations and measure class-score sensitivity along those directions; investigate stripes, zebra predictions, and different ResNet layers. | [Open in Colab](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/CAV/TCAV-resnet.ipynb) |
| **Transformer explanations** | Explore BERT token importance with gradient-weighted attention (Grad-SAM) and SHAP, visualize attention heads, and apply TCAV to a vision transformer. | [Open in Colab](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/Transformers/Transformers.ipynb) |
| **CNN attributions** | Inspect input gradients, gradient times input, CAM, Grad-CAM, and Integrated Gradients on ResNet; compare smoothing, convolutional layers, and attribution baselines. | [Open in Colab](https://colab.research.google.com/github/aimeloick-aims-ai/Trustworthy-AI/blob/main/Explainable-AI-Methods/CNN/cnn_attributions.ipynb) |

## Using the notebooks

Select **Open in Colab** to open a notebook from this repository. Install the dependencies imported by that notebook and make its required data and helper modules available in the runtime. Opening a notebook in Colab does not copy the rest of the repository into the runtime.

Some notebooks use Google Drive paths, external datasets, or pretrained models. Adapt the paths to your environment and follow any dataset access requirements. GPU acceleration can help with the image and transformer experiments.

## Project files

- `data/`: included tabular datasets and example images.
- Topic folders: notebooks and supporting Python modules or model files.
- `aimeloick_XAI_assignment_1.ipynb` and `aimeloick_XAI_assignment_2.ipynb`: original notebooks containing the experiments organized here.

## Current limitations

Saved outputs come from the original runs; the reorganized notebooks have not been verified from a fresh runtime. The Shapley notebook references `make_cf_dict`, `characteristic_function_r2`, and `sort_shapley_values` without their definitions. Existing incomplete experiments and environment assumptions remain in the code.

All nonempty code cells from the two original notebooks were retained. Empty cells, an Alibi comparison heading with no implementation, and an exercise-only prompt were omitted. Additional original template notebooks remain in the folder but are not included in the method guide above.
