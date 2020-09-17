# Exploring Income Level and its Affect on Teenage Birth Rates in Baltimore, MD and New York, NY 
## Background
It is interesting to consider how material childhood circumstances affect the likelihood of teenage births. Two cities, New York and Baltimore, have a $7k difference between their average household incomes of $35k and $28k [respectively.](https://opportunityinsights.org/) Do we expect to see the same teenage birth rate outcomes? We’ll take a look at the data from the [Opportunity Insights group's research](https://opportunityinsights.org/) which follows 20 million children from their childhood to mid-30s to see how income level plays a role.

## Business Question
***How does the income level of one’s parent(s) influence the fraction of women in Baltimore and New York City who, between the ages of 13-19 years old, give birth to a child?***

## Data Sources
We'll use open data from the [Opportunity Atlas](https://opportunityinsights.org/).
- Baltimore Data: [raw](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/Balti-RawData-TeenageBirthRate-Income-Race.xlsx) and [analyzed](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/Balti-Analysis-Income-TeenageBirthRate.xlsx)
- New York Data: [raw](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/NYC-RawData-TeenageBirthRate-Income-Race.xlsx) and [analyzed](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/NYC-Analysis-Income-TeenageBirthRate.xlsx)
- The excel files above contain raw and manipulated teenage birth rate data for neighborhoods by income level, along with this [data analysis](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/NYC-Balti-Analysis-Income-Race-Teenagebirthrate.xlsx) comparing the cities by income level and race.

## Data Analysis and Answer
The primary metric is parent income level categorized by:
1. All (baseline comparison)
1. High (75th percentile)
1. Middle (50th percentile)
1. Low (25th percentile)

**What fraction of women in each income level gave birth in their teenage years in New York?** 
![insert](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/nyc%20analysis%20birth%20rate%20by%20income.png)

**In Baltimore?**

![inserttoo](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/balti%20analysis%20birth%20rate%20by%20income.png)

Even within neighborhoods with fewer teenage births, low income accounts for overwhelming higher birth rates in both cities. This indicates that income level is an important social determinant when it comes to how likely an individual is to give birth as a teenager.

**How does  Baltimore and New York compare in their teenage birth rates?**
![insert](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/nyc%20balti%20analysis%20comp%20birth%20rate%20by%20income.png)

While Baltimore and New York have similar average household incomes, the graph above shows that there is greater income disparity in Baltimore as the percentage of women who give birth as a teen differs sharply between income levels. Wealth disparity is a variable that can be further exacerbated by race as the graph below shows that this is an issue that disproportionately affects Black women.

![insert](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/nyc%20balti%20analysis%20birth%20rate%20by%20race.png)

## Summary
It is clear that across neighborhoods and cities as a whole, regardless of varying levels of teen birth occurrences, low income strongly correlates to a higher teenage birth rate. Additional data that further explores race by income breakdown would be helpful as the links between income level and race in a historically segregated city such as Baltimore should be taken into further account.
