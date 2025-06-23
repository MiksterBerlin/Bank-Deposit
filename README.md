# Bank-Deposit
Comparing Classifiers to predict term deposit subscription

Dataset:
This dataset is based on "Bank Marketing" UCI dataset (please check the description at: http://archive.ics.uci.edu/ml/datasets/Bank+Marketing).
The data is enriched by the addition of five new social and economic features/attributes (national wide indicators from a ~10M population country), published by the Banco de Portugal and publicly available at: https://www.bportugal.pt/estatisticasweb.

Goal: 
This dataset was used to compare different classification models to optain the best possible features to improve the subscription to term deposits of bank clients.

Methods:
As the data set was imbalanced, oversampling was performed to reduce the recall of the models.
After feature engeneering and feature selection models was tested.

Models: 
1) Logistic Regression
2) KNeighbors classifyer
3) Decission tree classifyer
4) SVM

SVM & Logistic Regression were exclude because of lower performance.

After a Gridsearch and the adjusting of the performance metric, feature importance calculation was used to define a subset of features for the model.

Result interpretation was done using Shap explaination.

Results:
After ruling out Logarithmic Regression and SVM for poor results, we optimized K-Nearest Neighbors and Decision Tree classifiers. Key features included the Euribor 3-month rate, campaign call count, and consumer confidence index. Calling more than 3 or 4 times reduces success odds. The Euribor rate, a significant European interest benchmark, strongly correlates with the consumer price index and influences behavior. Students, retirees, and certain demographics show higher success rates, which fluctuate with interest rates. Prior negative credit behavior is exclusionary.




Dataset Citation:
  This dataset is publicly available for research. The details are described in [Moro et al., 2014]. 
  Please include this citation if you plan to use this database:

  [Moro et al., 2014] S. Moro, P. Cortez and P. Rita. A Data-Driven Approach to Predict the Success of Bank Telemarketing. Decision Support Systems, In press, http://dx.doi.org/10.1016/j.dss.2014.03.001

  Available at: [pdf] http://dx.doi.org/10.1016/j.dss.2014.03.001
                [bib] http://www3.dsi.uminho.pt/pcortez/bib/2014-dss.txt

1. Title: Bank Marketing (with social/economic context)

2. Sources
   Created by: Sérgio Moro (ISCTE-IUL), Paulo Cortez (Univ. Minho) and Paulo Rita (ISCTE-IUL) @ 2014
   
3. Past Usage:

  The full dataset (bank-additional-full.csv) was described and analyzed in:

  S. Moro, P. Cortez and P. Rita. A Data-Driven Approach to Predict the Success of Bank Telemarketing. Decision Support Systems (2014), doi:10.1016/j.dss.2014.03.001.
