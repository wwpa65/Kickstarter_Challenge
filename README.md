# Kickstarter_Challenge
Weekly Challenge for the Module 1

# Kickstarting with Excel

## Overview of Project

Louise, a play wrighter, wanted to start a crowdfunding to get help for starting her play called "Fever". initially we have performed data analysis to help find whether there are any specific factor that will help achieving a successful crowdfunding campaing by using data over 4000 crowdfunding projects. 

Her play Fever could reach close to its goal in a short amount of time. Now she is interested in knowing how different campaigns fared in relation to their launch dates and their funding goals. Her aim is to look for musicals in Great Britain.

A number of Excel methods were applied during the data analysis of crowdfunding campaign data. 

### Purpose

The purpose of this project was to analyze and visualize crowdfunding campaign outcomes based on their launch dates and their funding goals to understand the effect of the campain launch date or the funding goal on the success, failure, or cancellation outcome.

## Analysis and Challenges

(Initially, new columns were added into the starting spreadsheet with data. The deadline and lauched_at date were formatted from unixtype to correct date format (dd/mm/yyyy). In addition, "category and subcategory" column was split into two columns.) 

During this challenge project, the data were analyzed using Microsoft Excel as follows.
- Extracted Year into a new column "Year" from the date in the "Date Created Conversion" column in the kickstarter spreadsheet. 
- The data were analyzed by using pivot tables and line charts, and poivot line charts. 
- Only the campaign outcomes in "Successful", "Failed", and "Cancelled" were used in the pivot table. 
- The parent category in the pivot table was filtered to show only "theater" as the parent category. The campaign outcomes were sorted in descending order. 
- Pivot line charts were created using the pivot table to visualize the trends in the outcomes (based on launch date and based on goals).
- For the analysis of fuinding goals, the goal amount was categorized into ranges, and the number of successful, failed, or cancelled campaigns were counted.

Link to the spreadsheet (Kickstarter_Challenge.xlsx) is available in the repository: [Kickstarter_Challenge](Kickstarter_Challenge.xlsx)

### Analysis of Outcomes Based on Launch Date

A brief summary of the data analyis is outlined as follows. 
- A pivot table was created using kickstarter worksheet into a new worksheet and it was named "Theater Outcomes by Launch Date".
- The pivot table included "Date Created Conversion in rows, outcomes in columns, and the count of outcomes as sum values. 
- Dates were grouped into corresponding month.
- The Parent Category was filtered to include only "theater" parent category. 
- Only the "Successful", "Failed", and "Cancelled" columns were included in the pivot table. 
- The parent category in the pivot table was filtered to show only "theater" as the parent category. The campaign outcomes were sorted in descending order.
- Campaign outcomes were sorted in descending order.
- A line pivot chart was created by using the pivot table.

### Analysis of Outcomes Based on Goals

A brief summary of the data analyis is outlined as follows. 
- A new worksheet was created to include 8 columns: Goal, Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed, Percentage Canceled. 
- Funding goal was categorized into 12 categories: Less Than 1000, 1000 to 4999, 5000 to 9999, 10000 to 14999, 15000 to 19999, 20000 to 24999, 25000 to 29999, 30000 to 34999, 35000 to 39999, 40000 to 44999, 45000 to 49999, 50000 or More. 
- Using "COUNTIFS" function with conditions, the number of successful, failed, and cancelled campaigns were populated into respective columns. 
- The total number of campaigns and the percentage successful, percentage failed, and percentage canceled were calculated using formula.  
- A line chart was created by using percentages for successful, failed, and cancelled campaigns in y axis and the grouped categories in X axis. 

### Challenges and Difficulties Encountered


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

Based on the chart (Figure 1), 

1) Successful campaigns were increased over the launch dates in the first five months although there was a slight fluctuation between January and March) and then started to decline (again slight increase in October).

2) The peak highest successful campaigns were achieved for the campaigns those were launced in May.

![Theater Outcomes by Launch Date](Theater_Outcomes_vs_Launch.png)

### Figure 1. Theater Outcomes by Launch Date
- What can you conclude about the Outcomes based on Goals?
General tendancy is that the percentage of successful campaigns were gradually decreased with increase of the goal set for the crowdfunding. 

It is interesting that there was a range of goal amount where the percent success rate was increased again, and then decreased.  

![TheaterOutcomes by Goals](Outcomes_vs_Goals.png)

### Figure 2.Theater Outcomes by Goals

- What are some limitations of this dataset?

In this analysis, we have analyzed cumulative data for all years. However, the results for individual years may have differences and these data should also be reviewed for individual years before making decisions. Therefore, it is better to perform descriptive statistics to get a better overview of the campaigns over the years from 2009 - 2017. We may need more data points as well.  

- What are some other possible tables and/or graphs that we could create?
Descriptive statistics tables, distribution plots, and box plots. 
