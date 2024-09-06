# Spaceship Titanic 🚀


## References

- [Day — 13: 30 Days Machine Learning Projects Challenge
Spaceship Titanic🚀] (https://medium.com/@iabbasali/day-13-30-days-machine-learning-projects-challenge-a85b05e44dcf)

## Datasets

- [Spaceship Titanic - Predict which passengers are transported to an alternate dimension](https://www.kaggle.com/competitions/spaceship-titanic/data)

## Code

- [app.py](https://github.com/donb4iu/30dayML/blob/main/30days/day13/app.py)

## Execution

```
   /Users/donbuddenbaum/.pyenv/versions/3.12.3/bin/python /Users/donbuddenbaum/Documents/30dayML/30days/day13/app.py
(8693, 14) (4277, 13)
  PassengerId HomePlanet CryoSleep Cabin  Destination   Age VIP     \
0  0001_01     Europa     False     B/0/P  TRAPPIST-1e 39    False   
1  0002_01      Earth     False     F/0/S  TRAPPIST-1e 24    False   
2  0003_01     Europa     False     A/0/S  TRAPPIST-1e 58     True   
3  0003_02     Europa     False     A/0/S  TRAPPIST-1e 33    False   
4  0004_01      Earth     False     F/1/S  TRAPPIST-1e 16    False   

   RoomService  FoodCourt  ShoppingMall  Spa   VRDeck Name                \
0   0              0        0               0   0        Maham Ofracculy   
1 109              9       25             549  44           Juanna Vines   
2  43          3,576        0           6,715  49          Altark Susent   
3   0          1,283      371           3,329 193           Solam Susent   
4 303             70      151             565   2      Willy Santantines   

   Transported  
0  False        
1   True        
2  False        
3  False        
4   True        

train:
  PassengerId       0
HomePlanet      201
CryoSleep       217
Cabin           199
Destination     182
Age             179
VIP             203
RoomService     181
FoodCourt       183
ShoppingMall    208
Spa             183
VRDeck          188
Name            200
Transported       0
dtype: int64

test:
 
PassengerId         0
HomePlanet         87
CryoSleep          93
Cabin             100
Destination        92
Age                91
VIP                93
RoomService        82
FoodCourt         106
ShoppingMall       98
Spa               101
VRDeck             80
Name               94
/Users/donbuddenbaum/Documents/30dayML/30days/day13/app.py:24: FutureWarning: DataFrame.fillna with 'method' is deprecated and will raise in a future version. Use obj.ffill() or obj.bfill() instead.
  train[['HomePlanet', 'CryoSleep', 'Destination', 'VIP']] = train[['HomePlanet', 'CryoSleep', 'Destination', 'VIP']].fillna(method='ffill')
/Users/donbuddenbaum/Documents/30dayML/30days/day13/app.py:24: FutureWarning: Downcasting object dtype arrays on .fillna, .ffill, .bfill is deprecated and will change in a future version. Call result.infer_objects(copy=False) instead. To opt-in to the future behavior, set `pd.set_option('future.no_silent_downcasting', True)`
  train[['HomePlanet', 'CryoSleep', 'Destination', 'VIP']] = train[['HomePlanet', 'CryoSleep', 'Destination', 'VIP']].fillna(method='ffill')
/Users/donbuddenbaum/Documents/30dayML/30days/day13/app.py:25: FutureWarning: DataFrame.fillna with 'method' is deprecated and will raise in a future version. Use obj.ffill() or obj.bfill() instead.
  test[['HomePlanet', 'CryoSleep', 'Destination', 'VIP']] = test[['HomePlanet', 'CryoSleep', 'Destination', 'VIP']].fillna(method='ffill')
/Users/donbuddenbaum/Documents/30dayML/30days/day13/app.py:25: FutureWarning: Downcasting object dtype arrays on .fillna, .ffill, .bfill is deprecated and will change in a future version. Call result.infer_objects(copy=False) instead. To opt-in to the future behavior, set `pd.set_option('future.no_silent_downcasting', True)`
  test[['HomePlanet', 'CryoSleep', 'Destination', 'VIP']] = test[['HomePlanet', 'CryoSleep', 'Destination', 'VIP']].fillna(method='ffill')

train:
  HomePlanet        0
CryoSleep         0
Cabin           199
Destination       0
Age             179
VIP               0
RoomService     181
FoodCourt       183
ShoppingMall    208
Spa             183
VRDeck          188
Transported       0
dtype: int64

test:
  HomePlanet        0
CryoSleep         0
Cabin           100
Destination       0
Age              91
VIP               0
RoomService      82
FoodCourt       106
ShoppingMall     98
Spa             101
VRDeck           80
dtype: int64

train: 
 HomePlanet         3
CryoSleep          2
Cabin           6560
Destination        3
Age               80
VIP                2
RoomService     1273
FoodCourt       1507
ShoppingMall    1115
Spa             1327
VRDeck          1306
Transported        2
CabinDeck          8
CabinNum        1817
CabinSize          2
dtype: int64

test: 
 HomePlanet         3
CryoSleep          2
Cabin           3265
Destination        3
Age               79
VIP                2
RoomService      842
FoodCourt        902
ShoppingMall     715
Spa              833
VRDeck           796
CabinDeck          8
CabinNum         889
CabinSize          2
dtype: int64
/Users/donbuddenbaum/Documents/30dayML/30days/day13/app.py:45: FutureWarning: Series.fillna with 'method' is deprecated and will raise in a future version. Use obj.ffill() or obj.bfill() instead.
  train['CabinDeck'] = train['CabinDeck'].fillna(method='ffill')
/Users/donbuddenbaum/Documents/30dayML/30days/day13/app.py:46: FutureWarning: Series.fillna with 'method' is deprecated and will raise in a future version. Use obj.ffill() or obj.bfill() instead.
  train['CabinSize'] = train['CabinSize'].fillna(method='ffill')
/Users/donbuddenbaum/Documents/30dayML/30days/day13/app.py:48: FutureWarning: Series.fillna with 'method' is deprecated and will raise in a future version. Use obj.ffill() or obj.bfill() instead.
  test['CabinDeck'] = test['CabinDeck'].fillna(method='ffill')
/Users/donbuddenbaum/Documents/30dayML/30days/day13/app.py:49: FutureWarning: Series.fillna with 'method' is deprecated and will raise in a future version. Use obj.ffill() or obj.bfill() instead.
  test['CabinSize'] = test['CabinSize'].fillna(method='ffill')

train:
  HomePlanet      0
CryoSleep       0
Destination     0
Age             0
VIP             0
RoomService     0
FoodCourt       0
ShoppingMall    0
Spa             0
VRDeck          0
Transported     0
CabinDeck       0
CabinSize       0
dtype: int64

test:
  HomePlanet      0
CryoSleep       0
Destination     0
Age             0
VIP             0
RoomService     0
FoodCourt       0
ShoppingMall    0
Spa             0
VRDeck          0
CabinDeck       0
CabinSize       0
dtype: int64
      CryoSleep  Age  VIP  RoomService  FoodCourt  ShoppingMall  Spa   VRDeck  \
0     0         39    0     0              0          0             0     0     
1     0         24    0   109              9         25           549    44     
2     0         58    1    43          3,576          0         6,715    49     
3     0         33    0     0          1,283        371         3,329   193     
4     0         16    0   303             70        151           565     2     
...         ...  ...  ...          ...        ...           ...   ...     ...   
8688  0         41    1     0          6,819          0         1,643    74     
8689  1         18    0     0              0          0             0     0     
8690  0         26    0     0              0      1,872             1     0     
8691  0         32    0     0          1,049          0           353 3,235     
8692  0         44    0   126          4,688          0             0    12     

      Transported  HomePlanet_Earth  HomePlanet_Europa  HomePlanet_Mars  \
0     0            False              True              False             
1     1             True             False              False             
2     0            False              True              False             
3     0            False              True              False             
4     1             True             False              False             
...           ...               ...                ...              ...   
8688  0            False              True              False             
8689  0             True             False              False             
8690  1             True             False              False             
8691  0            False              True              False             
8692  1            False              True              False             

      Destination_55 Cancri e  Destination_PSO J318.5-22  \
0     False                    False                       
1     False                    False                       
2     False                    False                       
3     False                    False                       
4     False                    False                       
...                       ...                        ...   
8688   True                    False                       
8689  False                     True                       
8690  False                    False                       
8691   True                    False                       
8692  False                    False                       

      Destination_TRAPPIST-1e  CabinDeck_A  CabinDeck_B  CabinDeck_C  \
0      True                    False         True        False         
1      True                    False        False        False         
2      True                     True        False        False         
3      True                     True        False        False         
4      True                    False        False        False         
...                       ...          ...          ...          ...   
8688  False                     True        False        False         
8689  False                    False        False        False         
8690   True                    False        False        False         
8691  False                    False        False        False         
8692   True                    False        False        False         

      CabinDeck_D  CabinDeck_E  CabinDeck_F  CabinDeck_G  CabinDeck_T  \
0     False        False        False        False        False         
1     False        False         True        False        False         
2     False        False        False        False        False         
3     False        False        False        False        False         
4     False        False         True        False        False         
...           ...          ...          ...          ...          ...   
8688  False        False        False        False        False         
8689  False        False        False         True        False         
8690  False        False        False         True        False         
8691  False         True        False        False        False         
8692  False         True        False        False        False         

      CabinSize_P  CabinSize_S  
0      True        False        
1     False         True        
2     False         True        
3     False         True        
4     False         True        
...           ...          ...  
8688   True        False        
8689  False         True        
8690  False         True        
8691  False         True        
8692  False         True        

[8693 rows x 25 columns]

dtc_accuracy:  0.7389304197814837

dtc_confusion_matrix:  [[622 242]
 [212 663]]

rfc_accuracy:  0.7987349051178838

rfc_confusion_matrix:  [[723 141]
 [209 666]]

xgbc_accuracy:  0.7952846463484762
```