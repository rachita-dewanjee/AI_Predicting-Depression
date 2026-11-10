# Predicting Depression from Social Media Use

A machine learning project that predicts signs of depression from how people use social media.

## Data
`Predicting_Depression.csv` holds **305 anonymous survey responses** (collected in March 2022) about
social media habits. Each response has a binary `Result` label (158 positive, 147 negative).

Survey questions include:
- age, gender and profession
- how much time is spent on social media (rarely, almost never, often, frequently)
- the main purpose of using social media
- whether the person reveals mental breakdowns in posts, and the reason behind it
  (for example, no supportive family member or few real friends to share with)
- whether the person is connected with a mental health support forum

## Method
1. **Preprocessing:** drop unused columns, label-encode categorical answers (gender, purpose,
   revealing breakdowns, forum use) and one-hot encode time spent and reasons
2. **Features:** 10 features from the answers above
3. **Models:** Logistic Regression, Support Vector Machine, Decision Tree, K-Nearest Neighbours (k = 3),
   Random Forest and Gaussian Naive Bayes, each trained on an 80/20 train/test split
4. **Evaluation:** accuracy, confusion matrix, precision, recall and F1-score for every model

## Tech
Python, pandas, scikit-learn, Jupyter Notebook.

## Run
Open `predicting depression.ipynb` in Jupyter or Google Colab with `Predicting_Depression.csv` in the
same folder, and run the cells from top to bottom.
