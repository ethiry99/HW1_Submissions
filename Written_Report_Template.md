# Kickstarting with Excel

## Overview of Project
We have been provided a table of data from Kickstarter campaigns relating to arts and entertainment. Our client, Louise, is looking for information from the data concerning the success of campaigns in relation to their launch date (month it started) and funding goals.  We will use the data to graphically visualize each of these criteria. 


### Purpose
The information visualized from the data will be used by Louise to shape her campaign to maximize the likelyhood of success for her play *Fever*.  This will provide her information on what time of year to launch the campaign and how large her funding goal should be. 


## Analysis and Challenges
### Visualization #1 
The first visualization was created using a pivot table to count the number of Successful, Failed, & Cancelled campaigns.  It was filtered to only provide data on other campaigns characterized under the parent category of "theater".  A filter was created for Years but the visualization provided shows all Years.  This pivot table was used to create [line chart](https://github.com/ethiry99/HW1_Submissions/blob/main/Resources/Theater_Outcomes_vs_Launch.png) comparing the campaign outcomes based on the month they were launched.

### Visualization #1 Challenge

A challenge encountered in the 1st visualization was that the campaign start and end dates were provided in the [Unix date format](https://github.com/ethiry99/HW1_Submissions/blob/main/Excel%20Images/Unix%20Date%20%26%20Time%20example.png) which is the number of seconds since Jan 1, 1970.  In order to [convert](https://github.com/ethiry99/HW1_Submissions/blob/main/Excel%20Images/Unix%20Conversion%20to%20Excel%20Date.png) the listed seconds needed to be divided by 60 to get the number of minutes, the minutes divided by 60 again to get the number of hours, the hours divided by 24 to get the number of days.  The total number of days (on the order of 16,000) were then added to the orgin date of 1/1/1970.  We know had a orgin date in excel format that we could use in a pivot table.

### Visualization #2
The second visualization was created using the [COUNTIFS()](https://github.com/ethiry99/HW1_Submissions/blob/main/Excel%20Images/COUNTIFS%20example.png) statement to count the successful, failed, and cancelled campaigns. The countifs criteria included, campain goal (divided into ranges), outcome, and the subcategory of "plays".  The instances of campaigns that meet each criteria is detailed in the [table]().  Those counts were used to calculate percentages of success, failure, & cancellations. It is the percentage of each category that was used to create a line chart demonstrating a comparison amongst the outcomes.

### Visualization #2 Challenge
I attempted to "grab" the value ranges by using LEFT() and RIGHT() functions to create my greater than $x,000 and less than $x,000 but was not able to make it work or find suggestions via google to that effect. Because of this each range had to be hard coded into the function rather than being able to copy paste of cells using cell references.

### Analysis of Outcomes Based on Launch Date

### Analysis of Outcomes Based on Goals

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
