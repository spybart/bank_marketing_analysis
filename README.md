# Bank Marketing Analysis
## Comparing Classifiers

by Murat Tulca

jupyter notebook:
https://github.com/spybart/bank_marketing_analysis/blob/main/bank_marketing_analysis.ipynb

## Goal: Predict if Client Will Subscribe or Not

### Results of bank marketing analysis:

Having evaluated multiple classification models, we have seen that `SVC()` performed the best for this task. We used Recall as the evaluation metric, as we ideally want to minimize false positives (we don't want to miss any client that would subscribe).

Using our best model, we are able to determine the level of impact each feature has on term subscription:
* We can see that `emp.var.rate` (employment variation rate) is the most impactful feature in determining client subscription.
* Features with medium impact include `duration` (last contact duration), `nr.employed` (number of employees), and `pdays` (number of days that passed by after the client was last contacted from a previous campaign).
* The rest of the features have little to no impact on client term subscription.

Using our model, we were able to achieve an accuracy score of 0.94 and recall score of 0.69. This model will help to more efficiently allocate time and resources to clients that are more likely to subscribe.
