This repository presents a self-practice machine learning project focused on predicting the HOMO–LUMO energy gap for 5000 molecules from the QM9 dataset using Random Forest Regression and Decision Tree Regression models. The purpose of this project is to understand how ensemble-based regression models like Random Forest perform compared to a single Decision Tree, especially when handling scientific or molecular data containing complex relationships among variables.



The dataset used in this project is a subset of the QM9 molecular database, which provides quantum chemical properties for small organic molecules. Each sample in the dataset includes several physicochemical and quantum features such as moments of inertia (A, B, C), dipole moment (mu), polarizability (alpha), HOMO and LUMO orbital energies, mean square radius (r2), zero-point vibrational energy (zpve), internal energies (u0, u298), enthalpy (h298), Gibbs free energy (g298), heat capacity (cv), and corresponding atom-based energy values (u0\_atom, u298\_atom, h298\_atom, g298\_atom). The target variable in this project is the energy gap (gap) between the HOMO and LUMO orbitals, which is an important parameter in quantum chemistry as it helps determine molecular stability and reactivity.



In this implementation, the dataset was divided into training and testing sets using an 80–20 split. The Decision Tree Regressor was used as a baseline model, followed by the Random Forest Regressor for comparison. The Random Forest model was trained with 200 estimators and a fixed random state to ensure reproducibility. Both models were trained without any feature scaling or encoding since tree-based algorithms can handle raw numerical inputs directly.



Key observations from this project include the following:



The Decision Tree model performed well on the training data but showed signs of overfitting, making it less stable on unseen data.



The Random Forest model, on the other hand, provided smoother and more accurate predictions by averaging the results from multiple trees.



Random Forest Regression effectively reduced variance and produced more reliable results for predicting the HOMO–LUMO gap.



Through this project, I gained practical experience in understanding how decision tree-based models work, how Random Forest improves prediction stability through ensemble learning, and how to analyze molecular data using regression techniques. The project was implemented in Google Colab using Python and common libraries such as Pandas, NumPy, Matplotlib, and Scikit-learn. It serves as a part of my continuous learning and exploration of machine learning algorithms applied to real-world scientific datasets.

