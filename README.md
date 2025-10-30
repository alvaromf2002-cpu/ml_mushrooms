This repository is the deliverable of the **FSD311 Machine Learning Module of Supaero Data and Decision Sciences Major**. The project consists on an evaluation of a mushroom dataset applying several tools.

# Work description

## 1. Methodology
We framed the Secondary Mushroom dataset as a **binary classification** task (edible vs poisonous). The hypothesis assumed that **tree-based ensembles** (Random Forest, Gradient Boosting) outperform simpler models due to their ability to model non-linear interactions among morphological features. The evaluation employed 5-fold Stratified Cross-Validation with ROC-AUC as the primary metric.

## 2. Pedagogy
We visualized class distributions, feature histograms, and boxplots for interpretability. Results are summarized through confusion matrices, feature importances, and SHAP plots. These graphical elements make the reasoning traceable and transparent.

## 3. Depth of Reflection
**Exploration phase:** We analyzed feature distributions and identified mixed data types.
**Feature engineering:** Implemented imputation and one-hot encoding pipelines to ensure consistent preprocessing.
**Learning phase:** Compared six ML algorithms from the syllabus (Decision Tree, Naive Bayes, SVM, Bagging, Random Forest, Gradient Boosting).
**Hyperparameter tuning phase:** Applied Randomized Search and Bayesian Optimization to refine Random Forest parameters; key hyperparameters include number of trees, depth, and max features.
**Conclusion phase:** Random Forest achieved the highest ROC-AUC (~0.99). Bayesian optimization yielded marginal but consistent gains.

We also explored **Unsupervised Learning** through Isolation Forest anomaly detection, revealing potential outlier samples that may correspond to mislabeled instances.

## 4. Key Concepts (from the course)
AI · ML · Supervised vs Unsupervised · Feature · Feature Engineering · Correlation · Hyperparameter · Overfitting · Explainability.
Each concept is exemplified within this notebook through model training, cross-validation, feature analysis, and interpretability tools (permutation importance and SHAP).

## 5. Conclusions and Next Steps
- Tree ensembles dominate performance due to robustness against feature interactions.
- Anomaly detection can enhance data quality by spotting mislabeled or rare patterns.
- Future work: deeper Bayesian optimization with prior-informed search spaces, inclusion of Gaussian Processes for uncertainty estimation, and enhanced explainability (e.g., LIME or partial dependence plots).


"""
