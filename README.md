# Kickstarter Analysis

## Table of Contents
* [Overview](#overview)
* [Methods](#methods)
* [Results](#results)
* [Summary](#summary)

## Overview

This is an analysis of over 4000 Kickstarter crowdfunding campaigns to help a playwright, Louise, who wants to start a crowdfunding campaign for a play that she wrote called ***Fever***. She proposes to open the play in the US and has budgeted $10,000 for the project.  Louise has also shown an interest in crowdfunding data in Great Britain, in particular, a play called ***Foresight***, five plays that she enjoyed at the Edinburgh Festival Fringe, and musicals in general. 

## Methods

1. Campaign outcomes were colored coded in order to quickly identify campaigns that succeeded, failed, were cancelled or that are currently live.
2. Percentage funded was determined using the ROUND function and value shading to show the range of percentage funded from red (failed) through blue (well funded).
3. Kickstarter data was further broken down to determine the average donation of each project.  ![alt text](https://github.com/rkaysen63/kickstarter-analysis/blob/main/At%20a%20Glance.png)
4. Categories were further broken down into subcategories and pivot tables were created to look at the outcomes of campaigns by category and subcategory.  
5. Unix timestamps were converted into a day-month-year format and a pivot table was created to look for a relationship between outcomes and launch dates.
6. Search function was used to zero-in on a particular play, ***Foresight***, in order to look at the market in Great Britain and to glean more information about this particular play.  ***Walken on Sunshine*** was similarly located and evaluated.
7. Used VLOOKUP to find funding information about 5 plays that were performed at the Edinburgh Festival Fringe.
8. Success and failures of US plays were filtered separately.  Then the mean and median of goals and pledges were calculated and a comparison was made between successful and failed campaign goals and pledges.  Standard deviations were calculated for mean values and interquartile range was calculated for median values.
9. Created a box and whisker plot to campare campaign goals and total amounts pledge for musicals in Great Britain.

## Results

1. The median of the average donation for successful campaigns for US plays is $69 with an IQR of $53. Louise may be able to use this information to set a target donation that is likely to succeed and to offer incentives. 
2. Over half of the crowdfunding campaigns for plays in the US are successful.  412 successful campaigns of 671 plays. ![alt text](https://github.com/rkaysen63/kickstarter-analysis/blob/main/SubCategoryOutcomes.png)
3. An analysis of a time plot of launch dates shows that campaigns are more likely to succeed if they are kicked off in the month of May. ![alt text](https://github.com/rkaysen63/kickstarter-analysis/blob/main/MonthlyTrends.png)
4. The ***Foresight*** campaign was successful, reaching 100% of it's goal.  The average donation of $117.88 is higher than the US median for plays and there were only 17 backers.  It's goal of $2000 may have been easier to reach than Louise's since it was 1/5th ***Fever's*** goal.
5. ***Walken on Sunshine*** is a US play with the same goal of $10,000 as Louise's play, ***Fever***.  It had a successful campaign that was kickstarted in the US in April and the campaign ended in one month.  The average donation was $71.24, which is barely over the median average donation for US campaigns for plays.  ***Walken on Sunshine*** had 173 backers.
6. Five plays that Louise enjoyed at the Edinburgh Festival Fringe were funded by Kickstarter. All of 5 had successful funding campaigns.  The Median Goal and Median Pledge were at $2000 and $2020, respectively.   The median average donation was $36.61. ![alt text](https://github.com/rkaysen63/kickstarter-analysis/blob/main/Edinburgh%20Research.PNG)
7. By comparing the median of successful US campaign goals and pledges for plays to failed campaign goals and pledges, a couple of things are apparent.  The failed campaigns generally have higher fundraising goals than successful campaigns and Louise's goal of $10,000 is 233% over the median goal of successful campaigns thereby falling outside the range of outliers for successful campaigns. ![alt text](https://github.com/rkaysen63/kickstarter-analysis/blob/main/US%20Play%20Campaigns.png)
8. Box and whisker plot of campaign goals and pledges for musicals in Great Britain shows that the median goal of successful British campaigns is outside interquartile range of pledges.  Campaigns most likely to succeed would have a budget of $1500 or less.  ![alt text](https://github.com/rkaysen63/kickstarter-analysis/blob/main/British%20Musical%20Funding.png)

## Summary

Analysis of Kickstarter crowdfunding data for Louise's project, ***Fever***, gave mixed results.  While over half of the Kickstarter crowdfunding campaigns for plays in the US were successful, including some plays with goals much the same as hers, e.g. ***Walken on Sunshine***, the likelihood of success is somewhat diminished by her budget which is 1.5 times the interquartile range.  If Louise wants a successful campaign, she may consider reducing her budget, starting her campaign in May, and setting suggested donations of $25, $50 and $75.

As to her other interests in Great Britain's theater market, 
* ***Foresight's*** campaign was successful reaching 100% of it's goal with an average donation well above the US median for plays and with very few backers.
* The Edinburgh Festival Fringe research showed that all five plays that interested Louise, ***Be Prepared, Checkpoint 22, Cutting Off Kate Bush, Jestia and Raedon, The Hitchhiker's Guide to the Family*** were all successful crowd funding campaigns.  The median goal was $2000, median pledge was $2020, median average donation was $37, and median number of backers was 56.
* Analysis of the Kickstarter campaign goals and pledges for musicals in Great Britain indicate that Louise's budget of £4000 may be too high since it falls outside 1.5 times the interquartile range for pledges.  If she can bring her budget down under $2000 she may greatly increase her chances for a successful crowdfunding campaign.
