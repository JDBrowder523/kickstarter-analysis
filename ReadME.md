# Kickstarting with Excel

## Overview of Project
The objective this analysis is to determine what helps make a crowdfunding campaign successful. Using a dataset of over 4000 crowdfunding campaigns from 2009 through 2017, statistical analysis and data visualization techniques are used to help determine the optimal monetary goal and time period to launch a new kiskstarter crowdfunding campaign for a theater play.
For this analysis, the client, Louise, wishes to see the success and failure rates of other kickstarter campaigns for plays and theater based specifically on their launch date and funding goals.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
In order to analyze the outcomes based on the date the crowdfunding campaign was launched, the data was sorted using a pivot table with a corresponding line graph in Microsoft Excel.  The pivot table shows a breakdown of the number of successful, failed, and canceled outcomes based on the month the campaign was started.  The pivot table can be further filtered to show information specific to an individual category, which was "theater" for this analysis.  The pivot table can also be filtered by year to show how the month of the campaign affected the success, failure, or cancellation of the crowdfunding attempt for an individual year (Image 1). The corresponding line chart creates a simple and easy to read visualization of which months were the most and least successful for crowdfunding attempts (see Theater_Outcome_vs_Launch.png).
 			  


### Analysis of Outcomes Based on Goals
To determine the success rate of crowdfunding campaigns based on the goal amount of money to be raised, the percentage of successful, failed, and canceled campaigns needed to be determined.The source data was sorted based on a range of goal amounts to determine the relationship between the goal amount of money and the success rate of the campaign.   First, the number of successes, failures, and cancellations was determined using the =countifs() function in Microsoft Excel.  The function had to be tailored to only pull data within the goal range needed. Next, the =sum() function was used to determine the total number of campaigns for each goal range.  Lastly, the number of successful, failed, and cancelled outcomes was divided by the total number of campaigns to determine the percentages.  The percentages were used to create a line chart that clearly shows the difference between the successes and failures based on the goal amount of money (see Outcomes_vs_Goals.png). 
 

### Challenges and Difficulties Encountered
The main challenge I experienced during this project was with the pivot table for Theater Outcomes by Launch Date.  Initially, I had 4 column labels (cancelled, failed, live, and successful).  For this analysis, the "live" or current campaigns were not useful in our data set and needed to be removed.  At first I tried to filter this data to remove the "live" column using the original data set.  After much trial and error, I found that the pivot table can be filtered directly, allowing for simple manipulation of the data.
I had a slight issue with the =countifs() function but it was due to a typing error.  I was trying to use the =countif() function, which does not allow for as many parameters.  Once I figured out that I was using the wrong Excel function, this part of the analysis went smoothly.


##Results

###Conclusions based on Launch Date
1. The most successful months for theater crowdfunding campaigns are May-July.
2. The least successful months for theater crowdfunding campaigns are November-January.

###Conclusions based on Funding Goal
Smaller funding goals are much more successful than larger funding goals.  Goals under $20000 have a success rate over 50%, with goals under $5000 having a success rate above 70%.  Goal amounts between $35000 and $45000 also have a success rate above 60%.  However, there are much fewer examples of campaigns with this funding goal.

###Dataset Limitations
This dataset is limited by the number of campaigns that had a goal amount higher than $15000.  With so few total plays with a goal higher than $15000, the success percentages could be misleading. For example, the sample size of 9 plays is too small to trust the figure of "67% success rate" for campaigns with goals between $35000 and $45000. A larger sample size of campaigns in this goal range would return more accurate results.
This data is also limited by the lack of a genre category.  It would be helpful to be able to analyze genres including comedy, drama, historical, etc.  This additional information would allow us to analyze if backers prefer to support plays that are a comedy or a drama.  This would let Louise have more information on what her goal amount should be based on the type of play she is putting on.

###Other Analysis Recommendations 
To help analyze the data further, we could create a line graph that displays the success, failure, and cancellation rate based on the length of the crowdfunding campaign.  This would allow us to determine if short, aggressive campaigns are more effective than long, steady campaigns.
We could also use box plots to determine if there are any outliers that are skewing the data.  The Outcomes Based on Goal line chart shows a success rate of only 13% for goals higher than $50000 but there are 16 total campaigns with this goal amount.  A box plot would show whether this low success rate is due to one or more goals being astronomically high to the point that the goals would be almost impossible to meet.
