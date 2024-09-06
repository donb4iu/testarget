# Association Rule Learning Using FP-Growth 🥛🍞🧈



## References

- [Day — 28: 30 Days Machine Learning Project Challenge;
Association Rule Learning Using FP-Growth 🥛🍞🧈](https://medium.com/@iabbasali/day-28-30-days-machine-learning-project-challenge-8b6805cf3b8e)


## Datasets

- []()   

## Code

- [app.py](https://github.com/donb4iu/30dayML/blob/main/30days/day28/app.py)

## Execution
  
```
 #( 09/01/24@ 3:23PM )( donbuddenbaum@donbs-imac ):~/Documents/30dayML@main✗✗✗
   /Users/donbuddenbaum/.pyenv/versions/3.12.3/bin/python /Users/donbuddenbaum/Documents/30dayML/30days/day28/app.py
[[ True  True  True False  True  True False  True False False False]
 [ True  True  True  True  True  True False False False False False]
 [False False  True False False  True False  True  True False False]
 [ True False  True False False False False  True  True False  True]
 [False False  True False  True  True  True False  True  True False]]
['Banana', 'Biscuit', 'Bread', 'Coffee', 'Curd', 'Eggs', 'Ice cream', 'Milk', 'Salt', 'Sugar', 'Unicorn']
   Banana  Biscuit  Bread  Coffee   Curd   Eggs  Ice cream   Milk   Salt  Sugar  Unicorn
0    True     True   True   False   True   True      False   True  False  False    False
1    True     True   True    True   True   True      False  False  False  False    False
2   False    False   True   False  False   True      False   True   True  False    False
3    True    False   True   False  False  False      False   True   True  False     True
4   False    False   True   False   True   True       True  False   True   True    False
    support   itemsets
0       1.0        (2)
1       0.8        (5)
2       0.6        (7)
3       0.6        (4)
4       0.6        (0)
5       0.6        (8)
6       0.8     (2, 5)
7       0.6     (2, 7)
8       0.6     (4, 5)
9       0.6     (2, 4)
10      0.6  (2, 4, 5)
11      0.6     (0, 2)
12      0.6     (8, 2)
    support             itemsets
0       1.0              (Bread)
1       0.8               (Eggs)
2       0.6               (Milk)
3       0.6               (Curd)
4       0.6             (Banana)
5       0.6               (Salt)
6       0.8        (Bread, Eggs)
7       0.6        (Bread, Milk)
8       0.6         (Eggs, Curd)
9       0.6        (Bread, Curd)
10      0.6  (Bread, Curd, Eggs)
11      0.6      (Bread, Banana)
12      0.6        (Bread, Salt)
```