# Kickstarting with Excel

## Overview of Project
The kickstarter data set provided information about how an individual Louise started different fundraising campaigns launched in different countries since 2009. 
The Goal column tells us how much money each campaign will need to succeed.
The Pledged column tells us how much each campaign actually made.
The Outcomes column tells us if the campaign met its goal.
The Country column lists the country in which the campaign was started.

### Purpose
We would be analyzing the data to provide various insights with regards to campaigns that succeded, failed and are cancelled and how they fared corelating to different goal criterias and funding targets.

## Analysis and Challenges
We would analyzing the data for Category 'Theater' based on the Launch Data and sub-category 'Plays'.

### Analysis of Outcomes Based on Launch Date
The first analysis is based on the Launch data for Parent Category 'Theater' since 2009.
By looking at the chart, on a monthly basis the count of successful campaigns get a sudden rise from March till May. 
The count dips starting from May until September only to see a slight increase October to drop till December. 

This trend stands equally true for the failed campaigns as well. Relatively the Cancelled campaigns remained low. Theaters also occupies the top spot for the highest number of succesfull campaigns compared to other categories.

![Outcomes Based on Launch Date - Theater](https://github.com/c3crocks/kickstarter/blob/main/Resources/Theater_Outcomes_vs_Launch.png)

If we take look at the trend over years rise in pledges in Theater started from the year 2014 and contnued a similar trend year over year. 
From year 2010 to 2013 all campaigns have remained successful with 0 cancellation/failure. 

![Outcomes Based on Launch Date - Theater](https://github.com/c3crocks/kickstarter/blob/main/Additional_Images/Thetres_Outcome_LaunchDate.png)

Out of other Categories Journalism is an exception where all campaigns were cancelled. 

![Outcomes Based on Launch Date - Journalism](https://github.com/c3crocks/kickstarter/blob/main/Additional_Images/Journalism_Outcome_LaunchData.png)

### Analysis of Outcomes Based on Goals
In the chart of Outcomes based on Goals, we are looking at the Sub-Category 'Plays'.

The chart shows that campaigns with a goal 'less than $1000' have shown the highest success rate of 75.81% trailing by goal category '$1000 to $4999' at 72.61%.
Failure percentage also has the same 2 categories fighting for the top spot with 'less than 1000' at 24.19%.

No campaigns were cancelled for plays sub-category. 

![](https://github.com/c3crocks/kickstarter/blob/main/Resources/Outcomes_vs_Goals.png?raw=true)

Just by lookinga at the chart we can conclude that category 'less than 1000' category to be more successful. 

However if we take a look at the count chart below we can observe that the category '$1000 to $4999' has higher number of campaigns even though it fell short to prove its caliber on the percentage chart. 
We can observe that better insights can be seen by showing the Outcomes by Based on Goal by counts. 

![](https://github.com/c3crocks/kickstarter/blob/main/Additional_Images/PlayCount.png)

### Challenges and Difficulties Encountered
I encountered the following challenge while completing the assignment
#### Sorting Goal Categories 
- Sorting them as per requirements in the chart from the pivot table was something I couldn't figure out
- I used a sorting order in the end of the table to get it right only to face another issue where it showed up in the chart too
- Although I figured out by creating a line chart by selecting the dataset directly.
- Please refer to the highlighted section in the screenshot below

![](https://github.com/c3crocks/kickstarter/blob/main/Additional_Images/Outcomes_vs_Goal_Sorting.png)

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
	- The chances of a Theater act is less likely to fail in comparison to other campaign categories. 
		- From the given data, Theater is best option to launch campaigns starting from April to May
		- It would be best to avoid period between October to January. 
	- Among the 3 sub-categories, 'plays' remains most successfull while musical and spaces showed almost equal potential (Refer to the chart below)

![](https://github.com/c3crocks/kickstarter/blob/main/Additional_Images/Sub-Category_Outcome_LaunchDate.png) 

- What can you conclude about the Outcomes based on Goals?
	- The 'Less than 1000' category showed promising results based on the percentage of succesfful campaigns.
	- However the campaigns with goal category '1000 to 4999' remain the strongest contender for theater category with 387 successful campaigns compared to only 141 of 'Less than 1000'. 
	- Conducting more campaigns with '1000 to 4999' category would give promising results. 
	
- What are some limitations of this dataset?
	- The dataset provided information about each campaigns was limited. It would have been easier to categorize them under comedy, thriller, suspense and so on
		- This could also help us understand if themes affected the campaigns to fail
	- There was no information about the backers
		- is the pledge coming from an institution or individual
		- Reasons to participate
	- FX rates for currency at the time (USD to GBP, USD to EUR and so on) to precisely calculate the average donation in each country

- What are some other possible tables and/or graphs that we could create?

	- All images below are excluding Journalism since all campaigns were cancelled.

##### Count of Backers (Excluding Journalism)

![](https://github.com/c3crocks/kickstarter-analysis1/blob/main/Additional_Images/CountofBackers.png)

##### Count of Backers by Year (Excluding Journalism)

![](https://github.com/c3crocks/kickstarter-analysis1/blob/main/Additional_Images/CountofBackersOverTime.png)

##### Count of Backers by Country (Excluding Journalism)

![](https://github.com/c3crocks/kickstarter-analysis1/blob/main/Additional_Images/CountofBackersbycountry.png)

##### Count of Exceeded Goals and Underfunded Goal (Excluding Journalism)

The below analysis was done by counting campaigns that exceeded its funding goals. 
Expression used: 
if((Pledged/Goal)*100)-100 > 0 is 'Exceeded Goal'
if((Pledged/Goal)*100)-100 < 0 is 'Underfunded Goal'

![](https://github.com/c3crocks/kickstarter-analysis1/blob/main/Additional_Images/GoalsPie.png)



