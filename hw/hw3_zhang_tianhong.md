## Question 1.
<ol type="a">
 <li>True. Redundant attributes receive similar
weights and do not degrade the quality of the classifier. 
However, if the number of irrelevant or reduntant attributes
is large, the learning of the ANN model may suffer from 
overfitting, leading to poor generalization performance.</li>
 <li> False. SVM and ANN does not handle very large training data sets equally well. SVN is more robust
 to the presence of a large number of irelevant and redundant attributes than other classifiers.
</li>
 <li>False.The SVM learning problem can be formulated as a convex optimization problem, in which efficient algorithms are available to find the global minimum of the objective function. Neural Network tend to find only locally optimum solutions. They do not always produce the same decision boundaries. </li>
</ol>

## Question 2.
<ol type="a">
    <li>
        <ol> 
            <li> TP = 90, FP = 5, TN = 95, FN = 10
            <li> TP = 90, FP = 50, TN = 950, FN = 10
            <li> TP = 90, FP = 500, TN = 9500, FN = 10
        </ol>
    <li>
        <ol> 
            <li> p = 90/95 = 0.947, r = 0.9, F = 180/195 = 0.923, TPR/FPR = 18
            <li> p = 90/140 = 0.643, r = 0.9, F = 180/240 = 0.75, TPR/FPR = 18
            <li> p = 90/590 = 0.153, r = 0.9, F = 180/690 = 0.261, TPR/FPR = 18
        </ol>
    <li> T3 is strictly better than T4 (irrespective of skew). T3 has a higher TPR and a lower FPR than T4, and both TPR and FPR do not take into account the skew among the classes.
    <li> T1 has a lower TPR and lower FPR than T4, so it is worse but not strictly worse than T4; T2 has a higher TPR and a higher FPR than T4, so it is worse but not strictly worse than T4; Regarding with TPR/FPR, T1 = 50, T2 = 9.9, T4 = 18; T2 is worse than T4 (irrespective of skew) in this measure. 
    <li> Which classifiers may be better or worse than T4 (depending on skew)? 
        <ol>
        <li> For balanced skew case: T3 is better than T4 because of its high precision and high F-measure. T1 and T2 may be better or worse than T4, depending on different factors, e.g., if we want most of a classfier's positive predictions correct, we want a classifier with a high precision, than T1 is better suited. However, in cases that correctly identifying all the positive instances is what matters most, a high recall is preferred, so that T2 is better than T4. 
        <li> For medium skew case, T2 and T3 may be better than T4 due to their higher precision and recall. T1 may be better or worse than T4, take different factors into consideration. 
        <li> For high skew case, T1, T2 and T3 may all be better than T4. T1 may be worse than T4, since it has a lower recall. 
        </ol>
</ol>