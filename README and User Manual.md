# Fracture_Intensity_Predictor

Title of manuscript: Robust Fracture Intensity estimation from petrophysical logs and mud loss data: A Multi-level ensemble modeling Approach

Authors: Ahmad Azadivash, Hosseinali Soleymani, Atrina Seifirad, Amirali Sandani, Farshid Yahyaee, Ali Kadkhodaie

This code exemplifies a comprehensive machine learning workflow for a regression task in the oil and gas domain. It aims to predict the intensity of well logs, which are records of rock properties made during drilling. The fracture intensity value is critical for assessing potential oil and gas reserves.
The code first loads and prepares the input dataset, which contains measurements of 12 well log attributes like depth, density, porosity etc. It splits the data into training and test sets for modeling.
Various regression algorithms are implemented - ensemble methods like gradient boosting, random forests, extra trees as well as XGBoost, LightGBM, CatBoost. The models are trained on the data and evaluated using regression metrics: MAE, RMSE, MSE and R^2.
To optimize the hyperparameters, the code extracts the parameter values for each fitted model and logs them into a CSV file. This enables analyzing the optimal configurations.
For model analysis, the code generates insightful plots - residuals to detect biases, feature importance to identify key attributes, and actual vs predicted values to assess accuracy.
A key technique used is ensemble stacking. Two meta-learners are created by generating predictions from base models like random forests and using them as new features. The meta-learners are combined into a super learner model using Ridge regression for further improvement. Comparative bar plots are produced to evaluate the base and stacking models.
The code follows coding best practices - it has modular functions, descriptive names and detailed comments. It can serve as a template for harnessing machine learning to solve real-world regression problems in domains like oil and gas. The comprehensive model evaluation and validation provides trust and interpretability.
In summary, this code demonstrates an end-to-end ML workflow for fracture intensity prediction using ensembling and stacking techniques. The detailed analysis and plots aid model transparency and reliability, which is critical for industry adoption.

