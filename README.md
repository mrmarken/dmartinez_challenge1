# Kickstarting with Excel

## Overview of Project

### Purpose
This report outlines the results of crowdfunding campaigns specifically when kicking off Theater-related fund-raising campaigns across a calendar year. The data analysis presented herein is constrained to the 'Kickstarter' excel document containing data across various fund-raising campaigns. 

### Background
We're trying to help our client, Louise, better understand how different campaigns have fared in relation to their launch dates and funding goals. To do so, this document is outlining the outcome of various fund-raising initiatives across the parent category: "Theater." 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The following chart was created to provide an overview of the success rate for Kickstarter campaigns for each month throughout the years 2009 through 2017. 
[Theater_Outcomes_vs_Launch](https://github.com/mrmarken/dmartinez_challenge1/blob/main/resources/Theater_Outcomes_vs_Launch.png)
The data was obtained from the [Kickstarter_Challenge_DM.xlsx](https://github.com/mrmarken/dmartinez_challenge1/blob/main/resources/Kickstarter_Challenge_DM.xlsx) file by exclusively focusing in the parent category "Theater." 

This analysis was done by creating a pivot table and accompanying line chart to visualize the percentages for each of the three outcome categories: "success," "failed" and "canceled".  This was done for each entry in the Theater category.  Furthermore, the analysis took into consideration the dates the campaign was created and not when it was completed over the period of 2009 through 2017.

### Analysis of Outcomes Based on Goals
For this analysis, the data was further constrained to the sub-category of "plays" under the parent category of "Theater."  The ensuing chart, provides an overview of the percentage of successful vs failed campaigns given various fundraising goal targets: 
[Outcomes_vs_Goals.png](https://github.com/mrmarken/dmartinez_challenge1/blob/main/resources/Outcomes_vs_Goals.png)
This analysis was completed by constraining the target goals to be fall within the following ranges:
**Goal Ranges (in $)**
Less Than 1000
1000 to 4999
5000 to 9999
10000 to 14999
15000 to 19999
20000 to 24999
25000 to 29999
30000 to 34999
35000 to 39999
40000 to 44999
45000 to 49999
50000 or More

The ensuing chart shows the percentages of success/failure for each campaign given the ranges outlined above.

### Challenges and Difficulties Encountered
Some challenges/difficulties in this first Challenge centered on my little experience with github and uploading files via the command line.  
I also encountered some mistakes when building the second set of data (Outcomes_vs_Goals.png) because I tried using a Pivot Table instead of just inserting a line chart; it proved almost impossible to present the data using this approach as the pivot table had a specific way of organizing the timeline which amounted to an ascending order based on the first character of the cell value.
Additionally, I can see that not paying attention to the arguments in the "COUNTIFS" could lead to potential miscounting of the data.  It's important to ensure the "equal to or greater/less than" arguments are correct (inclusive of the upper/lower ranges).

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
Based on the data obtained in the "Outcomes based on Launch Date" graph, we can surmise the following:
1. Campaigns launched in the months of April through August had the most successful outcomes by numbers. 
   - A minimum of 71 campaigns were successfully completed each month
   - An average of 88.2 campaigns per month were successful, and
   - A maximum of 111 campaigns were launched in May; June followed in a close second with 100 successful campaigns.
2. A December launch date seems to have a similar likelihood of producing a successful campaign as a failed campaign.
   - December had 37 successful campaigns and 35 failed campaigns
   - This month had by far the highest rate of failure in the data analyzed at 47% for all campaigns launched in the time-period analyzed.


- What can you conclude about the Outcomes based on Goals?
Based on the data obtained in the "Outcomes based on Goal" graph, we can provide the following conclusions:
1. The most successful target goals for fund-raising campaigns seem to be:
   - Campaigns with targets of $999 or less which had a 76% success rate
   - Campaigns with targets between $1,001 - $5,000 which had a 73% success rate

2. The percentages of successful campaigns decrease as we look at the data with increasing goal ranges with a notable exception as outlined below.
   - The peak of failures seems to start at the goal target range between $25,000 to $29,999 (at 80%) 
   - The success rate takes a slight deviation from this pattern in the following two ranges: $35,000 to $39,999 (67% success) and $40,000 to $44,999 (67% success).  However, it is important to note that the total number of projects at these ranges (6 and 3, respectively) are relatively small and not much more analysis can be drawn from this dataset as it’s currently broken down.

- What are some limitations of this dataset?
  - The datasets do not currently allow us to make any direct correlations between the launch dates and the goal ranges.
  - Some data points may have too few samples to make any meaningful conclusions.
  - We still don’t have clear requirements from Louise and we may need to discuss these initial findings to uncover other needed data/information.


- What are some other possible tables and/or graphs that we could create?
  To obtain better analysis of the outcomes based on Launch date, there are a couple of items that can help us provide a better analysis:
  - A table or chart breaking down the percentages for each outcome by month
  - Constrain the data to "plays" only so that we can make more direct comparisons with the data in Outcomes Based on Goal
    - The ensuing datasets may give us more insights if we were able to make any correlations of the launch date vs. the target amount and what patterns, if any, exist

  - I'd also suggest we include a breakdown of the number of backers along with the average donation
  - It may also be helpful to understand how long each of the successful campaigns lasted
