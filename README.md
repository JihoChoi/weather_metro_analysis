# weather_metro_analysis
With KMA weather dataset &amp; Seoul metro dataset

## Visualization

### Sinchon station
![sinchon](https://github.com/skywalker023/weather_metro_analysis/blob/master/data/sinchon_station_usage.png?raw=true)

### Jamsil station
![jamsil](https://github.com/skywalker023/weather_metro_analysis/blob/master/data/jamsil_station_usage.png?raw=true)

### Gangnam station
![gangnam](https://github.com/skywalker023/weather_metro_analysis/blob/master/data/gangnam_station_usage.png?raw=true)

Displaying a very fixed pattern. Not that much variation.

## Variables
* 17:00~23:00 number of passenger on/off board
* Mean temperature, humidity, rainfall at night

## Target
* Usage of Sinchon station's last subway

## Model
* Gradient boost
* Random forest

## Result
* RMSE: 351

### Feature Importance
![feature importance](https://github.com/skywalker023/weather_metro_analysis/blob/master/data/feature_importance.png?raw=true)

As you can see, the incoming population between 7 P.M. and 8 P.M. has the highest importance when estimating the last train usage.



## Clustering by boarding pattern

### by "Getting on" pattern

![on-board](https://github.com/skywalker023/weather_metro_analysis/blob/master/data/clustering_by_onboard.png?raw=true)



### by "Getting off" pattern

![off-board](https://github.com/skywalker023/weather_metro_analysis/blob/master/data/clustering_by_offboard.png?raw=true)

### Discussion

* Can discriminate subway stations that are located in hot places, just by  "Getting on/off" pattern
* Classification might be possible: hot / not-hot
  * Further application need to be made to 5678 subway lines
* Further research might be fun: the gray area btw hot & not-hot areas