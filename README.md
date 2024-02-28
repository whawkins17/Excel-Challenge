# Excel-Challenge
# Background:

Crowdfunding platforms like Kickstarter and Indiegogo have been growing in success and popularity since the late 2000s. From independent content creators to famous celebrities, more and more people are using crowdfunding to launch new products and generate buzz, but not every project has found success. 

To receive funding, the project must meet or exceed an initial goal, so many organizations dedicate considerable resources looking through old projects in an attempt to discover “the trick” to finding success. 

For this Excel-Challenge, I have organized and analyzed a database of 1,000 sample projects to uncover any hidden trends through use of conditional formatting, pivot tables, graphs and an overview of a statistical summary. 

# Crowdfunding:

Through conditional formatting, modify and analyze the sample-project data. Conditional formatting is used to fill each cell in the outcome column with a different color, depending on whether the associated campaign was successful, failed, canceled, or is currently live. 

A new column is created called Percent Funded to show how much money a campaign made relative to its initial funding goal. Conditional formatting is used again to fill each cell in the Percent Funded column according to a three-color scale. The scale starts at 0 with a dark shade of red, and it should transition to green at 100 and blue at 200.

With the same data set, an additional column is created called Average Donation. Average Donation indicates how much each project backer paid on average. 

# Category/Sub-Category:

Two new columns, one called Parent Category and another called Sub-Category are created by using formulas to split the "Category and Sub-Category" column into two new columns. 

A new sheet within excel is created which includes a pivot table that analyzes the initial worksheet to count how many campaigns were successful, failed, canceled, or are currently live per category. A stacked-column pivot chart that can be filtered by country based on the table is also created. 

An additional new sheet is created with a pivot table that analyzes the initial sheet to count how many campaigns were successful, failed, or canceled, or are currently live per sub-category. A stacked-column pivot chart that can be filtered by country and parent category based on the table is also created. 

# Timeline:

The dates in the deadline and launched_at columns use Unix timestamps. Two new columns are created to convert data contained into Excel's date format. 1) Date Created Conversion is created to convert the data contained in launched_at into Excel's date format and 2) Date Ended Conversion is created to convert the data contained in deadline into Excel's date format.

A pivot table that has a column of Outcome, rows of Date Created Conversion, values based on the count of Outcome, and filters based on Parent Category and Years is created and reflected in a pivot-chart line graph for visualization.

# Conclusions:

Conclusion 1: Most campaigns fall into two categories: Successful and Unsuccessful/Failed. 

Conclusion 2: During the months June and July, there is an increase in successful campaigns.

Conclusion 3: The month of July has the highest number of successful campaigns with the months of January and December having the highest number of unsuccessful/failed campaigns. 

* These three conclusions shed light on the dynamics of crowdfunding campaigns, which include the distribution across outcomes, seasonal variations and potential trends over time. 

# Limitations:

Limitations of the data set include:
1. Lack of information on campaign categories/types.

2. The lack of data on funding amounts limits the ability to perform a thorough assessment on the financial impact of successful crowdfunding campaigns. 

3. The lack of data/understanding of regional trends or audience demographics.
   
# Additional Tables/Graphs to consider:

1. A table showing success rates for different project categories.

2. A graph that correlates funding amounts with successful/unsuccessful campaigns.

3. A regional map that shows distribution of successful campaigns: Benchmarks


# Crowdfunding Goal Analysis:

A new sheet with 8 columns containing: 
Goal, Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed, and Percentage Canceled.

In the Goal column, create 12 rows with the following headers:
* Less than 1000
* 1000 to 4999
* 5000 to 9999
* 10000 to 14999
* 15000 to 19999
* 20000 to 24999
* 25000 to 29999
* 30000 to 34999
* 35000 to 39999
* 40000 to 44999
* 45000 to 49999
* Greater than 50000

Using the COUNTIFS() formula, populate: Number Successful, Number Failed, and Number Canceled columns with the data within the ranges listed above. 

Using a mathematical formula, the percentage of projects that were successful, failed, or canceled per goal range are created and visually displayed within a line chart that graphs the relationship between a goal amount and its chances of success, failure, or cancellation.

# Statistical Analysis:

A statistical table includes one column for the number of backers of successful campaigns and one column for unsuccessful campaigns. A table containing a column for the number of backers of successful campaigns and a column for unsuccessful campaigns. The following values are evaluated for both successful and unsuccessful campaigns. 

* The mean number of backers
* The median number of backers
* The minimum number of backers
* The maximum number of backers
* The variance of the number of backers
* The standard deviation of the number of backers

# Statistical Analysis Review:

Creating a summary statistics table is one of the most efficient ways to characterize quantitative metrics.

For both the successful and unsuccessful/failed campaigns, the data is not evenly distributed, and both indicate outliers within the data. For that reason, it is best to use the median when summarizing the data. In my research, when utilizing either the mean or the median to explain data, the median is used when the distribution of data values is skewed or when there are clear outliers as mentioned previously. 

There is higher variability in the successful groups verses the unsuccessful/failed groups.







