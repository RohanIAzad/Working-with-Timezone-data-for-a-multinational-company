# Elevator Pitch
Multinational companies have business in different timezones of the world. 
The main task is to conduct an anlysis on the product sales of a multinational company and obtain information about its various retailer types, expressed in offset from UTC. The target is to display the average amount of sales that occured in each time zone.
In the data, getting all the datetime data in one timezone for this analysis.

### The data analysis process follows-
### 1. Ask
### 2. prepare
### 3. Process
### 4. Analyze
### 5. SHare
### 6. Act

# 1. Ask
The main task is to conduct an anlysis on the product sales of a multinational company and obtain information about its various retailer types, expressed in offset from UTC. The target is to display the average amount of sales that occured in each time zone.

# 2. Prepare
For the prepare phase, checking if there's the required data and if the data will be suitable to answer the questions. 
There's information about product sold, Revenue, retailer type, time zone which is necessary to answer the target question. The collected data is suitable for moving forward in the analysis process.  

# 3. process
The process stage involves creating new columns, taking information from other columns (feature engineering), cleaning missing values, looking for inaccurate entries.

1. Creatinga ne w column "date_time" by combining "DateOfSale" and "TimeOfSale"
2. Dropping unnecessary columns
3. Checking if the timezone in the data matches with all_timezones in pytz
4. Replacing the timezones in the data that are not available in pytz with the equivalent timezone in pytz.
5. Creating timezone aware objects for all records.

# 4. Analysis
1. Converting different timezones to UTC
2. information on DaylightSaving DST was also found. 
3. Gourping by Timezone and taking the mean of the "Sales Revenue"

# 5. Visualization
![7  Average sales per timezone](https://user-images.githubusercontent.com/43137227/166161811-a8f4c636-7dea-4f81-9d74-7d207353e538.PNG)


