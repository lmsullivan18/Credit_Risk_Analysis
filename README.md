# Credit Risk Analysis

## Overview
The purpose of this analysis was to apply machine learning to the real-world challenge of credit risk. I used different techniques to train and evaluate models with unbalanced classes. Using the analysis of the different techniques, I can make a recommendation as to which model should be used to predict credit risk.

## Results

In the first section we compared Naive Random Oversampling with SMOTE Oversampling.
- The results of the Naive Random Oversampling show that the accuracy score is about 65%. However, the precision when evaluating high risk loans is extremely low. This is not a useful prediction as it is more important in this instance to have a precise model. This is because approving a bad loan is more costly than missing out on the potential profit from a good loan.

![naive random oversampling](https://user-images.githubusercontent.com/74469315/113512607-6b3d9200-9533-11eb-8e7f-4b66fad9df02.PNG)

- The results of the SMOTE Oversampling are very similar to the native random oversampling. The accuracy is about 61% but the precision when evaluating high rick loans is extremely low.

![SMOTE](https://user-images.githubusercontent.com/74469315/113512611-6d9fec00-9533-11eb-9495-0c42979eac69.PNG)

In the second section we used Undersampling. 
- The results of the undersampling method show are even worse than the two oversampling methods. The accuracy score is lower at 51% and the precision is just as low for predicting high risk loans. 

Then, we used Combination (Over and Under) Sampling.
- The results of combination sampling were similar to those from oversampling. The accuracy score was about 63% and the precision for predicting high risk loans was extremely low.

![combination](https://user-images.githubusercontent.com/74469315/113512602-6842a180-9533-11eb-84a1-22ebfa4bd7bc.PNG)

In the last section we used Ensemble Learning.
- The Balanced Random Forest Classifier had a 66% accuracy rate and a 72% precision rate for predicting high risk loan candidates. This is the most accurate model run so far.

![balanced random forest](https://user-images.githubusercontent.com/74469315/113512583-5103b400-9533-11eb-86e1-4210561048a2.PNG)

- The results of the Easy Ensamble AdaBoost Classifier had a 93% accuracy rate and an 8% precision rate for predicting high risk loan candidates. This is a bit better than the oversampling methods, but still not a terrific model for predicting high risk loan candidates.

![easy ensamble](https://user-images.githubusercontent.com/74469315/113512603-6973ce80-9533-11eb-83a8-91e31091fcb7.PNG)

## Summary
In summary, most of the machine learning models were not great at predicting credit risk for high risk individuals. I recommend using the Balanced Random Forest Classifier model because it has the highest precision score for detecting high risk loan.
