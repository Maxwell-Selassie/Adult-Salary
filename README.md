*"Who earns more — the graduate, the professional, or the self-employed? A machine learning exploration of income drivers."*

***Introduction***

Money influences the choices we make every day—what career path we choose, how long we stay in school, or whether we pursue self-employment.

As a Ghanaian fascinated by economics and how societies function, I wanted to explore a simple but important question:

👉 What truly drives income?

Is it education, as parents emphasize?
Is it occupation, as many people chase white-collar jobs?
Or does work type (government, private, or self-employed) play the biggest role?

To explore this, I used the well-known Adult Income Dataset, originally extracted from the 1994 U.S. Census by Barry Becker. The dataset contains 48,842 individuals, each labeled with whether they earn above or below $50K annually.

Although U.S.-based, I interpret this dataset as if it applied to Ghana, since many of the same drivers of income—education, occupation, and work type—remain relevant here and worldwide.

***Problem Statement***

This project explores the factors that influence whether someone earns above or below a given income threshold.

Some guiding questions were:

Education vs Income: Does higher education guarantee higher pay?

Occupation vs Income: Do certain jobs consistently pay more?

Education vs Occupation: Which has more impact—your degree or your career path?

Workclass vs Income: Do self-employed people earn more than government or private workers?

On a personal level, the model helps me reflect on decisions such as:

Should I focus on my education, because good grades and higher degrees secure better pay?

Or should I build my career and network early, since opportunities and connections may outweigh formal education?

Is self-employment more rewarding than government or private sector jobs?

***Dataset***

Source: UCI Adult Dataset (1994 Census) – Barry Becker’s extraction

Size: 48,842 rows (subset of U.S. population in 1994)

Target: Income ( >50K vs ≤50K )

Key Features Used:

Age, Education, Occupation, Workclass, Marital Status

Race, Sex, Native Country, Hours Worked per Week

Capital Gain, Capital Loss

***Methodology***

The workflow followed:

**Data Cleaning & Preprocessing**

Handling missing values (e.g., “?” entries)

Scaling & polynomial feature expansion for numeric variables

**Encoding categorical variables**

One-Hot Encoding for low-cardinality columns

Target Encoding for high-cardinality columns

**Modeling**

Tried multiple models: Logistic Regression, Decision Trees, Random Forest, XGBoost

Hyperparameter tuning with GridSearchCV + Cross-Validation

Evaluation based on Log Loss, Accuracy, Precision, Recall, F1-score

**Interpretation**

Identified key drivers of income using feature importance and coefficients

Compared education vs occupation vs workclass impact


