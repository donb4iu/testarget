# A simple project with a simple Dataset

## References

- [Day — 1: 30 Days Machine Learning Projects Challenge; A simple project with a simple Dataset](https://medium.com/@iabbasali/day-1-30-days-machine-learning-project-challenge-77cd16756738)

## Code

- [app.py](https://github.com/donb4iu/30dayML/blob/main/30days/day1/app.py)

## Execution

```
#( 08/30/24@ 5:03PM )( donbuddenbaum@donbs-imac ):~/Documents/30dayML@main✗✗✗
   /Users/donbuddenbaum/.pyenv/versions/3.12.3/bin/python /Users/donbuddenbaum/Documents/30dayML/30days/day1/app.py
Current directory: /Users/donbuddenbaum/Documents/30dayML
CSV file loaded successfully.
(5, 5)
   CustomerID   Gender   Age   Annual Income (k$)   Spending Score (1-100)
0           1     Male    19                   15                       39
1           2     Male    21                   15                       81
2           3   Female    20                   16                        6
3           4   Female    23                   16                       77
4           5   Female    31                   17                       40
Index(['CustomerID', ' Gender', ' Age', ' Annual Income (k$)',
       ' Spending Score (1-100)'],
      dtype='object')
   CustomerID   Gender   Age  Annual Income  Spending Score
0           1     Male    19             15              39
1           2     Male    21             15              81
2           3   Female    20             16               6
3           4   Female    23             16              77
4           5   Female    31             17              40
Index(['CustomerID', 'Gender', ' Age', 'Annual Income', 'Spending Score'], dtype='object')
   CustomerID   Gender   Age  Annual Income
0           1     Male    19             15
1           2     Male    21             15
2           3   Female    20             16
3           4   Female    23             16
4           5   Female    31             17
0    39
1    81
2     6
3    77
4    40
Name: Spending Score, dtype: int64
training data
   CustomerID   Gender   Age  Annual Income
4           5   Female    31             17
0           1     Male    19             15
2           3   Female    20             16
3           4   Female    23             16
4    40
0    39
2     6
3    77
Name: Spending Score, dtype: int64
fit training data
   CustomerID  Gender   Age  Annual Income
4           5       0    31             17
0           1       1    19             15
2           3       0    20             16
3           4       0    23             16
   CustomerID  Gender   Age  Annual Income
1           2       0    21             15
4    40
0    39
2     6
3    77
Name: Spending Score, dtype: int64
1    81
Name: Spending Score, dtype: int64
svm_mae:  41.76673322864785
dt_mae:  42.0
mean_absolute_error:  41.433572019151185
lr_prediction:  [37.77327935]
lr_mas:  43.22672064777329
```