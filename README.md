# Kickstarting with Excel

## Overview of Project

### Purpose
While utilizing Kickstarter dataset my goal was to utilize function and visualize campaign outcomes based on their launch dates and their funding goals. I created two technical analysis Charts: Outcomes Based on Launch Date and Outcomes Based on Goals. I used my knowledge of pivot tables and graphing in Excel to visualize campaign outcomes.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
![Theater_Outcomes_vs_Launch.png](/resources/Theater_Outcomes_vs_Launch.png)

#### Chart creation methodology
To perform the analysis I took the following step:
1. Created pivot table with following characteristics: Filters - Parent Category and Years, Columns - Outcomes, Rows - Date Created Conversion, Values - Count of Outcomes.
2. Filtered Theater fundrasing campaigns and choose successful, failed and canceled from them.
3. Created chart for the successful, failed and canceled Theater campaigns.

#### General comments about chart
1. Successul campaigns launched in April, May and June, we can see the big peak in May and months near it.
2. We can see the peaks as well in the February and October.
3. Year minimum is in December, the quantity of failed campaign almost the same as successful.

### Analysis of Outcomes Based on Goals
![Outcomes_vs_Goals.png](/resources/Outcomes_vs_Goals.png)

#### Chart creation methodology
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

#### General comments about chart
We can clearly see that chart has 4 areas: campaigns with the small goals till 20K are more than 50% successful, than campaigns between 20K and 40K goals are than 50% failed, and between 40K and 45K successful again, but there are 6 campaign only. The more expencive campaigns failed.

### Challenges and Difficulties Encountered
1. Overall task wasn't too challenging, however it caused me to give it a second thought when I needed to remove Quoters from the Rows in Pivot Table at the sheet Theater Outcomes by Launch Date. 
2. At the sheet Outcomes Based on Goals one should pay attention to the formula at the last row, because it is different from another and should use >= mathematical symbol.
3. At the first step I don't even noticed, that the chart Outcomes_vs_Goals should has a goals describing on the x-axis. Only when I myself couldn't remember what the points mean, I saw that in the sample assignment the goals directly listed. 


## Results

>- What are two conclusions you can draw about the Outcomes based on Launch Date?
1. Overall Theater campaigns are most of the time two times more successful than they are failed.
2. The best months for launching Theater campaign are May and June, and the worst month is evidently December.

>- What can you conclude about the Outcomes based on Goals?

Campaigns with the small goals are usually more successful, then campaigns with the big goals: plays with the goals less than 1K have the best percentage of success ever, and when goals of plays exceed 20K the probability of success becomes less than 50%.

>- What are some limitations of this dataset?

There could be other variables that affect the final outcome. For example, the plays of some authors may be more successful than the plays of others. Or advertising campaigns applied in some cases may be more successful than in others.

>- What are some other possible tables and/or graphs that we could create?

1. Calculating and visualizing by percentage of successful/failed/canceled Theater campaigns by the time of year in the sheet "Theater Outcomes by Launch Date", could be more comprehensive than actual numbers. 
2. Considering we have not the canceled campaigns at the "Outcomes_vs_Goals" chart, maybe another type of chart could be more demonstrative for percentage of successful campaigns instead of line chart, which basically duplicates information. 
