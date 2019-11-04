# Fraud-detection-scorecard-model-establishment-and-evaluation
Individual project to implement what I learned about fraud detection in past internship in 51 Credit Card Inc. based on machine learning 

(Keep updating)

Special thanks: 
Thanks 51 Credit Card Inc. for the internship opportunity. It enabled me to learn about how to do risk management in a data science and Algorithm ways. Truly appreciate the help from my lovly colleague in that wonderful summer.

Thanks the data provider, PPDAI Group Inc.

Thanks the warmhearted internet friend from Stackoverflow and CSDN. They provide solutions for many problems I faced and also provide some baseline code for me to work on.

The data set is from a previous algorithm risk management competition established by PPDAI Group Inc (NYSE: PPDF), which locates in Shanghai and is one of the largest P2P small loan compamy in China.

https://ai.ppdai.com/mirror/showCompetitionRisk

----------------------------------------------------------------------------------------------------------------------
For me, the propose of this project is to implement traditional fraud detection score card model based on advanced algoritms. The traditional ways were learned from my part internship experience in 51 Credit Card Inc. (2051.HK), which locates in Hangzhou and is a unicorn in P2P loan and credit card management field.

The traditinal methods including special approach dealing with missing data in data cleaning, set continous variables into bins to make all features discrete, create bins based on chi-squared values and make them to have monotonous bad sample rate (in order to be meaningfull for interpretation), code bins with WOE, and selected important non-multicollinear features using IV, VIF value and logistic regression. What's more the probability predicted by model will be convert to a score, which is actually the meaning for 'Score Card' model.

In the company, my colleague use GBDT to train the fraud detection model in last summer. I will try many different methods to make the prediction.

After that, some good models will be evaluated based on KS and AUC.

Note: If you are interested in more advanced ways of risk management based on data science in this company, and you can understand Chinese, you can visit the wonderful Zhihu Column page made by my colleague, which contains many great articles.
https://zhuanlan.zhihu.com/c_1156982447794233344

----------------------------------------------------------------------------------------------------------------------

Brief Introduction of whole project:

•	Processed feature engineering base on time difference, time slicing, updating condition and data centralization.
•	Transformed original data into bins of monotonous bad sample rate based on chi-squared values and missing conditions.
•	Coded bins with WOE. Selected important non-multicollinear features using IV, VIF value and logistic regression.
•	Established logistic regression, GBDT, Xgboost, DNN and stacking models to predict default rates and transformed probabilities to scores of clients. The KS is higher than 0.45, AUC and accuracy all higher than 0.9.
