# Kickstarting with Excel Analysis

## Overview of the Project

Excel data analysis of past Kickstarter campaigns.

### Purpose

The client, Louise, wanted a data analysis of Kickstarter campaigns.  This investigation focused on success and failure of past campaigns.  Two areas of concern from the client were launch dates and funding goals.  In using techniques that include but not limited to VLOOKUP, SUM, COUNTIF, Pivot tables and graph creation, I was able to determine impact of funding goals and launch dates on the success/failure of a campaign.  

## Analysis and Challenges

The analysis will consist of two areas which are launch date and funding goals.  Launch date will explore if certain months launch date had any impact on success.  Funding goal will explore if the desired goal led to success or failure.  I will also detail challenges and difficulties that I experienced during the project.  

### Analysis of Outcomes Based on Launch Date

The analysis of outcomes based on launch date was achieved by certain steps.  First in the main workbook of Kickstarter, years were needed to be added in column section.  This was achieved by us of (YEAR) function.  To do this function, I used formula of =Year(Dates Created Conversion).  Once this was accomplished, a pivot table was created from data of Kickstarter worksheet.  This pivot table is in Outcomes Based on Launch Date workbook.  I then filtered the pivot sheets by Parent categories and Years.  Months were added to rows.  Outcomes were added to columns.  Count of outcomes were added to values.  I then filtered the data to only show theater Kickstarters.  Lastly, I created a line graph from the pivot table. 

### Analysis of Outcomes based on Goals 

To achieve the analysis of Outcomes based on Goals, I created a new workbook titled “Outcomes Based on Goals”.   In the workbook, I assigned Goal, Number of Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed and Percentage Canceled.  For Goals column, I assigned dollar ranges.   ![alt text] (https://courses.bootcampspot.com/courses/1021/files/1254186/preview). I then procedded to use COUNTIF function to populate Number of Successful, Canceled Failed columns.  The formula that was used is =COUNTIFS(Kickstarter!$D:$D,">=lower value of dollar amount",Kickstarter!$D:$D,"<=higher amount",Kickstarter!$F:$F,"type of outcome for the kickstarter",Kickstarter!$R:$R,"plays")").  To determine the total projects pertaining to goal, I used SUM().  The formula of this function was SUM(Number Successful, Number Failed and Number Canceled).   Percentage were determined by dividing the cell of goal to cell of the total project.  An example of this was taking B2/E2 which produced a successful percentage of 75.81% for a goal less than $1000.  Lastly, I created a line chart to visualize the data.  

### Challenges and Difficulties

I did run into some minor challenges and difficulties with each analysis.  In creating, the pivot table for Outcomes Based on Launch Goals, I first was unable to achieve the month in rows.  I was able to resolve the issue by trial and error.  The second challenge that I occurred with the analysis of the Outcomes Based on Goals.  Though this was attributed to user error.  First, I mistakenly did not include one of the goal categories.  I determined this when I used SUM function for table created compared to data of Kickstarter.  Next, when I was using COUNTIF function, I first chose the wrong column on Kickstarter workbook of pledged instead of goal.  I examined my formula and determined that I had selected E instead of D column.   Each difficulty and challenge, I was able to see that I needed to stay calm, double check work and at times slow down.   

## Results

### Conclusions of Outcomes based on Launch Date

![alt text] (https://github.com/bmliddicoat/kickstarter-analysis/blob/1d40f813548824148273b8fe6a87d75cddae63f0/Resources/Theature_Outcomes_VS_Launch.png)

The graph above helps display certain findings from analysis of outcomes based on launch for theater Kickstarters.  Certain months show higher numbers of total success and failure campaigns.  May (111 campaigns) and June (100 campaigns) are the best performing months for success based on total successful projects.  Though further investigation into the numbers, reveals that based on percentage of success versus failure the month of May has strongest historical data of success.  May success rate is around 67% of success and failure rate of 31%.  On the other hand, December is the poorest success rate (49%) and highest failure (46%).  Even though December only has 37 failures but that is out of total 75 campaigns.  In investigating the other months, a trend between 58% to 62% success rate.  On failure rate, the months have a range between 34% and 38%.  It can be determined that May is best month to launch a Kickstarter for theaters and December is the worst month.

### Conclusion of Outcomes based on Goals

It can be determined that lower the goal for funding, the higher rate of success will be achieved.  This highest rate of success is in the range lower $1000.  This trend continues of higher success to failure until goal between 15000 and 19999 where it becomes 50% for success and failure.  The trend of higher failure rate then increases with increase of higher goal.  Louise should aim to obtain funding no larger than 4999 if they want to have higher percentage of success.  

![alt text]  (https://github.com/bmliddicoat/kickstarter-analysis/blob/1d40f813548824148273b8fe6a87d75cddae63f0/Resources/Outcomes_vs_Goals.png)

The graph help visualize these findings of the analyzations of success and failure with goal.

### Limitations

The dataset does quantify certain areas.  These would pertain beyond the actual numbers.  This could include marketing within a campaign, possible effect of blurbs, world events that occurred during the time periods that could affect economy, possible campaigns being promoted on website at higher rate and possibly past success of campaigns by users that could lead to doners already in place.  The human impact on projects should be considered.  Another area that could be useful is type of play.  Are comedies vs drama as an example impact the results?

### Other Tables and Graphs

One table that could be used is a comparison between launch date and deadline.  This could explore what relationship between the two leads to success or failure.  We could also investigate average donations compared to success rate.  This could create a target of donors for the client.  Graphs that could be used include bar graphs to visualize these possible tables.  We could use pie graphs for each successful, failure and canceled month/goal.  If we took January per example, it would give client another way to see the impact of the month on the three outcomes.   

