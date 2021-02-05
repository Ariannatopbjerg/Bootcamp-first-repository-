# Kickstarter-Theater-Outcomes-Analysis
## Project Overview
The client; Louise, produced a play called *Fever*, which came close to its fundraising goal in a short amount of time. Louise is now curious about how different campaigns fared in relation to their launch dates and their fundrasing goals. In the data sheet that Louise has given, the campaigns are from various countries and years. Not only are there theater play campaigns, but a variety of crowdfunding projects. For this analysis, we will only be focusing on theater campaigns and theater play campaigns. 
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date & Challenges
#### Analysis
To analyze campaign outcomes based on launch date, I created a [pivot table](https://github.com/Ariannatopbjerg/Bootcamp-first-repository-/blob/main/Kickstarter_Challenge.xlsx) in worksheet "Theater Outcomes by Launch Date," to view this data and a [line graph](https://github.com/Ariannatopbjerg/Bootcamp-first-repository-/blob/main/Theater_Outcomes_vs_Launch.png) to visualize what the pivot table was displaying. 
Before I developed a pivot table, I first had to make a column; titled "Years" in the [kickstarter spreadsheet](https://github.com/Ariannatopbjerg/Bootcamp-first-repository-/blob/main/Kickstarter_Challenge.xlsx). I used the YEAR() function to collect the years from the “Date Created Conversion” column so I can use this new column in my pivot table, signifying launch dates of the campaigns I am looking at. 

I used fields “Date Created Conversion” for rows; removing subfields “Years2” and “Quarters” to just show months, “outcomes” for columns and values, and “Years” and “Parent Category” for filters. I then filtered the table to only show theater campaigns. I then reorganized the outcomes so successful campaigns are shown first and failed in the second column. I then created a line graph for the pivot table.  
#### Challenge
I did not have any difficulty producing the pivot table or the line graph. I did have to see which subfields I needed to cut to only show months but figured it out fairly quickly.
### Analysis of Outcomes Based on Goals & Challenges
#### Analysis
To visualize the percentage of successful, failed, and canceled plays based on the funding goal amount, I created a table. I used the COUNTIFS() function to collect the outcome and goal data for the “plays” subcategory first. This step can been seen in the [“Outcomes Based on Goals” worksheet](https://github.com/Ariannatopbjerg/Bootcamp-first-repository-/blob/main/Kickstarter_Challenge.xlsx), in columns B:D of the table. I then calculated total projects pertaining to each goal range by using the SUM() function; seen in column E. To get the percentages of the outcomes in each row, I used this formula: *(outcome value/total projects value)*100*. To make the percentages easier to read, I took out ‘*100*’ of the equation and used the percentage icon in excel instead. I then created a [line graph](https://github.com/Ariannatopbjerg/Bootcamp-first-repository-/blob/main/Outcomes_vs_Goals.png) to better visualize the data within the table. 
#### Challenge
There was no difficulty in creating the table or graph. What could be challenging is using the COUNTIF() function and getting all of the correct/necessary columns to get to value you want.
## Results
### Outcomes Based on Launch Date
In [“Theater Outcomes in Relation to Launch Date”](https://github.com/Ariannatopbjerg/Bootcamp-first-repository-/blob/main/Theater_Outcomes_vs_Launch.png) graph, the month that launched the most successful Kickstarter campaigns was May. However, January, March, September and November all had roughly the same number of failed campaigns launched. October also had the highest failed campaigns. This can be determined by examining the points along the trend lines of the chart. Overall, there are more successful campaigns than failed and canceled campaigns. The only time that Successful and failed campaigns were in equal was in the month of December.
### Outcomes Based on Goals
There were no canceled theater plays in the data set. According to the [graph](https://github.com/Ariannatopbjerg/Bootcamp-first-repository-/blob/main/Outcomes_vs_Goals.png), Theater play campaigns that exceeded $45,000 had a higher failed rate. There is a higher success rate when the campaign goals were less than $5000. This can indicate that plays that had goals on the lower price spectrum succeeded more than ones that set their goals too high. Can their be other factors affecting the failed campaings? Possibly. Should those other factors be analysed? Yes, if you have time to do so. 
### Was there any limitations of the dataset?
To be honest, I do not see any limitations to the kickstarter dataset. It had enough information to get the answers that I needed for Louise’s questions and concerns.
### Other possible tables and/or graphs that could have been created for this analysis
Since we are looking at data that is representing various countries, it would be interesting to see the outcomes for individual countries, like the US and GB. This way we can compare the two countries as well. 
