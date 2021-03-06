
Data Wrangling : The steps I followed are as below:

## 1. Delete the duplicates.

## 2. Go over the data points for every feature.

## 3. Clean the outliers.

## 4. Get rid of the null/missing values

### Deleting the Duplicates : 

There are only 29 duplicate observations. So this is so small that this could be overlooked and dropped.

### Feature/Column Check : 

When I examined the data points for each feature, I have come to the understanding that some features have only 2 unique values and the percentage of sole value out of 2 unique values is less that 0.1 percent. So this feature could be dropped. Then I decided to drop unnecessary features named ['seller','offerType','nrOfPictures','abtest', 'monthOfRegistration'].

### Adding a Feature : 

By having the advantage of 'yearOfRegistration' feature, I have come up with a 'Age' column. This feature will represent the age of the car, and age is an important factor in terms of determining the value of a car.

### Cleaning the Outliers : 

 Number of Cars with newer entries than 2016 : 14680
 Number of Cars with older entries than 1970 : 1738
 
 The first of one is the wrong entries since the data had been scraped in 2016. This should be filtered. The older cars would not bring any value to the target. And the number of these old cars are 1738. So this also would be filtered.
 
 Number of Cars with a Value higher than 100.000 : 403
 Number of Cars with a Value lower than 250 and equal to 0 : 19998 and 10777

 The cars with a high values of over 100.000 would mislead us. These should be handled as outliers.
 The number of lower value cars are more than I thought. So I will keep them for now.
 
 According to my research, the car with higher HP than 600 and lower HP than 5 are wrong entries. So I will handle these outliers by filtering.
 
 ### Missing Values and Nulls : 
 
I really had a difficult time to figure out how to deal with missing/null values. Specific to my data set, there is no option that dropping them all because I have 371000 data points. I know I will lose %30 observations. I will do further assesment following the modeling.
 
 ### Right after the modeling, I will come back and make assessment regarding the wrangling of the data set.
