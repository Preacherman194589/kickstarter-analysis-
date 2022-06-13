# Kickstarting with Excel

## Overview of Project
The project asked that we look at the Kickstarters Campaign Dataset to determine how much it would cost for Louise to budget a play “Fever” she wrote.  

### Purpose
The outcome of budget prices and launch dates allows Louise to have a better understanding on what it would cost her to budget and how much money she needs for pledges. 

## Analysis and Challenges
When looking at Kickstarters Campaign Dataset, it showed over 50000 plays throughout the world. The data sheet had to be analyzed in seven different ways, “Category Statistics, Subcategory, Theater Outcome by Launch date, Failed US Kickstartes, Successful US Kickstarters, Edinburg Research and Descriptive Statistics” The challenges were making sure you have the write formula to make such changes. 

As for the Theatre Outcome by launch date we had to convert the data format by using Unix Timestamp. As for Category and Subcategory we had to use the Pivotal Table to come up with a breakdown of categories.  

As for the failed and successful Data I used the drop-down filter and marked US and failure for failure outcome and successful for success outcome. The Edinburg research and Descriptive Statistics were someone different. 

I used [VLOOKUP(lookup_value,table_array,col_index_num,range_lookup)]for Edinburg research by applying the for plays that were highlighted to show Louise how they got started.  

The Descriptive Statistics we give Louise a better understanding of the plays that failed or was successful based on the mean, median and right or left skewed which is done based on formulas.    


### Analysis of Outcomes Based on Launch Date
I am using a pivot table by capturing all Kickstarter Dataset. 

I then extracted parent categories and years, placed them in the filter, and placed the outcomes in columns and values. I placed years in a row. After analyzing the data, I conducted a line chart below  

A screenshot ot the of the overall analysis was submitted to kickstarter-analysis GitHub repository

### Analysis of Outcomes Based on Goals
Created eight columns, “Goal, Number Successful, Number Failed, Number Canceled, Target Project, Percentage Successful, Percentage Failed, Percentage Canceled

Under the Goal column I posted the less than and greater than from $1000 to $50,000 and more

Using “=COUNTIFS” Formula, I was able to use the following using the Kickstar Dataset which was changed to Kickstarter _Challenge: =COUNTIFS('Kickstarter_Challenge  '!$D:$D,"<1000",'Kickstarter_Challenge  '!$F:$F, "successful", 'Kickstarter_Challenge  '!$R:$R, "plays")
Changing the greater than equal symbol and the successful, failed and canceled changed the numbers in the columns

A screenshot ot the of the overall analysis was submitted to kickstarter-analysis GitHub repository

### Challenges and Difficulties Encountered
The challenge was learning excel and knowing what formula is needed to gather the needed information. Example: Trying to convert the date from the years was not that difficult, but dealing with the pivot table and determining which data or field goes into the four outcomes (filters, columns, rows, or values) was a part of the trial and error. In time I learned that certain fields are only good for certain outcomes. 

Two more challenges or difficulties I encountered were 1. I was preparing the visualization and saw that the outcome based on the launch date graph displayed different color lines. Working with other students, I realized that my total numbers were right, but the numbers in the columns were showing ascending numbers, not descending numbers; once I changed the tab, the numbers and color line changed. 

The last issue was the outcome based on Goals which caused me more challenges than I thought; I realized that the fewer and greater symbols were turned around, which caused my numbers to be high. Once I realized the placement of the greater and equal symbol, my numbers aligned up. I also learned from the assistant team that when you're analyzing numbers, you must tab the whole column and not try to use a filter to get to a certain group of data. The formula recognized the whole data, not part of the data.   


## Results

- **What are two conclusions you can draw about the Outcomes based on Launch Date?** 
In May and June, the plays on Kickstarter Dataset had a successful outcome but also a higher failure. The failures or successes could be based on planned events, weather, finance, or other outcomes. Another concern was October; the outcome started to drop until February the following year. There could have been many events that could have contributed to the drop. I did not notice any canceled outcomes based on dates or goals.   

- **What can you conclude about the Outcomes based on Goals?**
The two areas that I noticed that benefited the success of the plays were, 1. when the monetary goal was under $5,000, especially between $1000 to $5000. The number of successful plays rose; however, more plays were performed based on the outcome. There were also a lot of failures, which could be contributed to unknown circumstances. Another observation was when the goal was over $25,000, it appeared that the successful number dropped, but the failure number rose.  

- **What are some limitations of this dataset?**
What I felt was missing was the population of income and the city/county where the plays were performed. Also, the price of the tickets and how much it would cost to develop a play.

- **What are some other possible tables and/or graphs that we could create?**
A list of the origin of plays performed that are more successful and are failures. The age group, gender, and economic income will also determine the outcome for the date and goal.   
