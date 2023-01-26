# CTR Prediction - 2022 DIGIX Global AI Challenge

# OBJECTIVE
Predict the Click Rate thrgouh cross-domain data from model ads and news feeds.

# DATA
This is 2022 DIGIX Global AI Challenge. I got the dataset here:
https://www.kaggle.com/datasets/xiaojiu1414/digix-global-ai-challenge

Notes for the data:
- It said to be a challenge for CTR prediction, but the label is 1 or 0, so I regarded it as click rate prediction.
- There are two training sets, as ads and news feeds.
- 7,675,517 observasitions
- 35 features, info are hidden: 

    -User’s profiles: age, gender, residence, etc.
    
    -User’s device specs: size, version, etc.
    
    -User behavior logs: refresh time
    
    -Ad material info: creative type, what app is the ad in, who is the client of the ad, etc.

# PROGRESS
## Data Cleaning
The data provided has been unified to same formats. The timestamps need to be deciphered. Some catogorical feature need to be OHC.

## EDA
- This a very unbalanced dataset, 98.4% | 1.56%

<img src="https://user-images.githubusercontent.com/73181107/214952369-4a0f3257-9ffd-4e50-8ef7-b82752eaadc8.png" width="300">


- time-consuming, run with smaller subset

## Model
### Models used
desicion tree, balanced random forest, XGBoost with GPU

### Baseline

all models tested are working badly for recall (~0.2)
    
## Checklist
- [ ] OHC categorical feature, and run in the model
- [ ] fine tune models
- [ ] try with TensorFlow

