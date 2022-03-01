# kickstarter_challenge

# kickstarting with excel

## Overview of Project 

### Purpose
The purpose of this analysis is to understand the outcomes of different campaigns based on their launch dates and their fundraising goals. The first chart provides a visual representation of the outcomes based on launch dates and the second chart shows the results based on fundraising goals. By comparing these two findings, it can be determined if there is a pattern for success or failures. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The analysis based on launch date was completed by extracting information from the Kickstarter sheet into a pivot table. The pivot table was filtered by parent category (theater) and years. Each row was separated by months and each column was separated by successful campaigns, failed campaigns, cancelled campaigns, and the grand total for each month.  After the chart was created, the information was transferred into a line graph which provides the visual of upward and downward trends for each campaign throughout the months of the year.  
 
![image](https://user-images.githubusercontent.com/99801608/156164520-57577909-17b0-4b83-8241-a7363f06230e.png)

![image](https://user-images.githubusercontent.com/99801608/156164583-42c9d551-fe78-4c47-9c85-cc021777ba88.png)

![image](https://user-images.githubusercontent.com/99801608/156164718-969981bf-01f6-487c-9e22-3481d72818e4.png)
 
### Analysis of Outcomes Based on Goals
The analysis of outcomes based on goals was completed by extracting campaign goals numbers from the kickstarter worksheet into a new worksheet. The numbers were divided into 5,000 dollar increments between 1,000 and 50,000 dollars.  Dollars under 1,000 and over 50,000 were given their own row.  The columns include number successful, number failed, number canceled, and totals for each row.  Each row was calculated by using the excel COUNTIFS formula and filtering criteria based on the dollar amount ranges, outcomes (successful, failed, or canceled), and the plays subcategory.  After each row was calculated, three additional columns were inputted.  These columns include percentage successful, percentage, failed, and percentage canceled.  To calculate the percentage, each cell in columns B, C, and D were divided by its respective cell in columns F, G, and H. 

![image](https://user-images.githubusercontent.com/99801608/156164214-f6ff578f-cbfe-4bdd-bf59-0a1a0caacd9a.png)

 A line graph was created with the information from the chart goals sheet.  The line graph has the percentages on the y-axis and the goals on the x-axis. A line graph makes it easier to read the data and see what dollar ranges offer the most successful outcomes of goals.  
 
 ![image](https://user-images.githubusercontent.com/99801608/156165026-b82f4e0b-b035-4401-86ed-dec65f113084.png)
 

### Challenges and Difficulties Encountered

On the outcomes based on launch dates, one of the main challenges involved filtering each row by month. Initially, it was filtered by years which made the information difficult to read and did not accurately show the difference based on launch date. By filtering an appropriate timeframe, such as months vs quarters vs years, the upward and downward trends are more obvious.  
The outcomes based on goal was more challenging. The challenge involved using ranges for the numbers. To overcome this challenge, the excel criteria and range had to be entered twice. The first criteria/range is for the lower number and the second criteria/range is for the higher number. 

Example: =COUNTIFS(kickstarter!F:F, "successful", kickstarter!D:D, ">=1000", kickstarter!D:D, "<=4999", kickstarter!R:R, "plays")


## Results

What are two conclusions you can draw about the Theater Outcomes by Launch Date?
It can be concluded that the launch date does affect the outcome of the campaign.  For the successful campaigns, there is an upward spike from May to July following by a downward trend from August to December. Therefore, spring and summer months are the best launch dates for success.  Overall, there are more successful campaigns than failed and cancelled.  
What can you conclude about the Outcomes based on Goals?
The higher the goal, the higher possibility of failure.  
What are some limitations of this dataset?
The cancelled data set is always zero.  It is unknown whether those campaigns would have changed the data if they were not canceled.  
What are some other possible tables and/or graphs that we could create?
Other possible charts include a pie chart and bar graph.
