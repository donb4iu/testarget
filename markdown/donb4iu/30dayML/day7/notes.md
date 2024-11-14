# Heart Disease Prediction 💓

![alt text](image.png)

## References

- [Day — 7: 30 Days Machine Learning Projects Challenge;
Heart Disease Prediction💓](https://medium.com/@iabbasali/day-7-30-days-machine-learning-projects-challenge-35759be25a8e)

https://youtu.be/trdAMww0ODg

## Datasets

- [Heart Disease Prediction Dataset](https://www.kaggle.com/datasets/utkarshx27/heart-disease-diagnosis-dataset) 

## Code

- [app.py](https://github.com/donb4iu/30dayML/blob/main/30days/day7/app.py)

## Execution

```
#( 08/30/24@ 5:12PM )( donbuddenbaum@donbs-imac ):~/Documents/30dayML@main✗✗✗
   /Users/donbuddenbaum/.pyenv/versions/3.12.3/bin/python /Users/donbuddenbaum/Documents/30dayML/30days/day7/app.py
   age  sex   chest pain type  resting blood pressure  serum cholestoral  fasting blood sugar  ...  exercise induced angina  oldpeak  ST segment  major vessels  thal  heart disease
0   70     1                4                     130                322                    0  ...                        0      2.4           2              3     3              2
1   67     0                3                     115                564                    0  ...                        0      1.6           2              0     7              1
2   57     1                2                     124                261                    0  ...                        0      0.3           1              0     7              2
3   64     1                4                     128                263                    0  ...                        1      0.2           2              1     7              1
4   74     0                2                     120                269                    0  ...                        1      0.2           1              1     3              1

[5 rows x 14 columns]
Index(['age', 'sex ', 'chest pain type', 'resting blood pressure',
       'serum cholestoral', 'fasting blood sugar',
       'resting electrocardiographic results', 'max heart rate',
       'exercise induced angina', 'oldpeak', 'ST segment', 'major vessels',
       'thal', 'heart disease'],
      dtype='object')
(270, 14)
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 270 entries, 0 to 269
Data columns (total 14 columns):
 #   Column                                Non-Null Count  Dtype  
---  ------                                --------------  -----  
 0   age                                   270 non-null    int64  
 1   sex                                   270 non-null    int64  
 2   chest pain type                       270 non-null    int64  
 3   resting blood pressure                270 non-null    int64  
 4   serum cholestoral                     270 non-null    int64  
 5   fasting blood sugar                   270 non-null    int64  
 6   resting electrocardiographic results  270 non-null    int64  
 7   max heart rate                        270 non-null    int64  
 8   exercise induced angina               270 non-null    int64  
 9   oldpeak                               270 non-null    float64
 10  ST segment                            270 non-null    int64  
 11  major vessels                         270 non-null    int64  
 12  thal                                  270 non-null    int64  
 13  heart disease                         270 non-null    int64  
dtypes: float64(1), int64(13)
memory usage: 29.7 KB
None
age                                     0
sex                                     0
chest pain type                         0
resting blood pressure                  0
serum cholestoral                       0
fasting blood sugar                     0
resting electrocardiographic results    0
max heart rate                          0
exercise induced angina                 0
oldpeak                                 0
ST segment                              0
major vessels                           0
thal                                    0
heart disease                           0
dtype: int64

 dtc_scores:  [0.61111111 0.7037037  0.77777778 0.72222222 0.83333333]

 dtc_scores.mean():  0.7296296296296296

 model:  DecisionTreeClassifier()  mean score:  0.7222222222222222

 model:  RandomForestClassifier()  mean score:  0.8074074074074072

 model:  XGBClassifier(base_score=None, booster=None, callbacks=None,
              colsample_bylevel=None, colsample_bynode=None,
              colsample_bytree=None, device=None, early_stopping_rounds=None,
              enable_categorical=False, eval_metric=None, feature_types=None,
              gamma=None, grow_policy=None, importance_type=None,
              interaction_constraints=None, learning_rate=None, max_bin=None,
              max_cat_threshold=None, max_cat_to_onehot=None,
              max_delta_step=None, max_depth=None, max_leaves=None,
              min_child_weight=None, missing=nan, monotone_constraints=None,
              multi_strategy=None, n_estimators=None, n_jobs=None,
              num_parallel_tree=None, random_state=None, ...)  mean score:  0.7814814814814814

 rfc score:  0.8888888888888888
```