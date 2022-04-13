# Kickstarting with Excel

## Overview of Project

### Purpose
While utilizing Kickstarter dataset my goal was to visualize campaign outcomes based on their launch dates and their funding goals.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
To perform the analysis I took the following step:
1. Created pivot table with following characteristics: Filters - Parent Category and Years, Columns - Outcomes, Rows - Date Created Conversion, Values - Count of Outcomes.
2. Filtered Theater fundrasing campaigns and choose successful, failed and canceled from them.
3. Created chart for the successful, failed and canceled Theater campaigns.

### Analysis of Outcomes Based on Goals
To perform the analysis I took the following step:
1. I made the table by given example,
2. I choose successful plays by the goal range with formulas like that:
 =COUNTIFS(Kickstarter!D:D, "<1000",Kickstarter!F:F, "successful", Kickstarter!R:R, "plays")
3. I choose failed plays by the goal range with formulas like that:
 =COUNTIFS(Kickstarter!D:D, "<1000",Kickstarter!F:F, "failed", Kickstarter!R:R, "plays")
4. And for canceled plays I put "canceled" in the appropriate place in the formula as well.
5. Then I used the SUMM formula to calculate the number of Total projects.
6. Percentage I calculate by formula =B2/$E2
7. Then I created chart for the Percentages.

### Challenges and Difficulties Encountered
Overall task wasn't too challenging, however it caused me to give it a second thought when I needed to remove Quoters from the Rows in Pivot Table at the sheet Theater Outcomes by Launch Date. 
At the sheet Outcomes Based on Goals one should pay attention to the formula at the last row, because it is different from another and should use >= mathematical symbol.


## Results

>- What are two conclusions you can draw about the Outcomes based on Launch Date?
1. Overall Theater campaigns are most of the time two times more successful than they are failed.
2. The best months for launching Theater campaign are May and June, and the worst month is evidently December.

>- What can you conclude about the Outcomes based on Goals?

Campaigns with the small goals are usually more successful, then campaigns with the big goals: plays with the goals less than 1K have the best percentage of success ever, and when goals of plays exceed 20K the probability of success becomes less than 50%.

>- What are some limitations of this dataset?

There could be other variables that affect the final outcome. For example, the plays of some authors may be more successful than the plays of others. Or advertising campaigns applied in some cases may be more successful than in others.

>- What are some other possible tables and/or graphs that we could create?

Calculating and visualizing by percentage of successful/failed/canceled Theater campaigns by the time of year in the sheet "Theater Outcomes by Launch Date", could be more comprehensive than numbers. 
