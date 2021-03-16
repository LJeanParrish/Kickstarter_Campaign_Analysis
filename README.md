# Kickstarter Campaign Analysis

## Background

Over $2 billion has been raised using the massively successful crowdfunding service, Kickstarter, but not every project has found success. 

Of the more than 300,000 projects launched on Kickstarter, only a third have made it through the funding process with a positive outcome.

Getting funded on Kickstarter requires meeting or exceeding the project's initial goal, so many organizations spend months looking through 

past projects in an attempt to discover some trick for finding success. 

The purpose of this project is to organize and analyze a database of 4,000 past projects in order to uncover any hidden trends.

![Kickstarter Table](Images/FullTable.png)


## Project

I used a database of 4,000 previous Kickstarter campaigns to analyze the information and made conclusions on campaign criteria that determined success or failure.

To do this, I used conditional formatting to fill each cell in the `state` column with a different color, depending on whether the associated campaign was successful, failed, or canceled, or is currently live.

I then created a `Percent Funded` column which used a formula to uncover how much money a campaign made to reach its initial goal.

Conditional formatting was then applied to the `Percent Funded` column ina three-color scale based on the success of funding. 

I then calculated the `Average Donation` from each backer for the project paid on average.

To better understand the project categories, I added new columns then used formulas to split the `Category and Sub-Category` column into two parts.

  ![Category Stats](Images/CategoryStats.png)

I then created a pivot table that visualized the count of campaigns that were successful, failed, canceled, or are currently live per category.

A second pivot table was then created that could be filtered by country based on the table created.

  ![Subcategory Stats](Images/SubcategoryStats.png)

To dive deeper into this data another pivot table was created to that counted successful, failed, canceled, or are currently live by sub-category.

I converted the `deadline` and `launched_at` columns from Unix timestamps. Next I created a new pivot table with a column of `state`, rows of `Date Created 
Conversion`, values based on the count of `state`, and filtered based on `parent category` and `Years`.

This was then visualized in a line graph.

At the conclusion of my analysis, I answered the following questions:

	* What are three conclusions we can draw about Kickstarter campaigns?
	* What are some limitations of this dataset?
	* What are some other possible tables and/or graphs that we could create?

Additional analysis was requested and as such I broke down the projects using the `COUNTIFS()` formula, count how many successful, failed, and 
canceled projects were created with goals within a series of rages. I then populated the `Number Successful`, `Number Failed`, and `Number Canceled` columns with this data.

Next I added the values in the `Number Successful`, `Number Failed`, and `Number Canceled` columns and populated the `Total Projects` column. 
Then, using a mathematical formula, I found the percentage of projects that were successful, failed, or canceled per goal range.

A line chart was created that graphed the relationship between a goal's amount and its chances at success, failure, or cancellation.

I used Excel to evaluate the following for successful campaigns, and then for unsuccessful campaigns:

  * The mean number of backers.

  * The median number of backers.

  * The minimum number of backers.

  * The maximum number of backers.

  * The variance of the number of backers.

  * The standard deviation of the number of backers.



