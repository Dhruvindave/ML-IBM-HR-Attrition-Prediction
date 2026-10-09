# IBM HR Attrition Prediction

A machine learning project that predicts employee attrition using the IBM HR Analytics dataset. It covers exploratory data analysis, feature engineering, preprocessing, model comparison, and hyperparameter tuning using scikit-learn.

**[🚀 Live Demo](https://tinyurl.com/v78ebmmj)** · **[GitHub Repository](https://github.com/Dhruvindave/ML-IBM-HR-Attrition-Prediction)**

## Key Features

* Exploratory Data Analysis (EDA)
* Feature engineering for employee tenure and career progression
* Preprocessing with `ColumnTransformer` and `OneHotEncoder`
* Comparison of Logistic Regression, Random Forest, and Decision Tree
* Hyperparameter tuning with `GridSearchCV` and stratified 5-fold cross-validation
* Interactive attrition prediction interface

## Model Evaluation

| Model                     | Test ROC-AUC |
| ------------------------- | -----------: |
| Logistic Regression       |       0.8099 |
| Random Forest             |       0.7841 |
| Decision Tree             |       0.6467 |
| Tuned Logistic Regression |       0.8099 |
| Tuned Random Forest       |       0.7876 |

The tuned Logistic Regression model achieved a cross-validation ROC-AUC of **0.8459**.

Baseline Logistic Regression results:

* Accuracy: 86.39%
* Precision: 62.07%
* Recall: 38.30%
* F1-score: 47.37%

The results highlight why accuracy alone is insufficient for imbalanced attrition data, where missing employees likely to leave is an important consideration.

## Tech Stack

* **Language:** Python
* **Data Analysis:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** scikit-learn

## Run Locally

```bash
git clone https://github.com/Dhruvindave/ML-IBM-HR-Attrition-Prediction.git
cd ML-IBM-HR-Attrition-Prediction

python -m venv .venv
source .venv/bin/activate

pip install -r requirements.txt
streamlit run app.py
```

Replace `app.py` if your application's entry-point filename differs.

## Limitations

The model captures patterns in the evaluated dataset and does not guarantee predictions will generalize to other organizations. It is intended for learning and analysis, not as a standalone tool for employment decisions.

**[Try the Live Demo](https://tinyurl.com/v78ebmmj)** · **[Explore the Code](https://github.com/Dhruvindave/ML-IBM-HR-Attrition-Prediction)**
