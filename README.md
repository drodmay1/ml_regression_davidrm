# Predicting Medical Insurance Charges with Regression

This project explores the Medical Cost Personal Dataset to build and evaluate regression models that predict insurance charges based on features like age, BMI, smoker status, and more.

## Files in This Repository

- [`regression_davidrm.ipynb`](./regression_davidrm.ipynb): Main notebook with full ML workflow, analysis, and reflections.
- [`data/insurance.csv`](./data/insurance.csv): Dataset used for the project.
- [`peer_review.md`](./peer_review.md): Peer review and feedback for a classmate’s project.

## Project Summary

The goal of this project was to predict individual insurance charges using a regression model. I explored the data, handled preprocessing (including encoding and scaling), and compared several models using pipelines. I found that:
- Smoker status is the strongest predictor of insurance charges.
- Scaling improved model performance slightly.
- Adding polynomial features didn’t improve results and added unnecessary complexity.

## Models Used

- Linear Regression (baseline)
- Pipeline 1: Imputer → Scaler → Linear Regression
- Pipeline 2: Imputer → PolynomialFeatures (degree=3) → Scaler → Linear Regression

Models were compared using:
- R² Score
- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)

## How to Run Locally

1. Clone the repository:

```bash
git clone https://github.com/drodmay1/ml_regression_davidrm.git
cd ml_regression_davidrm
```

2. Create and activate a virtual environment:
   
```bash
python3 -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

3. Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

4. Launch the notebook
   
```bash
jupyter notebook
```

5. Open and run `regression_davidrm.ipynb`

## Final Notes

This project helped me practice the full machine learning workflow using real-world data. It was a great intro to pipelines, evaluation metrics, and thinking critically about what makes a model good (or not so good).


