# Kickstarting with Excel

## Project Overview 

### Purpose
The purpose of this analysis was to explore the outcomes of different kickstarters campaigns for plays. We compared successful, failed, and canceled play campaigns to  their launch dates and funding goals.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
![Theater Outcomes Based by Launch Date](https://github.com/NikWalker/kickstarter_analysis2/blob/main/Theater_Outcomes_vs_Launch.png?raw=true)

Based on the launch date outcomes for Theater, campaigns started during the month of May has the highest rate of success. We see a sharp spike in successful outcomes from April to May. Note that we see a steady decrease of successfull outcomes as the summer months continue with winter having the least amount of successful outcomes. When looking at the failed play campaigns, the amount failed from month to month remain generally consistant throughout the year. 

### Analysis of Outcomes Bassed on Goals
![Outcome based of goal](https://github.com/NikWalker/kickstarter_analysis2/blob/main/Outcomes_vs_Goals.png?raw=true)

The most successful play campaigns were those that had a goal under $1000, with a success rate of 76%. After we start seeing goals over five thousand we see a near twenty percent drop once the goals reach ten thousand. This downward trend of successful campaigns continues to drop to a low success rate of twenty percent as the goal totals reach near $35,000. There is however an increased success rate of 67% of campaigns between $35,000 and $50,000. After a plays goal exceeds that $50,000 mark, there does not seem to be a chance for a successful campaign. Since, we are comparing the successful versus the failed kickstarters, the inverse of the prior is true. We see an increase of failed campaigns as the goal price increases. 

### Challenges and Difficulties Encountered 
I created my parameters with the COUNTIFS Function to look at the goals of play kickstarter campaigns. I ran my equations for number of successful and number of failed campaign goals. When doing this I used "less than" and "greater then" symbols to set up the goal amount ranges, (ie. >1000 to <4999.) When I did this the percentages were not matching up with the example goal graph. So I used the sum function to total the successful and failed campaigns. I cross referenced this total by filtering out successful/failed plays on the kickstarter workbook, only to find out that my total number of successful and failed campaigns did not match. Some of my data was missing. I spent some time trouble shooting to find the lost data and then found out that the data I was missing was equal to the parameters of the goal column. So I had to go back to each of my COUNTIFS equations and change each of the "less than" and "greater than" signs to reflect "less than or equal to" and "greater than or equal to." (Ie. >=1000 to <=4999) This accounted for my missing data points.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

From the outcomes based of launch dates we can conclude that starting a theater kickstarter during the month of May should have the highest amount of success. From this data we cannot conclude why May has the most success, but the successful campaigns decrease throughout the rest of the year after that. On the other hand, the amount of failed theater campaigns seems to be pretty consistant throughout the entire year. This may indicate that the failures were due to other variables within the Kickstarter, that did not have to do with the launch date.

- What can you conclude about the Outcomes based on Goals?

Based on the play kickstarter goal amounts, we see the highest success rates in campaigns under five thousand. There is another spike in successful kickstarters between $35,000 and $50,000 at 67 percent successful. Also, having a goal over $45,000 does not seem to have much success at all. 

- What are some limitations of this dataset?
 
With this data set we can see when the best time of year is to start a campaign, however we do not have any data to suggest why it is the best time to start. At the same time, we do not have the data to express what made the other campaigns fail. 

- What are some other possible tables and/or graphs that we could create?

We could further our study by making stacked column chart to better show the difference in amounts of successful and failed campaigns 
