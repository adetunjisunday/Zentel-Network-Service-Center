# ZENTEL NETWORK PERFORMANCE REPORT
## ***TEAM DATA CATALYSTS- 4th Position, DataFestAfrica Datathon***

## INTRODUCTION

This data is from Zentel Network Service Center. Everyday, customers log their different types of complaints across their branches and expect quick responses and resolutions to their queries. This is however contained in the service level agreement with Zentel.
The service center has different managers and operators looking into the customers' issues and performance can be measured weekly and daily.

## The Problem

Zentel Network Service Center needs a dashboard to monitor the performance of their customer service agents and easily find out issues that might be affecting their performance daily or weekly.

## Solution Approach

We understand that there are two major stakeholder categories that might find our dashboard useful: the top executives and the managers. 

The top executives will need to see a general overview of the performances of the managers' teams. While the managers will want to see the performance of his or her team operators. 

Hence, our dashboard is divided into a general overview for top executives and a ground level overview where the managers will see performances of operators in their teams.

To prevent the managers from a particular team from seeing the performances of another team, we introduced row level security while designing our PowerBI dashboard.

## Data Transformation

With PowerBI, we carried out the following tasks: 

- Null values were removed
- The date columns were split into day, week and month columns
- The first Response Time and Turn around Time columns were derived. 
- The code for service type was extracted by splitting the column by delimiter.
- Relationships amongst tables were created
- Use of DAX measures


## Data Modelling

After creating relevant relationships between our tables, this is our entity relationship diagram:

![](Entity%20Relationship%20Diagram.PNG)

There are five dimension tables and one fact table where the "Service Data" table is the fact table.
 
# Data Visualization

[HERE IS THE LINK TO OUR DASHBOARD](https://app.powerbi.com/view?r=eyJrIjoiNzQyMmUwZTktZjU5OS00N2FlLWIzOTAtYjhjYmExZjUyNzQ2IiwidCI6ImVhMTJjZDQzLTY2NTYtNDFmYi05NmQwLThlMDkyMjg0YjIzOCJ9)

The first page is tailored for the C-executives to monitor the general overview of the different teams. While the second page is tailored for the managers to view the performances of their respective team operators.

# Findings
There are a total of 5998 tickets over 30 days with an average response time of 274 seconds which is way above the target of 15 seconds. This is a very poor performance. 

![avg resp time](https://user-images.githubusercontent.com/107109434/201456821-77dfcf4c-34a4-444a-af8a-4473de7652d8.PNG)

The average response time is 145 minutes compared to the target of 180 minutes. In this case the resolution time is actually in good shape. 

![avg res t](https://user-images.githubusercontent.com/107109434/201456894-4a1801ed-870f-49a6-b167-bad264821334.PNG) 

Seeing that the average response is way higher than the target, most of these tickets have response times exceeding 10 seconds. According to our findings, 1053 tickets exceeded 10 seconds. This is just 18% and not even up to a quater of the total number of tickets.  

![10 sec](https://user-images.githubusercontent.com/107109434/201457019-d36974f5-1485-4338-a58c-93133b54473c.PNG)

### Who and what could be the cause of this? 

***Let’s begin with the who!***

### Wale and Victor are at both extremes

No manager actually has average response time less than 15 seconds. However, relatively, Victor seems to be the best even with his high ticket volume. 

And Wale is the manager with the worst performance. But who on Wale’s team is severely affecting the team’s performance? 

![wale](https://user-images.githubusercontent.com/107109434/201457458-52b870ab-6a28-43f7-a93a-4dcb01f2bcbc.PNG)

### Akin (in Wale's team) needs to be cautioned

Akin has the worst performance regarding the response time in three different days irrespective of the low ticket volume that he has. 

![akin](https://user-images.githubusercontent.com/107109434/201457581-4055f7c4-2778-48e7-b4f8-76a5c927c83d.PNG)

### But should Akin be pardoned? Probably if he has fast resolution time.

Unfortunately, Akin still has the worst performing resolution time in two different days. He really needs to be put in check 

![akin taat](https://user-images.githubusercontent.com/107109434/201457646-ffe13b3a-89a8-4818-93a8-df35bd29204b.PNG)

### Wale’s team is still performing badly in resolution time

Wale’s team is still performing badly in the resolution time. His team needs to be put on a close watch. Victor however is performing well even with the high ticket volume and needs to be rewarded to encourage him for managing his team well.

![res managers](https://user-images.githubusercontent.com/107109434/201457840-4c4a67c3-6ede-473c-aed5-9e4b49db6b8d.PNG)

**Now that we know the who. Let’s go over to the what.**

### The working times matter

Times between 8am and 3pm have constant resolution time unlike outside the times where they are fluctuating. This could be that most of the operators don’t have suitable schedules to still work efficiently outside 8am to 3pm. 

![rt vs vt](https://user-images.githubusercontent.com/107109434/201458027-09a4e647-86c6-40af-9e2f-69665bc495cd.PNG)

### Channels of notification

Another major factor that is causing delay in the ticket response time is the channels of notification which is a medium in which the operators track requests of tickets directed to them. 

Social media is most used channel in which customers' complaints come in. It's most likely that the delayed response time for social media channel is due to this high volume coming in through social media. 

However, we noticed that the response times vary across the different teams. Let's focus on Victor and Wale.

*Victor's channel of notification* 

![channel vic](https://user-images.githubusercontent.com/107109434/201459893-1d89ccb0-d718-4d21-b3a8-5637b0738b18.PNG)


*Wale's channel of notification*

![channel wale](https://user-images.githubusercontent.com/107109434/201460029-3046e6ed-909b-4d5d-a940-b12be3e37a81.PNG) 

### How can we help managers improve the resolution times of their respective teams.

The managers might see a particular ticket has surpassed the 3 hours (180 minutes) resolution time but he can't do much about it because he doesn't know the particular operator in his team that's handling it. 

Hence, in our dashboard, we added a table where managers could track the active tickets that has gone beyond the 3 hours resolution time and also see the team operator responsible so the manager can easily find out why that particular complaint is still being worked on. 

![esc](https://user-images.githubusercontent.com/107109434/201460755-6dec3bc3-d74b-47da-a17a-6fb7db1011b1.PNG)


## Recommendations

* The managers should sit together and discuss the way they manage their teams so that the slacking teams (example Wale's) can draw insights on how to manage their teams for better performances.

* Wale’s team should be closely watched. While this is being done, the operators particularly under Wale should be managed by Victor as it could increase their performance.

* Based on the abnormal turnout of response time and resolution time outside the time range of 8am to 3pm, the shift times of team members should be readjusted to improve efficiency.

* The tickets handled by Victor's team alone is much. These tickets should be spread out across different teams but only after the other teams have been worked on so that the efficiency of other teams won't reduce further.

* The company should establish good alert systems for the channels of notification. A good case is a pop of sms instead of checking emails at intervals.




