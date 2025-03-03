# Mod17_Comparing_Classifiers

### Overview

This overall ask in this excercise is to compare the performance of different classifiers such as KNN, SVM, Logistic Regression, and Decision Trees. To acomplish this goal Portuguese banking instute's marketing data has been provided. The goal is to idetify best classifier to forecast if the customer will subscribe to a long-term deposit or not.

### Business Understanding

The objective of this project is to help the Portuguese banking institute to run a successful marketing campaign. Help them predict the customer conversion chances accurately, i.e. predict what are the chances that customer will subscribe to a long-term deposit. This will help them optimize their campaigns which will help with bussiness growth.

### Model Performance Summary
|Model	|Train Time	|Train Accuracy	|Test Accuracy	|Precision	|Recall	|F1	|AUC|
|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|
|Logistic R|egression	|28.205422	|0.911286	|0.908767	|0.653179	|0.405891	|0.500665	|0.931548|
|Decision Trees	|12.349532	|0.930160	|0.910386	|0.607547	|0.578305	|0.592565	|0.929184|
|KNN	|59.759074	|1.000000	|0.903020	|0.639769	|0.318966	|0.425695	|0.903716|

### Conclusion

**Logistic Regression:**
The logistic regression offeres a best AUC score of 93%. Accuracy is much lower when compred to decision tree. Training time was more than double of DT. 

**KNN:**
The KNN algorithm took longet to train. The accuracy was 90% and AUC also around 90% which is lowest comare to DT and LR. C

**SVM:**
The SVM had to be performed on a subset of 5,000 datapoint and required extremely long fit time. For a subset of 10% of the data the gridsearch and fit time took over 100 minutes. For the impracticality of such model in real time and lackluster result, I do not believe such model to be optimal.

**Decision Tree:**
The decision tree offered a very similar AUC compared to the logistic regression close to 93%. Accuracy is also very close to LR but much higher F1 score. Prcision is little lower. Overall it took the least time with highest AUC score.

**Choice of the Model:**
- Decision Tree has best Performance, AUC comparable to Logistic Regression at 0.93 and best F1 at 0.59.
- Training time is also least when compared to LR, KNN and SVM.

**Future:**
These models an be further exlplored with differnet feature selections.

- Exploring further parameters for the top two models (logistic regression and decision trees). Particularly decision tree because of least time to train with highest score.
- Include more features in the analysis, this may increase the time to train but model efficency may improve.