# Class Imbalance Problem

## What are the two challenges posed by class imbalance for classification?
   1. It can be difficult to find sufficiently many labeled samples of a rare class.
   2. Alternative evaluation metrics, which are sensitive to the skew, are needed to capture different criteria of performance than accuracy.
## Things to consider when building classifiers with class imbalance.
   1.  We need to ensure that the learning algorithm is trained over a data set that has adequate representation of both the majority as well as the minority classes
    - Oversampling (pros and cons)
    - Undersampling (pros and cons)
        - *Synthetic Minority Oversampling Technique*
        - **NOTICE**: duplicating a positive instance is analogous to doubling its weight during the training stage. Hence, the effect of oversampling can be alternatively achieved by assigning higher weights to positive instances than negative instances. This method of weighting instances can be used with a number of classifiers such as logistic regression, ANN, and SVM.
2.   Having learned a classification model, we need a way to adapt its classification decisions (and thus create an appropriately tuned classifier) to best match the requirements of the imbalanced test set.
        - For a SVM, the signed distance of an instance from the positive margin hyperplane can be used as a classification score.
        - For a decision tree, test instances belonging to a leaf in a decision tree can be assigned a score based on the fraction of training instances labeled as positive in the leaf.
## How to evaluate performance with class imbalance?
   - skew: $\alpha = P/(P+N)$
   - Evaluation measures that **do not** take into account the skew among the classes: TPR (also called: recall, r, sensitivity), TNR, FPR, FNR
   - Evaluation measures that is sensitive to the skew: precision, F-measure, G-measure.