# Week 02 Log — SVM & ANN

## What I worked on
- Built and evaluated SVM classifiers (linear vs kernel) and tuned RBF hyperparameters.
- Built an ANN (MLP) classifier and compared activation functions.

## Dataset & preprocessing
- Dataset: Breast Cancer Wisconsin (sklearn built-in), binary classification
- Split: 80/20 (stratified), random_state=42
- Scaling: StandardScaler

## Experiments & results
### SVM
- Kernels tested: linear, RBF, polynomial
- Best tuned model: RBF(C=1, gamma=0.01)
- Best SVM accuracy: ≈ 0.982 (112/114)
- Outputs saved to `images/`:
  - week02_svm_kernel_comparison.png
  - week02_svm_confusion_matrix.png
  - week02_svm_rbf_tuning_table.csv

### ANN (MLP)
- Activations tested: logistic, tanh, relu
- Result: all activations achieved the same accuracy in this run (≈ 0.956)
- Best activation (tie): logistic (selected as first in sorted order)
- Best ANN accuracy: ≈ 0.956 (109/114)
- Outputs saved to `images/`:
  - week02_ann_activation_comparison.png
  - week02_ann_confusion_matrix.png

## Issues / fixes
- Ensured the notebook kernel used the project `.venv` environment so required packages were available.

## Next steps
- Use cross-validation for more robust model selection.
- Experiment with different network sizes/regularisation for ANN.