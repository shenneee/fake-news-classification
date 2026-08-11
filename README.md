# Fake News Detection Using Machine Learning

A Social Web Analytics research project that compares traditional machine learning models for classifying real and fake news using the **FakeNewsNet** dataset.

The project compares **Multinomial Naive Bayes, Logistic Regression, and Linear SVM** using two feature sets:

* **Headline-only:** TF-IDF features from news headlines
* **Combined:** TF-IDF features + tweet count and other handcrafted features

Models are evaluated using accuracy, precision, recall, F1-score, ROC-AUC, and confusion matrices. The results are also exported for visualization in **Microsoft Power BI**.

## Dataset

The project uses the FakeNewsNet dataset containing data from **PolitiFact** and **GossipCop**.

The original CSV files are not included due to their large size.

**Dataset source:**
[Harvard Dataverse — FakeNewsNet](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/UEMMHS)

The following files are required:

```text
politifact_fake.csv
politifact_real.csv
gossipcop_fake.csv
gossipcop_real.csv
```

Place the CSV files in the same directory as the Python script.

## How to Run

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn
```

Then run:

```bash
python fake_news_analysis.py
```

The script generates EDA visualizations, confusion matrices, ROC curves, feature importance results, model comparison results, and a CSV export for Power BI.

## Technologies

* Python
* Pandas & NumPy
* Scikit-learn
* Matplotlib & Seaborn
* SciPy
* Microsoft Power BI

## Academic Project

Developed as part of a university **Social Web Analytics** research assignment.
