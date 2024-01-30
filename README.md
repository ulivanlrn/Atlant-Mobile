# Working experience in Ltd. the company "Atlant-Mobile"
## Here I put some code snippets, which illustrate my approach to some data analysis problems from my last place of work.
### In the file Preprocessing.ipynb my approach for handling outliers is presented. The idea is as follows:
- For each feature the main focus is on the values located above 90% percentile mark (the right tail of the distribution) and below 5% percentile mark (the left tail). First the right tail is considered, then the same procedure is applied to the left tail of the distribution.
- For each feature the best percentile is searched in the right tail; the best one is identified by the function one_factor_analysis_gini.
- This function computes the metric gini = 2 * roc_auc - 1 based on transmitted feature and percentile.
- After the best percentile for the feature is determined, the value corresponding to it is found. All higher values in the feature are substituted by it. 
### In the file Models.ipynb main steps are shown for the following tasks: 
* training and evaluating the CatBoostClassifier model;
* selection of hyperparameters` optimal values for the LGBMClassifier model.
