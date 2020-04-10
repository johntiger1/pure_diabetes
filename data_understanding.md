Understanding the data:
we have a couple of data dictionaries, sent by Shuang.

Variables of interest are all in PEvent:
1. fday_diab
2. newdiab

Useful info:
Predictors: variables available as predictors are baseline variable, food frequency and physical activity.

- Baseline variables: PBline_04Apr19.dta

- Food frequency: Combffq_04Apr19.dta

- Physical activity: Combpaq_04Apr19.dta


If you are interested in using longitudinal data for prediction, they are in PFollow_04Apr19.dta. However, including time series as predictors in a risk prediction model do not have much value in clincial practice, since these data are not available for most of the population.


I have tried Cox PH model and random survival forest combined with variable importance method on this data set. These are methods for survival analysis, if you decide to treat it as a classification problem as a start, I would suggest random forest and gradient boosting, maybe DNN, benchmarking against logistic regression.



