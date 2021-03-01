<h1>Kickstarting with Excel</h1>

<h2>Overview of Project</h2>

<h3>Background</h3>
<p>
  After Louise's play, <i>Fever</i>, came close to its fundraising goal in a short amount of time, Louise is seeking further analysis surrounding the impact of launch date on theather campaign outcomes as well as the impact of fundraising goals on play campaign outcomes.
</p>
<h3>Purpose</h3>
<p>
  The purpose of this project is to determine two items:
  <ol>
    <li>The effect, if any, that campaign launch date has on theater campaign outcomes.</li>
    <li>The effect, if any, that campaign goal amounts have on play campaign outcomes.</li>
</p>


<h2>Analysis and Challenges</h2>

<h3>Analysis of Outcomes Based on Launch Date</h3>
<p>
With the data, a pivot table was created using "outcomes" for columns, "Parent Category" and "Years" served as filters, while rows were separated into months of the year via the "Date Created Conversion" column, and finally the data populating this table was a count of outcomes.  Finally, the "Parent Category" filter was set to "theater" as the purpose of this analysis is to determine the effect, if any, that campaign launch dates have on theater campaign outcomes.
</p>
<p>
Upon creating the pivot table, it was determined that a pivot chart in the form of a line graph with markers would be a beneficial visual to assist in analysis (see Exhibit 1.1).
</p>
<p align="center">
<img src="https://github.com/tc9993/kickstarter-challenge/blob/main/Resources/Theater_Outcomes_vs_Launch.png?raw=true" alt="Theater Outcomes Based on Launch Date" height=66% width=66%><br>
<span style="font-size:10pt"><b>Exhibit 1.1:</b> Theater Outcomes Based on Launch Date</span>
</p>
<p> 
In reviewing Exhibit 1.1, corroborated by the pivot table found within <a href="https://github.com/tc9993/kickstarter-challenge/blob/main/Kickstarter_Challenge.xlsx" target="_blank">the provided workbook</a>, on sheet "Theater Outcomes by Launch Date", May, followed by June, were the months in which:
  <ul>
    <li>The most campaigns were launched.</li>
    <li>The most campaigns had successful outcomes.</li>
    <li>The greatest difference between total successful and total failed campaigns.</li>
  </ul>
</p>

<h3>Analysis of Outcomes Based on Goals</h3>
<p>
To evaluate the impact of outcomes based on goals, the first thing to do was define the appropriate ranges for goals, which in this case was determined to be <1,000, 1,000-4,999, and then increments of 4,999 up to 49,999 and then >50,000.  From there determining the totals per outcome (successfull, failed, canceled) and then further breaking that down into percentages.
</p>
<p>
Once filtered, it was then time to create a visual displaying the difference in total successes, failures, and cancelations based on those goals (see Exhibit 2.1).  In this case using percentages for the Y-axis, as opposed to totals, was determined to be more relevant due to the vast difference in totals across goal ranges (i.e. There were 534 campaigns in the 1,000 to 4,999 range but only 1 campaign with a goal between 45,000 and 49,9999) which would have affected the visual interpretation of the data.
</p>
<p align="center">
  <img src="https://github.com/tc9993/kickstarter-challenge/blob/main/Resources/Outcomes_vs_Goals.png?raw=true" alt="Play Outcomes Based on Goal" height=66% width=66%><br>
  <span style="font-size:10pt"><b>Exhibit 2.1:</b> Play Outcomes Based on Goal</span>
</p>
<p>
Upon reviewing Exhibit 2.1, backed up by the data found within <a href="https://github.com/tc9993/kickstarter-challenge/blob/main/Kickstarter_Challenge.xlsx" target="_blank">the provided workbook (also linked above)</a>, on sheet "Outcomes Based on Goals" you see a an inverse relationship wherein the percentage of successful campaigns decreases as the goal increases, up to the 25,000 to 29,999 range.  Inversely, failed campaigns trend upwards along with campaign goal.  Given that there were no canceled campaigns and the sum of both successful and failed campaigns must be 100, it makes complete sense to see the two lines react inversely to their counterpart.
</p>

<h3>Challenges and Difficulties Encountered</h3>
<p>
While no challenges were incurred while performing the analysis of outcomes based on launch date, getting the rows to appear as months as opposed to quarters or years could have been challenging without Excel experience, as the pivot table initially provided the rows as quarters.
  <br>
One challenge incurred while analysing the outcomes based on goals was ensuring applying the proper filters were applied to each field via the COUNTIFS() function.  It took some rubber duck debugging style talking aloud to determine the filters.  During the first attempt, the subcategory of "plays" was left out as a filter, meaning the data set was too large and not specific to the impact of goals on outcomes <i>of plays</i>.  Once talking it through, it was no longer a challenge to go back and add that critera to the COUNTIFS() function.  A second potential challenge arose, seeing a full column of "0's" in the canceled column.  While usually a cause for alarm, a quick look at the full data set confirmed that there were, in fact, no canceled play campaigns.
</p>

<h2>Results</h2>

<h3>What are two conclusions you can draw about the Outcomes based on Launch Date?</h3>
<p>
In reviewing the data, May and June, are the most popular months, repsectively, to start a kickstarter campaign.  Additionally, these months have yielded the most total successfull outcomes with May at 111 total successes and June at 100.  Furthermore, the total number of failures and cancelations during these months is not drastically higher than in other months, meaning the difference in successes and failures differs most in May, then June.  In sum, the data shows that starting a theater campaign with Kickstarter should be done in May or June to yield the best chance of a successful outcome.
</p>
<p>
While May and June are the most ideal months to start a theater campaign, December is statistically the worst month to start such a campaign.  December sees the fewest number of campaigns started, and of those that do begin in the year's final month fewer than 50% (37 out of 75 total) achieve success with 35 failing and another 3 canceling.
</p>
  
<h3>What can you conclude about the Outcomes based on Goals?</h3>
<p>
Using Exhibit 2.1, there is evidence to suggest that there is an inverse relationship between rate of success and campaign goal where there are large quantities of data.  Using the tabulated data on sheet "Outcomes Based on Goals" you see a major drop off in the number of campaigns after the 10,000 to 14,999 range. The downward trend in successful campaigns against rising campaign goals continues until the 35,000 to 39,999 range where from there until the end of the graph there appears to be no relationship between campaign goal and outcome, however at this point there is not a large quantity of data and so any failure or success is magnified (i.e. 45,000 to 49,999 had 1 campaign that failed out of 1 total campaign sending the success rate to 0%) on the graph.  To have the best chance at success, a play's goal should remain under 4,999.
</p>
<h3>What are some limitations of this dataset?</h3>
<p>
In reviewing the case for which month a theater campaign should begin, there is an absence of "why" May and June are the most successful months.  Could it be that people are willing to spend their tax refunds during these months or does warmer weather induce theater-fever among the masses?  With what we have, it is not possible to establish a correlation between months of the year and campaign success likelihood.
</p>
<p>
In making the case for campaign goals vs. outcome, it may be that we set our ranges to be too large to make meaningful analysis.  When we see such an uneven spread of totals right off the bat, it may be wise to define the quartiles and then set the universe of ranges within a smaller margin and then divide them in the rows as we did further from there.
</p>
<h3>What are some other possible tables and/or graphs that we could create?</h3>
<p>
There are several options that come to mind.  First we could create a box and whisker plot specific to theater and/or plays (whichever we want to drill into) to get an idea of the measurements of central tendency.  This could better assist us in an analysis like the goals vs. outcomes where we may be able to better decide what the ranges should be for each category (i.e. it may have been wiser to increment the groupings by 1999 instead of 4999 and set the final group as "greater than 35000", no basis for that, just thought).
</p>
<p>
Additionally, some pie charts comparing the outcomes of the different parent categories or even subcategories of theater could have also further helped our understanding of the performance of theater campaigns across all campaigns and further the different theater subcategories performances against one another.
</p>
<p>
Finally, collecting data from other fundraising websites could also benefit our analysis, for instance there may be sites more dedicated to raising funds for the arts as opposed to raising funds for technology or businesses.
</p>
