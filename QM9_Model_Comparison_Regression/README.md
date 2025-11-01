This project is a self-practice comparative study of various regression models applied to the QM9 molecular dataset. The goal is to predict the HOMO–LUMO energy gap, an important quantum chemical property that indicates molecular stability and reactivity.



A subset of 5000 molecules from the QM9 dataset was used, each described by several quantum chemical features such as:



A, B, C (rotational constants)



μ (dipole moment)



α (isotropic polarizability)



HOMO and LUMO (molecular orbital energies)



r² (electronic spatial extent)



ZPVE, U₀, U₂₉₈, H₂₉₈, G₂₉₈ (energy-related properties)



Cv (heat capacity)



U₀\_atom, U₂₉₈\_atom, H₂₉₈\_atom, G₂₉₈\_atom (atomic-level energy measures)



These features were used as input variables to predict the HOMO–LUMO gap (target variable).



The project compares the performance of five popular regression models:



a. Multiple Linear Regression



b. Polynomial Regression



c. Support Vector Regression (SVR)



d. Decision Tree Regression



e. Random Forest Regression



All models were trained and evaluated using the same dataset split (80% training, 20% testing) to ensure a fair comparison. The R² score was used as the evaluation metric to measure how well each model predicts the target variable.



Model Performance (R² Scores):

Model	                        R² Score



Multiple Linear Regression	0.9999990

Polynomial Regression	        0.9049225

Support Vector Regression	0.9913729

Decision Tree Regression	0.9902184

Random Forest Regression	0.9970497



Summary of Results:



1. Multiple Linear Regression achieved the highest R² score, showing an almost perfect fit for this dataset.



2\. Random Forest Regression also performed very well, indicating that ensemble methods can capture complex relationships effectively.



3\. SVR and Decision Tree Regression provided good results but were slightly less accurate than Random Forest.



4\. Polynomial Regression had the lowest R² score, likely due to overfitting and limited generalization.



Key Learnings:



1. Linear models can perform exceptionally well when the dataset has strong linear relationships between variables.



2\. Ensemble-based methods such as Random Forest offer robust and stable predictions, even when data relationships are slightly non-linear.



3\. This exercise provided a hands-on understanding of how different regression algorithms behave on the same dataset and how the R² metric helps measure model performance.



This project was done purely for self-learning and experimentation to explore the comparative strengths of regression models in predicting quantum chemical properties.

