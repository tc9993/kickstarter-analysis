# kickstarter-analysis
Performing analysis on Kickstarter data to uncover trends

<h2>Analyses</h2>
  
<h3>US Campaign</h3>
  
  <b>Title</b>: Fever<br>
  <b>Country:</b> United States<br>
  <b>Category:</b> Theater<br>
  <b>Subcategory:</b> Play<br>
  <b>Desired Goal:</b> $10,000<br>
  
<p>
Upon reviewing all Kickstarters for the subcategory "Plays" from the U.S., we find that there is a high rate of success as 62% of all campaigns ended successfully, including live, ongoing campaigns (see Exhibit 1.1).  Upon drilling down into the specifics of successes and failures, for U.S. Plays campaigns, we find some vast differences in the measures of central tendency.  Upon reviewing the measures of central tendency for goals and pledges for both Successful and Failed campaigns in the U.S. (see Exhibit 1.2 for Goal-related measurements or the "Descriptive Statistics" sheet within the included excel file for goal- and pledge-related data in one place), Failed campaigns' mean goal was $10,554 with a standard deviation of $21,968, while successful campaign goals averaged $5,049 with a standard deviation of $7,749.
</p>
<p>
<img src="https://github.com/tc9993/kickstarter-analysis/blob/main/Theater_Plays_Outcomes.png?raw=true" alt="US Play Outcomes Pie Chart" height=50% width=50%><br>
<b>Exhibit 1.1:</b> Pie Chart of all U.S. campaign outcomes of subcategory "Plays"
</p>
<p>
Continuinig with analysis of the measurements of central tendency, you will find that both successful and failed campaign average goals are just slightly greater than the upper quartile of their respective outcome's, this tells us that more than 75% of all campaign goals, despite their outcome, are less than the mean goal and thus that the data is skewed to the right and so some extremely high campaign goals are prevalent in measuring these central tendencies.
</p>
<p>
  <table style="width:100%">
  <tr>
    <th></th>
    <th>Successful</th>
    <th>Failed</th>
  </tr>
  <tr>
    <td>Mean Goal</td>
    <td>$5,049</td>
    <td>$10,554</td>
  </tr>
  <tr>
    <td>Median Goal</td>
    <td>$3,000</td>
    <td>$5,000</td>
  </tr>
  <tr>
    <td>Standard Deviation of Goal</td>
    <td>$7,749</td>
    <td>$21,968</td>
    </tr>
    <td>Upper Quartile of Goal</td>
    <td>$5,000</td>
    <td>$10,000</td>
    </tr>
    <tr>
  <td>Lower Quartile of Goal</td>
  <td>$1,500</td>
  <td>$8,000</td>
  </tr>
  <tr>
  <td>IQR of Goal</td>
  <td>$3,500</td>
  <td>$8,000</td>
  </tr>
</table>
<br>
<b>Exhibit 1.2:</b> Campaign Goal Measures of Central Tendency
</p>
<p>
  Overall, the recommendation would be to lower the desired goal/cost of production in any way possible to get closer to, ideally below, the $5,000 mark, as a goal of $10,000 falls just below the average goal of failed campaigns despite the general success of U.S. plays reaching their campaign goal at 62%.
  </p>
  <br>
<h3>Great Britain Campaign</h3>
  
  <b>Country:</b> Great Britain<br>
  <b>Category:</b> Theater<br>
  <b>Subcategory:</b> Musical<br>
  <b>Desired Goal:</b> £4,000<br>
  <p>
  In taking a look at campaigns in Great Britain (GB) for musicals, we initially find that successful campaigns, by percentage, come in at about 39% when including "Canceled" campaigns along with successful and failed (see Exhibit 2.1).  Though the data sample in this case is much smaller than the U.S. Plays data sample was. 
</p>
  <p>
  <img src="https://github.com/tc9993/kickstarter-analysis/blob/main/GB_Musical_Outcomes.png?raw=true" alt="GB Musical Outcomes Pie Chart" height=50% width=50%><br>
<b>Exhibit 2.1:</b> Pie Chart of all GB campaign outcomes of subcategory "Musical"
  </p>
  <p>
  Looking at a box and whisker plot (see Exhibit 2.2) we can see that the mean goal of all GB Musicals is right at £4,000, while the median goal is much lower at £2,000.  Right away this tells us that there are outliers skewing this data sample as seen on the chart at about the £15,000 mark.  Half of all campaign goals are £2,000 or less.  This £2,000 mark is still greater than the upper quartile of all GB Musical campaign pledges, £1,664, where the mean was £1,151.
  </p>
  <p>
<img src="https://github.com/tc9993/kickstarter-analysis/blob/main/GB_Musicals_BW_Plot.png?raw=true" alt="GB Musicals Box and Whisker Plot" height=57% width=57%><br>
  <b>Exhibit 2.2:</b> Box and Whisker Plot of GB Musical Campagins
  </p>
  <p>
  Overall, the recommendation is, once again, to bring the desired goal of this campaign down as close to, if not below £2,000 as possible.  This would meet the median of all GB Musical campaigns as well as the mean goal of successful campaigns (£2,080), but would still exceed the upper quartile of pledges achieved.  It is possible that the number of canceled campaigns is what has resulted in the lower quartile being £0, that still does not tell the full story as "Canceled" campaigns make up 19% of GB Musicals, and at least 25% of all pledges were £0.  Thus the lower the campaign goal, the more likely the pledges will meet or exceed said goal. 
