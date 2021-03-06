# New York City Taxi Demand Prediction
## Problem Statement
To find number of pickups, given location cordinates(latitude and longitude) and time, in the query region and surrounding regions.
## Data Source:
Data can be downloaded from here:
http://www.nyc.gov/html/tlc/html/about/trip_record_data.shtml

__Here, we have used Jan- 2015 and Jan- 2016 data.__

## Objectives & Constraints 
__Objectives:__ Our objective is to predict the number of pickups as accurately as possible for each region in a 10min interval. We will break up the whole New York City into regions, that we will discuss later in the blog. Now, the 10min interval is chosen because in NYC one can commute 1 mile in approximately 10 minutes given the traffic is normal at that particular time.

__Constraints:__ 
* __Latency__ Given a location and current time of a taxi driver, as a taxi driver, he/she excepts to get the predicted pickups in his/her region and the adjoining regions in few seconds. Hence, there is a medium latency requirement.

* __Interpretability:__ As long as taxi driver gets good prediction result, he/she is not be much interested in the interpretability of the result. He/she is not much interested in why he/she is getting this result. Hence, there is a no interpretability required.

* __Relative Errors:__ Mean Absolute Percentage Error will be the relative error we will consider. Let say the predicted pickups for a particular location are 100, but actual pickups are 102, the percentage error will be 2% and Absolute error is 2. The taxi driver will be more interested in the percentage error than the absolute error. Let say in some region the predicted pickups are 250, and if taxi driver knows that the relative error is 10% then he/she will consider the predicted result to be in the range of 225 to 275, which is considerable.

__Our goal is to reduce the percentage error is low as possible.__


