# Work experience at Atlant-Mobile Ltd.
## Here, I provide code snippets that illustrate my approach to several data analysis problems from my last place of work.
### In the file Preprocessing.ipynb my approach for handling outliers is presented. The idea is as follows:
- For each feature the main focus is on the values located above the 90% percentile mark (right tail of the distribution) and below the 5% percentile mark (left tail). First, the right tail is considered, then the same procedure is applied to the left tail of the distribution.
- For each feature the best percentile is searched in the right tail; the best one is identified by the function one_factor_analysis_gini.
- This function computes the metric gini = 2 * roc_auc - 1 based on transmitted feature and percentile.
- After the best percentile for the feature is determined, the corresponding value is found. All higher values in the feature are substituted by it. 
### In the file Models.ipynb main steps are shown for the following tasks: 
* training and evaluation of CatBoostClassifier;
* optimal hyperparameter selection for LGBMClassifier.
