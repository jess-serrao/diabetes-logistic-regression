# Data

This project uses the [Pima Indians Diabetes Database](https://archive.ics.uci.edu/dataset/15/pima+indians+diabetes) from the UCI Machine Learning Repository.

The dataset contains 768 de-identified records and eight numeric predictor variables. The target variable, `Outcome`, indicates whether the diabetes outcome is positive (`1`) or negative (`0`).

## Files

The original dataset was divided into training, validation, and test datasets for model development and evaluation.

| File | Purpose |
|---|---|
| `train_diabetes.csv` | Used to train the logistic-regression models. |
| `val_diabetes.csv` | Used to compare model settings and select the final model. |
| `test_diabetes.csv` | Used only for final evaluation of the selected model. |

## Variables

| Variable | Description |
|---|---|
| `Pregnancies` | Number of pregnancies. |
| `Glucose` | Plasma glucose concentration. |
| `BloodPressure` | Diastolic blood pressure. |
| `SkinThickness` | Triceps skin-fold thickness. |
| `Insulin` | Two-hour serum insulin. |
| `BMI` | Body mass index. |
| `DiabetesPedigreeFunction` | Diabetes pedigree function. |
| `Age` | Age in years. |
| `Outcome` | Diabetes outcome: `0` = negative; `1` = positive. |

## Source and License

Source: UCI Machine Learning Repository, Pima Indians Diabetes Database.

This dataset is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Please provide appropriate attribution to the original dataset source when reusing this repository.
