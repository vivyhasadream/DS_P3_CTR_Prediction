# CTR Prediction - 2022 DIGIX Global AI Challenge
CTR prediction through cross-domain data from ads and news feeds


# DATA
https://www.kaggle.com/datasets/xiaojiu1414/digix-global-ai-challenge

It provived with 2 training set, and 2 testing set.

Testing sets are without the labels for prediction, it might be used for submissions.

Only the training set for the ads was used at the current stage.

7,675,517  ~7.6M

35 features

    User’s profiles: age, gender, residence, etc.

    User’s device specs: size, version, etc.

    User behavior logs: refresh time

    Ad material info: creative type, what app is the ad in, who is the client of the ad, etc.


# OBJECTIVE
Predict the CTR, which is the feature called 'label' in the dataset.


# PROGRESS
**1. data cleaning**

    **1.1 full dataset:** half way done

    **1.2 subset:** sample size 100K, for quicker EDA

**2. EDA**

    **2.1 full dataset: **not done yet

    **2.2 subset: **sample size 100K

**3. model**

    **3.1 baseline attempts: **

    train and test on the full baseline

    models tested: desicion tree, balanced random forest

   ** 3.2 subset:** for easier testing 

    train and test on 100K 

    models tested: desicion tree, balanced random forest, xgboost

    **3.3 using XGBoost with GPU**

    test on both subset and full dataset
    

# CURRENT CONCLUSION
**- models:**

    all models tested are working badly for recall (~0.2), 

    new models should be introduced,

    or use neural network.

**- features:**

    in the dataset are not directly related to the target,

    needs to be constructed more.
    
    and consider to combine the two datasets together.

