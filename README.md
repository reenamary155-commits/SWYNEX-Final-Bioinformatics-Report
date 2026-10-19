# SWYNEX – Final Bioinformatics Report

Task 4 of my Bioinformatics Internship with SWYNEX Technologies.

## 1. Question
Can the measured characteristics of cell nuclei be used to accurately distinguish malignant tumours from benign tumours, and which features are most predictive of malignancy?

## 2. Data
- Dataset: Breast Cancer Wisconsin (Diagnostic), UCI Machine Learning Repository
- Link: https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic
- 569 samples (212 malignant, 357 benign), 30 numeric features from digitised images of fine needle aspirates of breast masses
- Missing values: 0

## 3. Methods
- Tools: Python, pandas, seaborn, matplotlib, scikit-learn (Google Colab)
- Checked data size, missing values and class counts
- Made three charts: diagnosis counts, worst radius by diagnosis, correlation of mean features
- Trained a logistic regression model (75% training, 25% test, standardised features)

## 4. Results
- 357 benign and 212 malignant samples (about 37% malignant)
- Average worst radius: about 21.1 (malignant) vs 13.4 (benign)
- Mean radius and mean area are almost perfectly correlated (about 0.99)
- Logistic regression test accuracy: about 96.5% on 143 unseen samples

## 5. Limitations
- Small, curated dataset from one source; results may not hold for other labs or patients
- Classes are unequal, so accuracy alone can mislead
- Many features are highly correlated, so individual model coefficients should not be over-interpreted
- Shows patterns, not causes
- Student learning project, not a diagnostic tool

## 6. References
1. Wolberg, W., Mangasarian, O., Street, N., & Street, W. (1995). Breast Cancer Wisconsin (Diagnostic). UCI Machine Learning Repository.
2. Pedregosa, F. et al. (2011). Scikit-learn: Machine Learning in Python. Journal of Machine Learning Research, 12, 2825–2830.
3. Waskom, M. L. (2021). seaborn: statistical data visualization. Journal of Open Source Software, 6(60), 3021.
4. McKinney, W. (2010). Data structures for statistical computing in Python. Proceedings of the 9th Python in Science Conference.

## Files
- `SWYNEX_Final_Bioinformatics_Report.ipynb`: full notebook with charts and interpretation
