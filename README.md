# Prediction-of-Heart-Diseases-Using-Machine-Learning-Algorithms

**Dataset Used**

https://www.kaggle.com/ronitf/heart-disease-uci

**Aim**

The project was focused on finding the answers to the three questions that we had in mind and
the first one was identifying the risk factors, identifying the frequency of disease based on
gender and identifying the survival rate based on age and gender and for that we wanted to see
that how our predictor ‘Y’ gets affected by the 13 features(X) given in the dataset and it can be 
seen from the correlation matrix that there was no single feature that was highly correlated with
our ’target’ value.

**Methodology Used**

This project predicts the heart disease by exploring the algorithms namely Logistic Regression,
SVM, KNN, Naive Bayes Decision trees, Random Forest. The data was divided into train and
test set and We found out the accuracies of all the algorithms by applying these on our test data
and recorded the accuracies. The hyperparameter tuning of KNN, SVM, Decision Trees and
Random forest was also done to check and compare the different accuracies with changing
parameter values. The highest accuracy of 88.59% was obtained with Logistic Regression and
the total misclassified cases were less in case of LR as compared to other algorithms in the
experiment. The accuracy above 70% is good and all the other models showed the accuracy
more than 70% in this experiment so we can say that all the above-mentioned algorithms are
appropriate for predicting the heart diseases though they can still be given priority based on the
predictions of False Positives and False Negative outcomes. Table 1 shows the results of
accuracies of the algorithms.

The dataset has been curated from Kaggle and per the description given on Kaggle the
original dataset had 76 attributes, but we have used 14 attributes that includes one
“Target” variable here as the previous experiments have also been done on only 14 
attributes and the desired results have been achieved.

**ALGORITHMS USED**

As discussed above we have used six machine learning models for predicting the heart disease
in a patient and to analyse up to optimal performance among all. The short description of each
model explained in this section.

**LOGISTIC REGRESSION**

While generating the model the threshold was 0.5 which means that for probability values
greater than 0.5, the model predicts the dependent variable to be 1 and for values less than or
equal to 0.5, the model predicts the dependent variable to be 0.

**DECISION TREE**

Decision Tree is tree-like structure that classifies instances by sorting them based on the values
of the variables. Each node in a decision tree represents a variable in an instance to be classified,
and each branch represents a value that the node can assume. In the experiment the max depth
of decision tress was changed 10 times for tuning and the accuracy results for all of them were
obtained. We selected max depth 3 as it provided the maximum accuracy and the minimum TN
and FN cases.

**RANDOM FOREST**

The final predictions of the random forest are made by averaging the predictions of each
individual tree, which enhances the prediction accuracy for unseen data. The hyperparameter
tuning was performed for the estimators of the random tree and for the final model the
parameter that gave the best accuracy was chosen which was 60.

**SUPPORT VECTOR MACHINES**

For our model, the c value of 0.001 was selected for the SVM as it showed good accuracy and
minimum FP and FN cases after performing the tuning at different c values.

**K NEAREST NEIGHBOR**

For our model, the hyperparameter tuning was done for the present modelling, the whole
process is repeated fifteen times each with a k value starting from 1 to 15 and then the highest
performing parameter was selected which in this case was k=7.

**NAÏVE BAYES**

A Naive Bayes classifier assumes that the presence or absence of a particular attribute of a
class is independent to the presence or absence of any other attribute of that class. It is often
used to compute posterior probabilities of given observations and make decisions on higher
probability

**CONCLUSIONS**

Based on the experiment we can say that Machine learning is the future of healthcare industry
in detecting the diseases and facilitating the task of healthcare workers in providing best care.
All the above-mentioned algorithms performed well in terms of accuracy but could not perform
well in terms of FN and FP cases which cannot be ignored. Logistic Regression was selected 
as our final model because of the good F1 score and less misclassified cases. We found out that
age is an important factor as with age the risk of getting a heart disease increases and if the
trace in the ST segment is abnormally low below the baseline, this can lead to a Heart Disease.
Our experiment also showed that the females are prone to heart diseases as compared to Males
and hence the frequency of survival rate greatly depends on age and gender.

