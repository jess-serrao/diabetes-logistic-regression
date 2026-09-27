# Diabetes Prediction: Regularized Logistic Regression

This project evaluates logistic-regression models for predicting a binary diabetes outcome using clinical and demographic predictors. It compares custom and scikit-learn implementations of L1 (Lasso), L2 (Ridge), and Elastic Net regularization.

## Project Goals

- Build a custom logistic-regression model using gradient descent.
- Compare L1, L2, and Elastic Net regularization.
- Use a validation dataset to select the final model.
- Evaluate the selected model once on a held-out test dataset.
- Interpret model performance using accuracy, F1 score, and a confusion matrix.

## Data

The project uses the [Pima Indians Diabetes Database](https://archive.ics.uci.edu/dataset/15/pima+indians+diabetes) from the UCI Machine Learning Repository.

The data are divided into training, validation, and test datasets:

- `train_diabetes.csv` — model training
- `val_diabetes.csv` — model selection and tuning
- `test_diabetes.csv` — final model evaluation

See [data/README.md](data/README.md) for variable definitions, source information, and attribution.

## Methods

The analysis includes:

1. A custom logistic-regression implementation using NumPy and gradient descent.
2. Evaluation of learning rate, convergence, and regularization.
3. scikit-learn logistic-regression models using:
   - L1 regularization
   - L2 regularization
   - Elastic Net regularization
4. Model selection using validation-set performance.
5. Final evaluation of the selected model on the held-out test set.

## Results

L1-regularized logistic regression was selected based on validation performance. On the held-out test set, the final model achieved:

| Metric | Result |
|---|---:|
| Accuracy | 83.1% |
| F1 Score | 0.69 |
| True Negatives | 98 |
| False Positives | 3 |
| False Negatives | 23 |
| True Positives | 30 |

Because the outcome classes are imbalanced, F1 score was used as the primary performance measure. L1 regularization also supports interpretability by shrinking less informative feature coefficients to zero.

## Repository Structure

```text
.
├── README.md
├── requirements.txt
├── .gitignore
├── data/
│   └── README.md
└── notebooks/
    └── diabetes_logistic_regression.ipynb
