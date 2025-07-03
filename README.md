# AI-ML-Task 7

1. Importing Libraries

             > You load all the essential libraries:
                     > pandas, numpy: data manipulation
                     > matplotlib.pyplot, seaborn: visualization
                     > sklearn: modeling (SVC, scaling, evaluation metrics, GridSearchCV, etc.)

2. Data Loading and Preprocessing

             > Loads the Breast Cancer dataset.
             > Removes columns like 'id' or 'Unnamed' (non-informative).
             > Converts the target column diagnosis from categorical (M, B) to binary numeric (1, 0).

3. Feature & Target Separation + Scaling

             > X: all features
             > y: target label
             > X_scaled: standardized version of X to improve SVM performance

4. Splitting Dataset and Training SVMs

             > Splits the data into:
                 > 80% Training
                 > 20% Testing
             > Ensures fair evaluation on unseen data

5. Train SVM Models (Linear and RBF)

             > Trains two different SVM classifiers:
                 > svm_linear: Assumes classes are linearly separable
                 > svm_rbf: Uses non-linear RBF kernel for complex decision boundaries

6. Model Evaluation (Accuracy, Report, Matrix)

             > Evaluates model performance on the test set using:
                 > Classification Report: Shows precision, recall, F1-score
                 > Confusion Matrix: Shows TP, FP, FN, TN
                 > Accuracy: Overall correct predictions

7. Decision Boundary Visualization (2 Features)

             > Selects only 2 features to visualize in 2D: radius_mean, texture_mean
             > Retrains SVMs on these 2D features to enable boundary plotting

8.Hyperparameter Tuning:
            
             > Uses GridSearchCV to find the best C and gamma values for RBF kernel using 5-fold cross-validation.

9.Cross-Validation Evaluation:

             > Evaluates the best model on the full dataset using 5-fold cross-validation for more reliable accuracy.

10.Synthetic Data Plot (Bonus):

             > Creates a 2D synthetic dataset for a clean visual demonstration of how RBF SVM separates classes.


