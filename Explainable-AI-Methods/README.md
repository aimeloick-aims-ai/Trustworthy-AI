---
noteId: "df6c83b0bb4e11f1877d9711971aaae6"
tags: []

---

# XAI Methods

My experiments with surrogate models, loan counterfactuals, LIME, Shapley values, SHAP, PDP, ALE, LOFO, SAGE, TCAV, transformer explanations, and CNN attributions.

The notebooks listed below contain my code, explanations, and saved outputs from `aimeloick_XAI_assignment_1.ipynb` and `aimeloick_XAI_assignment_2.ipynb`. Both originals remain unchanged in the repository root. No new method implementations or results were added. Assignment headings were renamed by topic. Existing helper modules, data, and model files remain available.

## Source mapping

Source numbers refer to the two original notebooks. Cell numbers are one-based, including Markdown cells. Shared setup is copied where needed: SAGE includes the earlier model setup, transformer TCAV includes concept-data setup, and CNN includes device selection.

| Notebook | Source | Source cells |
| --- | --- | --- |
| [interpretations.ipynb](interpretations.ipynb) | 1 | 1, 4, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 28, 29, 30, 31, 33 |
| [Counterfactuals/Counterfactuals_multiobj.ipynb](Counterfactuals/Counterfactuals_multiobj.ipynb) | 1 | 1, 2, 3, 5, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53 |
| [LIME/titanic_LIME.ipynb](LIME/titanic_LIME.ipynb) | 1 | 7, 57, 58, 59, 60, 61, 62, 63, 64, 65, 66, 67, 68 |
| [LIME/image_LIME.ipynb](LIME/image_LIME.ipynb) | 1 | 6, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99, 100 |
| [Shapley_SHAP/Shapley.ipynb](Shapley_SHAP/Shapley.ipynb) | 1 | 8, 102, 103, 104, 105, 106, 107, 108, 109, 110, 111, 112, 113, 114, 115, 116, 117, 118, 119, 120, 121, 122, 123, 124, 125, 126 |
| [Shapley_SHAP/SHAP.ipynb](Shapley_SHAP/SHAP.ipynb) | 1 | 9, 127, 128, 129, 130, 131, 132, 133, 135, 136, 137, 138, 139, 140, 141, 142, 143, 144, 145, 146, 147, 148, 149, 150, 151 |
| [PDP_ALE/partial_dependence_plot.ipynb](PDP_ALE/partial_dependence_plot.ipynb) | 2 | 1, 2, 3, 4, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 46, 47, 48, 49, 50, 51, 52, 53, 54 |
| [PDP_ALE/accumulated_local_effects.ipynb](PDP_ALE/accumulated_local_effects.ipynb) | 2 | 55, 56, 57, 58, 59, 60, 61, 62, 64, 65, 66, 67, 68, 69, 70, 71 |
| [LOFO_SAGE/LOFO.ipynb](LOFO_SAGE/LOFO.ipynb) | 2 | 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 91, 92 |
| [LOFO_SAGE/SAGE.ipynb](LOFO_SAGE/SAGE.ipynb) | 2 | 73, 74, 75, 76, 77, 78, 79, 80, 93, 95, 96, 97, 98, 99, 100, 101, 102, 103, 104, 105, 106, 107, 108, 109, 110, 111, 112, 113, 114, 115, 116, 117, 118, 119, 120, 121, 122, 123, 125, 126, 127, 128, 129, 130, 131, 132, 133, 134, 135 |
| [CAV/TCAV-resnet.ipynb](CAV/TCAV-resnet.ipynb) | 2 | 137, 138, 139, 140, 141, 142, 143, 144, 145, 146, 147, 148, 149, 150, 151, 152, 153, 154, 155, 156, 157, 158, 159, 160, 161, 162, 163, 164, 165, 166, 167, 168, 169, 170, 171, 172, 173, 174, 175, 176, 177, 178, 179, 180, 181, 182, 183, 184, 185, 186, 187, 188, 189, 190, 191, 192, 193, 194, 195, 196, 197, 198, 199, 200, 201, 202 |
| [Transformers/Transformers.ipynb](Transformers/Transformers.ipynb) | 2 | 140, 141, 142, 143, 144, 145, 146, 147, 148, 149, 150, 151, 152, 153, 203, 204, 205, 206, 207, 208, 209, 210, 211, 212, 213, 214, 215, 216, 217, 218, 219, 220, 221, 222, 223, 224, 225, 226, 227, 228, 229, 230, 231, 232, 233, 234 |
| [CNN/cnn_attributions.ipynb](CNN/cnn_attributions.ipynb) | 2 | 142, 235, 236, 237, 238, 239, 240, 241, 242, 243, 244, 245, 246, 247, 248, 249, 250, 251, 252, 253, 254, 255, 256, 257, 258 |

## Content not transferred

- Source 1, cell 27: Empty cell.
- Source 1, cell 32: Empty cell.
- Source 1, cell 54: Alibi comparison heading; no implementation was submitted.
- Source 1, cell 55: Empty cell.
- Source 1, cell 56: Empty cell.
- Source 1, cell 101: Empty cell.
- Source 1, cell 134: Empty cell.
- Source 2, cell 5: Empty cell.
- Source 2, cell 45: Empty cell.
- Source 2, cell 63: Empty cell.
- Source 2, cell 94: Empty cell.
- Source 2, cell 124: Empty cell.
- Source 2, cell 136: Exercise prompt; the preceding analysis and results are retained.

All nonempty code cells from both submissions were transferred, including duplicate experiments and incomplete code. No missing implementations were invented.

## Original execution limitations

Code and saved outputs were preserved, not rerun. Several cells require Google Colab, Google Drive paths, downloads, or authentication. Paths remain as submitted. The Shapley section calls `make_cf_dict`, `characteristic_function_r2`, and `sort_shapley_values` without defining them in the submission. Other original implementation issues remain. These notebooks are not verified to run from a fresh local kernel; saved outputs belong to the original runs.

## Remaining template files

Three unmatched template notebooks remain unchanged pending removal approval: `import_tests.ipynb`, `Counterfactuals/Counterfactuals_titanic.ipynb`, and `CNN/cnn_interpretability.ipynb`. They are not part of the source mapping above. The submitted counterfactual work uses loan data; the submitted CNN work is in `CNN/cnn_attributions.ipynb`.
