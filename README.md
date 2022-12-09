# Capstone-Project-Machine-Learning-Classification
Health Insurance Cross Sell Prediction.
Capstone project on Machine Learning Classification Health Insurance Cross Sell Prediction.

1) Problem Statement
• Our client is an Insurance company that has provided Health Insurance to its customers now they need your help in building a model to predict whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company.

• An insurance policy is an arrangement by which a company undertakes to provide a guarantee of compensation for specified loss, damage, illness, or death in return for the payment of a specified premium. A premium is a sum of money that the customer needs to pay regularly to an insurance company for this guarantee.

• For example, you may pay a premium of Rs. 5000 each year for a health insurance cover of Rs. 200,000/- so that if, God forbid, you fall ill and need to be hospitalised in that year, the insurance provider company will bear the cost of hospitalisation etc. for upto Rs. 200,000. Now if you are wondering how can company bear such high hospitalisation cost when it charges a premium of only Rs. 5000/-, that is where the concept of probabilities comes in picture. For example, like you, there may be 100 customers who would be paying a premium of Rs. 5000 every year, but only a few of them (say 2-3) would get hospitalised that year and not everyone. This way everyone shares the risk of everyone else.

• Just like medical insurance, there is vehicle insurance where every year customer needs to pay a premium of certain amount to insurance provider company so that in case of unfortunate accident by the vehicle, the insurance provider company will provide a compensation (called ‘sum assured’) to the customer.

• Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

• Now, in order to predict, whether the customer would be interested in Vehicle insurance, you have information about demographics (gender, age, region code type), Vehicles (Vehicle Age, Damage), Policy (Premium, sourcing channel) etc.

2) Attribute Information
• id : Unique ID for the customer

• Gender : Gender of the customer

• Age : Age of the customer

• Driving_License 0 : Customer does not have DL, 1 : Customer already has DL

• Region_Code : Unique code for the region of the customer

• Previously_Insured : 1 : Customer already has Vehicle Insurance, 0 : Customer doesn't have Vehicle Insurance

• Vehicle_Age : Age of the Vehicle

• Vehicle_Damage :1 : Customer got his/her vehicle damaged in the past. 0 : Customer didn't get his/her vehicle damaged in the past.

• Annual_Premium : The amount customer needs to pay as premium in the year

• PolicySalesChannel : Anonymized Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.

• Vintage : Number of Days, Customer has been associated with the company

• Response : 1 : Customer is interested, 0 : Customer is not interested

3) Feature Engineering
In the data we used it has Primum and Age both has outliers, outlier capping is done with upper limit as 0.95 and lower limit as 0.05 for both the features. SMOTE is used used for over sampling due to class imbalance in the dependent variable. With the help of Heat map we reduced highly co-related features, with VIF we finalise our features and performed various models.

4) Hypothesis
• With EDA we can justify our hypothesis. • Vehicle previously insured will affect Response.(Fail to reject.) • Age will not affect Response.(Reject) • Driving license will not affect Response.(Reject) • There will be positive co relation in Vintage and Response.(Reject) • Vehicle damage will affect Response.(Fail to reject)

5) Model Implementation
After implementing various models on the given data such as Logistic Regression, Decision Tree Classifier, XG boost, Naïve Bays Classifier, SGD Classifier, Cat Boost Classifier, KNN Classifier, Gradient Boosting Classifier, AdaBoost Classifier, Random Forest Classifier. We get maximum accuracy with Decision Tree Classifier, Random Forest Classifier, XG boost but in case of Decision Tree and Random forest accuracy is decreased for testing data it is the case of Over fitting. In case of XG Boost accuracy decreases but with less percentage here there is no problem of overfitting. XG Boost with train and test accuracy as 0.88 and 0.81 Decision Tree Classifier with train and test accuracy 0.99 and 0.80 Random Forest Classifier with train and test accuracy as 0.99 and 0.81

6) Conclusion
• There will be more profit if company sells both health and vehicle insurance.

• Previously insured is important feature for cross sell.

• After implementation of various models we got best results from Decision tree classifier, Random forest classifier and XG boost classifier.

• Decision tree and Random forest are over fitting so finally we decide to go with XG boost.

• XG boost with train accuracy as 0.88 and test accuracy of 0.81

7) References
[1] “A Study on a car Insurance purchase Prediction Using Two-Class Logistic Regression and Two-Class Boosted Decision Tree” by Su Hyun AN1 , Seong Hee YEO2 , Minsoo KANG3

[2]”A study on the meaning of automobile in the no insurance automobile injury insurance” by Choi, B. G

[3]”Cross-selling through database marketing: a mixed data factor analyzer for data augmentation and prediction” by Wagner A. Kamakura

Any suggestions are welcomed...
