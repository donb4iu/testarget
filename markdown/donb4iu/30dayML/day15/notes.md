# Students Performance Prediction 🧑‍🎓

![alt text](image.png)

## References

- [Day — 15: 30 Days Machine Learning Projects Challenge;
Students Performance Prediction 🧑‍🎓] (https://medium.com/@iabbasali/day-15-30-days-machine-learning-projects-challenge-da1a9bb77962)

## Datasets

- [Student Performance (Multiple Linear Regression)](https://www.kaggle.com/datasets/nikhil7280/student-performance-multiple-linear-regression)

## Code

- [app.py](https://github.com/donb4iu/30dayML/blob/main/30days/day15/app.py)

## Execution


```
#( 08/31/24@10:45AM )( donbuddenbaum@donbs-imac ):~/Documents/30dayML@main✗✗✗
   /Users/donbuddenbaum/.pyenv/versions/3.12.3/bin/python /Users/donbuddenbaum/Documents/30dayML/30days/day15/app.py
   Hours Studied  Previous Scores Extracurricular Activities  Sleep Hours  Sample Question Papers Practiced  Performance Index
0              7               99                        Yes            9                                 1               91.0
1              4               82                         No            4                                 2               65.0
2              8               51                        Yes            7                                 2               45.0
3              5               52                        Yes            5                                 2               36.0
4              7               75                         No            8                                 5               66.0
Hours Studied                       0
Previous Scores                     0
Extracurricular Activities          0
Sleep Hours                         0
Sample Question Papers Practiced    0
Performance Index                   0
dtype: int64
(10000, 6)
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 10000 entries, 0 to 9999
Data columns (total 6 columns):
 #   Column                            Non-Null Count  Dtype  
---  ------                            --------------  -----  
 0   Hours Studied                     10000 non-null  int64  
 1   Previous Scores                   10000 non-null  int64  
 2   Extracurricular Activities        10000 non-null  object 
 3   Sleep Hours                       10000 non-null  int64  
 4   Sample Question Papers Practiced  10000 non-null  int64  
 5   Performance Index                 10000 non-null  float64
dtypes: float64(1), int64(4), object(1)
memory usage: 468.9+ KB
None
       Hours Studied  Previous Scores   Sleep Hours  Sample Question Papers Practiced  Performance Index
count   10000.000000     10000.000000  10000.000000                      10000.000000       10000.000000
mean        4.992900        69.445700      6.530600                          4.583300          55.224800
std         2.589309        17.343152      1.695863                          2.867348          19.212558
min         1.000000        40.000000      4.000000                          0.000000          10.000000
25%         3.000000        54.000000      5.000000                          2.000000          40.000000
50%         5.000000        69.000000      7.000000                          5.000000          55.000000
75%         7.000000        85.000000      8.000000                          7.000000          71.000000
max         9.000000        99.000000      9.000000                          9.000000         100.000000
   Hours Studied  Previous Scores Extracurricular Activities  Sleep Hours  Sample Question Papers Practiced
0              7               99                        Yes            9                                 1
1              4               82                         No            4                                 2
2              8               51                        Yes            7                                 2
3              5               52                        Yes            5                                 2
4              7               75                         No            8                                 5
   Hours Studied  Previous Scores  Sleep Hours  Sample Question Papers Practiced  Extracurricular Activities_No  Extracurricular Activities_Yes
0              7               99            9                                 1                          False                            True
1              4               82            4                                 2                           True                           False
2              8               51            7                                 2                          False                            True
3              5               52            5                                 2                          False                            True
4              7               75            8                                 5                           True                           False
svr_mae:  1.8384445448641031
lr_mae:  1.6313121603176195
lr_pipeline_mae:  1.6313062853875844

```