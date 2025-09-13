// Student Performance Prediction – Linear vs Polynomial Regression
_Overview

This project applies Linear Regression and Polynomial Regression to predict students’ Final Scores.
The dataset contains 50 student records, including study hours, attendance, previous scores, and extracurricular participation.

_Dataset

Rows: 50

Columns:

Hours_Studied

Attendance_Percentage

Previous_Score

Extra_Curricular (Yes/No → encoded as 1/0)

Final_Score (target variable)

Other metadata (StudentID, Grade)

Methods:
_Linear Regression

Assumes a straight-line relationship between inputs (X) and output (Y).​

_Polynomial Regression

Generates higher-order features (squares, interactions).

Captures non-linear relationships.

 _Results
Linear Regression

R² Score: 0.997

MSE: 0.76

Feature Effects:

Previous Score → strongest positive predictor (+1.06).

Extracurricular → positive impact (+1.28).

Attendance → small positive effect (+0.04).

Hours Studied → slight negative coefficient (-0.63).

Polynomial Regression (degree=2)

R² Score: ≈ 0.999 (slightly higher).

MSE: even smaller than Linear.

Captured more complexity, but risk of overfitting since dataset is small.

_Insights

Previous academic performance is the best predictor of final results.

Participation in extracurricular activities positively influences performance.

Good attendance helps, but not as strongly.

Polynomial regression fits slightly better, but linear regression is already very strong and more interpretable.

_Tech Stack

Python

pandas

NumPy

Matplotlib

Scikit-learn
