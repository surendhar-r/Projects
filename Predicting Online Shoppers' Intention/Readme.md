# Predicting Online Shoppers' Intention Using R

E-commerce has grown significantly over the past couple of decades and has become a necessity for retail stores to stay competitive. This project aims to determine the main attributes that influence online shopping sale conversions based on a large dataset over a one-year period from the UCI Machine Learning Repository, which was derived from Google Analytics metrics. Using classification techniques, it was determined that the PageValues attribute has a considerable influence on Revenue. As such, the recommendation is that the company shift resources to study this attribute for improved online sales performance.

## Dataset Overiew

This dataset was sourced from UC Irvine Machine Learning Repository: http://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset

The online_shoppers_intention dataset has 12,330 sessions and 18 attributes (10 numerical and 8 categorical) of different users in a one-year period. Of the 12,330 sessions, 84.5% were class of non-interest samples that did not result in a conversion (i.e., Revenue = NO), while the rest were class of interest and did result in a conversion (i.e., Revenue = YES). Each record belongs to a different user in a one-year period without any bias to a particular user, campaign, special day, or month. For unknown reasons, the dataset did not include the months January and April, and they were assumed insignificant.

The 18 attributes are defined here:
Administrative, Administrative_Duration, Informational, Informational_Duration, ProductRelated, ProductRelated_Duration - depict the different types of pages visited and the amount of time spent in seconds of each category
BounceRates – the percentage of visitors who enter the site and then leave without visiting any other pages
ExitRates – the percentage of last page views for a specific webpage
PageValues – the average value for a webpage that a user visited before completing a transaction. This value indicates the importance of a particular web page based on Google Analytics.
SpecialDay – visit made on or near a holiday. The value will take a maximum value of 1 on the day of the holiday and will take a fractional value in the days preceding and following the holiday.
Month –month the visit was made
VisitorType –visitor is new or returning
Weekend –visit was made on the weekend or on a weekday
Revenue – signifies whether a purchase was made by a customer or not. This is the target variable.
OperatingSytems, Browser, Region, TrafficType – categorical data that is numerically represented, but definition of their values is missing.

## Preprocessing Data

A few attributes in the dataset, including Browser, Region, Traffic Type, and Operating Systems, are categorical and the description of these attributes could not be found; therefore, they were omitted from the analysis.
The remaining categorical attributes, including VisitorType, Revenue, Month, and Weekend, were converted into factors.

## Empirical Analysis

The dataset was partitioned into two sets, 75% for training and 25% for validation. The data is analyzed using numerous models; however, only two notable ones are considered in detail: logsitic regression and random forest models.

## Conclusion

It was determined that the PageValues attribute was the best predictor of Revenue. After considering multiple different models, it was deemed that random forest generated the model with the highest accuracy of 90.2%, while the logit model had the highest precision of 82.79%.
It is important to note that no one model is best, but it depends on the circumstances and required output. Other attributes that were not included in the dataset, such as the type of online store and shopper demographics could be important to ensuring a high-fidelity model.
