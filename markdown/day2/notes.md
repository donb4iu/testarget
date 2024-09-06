# Wine Quality Prediction 🍷

![alt text](image.png)

## References

- [Day — 2: 30 Days Machine Learning Projects Challenge;
Wine Quality Prediction🍷](https://medium.com/@iabbasali/day-2-30-days-machine-learning-projects-challenge-9fb626063275)

## Datasets

- [Wine Quality Dataset](https://www.kaggle.com/datasets/rajyellow46/wine-quality)

## Code

- [app.py](https://github.com/donb4iu/30dayML/blob/main/30days/day2/app.py)

## Execution

```
#( 08/30/24@ 5:05PM )( donbuddenbaum@donbs-imac ):~/Documents/30dayML@main✗✗✗
   /Users/donbuddenbaum/.pyenv/versions/3.12.3/bin/python /Users/donbuddenbaum/Documents/30dayML/30days/day2/app.py
2.1.1
    type  fixed acidity  volatile acidity  citric acid  residual sugar  chlorides  free sulfur dioxide  total sulfur dioxide  density    pH  sulphates  alcohol  quality
0  white            7.0              0.27         0.36            20.7      0.045                 45.0                 170.0   1.0010  3.00       0.45      8.8        6
1  white            6.3              0.30         0.34             1.6      0.049                 14.0                 132.0   0.9940  3.30       0.49      9.5        6
2  white            8.1              0.28         0.40             6.9      0.050                 30.0                  97.0   0.9951  3.26       0.44     10.1        6
3  white            7.2              0.23         0.32             8.5      0.058                 47.0                 186.0   0.9956  3.19       0.40      9.9        6
4  white            7.2              0.23         0.32             8.5      0.058                 47.0                 186.0   0.9956  3.19       0.40      9.9        6
                       count        mean        std      min       25%        50%        75%        max
fixed acidity         6487.0    7.216579   1.296750  3.80000   6.40000    7.00000    7.70000   15.90000
volatile acidity      6489.0    0.339691   0.164649  0.08000   0.23000    0.29000    0.40000    1.58000
citric acid           6494.0    0.318722   0.145265  0.00000   0.25000    0.31000    0.39000    1.66000
residual sugar        6495.0    5.444326   4.758125  0.60000   1.80000    3.00000    8.10000   65.80000
chlorides             6495.0    0.056042   0.035036  0.00900   0.03800    0.04700    0.06500    0.61100
free sulfur dioxide   6497.0   30.525319  17.749400  1.00000  17.00000   29.00000   41.00000  289.00000
total sulfur dioxide  6497.0  115.744574  56.521855  6.00000  77.00000  118.00000  156.00000  440.00000
density               6497.0    0.994697   0.002999  0.98711   0.99234    0.99489    0.99699    1.03898
pH                    6488.0    3.218395   0.160748  2.72000   3.11000    3.21000    3.32000    4.01000
sulphates             6493.0    0.531215   0.148814  0.22000   0.43000    0.51000    0.60000    2.00000
alcohol               6497.0   10.491801   1.192712  8.00000   9.50000   10.30000   11.30000   14.90000
quality               6497.0    5.818378   0.873255  3.00000   5.00000    6.00000    6.00000    9.00000
Index(['type', 'fixed acidity', 'volatile acidity', 'citric acid',
       'residual sugar', 'chlorides', 'free sulfur dioxide',
       'total sulfur dioxide', 'density', 'pH', 'sulphates', 'alcohol',
       'quality'],
      dtype='object')
['white' 'red']
type                     0
fixed acidity           10
volatile acidity         8
citric acid              3
residual sugar           2
chlorides                2
free sulfur dioxide      0
total sulfur dioxide     0
density                  0
pH                       9
sulphates                4
alcohol                  0
quality                  0
dtype: int64
   type  fixed acidity  volatile acidity  citric acid  residual sugar  chlorides  free sulfur dioxide  total sulfur dioxide  density    pH  sulphates  alcohol  quality
0     1            7.0              0.27         0.36            20.7      0.045                 45.0                 170.0   1.0010  3.00       0.45      8.8        6
1     1            6.3              0.30         0.34             1.6      0.049                 14.0                 132.0   0.9940  3.30       0.49      9.5        6
2     1            8.1              0.28         0.40             6.9      0.050                 30.0                  97.0   0.9951  3.26       0.44     10.1        6
3     1            7.2              0.23         0.32             8.5      0.058                 47.0                 186.0   0.9956  3.19       0.40      9.9        6
4     1            7.2              0.23         0.32             8.5      0.058                 47.0                 186.0   0.9956  3.19       0.40      9.9        6
[6 5 7 8 4 3 9]
X_train.shape:  (5197, 12) X_test.shape:  (1300, 12)
[1 1 0 ... 1 1 1]
0.7469230769230769
[1 0 1 ... 0 0 1]
0.6746153846153846
0.7407692307692307
```