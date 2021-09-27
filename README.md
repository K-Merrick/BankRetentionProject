# BankRetentionProject

Beta Bank has found that a small portion of customers are leaving every month. Analysts at the bank determined that it is cheaper to retain the customers it has than to attract new customers. In light of this finding, Beta Bank requested that we create a model that can predict whether a customer will leave the bank soon. Using data on clients' past behavior and termination of contracts with the bank, our task if to build a model with an F1 score of at least .59. In order to meet this requirement, we will test various classification models and determine the probability threshold that allows for the optimal F1 score.

**Conclusion**: For this project, Beta Bank instructed us to create a model that that predicts whether individuals will leave the bank soon; they desired that this model has an f1-score of at least .59. By way of properly preparing, encoding, and balancing the data, we were able to construct a model that provided an f1-score higher than .59. The scores from our models are summarized as follows:

1) RF_Grid: Model chosen for highest f1-score.

    ** Normal Threshold: F1 = 0.6, Recall = 74
    ** Threshold Moved (.65): F1 = .61, Recall = .63

2) RF_Grid2: Model chosen for highest recall score.

    ** Normal Threshold: F1 = .57, Recall = .77

Based on these findings, Beta Bank has various options. Clearly, the model with the highest f1-score is the RF_Grid model with a higher threshold. This model also has a recall score that indicates the model was able to accurately classify approximately 2/3 of the actual positives. If Beta Bank's cost per individual they actively try to keep with the bank is sufficiently low, they may be more interested in the RF_Grid2 model, which has a higher recall score that the other model; given it's score, it was able to accurately classify approximately 80% of actual positives. Of course, the metric that would best suit Beta Bank depends largely on the predicted cost of keeping an individual with the bank; if this cost is high, then it would certainly be better to find a model with the best precision and recall balance.
