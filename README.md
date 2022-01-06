# Kickstarter Outcomes and Goals

## Overview of Project

### The purpose of this project was to assist my client in comparing the outcomes of kickstarter campaigns in relation to their launch dates and funding goals. The data for this project was downloaded and used in a previous project where I helped our client launch a kickstarter campaign for her play, *Fever*. The data included crowdfunding data from thousands of campaigns including: launch date, goal, category, outcomes, etc. Using this data in our previous project resulted in a successful campaign for my client. The current project used the same data to construct visualizations that display the outcome of theater campaigns in relation to their launch dates and goals, so that I can compare them to each other and to my client's campaign. 
Data [Kickstarter_Challenge] (https://github.com/Lan-kdl/kickstarter-analysis/blob/main/Kickstarter_Challenge%20-%20Copy.zip)

## Analysis and Challenges

### To perform the analysis of Outcomes Based on Launch Date, I started with the downloaded data from the previous project titled "Kickstarter_Challenge". First, I created a "Years" column which was filled using the YEAR() function and the data from the "Date Created Conversion" column.
![Steps_of_Analysis_of_Launch](https://user-images.githubusercontent.com/95589611/148433480-9b44125a-c169-41a8-a2cc-06af1e7e48b0.png)
![Steps_of_Analysis_of_Launch_2](https://user-images.githubusercontent.com/95589611/148433709-2e8ae343-9ce3-4e24-aee0-1132abd4d3fa.png)
Steps to using the YEAR() Funtion were found using [Microsoft Support](https://support.microsoft.com/en-us/office/year-function-c64f017a-1354-490d-981f-578e8ec8d3b9)
### Then, I created a pivot table in a new sheet which I labeled "Theater Outcomes by Launch Date". 
![Steps_of_Analysis_of_Launch_3](https://user-images.githubusercontent.com/95589611/148433629-a97de5b7-3cfc-44da-acec-7d428e677548.png)
### I filtered the pivot table by "Parent Category" and "Years". In rows, I put the "Date Created Conversion"; I put the "Outcome" into values and columns. I then filtered the pivot table to display successful, failed, and canceled outcomes and filtered the "Parent Category" to display only theater. 
![Steps_of_Analysis_of_Launch_4](https://user-images.githubusercontent.com/95589611/148433820-77795581-71a1-4377-b370-261c57d434d7.png)
![Steps_of_Analysis_of_Launch_5](https://user-images.githubusercontent.com/95589611/148433834-96e69d0d-e1c1-463f-932d-a6c680b5b705.png)
### From the pivot table, I created a line chart which displayed the relationship between outcomes and launch dates. 
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/95589611/148433875-decb2461-911c-40c9-8e87-290032c33d4a.png)

### To perform the analysis of Outcomes Based on Goals, I once again drew from the previously downloaded data. I created a new sheet labeled "Outcomes Based on Goals" and created columns detailing the number and percentage of successful, failed, and canceled outcomes alongside grouped goals ranging from less than 1,000 to more than 50,000. 
![Steps_of_Analysis_of_Goals](https://user-images.githubusercontent.com/95589611/148434012-33dddd38-cdba-4731-a15f-db1a163cce23.png)
![Steps_of_Analysis_of_Goals_2](https://user-images.githubusercontent.com/95589611/148434025-a3c9a3ab-221a-4f29-b6ab-621ee26c1ebc.png)
### I filled each of these columns using the COUNTIF() Function. 
![Steps_of_Analysis_of_Goals_3](https://user-images.githubusercontent.com/95589611/148434072-bcb0fa60-726e-401d-b030-5a85f2eb28bd.png)
Steps to using the COUNTIF() Funtion were found using [Microsoft Support] (https://support.microsoft.com/en-us/office/countif-function-e0de10c6-f885-4e71-abb4-1f464816df34)
### I then used the SUM() Function for the "Total Projects" column and calculated the percentages by dividing the appropriate value for each outcome by the total number of projects for the specific range of goals. 
![Steps_of_Analysis_of_Goals_4](https://user-images.githubusercontent.com/95589611/148434124-a00afdf6-3f9d-4b2c-a86a-b130bd282bee.png)
![Steps_of_Analysis_of_Goals_5](https://user-images.githubusercontent.com/95589611/148434140-b0fc9c4e-d4b5-471f-ae66-9eea7026e3f2.png)
### With this data, I created a line chart visualization which displayed the relationship between goals and outcomes. 
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/95589611/148434159-a9dcd342-0290-4584-ac0c-53201abba500.png)

## Challenges

### There were a couple of challenges during the analysis portion of this project. The first, was understanding how to obtain the serial number for the YEAR() Function. I quickly solved this problem by entering the Function, then manually selecting the cell in which I wanted to pull my data from. This automatically filled my Function with the needed serial number. Another challenge I faced was making the "Outcomes Based on Goals Chart" readable. This was challenging because the goal ranges were written in large numbers which were clustered together in the x-axis of the chart. Originally, the chart looked busy and it was difficult to read and seperate the values in the x-axis. To fix this, I had to click on the x-axis values and play with the spacing and font size until the values were seperate from eachother and readable. 

## Results

- Two conlusions I can draw from the Outcomes Based on Launch Date are that there is a greater likelyhood of a successful campaign when launched in the month of May or in the months that closely follow May because the separation between successful and failed or canceled campaigns is the greatest during this time with May having 111 successful campaigns and only 52 failed campaigns. I would also conclude that December has the highest chance of failure as the number of successful outcomes and failed outcomes in that month is seperated by only two succesful campaigns. 
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/95589611/148435130-0d8555bd-ddc8-425d-9f27-edecb25519cd.png)
- From the analysis of Outcomes Based on Goals I can conclude that the campaigns with the greatest chances for success had goals of less than 1,000 as 75.8% of campaigns with goals in this range were successful, whereas the greatest risk for failure was from campaigns with a goal between 45,000 and 49,999 as these failed 100% of the time. It should be noted that this percentage could be a result of the small amount of total campaigns within that goal range. It may be more useful to know that campaigns with a budget over 50,000 failed 83% of the time as did campaigns with a budget between 25,000 and 29,999 which failed 80% of the time. 
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/95589611/148435157-d379f49a-13ac-4942-8c80-25817461c068.png)
- Some limitations of this data set were the excess in variables which were unessary to the project and cluttered the data set. If our purpose for either of these projects was to simply launch a successful campaign, then it would not be nessary for me to know the blurb of each campaign. I would substitute this section with the genre section. I would also not need to know which campaigns were "Staffed Picked" and the "Amount Pledged" became redundant due to the "Outcomes" column. Another limitation is that while there is a column which tells us in what currency the goals and pledges are in, it would be better to translate them into one type of currency in another column so that we could see exactly how much the goals were comparitivley. 
- There are many other tables and graphs we could create from this dataset. We could examine the Outcome in relation to Country. We could also determine the length that each campaign was open for using the "Date Created Conversion" and "Date Ended" columns, and then make a graph comparing the length of the campaign to its outcome. We could also take a look at the number of "Backers" in relation to "Amount Pledged". 
