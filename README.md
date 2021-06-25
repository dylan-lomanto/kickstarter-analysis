# An Analysis of Kickstarter Campaigns
##### Module 1 - Performing analysis on Kickstarter data to uncover trends
### Overview of Project
  Louise, the client and playwright of *Fever*, did not meet her fundraising goal for her play on Kickstarter by a small margin.  She wishes to examine campaign outcomes of other theater projects funded through Kickstarter based upon launch dates and funding goals to determine whether or not she can alter either variable to have success in a future fundraising campaign.  The dataset analyzed consists of 1,394 Kickstarter theater campaigns between 2010 and 2017.
### Analysis and Challenges
  Two analyses were run on the dataset; 'Outcomes Based on Launch Date' and 'Outcomes Based on Goals'.  
##### Analysis of Outcomes Based on Launch Date 
A pivot table was created to determine the count of campaign outcomes (successful, failed, and canceled) based upon their creation date. Currently live campaigns were excluded from the results. The variable 'Parent Category' was used to filter for only theater projects. 

![](Outcomes_vs_Launch_Date_Pivot_Table.PNG)

Subsequently, the pivot table was used to create a line chart to visualize the findings. 

![](Theater_Outcomes_vs_Launch.PNG)

##### Analysis of Outcomes Based on Goals
A table was created with goal range dollar figures on the y-axis and counts and percentages of outcomes (successful, failed, and canceled) on the x-axis. The full dateaset was filtered to only show results for the subcategory "plays". The COUNTIFS() function was then used to populate the table with the number of outcomes for each goal range.

![](Outcomes_vs_Goals_Table.PNG)

The percentage columns were then used to create a line chart of the outcomes vs the goal ranges.

![](Outcomes_vs_Goals.png)

##### Challenges and Difficulties Encountered
The majority of the difficulties encountered related to the syntax of the COUTIFS() function. The notation became quite long for some cells and I struggled to properly write it down until I discovered that I could switch tabs and select a column and sheet instead of writing it out character by character.    
### Results
##### Outcomes Based on Launch Date
1. The most successful month to launch a theater campaign on Kickstarter is May, by a wide margin.  Not only does May have the highest number of successful campaigns, it has the widest separation between the number of successful and failed campaigns (both in terms of counts of outcomes and relative to total campaigns launched) indicating that the month of May has the highest percentage of successful outcomes.  
2. The successful and failed campaign lines tend to mirror one another in shape, indicating that the percentage of successful campaigns remains similar year-round, with the exception of December.  In December the lines nearly intersect, indicating that it has the lowest percentage of successful campaigns and is thus the worst month to launch a campaign.
##### Outcomes Based on Goals
The goal ranges that have a higher percentage of successful outcomes than failed outcomes are <1000, 1000 to 4999, 5000 to 9999, 10000 to14999, 35000 to 39999, and 40000 to 44999.  The goal range with the largest percentage of successful campaigns is <1000, indicating that this range is the most likely to be successful. The percentage of successful campaigns there, with a brief return to more the 50% succes in the 35000 to 44999 ranges. 
#### Limitations and Alternate Tables/Charts
