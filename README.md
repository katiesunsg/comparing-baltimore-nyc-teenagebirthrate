# Exploring Income Level and its Effect on Teenage Birth Rates in Baltimore, MD and New York, NY 
## Background
It is interesting to consider how material childhood circumstances affect the likelihood of teenage births. New York City and Baltimore have a $7k difference between their average household incomes of $35k and $28k [respectively,](https://opportunityinsights.org/) but do we expect similar teenage birth rate outcomes? We’ll take a look at data from the [Opportunity Insights group](https://opportunityinsights.org/) which follows 20 million children from childhood to mid-30s to determine how income level plays a role.

## Business Question
***How does the income level of one’s parent(s) influence the fraction of women in Baltimore and New York City who, between 13-19 years old, gave birth and is this indicative of a greater wealth inequality issue?***

## Data Sources
We'll use open data from the [Opportunity Atlas](https://opportunityinsights.org/).
- Baltimore Data: [raw](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/Balti-RawData-TeenageBirthRate-Income-Race.xlsx) and [analyzed](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/Balti-Analysis-Income-TeenageBirthRate.xlsx).
- New York Data: [raw](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/NYC-RawData-TeenageBirthRate-Income-Race.xlsx) and [analyzed](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/NYC-Analysis-Income-TeenageBirthRate.xlsx).
- The excel files contain teenage birth rate data for neighborhoods by income level. This [data analysis](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/NYC-Balti-Analysis-Income-Race-Teenagebirthrate.xlsx) compares the cities by income level and race.

## Data Analysis
The primary metric is parent income level categorized by:
1. All (baseline comparison)
1. High (75th percentile)
1. Middle (50th percentile)
1. Low (25th percentile)

**What fraction of women in each income level gave birth in their teenage years in New York?** 
![insert](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/nyc%20analysis%20birth%20rate%20by%20income.png)

**In Baltimore?**

![inserttoo](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/balti%20analysis%20birth%20rate%20by%20income.png)

Even within neighborhoods with fewer teenage births, low income results in higher birth rates in both cities. This indicates that income is an important social determinant when it comes to how likely an individual is to give birth as a teenager.

**How do Baltimore and New York teenage birth rates compare?**

![insert](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/nyc%20balti%20analysis%20comp%20birth%20rate%20by%20income.png)

**By race?**

![insert](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/nyc%20balti%20analysis%20birth%20rate%20by%20race.png)

While Baltimore and New York have similar average household incomes, the first graph above shows that there is greater income disparity in Baltimore as the percentage of women who give birth as a teen differs sharply between income levels. Wealth disparity and teenage birth rates can be tied to race as the second graph above shows that Black women are disproportionately affected.

## Summary
It is clear that across neighborhoods and cities, regardless of varying levels of teen births, low income strongly correlates to a higher teenage birth rate. Additional data that explores race by income breakdown would be helpful as the links between income and race in a historically segregated city like Baltimore should be taken into further account. These findings mean that (racially based) income inequality is a variable to keep in mind as we consider how social mobility potential will affect us as students now, and in the future.

# Python Exploration
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1W82TXkYcVpPmvl7zt6VL6KDrXSD9nzYi?usp=sharing)
We revisited this data using python in the Google Colaboratory notebook linked above. For our python data analysis, we used a combination of pandas, numpy, and plotly express to filter the data, form pivot tables, and create various data visualizations. 

**What do our findings show us?** 

In our python analysis, we focused on data visualizations using bar graphs. Our data once again showed us that teenage birth rates are disproportionately distributed across neighborhoods in both cities, with teenage birth rates being slightly higher when accounting for lower income births compared to all income births. While there was no new findings, the contrast between Baltimore and New York City was highlighted in Baltimore having higher teenage birth rates on average compared to New York.

**Revisiting teenage birth rates in Baltimore City vs. New York City by all-income**
![attach](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/baltiallincomebar.png)
![attachalso](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/nycallincomebar.png)
![attachthird](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/baltinycallincome.png)

Using Plotly express, we can create bar graphs to look at teenage birth rates within each city and in comparison to each other. The first two bar graphs above show the teenage birth rates by neighborhood in Baltimore City and New York City. The third graph shows the average overall teenage birth rate for the two cities for all income births, in which we can see that Baltimore's average teenage birth rate is ~0.4 with New York lower at at ~0.15. This implies that, on average, for a random neighborhood in Baltimore, nearly 40% of women will have given birth as a teenager compared to around 15% in a random neighborhood in New York. 

**Focusing on teenage birth rates by low-income**
![attachfour](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/baltilowincomebar.png)
![attachfive](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/nyclowincomebar.png)

From the two graphs above that focus on low-income births, we can clearly see that teenage birth rates increased for both cities. However, we see that the percentage of teenage births to women from low-income households appears to now be much higher on average across neighborhoods in Baltimore compared to the smaller average increase for New York neighborhoods. 

![attachfinal](https://github.com/katiesunsg/comparing-baltimore-nyc-teenagebirthrate/blob/master/Python%20Pivot%20Table%20Balti%20vs.%20New%20York.png)

Using the pivot tables in Python, we can see that the table above shows that Baltimore has higher teenage birth rates vs. New York across income levels, but it is especially stark in Baltimore's 45% vs. New York's 18% for low-income. This seems to suggest that income effects may be stronger in determining teenage birth rates in Baltimore than New York. This further reiterates our previous reccomendation that policies aimed at reducing teenage birth rates should prioritize low-income families especially in Baltimore.

## Summary and Future Steps
Additional data that might be useful for further analysis would be looking into race breakdown by neighborhoods and the relative poverty of each neighborhood. While we can see that lower income is linked to slightly higher teenage birth rates, it would be useful to determine whether it is race or income that is more likely to be able to successfully predict teenage birth rates. In addition, it would be worthwhile to explore how Baltimore and New York City differ in their neighborhood make-up in terms of racial segregation, average household income, and even other potential teenage birth rate factors such as level of education.
