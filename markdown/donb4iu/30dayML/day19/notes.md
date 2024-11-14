# Apriori Algorithm🥛🍞🧈

![alt text](image.png)

## References

- [Day — 19: 30 Days Machine Learning Projects Challenge;
Apriori Algorithm🥛🍞🧈](https://medium.com/@iabbasali/day-19-30-days-machine-learning-projects-challenge-2a376b9d3438)

## Datasets
**didn't use any datasets**
- [Market Basket Analysis](https://www.kaggle.com/code/xvivancos/market-basket-analysis#header)   

## Code

- [app.py](https://github.com/donb4iu/30dayML/blob/main/30days/day19/app.py)


## Execution


```
#( 08/31/24@ 4:40PM )( donbuddenbaum@donbs-imac ):~/Documents/30dayML@main✗✗✗
   /Users/donbuddenbaum/.pyenv/versions/3.12.3/bin/python /Users/donbuddenbaum/Documents/30dayML/30days/day19/app.py
   Transaction ID                        Items
0               1                [bread, milk]
1               2  [bread, diaper, beer, eggs]
2               3   [milk, diaper, beer, cola]
3               4  [bread, milk, diaper, beer]
4               5  [bread, milk, diaper, cola]
   Transaction ID                   Items
0               1              bread,milk
1               2  bread,diaper,beer,eggs
2               3   milk,diaper,beer,cola
3               4  bread,milk,diaper,beer
4               5  bread,milk,diaper,cola
   beer  bread  cola  diaper  eggs  milk
0     0      1     0       0     0     1
1     1      1     0       1     1     0
2     1      0     1       1     0     1
3     1      1     0       1     0     1
4     0      1     1       1     0     1
    beer  bread   cola  diaper   eggs   milk
0  False   True  False   False  False   True
1   True   True  False    True   True  False
2   True  False   True    True  False   True
3   True   True  False    True  False   True
4  False   True   True    True  False   True
/Users/donbuddenbaum/.pyenv/versions/3.12.3/lib/python3.12/site-packages/mlxtend/frequent_patterns/fpcommon.py:109: DeprecationWarning: DataFrames with non-bool types result in worse computationalperformance and their support might be discontinued in the future.Please use a DataFrame with bool type
  warnings.warn(
    support               itemsets
0       0.6                 (beer)
1       0.8                (bread)
2       0.4                 (cola)
3       0.8               (diaper)
4       0.8                 (milk)
5       0.4          (beer, bread)
6       0.6         (diaper, beer)
7       0.4           (beer, milk)
8       0.6        (diaper, bread)
9       0.6          (milk, bread)
10      0.4         (diaper, cola)
11      0.4           (cola, milk)
12      0.6         (diaper, milk)
13      0.4  (diaper, beer, bread)
14      0.4   (diaper, beer, milk)
15      0.4  (diaper, milk, bread)
16      0.4   (diaper, cola, milk)
    support               itemsets
0       0.6                 (beer)
1       0.8                (bread)
2       0.4                 (cola)
3       0.8               (diaper)
4       0.8                 (milk)
5       0.4          (beer, bread)
6       0.6         (diaper, beer)
7       0.4           (beer, milk)
8       0.6        (diaper, bread)
9       0.6          (milk, bread)
10      0.4         (diaper, cola)
11      0.4           (cola, milk)
12      0.6         (diaper, milk)
13      0.4  (diaper, beer, bread)
14      0.4   (diaper, beer, milk)
15      0.4  (diaper, milk, bread)
16      0.4   (diaper, cola, milk)
       antecedents     consequents  antecedent support  consequent support  support  confidence      lift  leverage  conviction  zhangs_metric
0         (diaper)          (beer)                 0.8                 0.6      0.6        0.75  1.250000      0.12         1.6       1.000000
1           (beer)        (diaper)                 0.6                 0.8      0.6        1.00  1.250000      0.12         inf       0.500000
2         (diaper)         (bread)                 0.8                 0.8      0.6        0.75  0.937500     -0.04         0.8      -0.250000
3          (bread)        (diaper)                 0.8                 0.8      0.6        0.75  0.937500     -0.04         0.8      -0.250000
4           (milk)         (bread)                 0.8                 0.8      0.6        0.75  0.937500     -0.04         0.8      -0.250000
5          (bread)          (milk)                 0.8                 0.8      0.6        0.75  0.937500     -0.04         0.8      -0.250000
6           (cola)        (diaper)                 0.4                 0.8      0.4        1.00  1.250000      0.08         inf       0.333333
7           (cola)          (milk)                 0.4                 0.8      0.4        1.00  1.250000      0.08         inf       0.333333
8         (diaper)          (milk)                 0.8                 0.8      0.6        0.75  0.937500     -0.04         0.8      -0.250000
9           (milk)        (diaper)                 0.8                 0.8      0.6        0.75  0.937500     -0.04         0.8      -0.250000
10   (beer, bread)        (diaper)                 0.4                 0.8      0.4        1.00  1.250000      0.08         inf       0.333333
11    (beer, milk)        (diaper)                 0.4                 0.8      0.4        1.00  1.250000      0.08         inf       0.333333
12  (diaper, cola)          (milk)                 0.4                 0.8      0.4        1.00  1.250000      0.08         inf       0.333333
13    (cola, milk)        (diaper)                 0.4                 0.8      0.4        1.00  1.250000      0.08         inf       0.333333
14          (cola)  (diaper, milk)                 0.4                 0.6      0.4        1.00  1.666667      0.16         inf       0.666667
       antecedents     consequents  antecedent support  consequent support  support  confidence      lift  leverage  conviction  zhangs_metric
0         (diaper)          (beer)                 0.8                 0.6      0.6        0.75  1.250000      0.12         1.6       1.000000
1           (beer)        (diaper)                 0.6                 0.8      0.6        1.00  1.250000      0.12         inf       0.500000
2         (diaper)         (bread)                 0.8                 0.8      0.6        0.75  0.937500     -0.04         0.8      -0.250000
3          (bread)        (diaper)                 0.8                 0.8      0.6        0.75  0.937500     -0.04         0.8      -0.250000
4           (milk)         (bread)                 0.8                 0.8      0.6        0.75  0.937500     -0.04         0.8      -0.250000
5          (bread)          (milk)                 0.8                 0.8      0.6        0.75  0.937500     -0.04         0.8      -0.250000
6           (cola)        (diaper)                 0.4                 0.8      0.4        1.00  1.250000      0.08         inf       0.333333
7           (cola)          (milk)                 0.4                 0.8      0.4        1.00  1.250000      0.08         inf       0.333333
8         (diaper)          (milk)                 0.8                 0.8      0.6        0.75  0.937500     -0.04         0.8      -0.250000
9           (milk)        (diaper)                 0.8                 0.8      0.6        0.75  0.937500     -0.04         0.8      -0.250000
10   (beer, bread)        (diaper)                 0.4                 0.8      0.4        1.00  1.250000      0.08         inf       0.333333
11    (beer, milk)        (diaper)                 0.4                 0.8      0.4        1.00  1.250000      0.08         inf       0.333333
12  (diaper, cola)          (milk)                 0.4                 0.8      0.4        1.00  1.250000      0.08         inf       0.333333
13    (cola, milk)        (diaper)                 0.4                 0.8      0.4        1.00  1.250000      0.08         inf       0.333333
14          (cola)  (diaper, milk)                 0.4                 0.6      0.4        1.00  1.666667      0.16         inf       0.666667

```