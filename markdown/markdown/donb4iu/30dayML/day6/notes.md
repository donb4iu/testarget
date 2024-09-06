# California Housing Prices 🗺️

![alt text](image.png)

## References

- [Day — 6: 30 Days Machine Learning Projects Challenge;
California Housing Prices🗺️](https://medium.com/@iabbasali/day-6-30-days-machine-learning-projects-challenge-e934c2ca1abe)


**Hands-on Machine Learning with Scikit-Learn, Keras & TensorFlow**


## Datasets

- [California Housing Prices](https://www.kaggle.com/camnugent/california-housing-prices)

## Code

- [app.py](https://github.com/donb4iu/30dayML/blob/main/30days/day6/app.py)

## Execution

```
#( 08/30/24@ 5:09PM )( donbuddenbaum@donbs-imac ):~/Documents/30dayML@main✗✗✗
   /Users/donbuddenbaum/.pyenv/versions/3.12.3/bin/python /Users/donbuddenbaum/Documents/30dayML/30days/day6/app.py
   longitude  latitude  housing_median_age  total_rooms  total_bedrooms  population  households  median_income  median_house_value ocean_proximity
0    -122.23     37.88                41.0        880.0           129.0       322.0       126.0         8.3252            452600.0        NEAR BAY
1    -122.22     37.86                21.0       7099.0          1106.0      2401.0      1138.0         8.3014            358500.0        NEAR BAY
2    -122.24     37.85                52.0       1467.0           190.0       496.0       177.0         7.2574            352100.0        NEAR BAY
3    -122.25     37.85                52.0       1274.0           235.0       558.0       219.0         5.6431            341300.0        NEAR BAY
4    -122.25     37.85                52.0       1627.0           280.0       565.0       259.0         3.8462            342200.0        NEAR BAY
       longitude  latitude  housing_median_age  total_rooms  total_bedrooms  population  households  median_income  median_house_value ocean_proximity
20635    -121.09     39.48                25.0       1665.0           374.0       845.0       330.0         1.5603             78100.0          INLAND
20636    -121.21     39.49                18.0        697.0           150.0       356.0       114.0         2.5568             77100.0          INLAND
20637    -121.22     39.43                17.0       2254.0           485.0      1007.0       433.0         1.7000             92300.0          INLAND
20638    -121.32     39.43                18.0       1860.0           409.0       741.0       349.0         1.8672             84700.0          INLAND
20639    -121.24     39.37                16.0       2785.0           616.0      1387.0       530.0         2.3886             89400.0          INLAND
(20640, 10)
longitude               0
latitude                0
housing_median_age      0
total_rooms             0
total_bedrooms        207
population              0
households              0
median_income           0
median_house_value      0
ocean_proximity         0
dtype: int64
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 20640 entries, 0 to 20639
Data columns (total 10 columns):
 #   Column              Non-Null Count  Dtype  
---  ------              --------------  -----  
 0   longitude           20640 non-null  float64
 1   latitude            20640 non-null  float64
 2   housing_median_age  20640 non-null  float64
 3   total_rooms         20640 non-null  float64
 4   total_bedrooms      20433 non-null  float64
 5   population          20640 non-null  float64
 6   households          20640 non-null  float64
 7   median_income       20640 non-null  float64
 8   median_house_value  20640 non-null  float64
 9   ocean_proximity     20640 non-null  object 
dtypes: float64(9), object(1)
memory usage: 1.6+ MB
None
          longitude      latitude  housing_median_age   total_rooms  total_bedrooms    population    households  median_income  median_house_value
count  20640.000000  20640.000000        20640.000000  20640.000000    20433.000000  20640.000000  20640.000000   20640.000000        20640.000000
mean    -119.569704     35.631861           28.639486   2635.763081      537.870553   1425.476744    499.539680       3.870671       206855.816909
std        2.003532      2.135952           12.585558   2181.615252      421.385070   1132.462122    382.329753       1.899822       115395.615874
min     -124.350000     32.540000            1.000000      2.000000        1.000000      3.000000      1.000000       0.499900        14999.000000
25%     -121.800000     33.930000           18.000000   1447.750000      296.000000    787.000000    280.000000       2.563400       119600.000000
50%     -118.490000     34.260000           29.000000   2127.000000      435.000000   1166.000000    409.000000       3.534800       179700.000000
75%     -118.010000     37.710000           37.000000   3148.000000      647.000000   1725.000000    605.000000       4.743250       264725.000000
max     -114.310000     41.950000           52.000000  39320.000000     6445.000000  35682.000000   6082.000000      15.000100       500001.000000
['NEAR BAY' '<1H OCEAN' 'INLAND' 'NEAR OCEAN' 'ISLAND']
ocean_proximity
<1H OCEAN     9136
INLAND        6551
NEAR OCEAN    2658
NEAR BAY      2290
ISLAND           5
Name: count, dtype: int64

 train_set.shape:  (16512, 10)  test_set.shape:  (4128, 10)
median_house_value    1.000000
median_income         0.688075
total_rooms           0.134153
housing_median_age    0.105623
households            0.065843
total_bedrooms        0.049686
population           -0.024650
longitude            -0.045967
latitude             -0.144160
Name: median_house_value, dtype: float64

 median min income:  0.4999  median max income:  15.0001
   longitude  latitude  housing_median_age  total_rooms  total_bedrooms  population  households  median_income  median_house_value ocean_proximity income_cat
0    -122.23     37.88                41.0        880.0           129.0       322.0       126.0         8.3252            452600.0        NEAR BAY          5
1    -122.22     37.86                21.0       7099.0          1106.0      2401.0      1138.0         8.3014            358500.0        NEAR BAY          5
2    -122.24     37.85                52.0       1467.0           190.0       496.0       177.0         7.2574            352100.0        NEAR BAY          5
3    -122.25     37.85                52.0       1274.0           235.0       558.0       219.0         5.6431            341300.0        NEAR BAY          4
4    -122.25     37.85                52.0       1627.0           280.0       565.0       259.0         3.8462            342200.0        NEAR BAY          3

 training: 
 income_cat
3    5789
2    5265
4    2911
5    1890
1     657
Name: count, dtype: int64

 testing: 
 income_cat
3    1447
2    1316
4     728
5     472
1     165
Name: count, dtype: int64
longitude               0
latitude                0
housing_median_age      0
total_rooms             0
total_bedrooms        155
population              0
households              0
median_income           0
ocean_proximity         0
dtype: int64

 housing_num_tr:  [[ 0.70903084 -0.73611778 -0.05246406 ...  0.98070311  1.00253757
  -0.19279129]
 [ 1.12365056 -0.68468381 -1.80430733 ...  1.3601267   1.76722451
  -0.12359366]
 [ 1.20357726 -0.97926016 -1.96356581 ...  1.33251607  1.18574381
  -0.06156895]
 ...
 [ 0.60912247 -0.79690337 -0.21172254 ...  0.87115123  0.77153839
  -0.45386467]
 [-0.84953969  1.16693897  1.85863769 ... -0.87188158 -0.7206632
  -0.88218324]
 [ 0.59413622 -0.74546941  0.50494062 ...  0.3367518   0.12367862
  -0.8303905 ]]

 error:  44910.39810668254

 error:  0.0

 scores:  [71786.14711657 67817.77552503 72850.36479689 70365.02849891
 67148.89781079 68440.02858579 69839.566857   66283.0089256
 71907.24657023 68524.25094771]

 mean scores:  69496.23156345093

 rfr score:  [50238.09440456 48666.39106463 48728.45271961 51676.23310681
 46551.34457133 47584.74314169 48263.70839594 49397.91483999
 50909.8224312  48745.61553926]  rfr mean score:  49076.232021502234
```
