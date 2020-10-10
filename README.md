# ELECTION ANALYSIS
Create an Election Analysis "PyPoll" with Python
## Overview of Project
A Colorado Board of Elections employee has given you the following task to complete the election audit of a recent local congressional election.

1. Calculate the total number of votes cast.
2. Get a complete list of candidates who received votes.
3. Calculatae the total number of votes each candidate received.
4. Calculate the percentage of votes each candidate won.
5. Determine the winner of the election based on popular vote.

## Resources

* Data Source: election_results.csv
* Software: Python 3.9, Visual Studio Code 1.50.0

For more information, read the [`Documentation on Python data typess`](https://docs.python.org/3.6/library/stdtypes.html#numeric-types-int-float-complex). 

## Analysis and Challenges
In this project, our final Python script will need to be able to deliver the following information when the script is run: 

1. Total number of votes cast
2. A complete list of candidates who received votes
3. Total number of votes each candidate received
4. Percentage of votes each candidate won
5. The winner of the election based on popular vote

#### Our Challenge Data Background
> After giving you an overview of the election audit tasks, we wants to go over the steps required in detail. Showing you a technique commonly used by programmers to write steps of their code, which is called `pseudocode`. Pseudocode will make the audit easier to present to nontechnical colleagues and stakeholders.

To facilitate the design process, programmers use `pseudocode` to create models or flowcharts for their programs. 
Pseudocode is like a roadmap of what you think your code will look like or the steps you'll take to complete the task at hand.

Pseudo means **"fake,"** so pseudocode is essentially fake code. Pseudocode is an informal language that has no syntax rules and is not meant to be executed. The point of using pseudocode is to focus on the overall design of the program.


### Analysis of Outcomes Based on Launch Date
 
#### Deliverable Requirements with detail analysis:
**1. Total number of votes cast**

> In the "Years" column, use the `YEAR()` function to extract the year from the “Date Created Conversion” column.


![name-of-you-image](https://github.com/emmanuelmartinezs/kickstarter-analysis/blob/master/artifacts_images/A%20Years%20column%20is%20created.PNG?raw=true)


**2. A complete list of candidates who received votes.**

> Created a pivot table from the KickStarter worksheet, and placed the pivot table in a new sheet.


![name-of-you-image](https://github.com/emmanuelmartinezs/kickstarter-analysis/blob/master/artifacts_images/Pivot%20Table%20for%20Outcomes%20Based%20on%20Launch%20Date.PNG?raw=true)


**3. Total number of votes each candidate received.**

> Placed the appropriate pivot table pivot table based on Parent Category and the Years data filtered.


![name-of-you-image](https://github.com/emmanuelmartinezs/kickstarter-analysis/blob/master/artifacts_images/Pivot%20table%20filters%20on%20Parent%20Category%20and%20Years.PNG?raw=true)


**4. Percentage of votes each candidate won.**

> Placed the appropriate pivot table fields.


![name-of-you-image](https://github.com/emmanuelmartinezs/kickstarter-analysis/blob/master/artifacts_images/A%20Years%20column%20is%20created.PNG?raw=true)


**5. The winner of the election based on popular vote.**

> Placed the appropriate filter on pivot table.


![name-of-you-image](https://github.com/emmanuelmartinezs/kickstarter-analysis/blob/master/artifacts_images/Filtered%20on%20Theater.PNG?raw=true)



## Summary

#### The analysis of the election show that:
**1. A new sheet is created with eight columns and twelve rows, according to the instructions.**

> In the new sheet, create the following columns to hold the data:
> - Goal
> - Number Successful
> - Number Failed
> - Number Canceled
> - Total Projects
> - Percentage Successful
> - Percentage Failed
> - Percentage Canceled.

> In the “Goal” column, create the following dollar-amount ranges so projects can be grouped based on their goal amount.


![name-of-you-image](https://github.com/emmanuelmartinezs/kickstarter-analysis/blob/master/artifacts_images/eight%20columns%20and%20twelve%20rows.PNG?raw=true)


**2. The `COUNTIFS()` function is used to populate the "Number Successful," "Number Failed," and "Number Canceled" columns, based on the project "outcome," the "goal" amount using the goal ranges in Step 3, and the Subcategory "plays".**

> Used `COUNTIFS()` functions to populate the "Number Successful," "Number Failed," and "Number Canceled" columns by filtering on the Kickstarter "outcome" column, on the "goal" amount column using the ranges created, and on the "Subcategory" column using "plays" as the criteria.Created a pivot table from the KickStarter worksheet, and placed the pivot table in a new sheet.


![name-of-you-image](https://github.com/emmanuelmartinezs/kickstarter-analysis/blob/master/artifacts_images/The%20COUNTIFS()%20function.PNG?raw=true)


**3. The `SUM()` function is used on each row to add the "Number Successful," "Number Failed," and "Number Canceled" columns to populate the "Total Projects" column.**

> Use the `SUM()` function to populate the "Total Projects" column with the number of successful, failed, and canceled projects for each row.


![name-of-you-image](https://github.com/emmanuelmartinezs/kickstarter-analysis/blob/master/artifacts_images/The%20SUM()%20function.PNG?raw=true)


**4. The percentages of successful, failed, and canceled projects are calculated based on the data from the "Total Projects," "Number Successful," "Number Failed," and "Number Canceled" columns.**

> Calculated the percentage of successful, failed, and canceled projects for each row.


![name-of-you-image](https://github.com/emmanuelmartinezs/kickstarter-analysis/blob/master/artifacts_images/The%20percentages.PNG?raw=true)


**5. A line chart is created and saved as **[Outcomes_vs_Goals.png]** with the goal-amount ranges on the x-axis, the percentage of successful, failed, or canceled projects on the y-axis, and an appropriate title.**

> Created a line chart titled "Outcomes Based on Goal" to visualize the relationship between the goal-amount ranges on the x-axis and the percentage of successful, failed, or canceled projects on the y-axis.


![name-of-you-image](https://github.com/emmanuelmartinezs/kickstarter-analysis/blob/master/artifacts_images/Outcomes_vs_Goals.PNG?raw=true)



### Challenges and Difficulties Encountered

Biggest challenge was filtering the pivot table to visualize the relationship between parent category and years, adding the correct dataset into the Columns, Rows and Values.


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

> As Conclusions, our Line charts we can see by looking at our data that the months of **May and June** both have a greater success rate.
> A bar chart **wouldn't** be able to convey this information in the same manner.



![name-of-you-image](https://github.com/emmanuelmartinezs/kickstarter-analysis/blob/master/artifacts_images/Theater_Outcomes_vs_Launch.PNG?raw=true)



- What can you conclude about the Outcomes based on Goals?

> As Conclusion, our Outcomes based on Goals measures using line chart of central tendency work in practice help us finding the mean and median for each dataset's (the failed and successful campaigns).


![name-of-you-image](https://github.com/emmanuelmartinezs/kickstarter-analysis/blob/master/artifacts_images/Outcomes_vs_Goals.PNG?raw=true)


- What are some limitations of this dataset?

> Some limitation can be that we'd like to know the deviations from the actual dataset, but because we don't know, these deviations have a subtle and slight bias to them. 


- What are some other possible tables and/or graphs that we could create?

> - Box Plots
> - Pie Graph
> - Column Graph
> - Line Graph
> - Area Graph
> - Scatter Graph





