# Kickstarting with Excel


## Overview of Project
Looking at Kistarter project dataset to know how different campaigns fared in relation to their launch date and their funding goals


### Purpose

This analysis examines different campaigns fared in relation to their launch dates and their funding goals. 
The sourse dataset is included as well. ![Kickstarter_Challenge](/Kickstarter_Challenge.xlsx.xlsx). 

Deliverable 1: 
* To visualize Kickstarter campaign outcomes based on their launch date
* To realize the success or failure of a Kickstarter campaign (especially theater) during the year
* To determine the month that launch the most successful Kickstarter campaigns

Deliverable 2
* Assess the success, failure and cancellation of Kickstarter campaigns based on fundraising goals
* To plan on selecting Kickstarter campaigns based on the percentage of successful campaigns in each defined goal amount range
* Possibly a selection of candidate Kickstarter campaigns that have no effect on the long-term  funding goals of the project


## Analysis and Challenges


### Analysis of Outcomes Based on Launch Date

The month that launched the most successful and failed Kickstarter theater campaigns was May. However, except for October, the number of successful launched campaigns after peak has experienced a downward trend and, in the July, and October, the failed Kickstarter theater campaigns rate is very close to peak.
Furthermore, by glancing at the “Theater outcomes by Lunch Date”, we can specify that the number of successful and Failed theater Kickstarter campaigns has not changed significantly during the following months:

![Theater_Outcomes_vs_Launch](/resources/Theater_Outcomes_vs_Launch.png)
* January
* March
* September
* November


### Analysis of Outcomes Based on Goals

In general, the percentage of successful Kickstarter campaigns accompanied with plays subcategory for the goal amount range less than 35000 and greater than 45000 has suffered a downward behavior, while with similar range, the percentage of the failed Kickstarter campaigns has experienced an upward growth. In other words, the successful and failed campaigns interact with each other in the recent ranges. 
In addition to, in the goal amount range 35000-44999, there is no noticeable change in the rate of progress or regression of the successful and failed Kickstarter campaigns.
It is noteworthy that percentage of the successful Kickstarter campaigns in the goal amount range 45000-49999 is zero and we have 100% failure experience.

![Zero_Success](/resources/Zero_Success.png)

 Furthermore, we only compare the "Percentage Failed" and "Percentage Successful" because of zero "Percentage Canceled" and they are complimentary of each other to reach 100%. In other words, increasing one of them is accompanied by decreasing the other and no other factor will affect these results.  

![Outcomes_vs_Goals](/resources/Outcomes_vs_Goals.png)


### Challenges and Difficulties Encountered

* To populate the “Number successful”, “Number Failed” and “Number Canceled”, columns and using the “countifs”, I got confused and thought that I should filter the columns of Kickstarter based on successful/Failed/canceled as well as subcategory based on plays but after checking the data set, I realized that it does not matter if it is filtered or not. However, the “countifs” performs this filtering.
* Because in the “Canceled Number” column, all the cells got a value of 0, thus I was not sure if all columns would be zero or not. By filtering the outcomes using “Canceled” along with subcategory using “plays”and checking the data set, I could not find a common point and I made sure that the column D in the outcomes based on goals sheet correctly selected.
* In chart “ Outcomes_ vs_Goals”, the values on the vertical axis did not conclude the percentage symbol ”%”, I could solve this problem by right click on the column and selecting “Format cell/Percentage”. 


![Missing Percentage](/resources/Missing%20Percentage.png)  


## Results

What are two conclusions you can draw about the Outcomes based on Launch Date?

* The most successful Kickstarter campaigns launched in May and since then, the number of successful campaigns has dropped significantly by the end of year.
* The percentage of successful campaigns in certain months like January, March, September and November is almost the same and the fluctuations related to these campaigns are more from April to September.


What can you conclude about the Outcomes based on Goals?
The percentage of successful Kickstarter campaigns is the most in the goal amount range less than 1000 and the lower percentage is 0% that occurs in the range 45000-49999.

What are some limitations of this dataset?

* We do not have the background of demographic information and we do not know "Is there sufficient experience for the population that has provided this data set?". 
It means that the data may have impurities or outliers.  

* Some categories are much more popular like theater and drive more traffic than others.

What are some other possible tables and/or graphs that we could create?
* Use measures of central tendency for each set of failed or successful campaigns based on funding goals
* Make the same table/graph of outcomes based on either goals or pledged by filtering outcomes based on other subcategories or any other column that makes sense.   
