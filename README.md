# Credit Risk Analysis

## Objects: :credit_card:

* Explain how a machine learning algorithm is used in data analytics.
* Create training and test groups from a given data set.
* Implement the logistic regression, decision tree, random forest, and support vector machine algorithms.
* Interpret the results of the logistic regression, decision tree, random forest, and support vector machine algorithms.
* Compare the advantages and disadvantages of each supervised learning algorithm.
* Determine which supervised learning algorithm is best used for a given data set or scenario.
* Use ensemble and resampling techniques to improve model performance.


The objective of this project was to focused on cultivating knowledge and skills in data preparation, statistical reasoning, and machine learning (ML),  to analyze credit risk to provide a quicker and more reliable loan experience, with the support of the tools we could provide a quicker and more reliable loan experience  which were required for solving a real-world challenge: credit card risk. During the completion of this project we mainly leveraged the powerful features offered by Scikit-learn User Guide - Supervised Learning, Python imbalanced-learn, and their supporting packages/libraries/dependencies that let us explore, train, and study various supervised learning models and resources, such as random oversampling technique (RandomOverSampler), synthetic minority oversampling technique (SMOTE), cluster centroid undersampling technique (ClusterCentroids), and a combination of SMOTE and edited nearest neighbors algorithms (SMOTEENN) to predict credit risk. 


### Resources

`Dataset:`


- [x] credit_risk_resampling.ipynb
- [x] credit_risk_ensemble.ipynb


`Software used:`


- [x] Python 3.7
- [x] Jupyter Notebook
- [x] NumPy, version 1.11 or later
- [x] SciPy, version 0.18 or later
- [x] Scikit-learn, version 0.21 or later
- [x] Logistic Regression and Random Forest models
- [x] Ensemble and resampling techinques


> ## Credit Risk Ensemble

**Split the Data into Training and Testing**

![Capture](https://user-images.githubusercontent.com/114257085/218911408-5787b51c-c2f1-45ad-b379-c832d8098bc7.PNG)

**Ensemble Learners**

![Capture](https://user-images.githubusercontent.com/114257085/218911932-f8d97dc1-7186-4afb-a361-73a6f8d42833.PNG)
![Capture](https://user-images.githubusercontent.com/114257085/218912296-f65f765d-a99c-4cfc-baf8-92cef2214f4d.PNG)

**Easy Ensemble AdaBoost Classifier**


![Capture](https://user-images.githubusercontent.com/114257085/218912760-ad213142-e3a6-4f93-a829-2998332dd054.PNG)

> ## Credit Risk Resampling Techniques

![Capture](https://user-images.githubusercontent.com/114257085/218913232-ee5e159b-2c2b-4e97-827b-78cf2ffc7baf.PNG)



**Naive Random Oversampling**

Oversampling is a great strategy. The idea is simple and intuitive: If one class has too few instances in the training set, we choose more instances from that class for training until it's larger.

![Capture](https://user-images.githubusercontent.com/114257085/218913393-895def40-0518-49de-8d13-65144c7ab7af.PNG)

**SMOTE Oversampling**

![Capture](https://user-images.githubusercontent.com/114257085/218913509-2ebdcb8c-e096-4112-b11f-d616fa335f53.PNG)

**Undersampling**

![Capture](https://user-images.githubusercontent.com/114257085/218913667-99197e64-e2dd-4edd-8a8d-5e752f06e29e.PNG)

**Combination (Over and Under) Sampling**

![Capture](https://user-images.githubusercontent.com/114257085/218913994-59b83485-7756-4769-b489-198539517b73.PNG)


## Summary:

All deliverables have been completed and analyzed according to the assignment requirements, including code refactoring, properly formatted outputs, and quality assurance for ensuring accurate results. I hope our users and stakeholders will be able to benefit from the condensed summary statistics tables instead of bulleted lists and easily compare the results achieved by applying various machine learning algorithms before drawing the final conclusions.


In the financial industry, sensitivity is more valuable than precision for analyzing risk and default rates on loan candidates. This because banks want to be able to mark all of the high-risk individuals as high-risk for them not to default. It doesn't matter if it is not as precise as long as the posible defaults are marked as that.

In terms of precision, all six algorithms had a really low precision rate for high risk individuals. The highest one was the Easy Ensemble AdaBoost Classifier with 7% precision which is still considered pretty low for finding these high risk individuals not to give loans to. This means that out of all the customers marked as high-risk 7% were actually high-risk. On the other hand, all the models had a perfect precision for low-risk individiauls meaning that all of the low-risk customers were marked as that.

Having this in mind, precision is not telling us much information to compare the algorithms, so we should take a look at sensitivity. The model with the highest sensitivity was the easy ensemble adaboost classifier (91% for high-risk and 94% for low-risk individuals), meaning that 91% of the time all the high-risk individuals are marked as high-risk individuals. Followed by this model, the other two with high recall were the Random Forest Classifier (67%) and SMOTEENN Resample (70%).

And last but not least, we are going to look at the balanced accuracy score to make the final decision of which model to use. The accuracy score stands for how correct was the model, meaning out of all the predictions how many of them were true to the classification. As we were able to see, the model with the highest accuracy score by far was the Easy Ensemble AdaBoost Classifier. So, this should be the one we chose because of its high accuracy, highest precision, and highest sensitivity.





