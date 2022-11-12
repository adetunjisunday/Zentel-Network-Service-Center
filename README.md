# Zentel-Network-Service-Center
# ***TEAM DATA CATALYSTS- 4th Position***

# INTRODUCTION
This is data from Zentel Network Service Center. Everyday, customers log their different types of complaints across their branches and expect quick responses and resolutions to their queries. This is however contained in the service level agreement with Zentel.
The service center has different managers and operators looking into the customers' issues and performance can be measured weekly and daily.
# The Problem
Zentel Network Service Center needs a dashboard to monitor the performancw of their customer service agents and easily find out issues that might be affecting their performance daily or weekly.
# Solution Apporach
We understand that there are two major stakeholder categories that might find our dashboard useful: the top executives and the managers. The top executives will need to see a general overview of the performances of the managers' teams and each managers will want to see the performance of his or her team operators. Hence, our dashboard is divided into a general overview for top executives and a narrow overview where the managers will see performances of operators in their teams.
# Data Transformation
With Power Query, we carried out the following tasks: null columns and rows were removed, the table was split into day, week and month, first Response Time and Turn around Time columns were calculated, code for service type was extracted by splitting the column by delimiter.
# Data Visualization
With PowerBI, we carried out the following tasks: DAX measures were created, the relationships amongst the tables were established.
HERE IS THE [LINK](https://app.powerbi.com/view?r=eyJrIjoiNzQyMmUwZTktZjU5OS00N2FlLWIzOTAtYjhjYmExZjUyNzQ2IiwidCI6ImVhMTJjZDQzLTY2NTYtNDFmYi05NmQwLThlMDkyMjg0YjIzOCJ9) TO OUR DASHBOARD

# Follow-Up Questions
There are a total of 5998 tickets over 30 days with an average response time of 274 seconds which is way above the target of 15 seconds. This is however a very poor performance. <br/>
![avg resp time](https://user-images.githubusercontent.com/107109434/201456821-77dfcf4c-34a4-444a-af8a-4473de7652d8.PNG)
<br/>

The average response time is 145 minutes compared to the target of 180 minutes. In this case the resolution time is actually in good shape. <br/>
![avg res t](https://user-images.githubusercontent.com/107109434/201456894-4a1801ed-870f-49a6-b167-bad264821334.PNG) 

Seeing that the average response is way higher than the target, most of these tickets have response times exceeding 10 seconds. According to our findings, 1053 tickets exceeded 10 seconds. This is just 18% and not even up to a quater of the total number of tickets.  <br/>
![10 sec](https://user-images.githubusercontent.com/107109434/201457019-d36974f5-1485-4338-a58c-93133b54473c.PNG)

***Who and what could be the cause of this? Let’s start with the who!***

### Wale and Victor are at both extremes
No manager actually has response time less than 15 seconds. However, relatively, Victor seems to be the best even with his high ticket volume. And Wale is the manager with the worst performance. But who on Wale’s team is severely affecting the team’s performance? <br/>
![wale](https://user-images.githubusercontent.com/107109434/201457458-52b870ab-6a28-43f7-a93a-4dcb01f2bcbc.PNG)

### Akin needs to be cautioned
Akin has the worst performance regarding the response time in three different days irrespective of the low ticket volume that he has. <br/>
![akin](https://user-images.githubusercontent.com/107109434/201457581-4055f7c4-2778-48e7-b4f8-76a5c927c83d.PNG)

But should Akin be pardoned? Maybe if he has high turn around time. Akin still has the worst performing resolution time in two different days. He really needs to be put in check <br/>

![akin taat](https://user-images.githubusercontent.com/107109434/201457646-ffe13b3a-89a8-4818-93a8-df35bd29204b.PNG)

### Wale’s team is still performing badly in resolution time
Wale’s team is still performing badly  in the resolution time. His team needs to be on a close watch. Victor however is performing well even with the high ticket volume.<br/>
![res managers](https://user-images.githubusercontent.com/107109434/201457840-4c4a67c3-6ede-473c-aed5-9e4b49db6b8d.PNG)

***Now that we know the who. Let’s go over to the what.*** <br/>
### The working times matter
Times between 8am and 3pm have constant resolution time unlike outside the times where they are fluctuating. This could be that most of the operators don’t have suitable schedules to still work efficiently outside these times. <br/>

![rt vs vt](https://user-images.githubusercontent.com/107109434/201458027-09a4e647-86c6-40af-9e2f-69665bc495cd.PNG)

### Channels of notification
Another major factor that is causing delay in the ticket response time is the channels of notification which is a medium in which the operators track requests of tickets directed to them. Social media is most used channel in which the reports came in across all managers leading to longer delay in response time in other channels which however varies per managers.<br/>
![channel vic](https://user-images.githubusercontent.com/107109434/201459893-1d89ccb0-d718-4d21-b3a8-5637b0738b18.PNG) <br/>
*Victor's channel of notification* <br/>
![channel wale](https://user-images.githubusercontent.com/107109434/201460029-3046e6ed-909b-4d5d-a940-b12be3e37a81.PNG) <br/>
*Wale's channel of notification* <br/>

It is however noted that the most breached SLA is the 10 seconds response time when issues are raised. Also, the possibility of inadequate awareness can arise when the channels cannot serve a roun o'clock and fast notifiation system. For instance, in a situation whereby ther is mistake of logging ticket to the wrong team, without any fast notification method it will hamper the response time which is to be served as soon as possible.

## We built a monitoring system in which active tickets which have passed their resolution time can easily be escalated to their specific manager where he can swiftly see and track them.  <br/>
![esc](https://user-images.githubusercontent.com/107109434/201460755-6dec3bc3-d74b-47da-a17a-6fb7db1011b1.PNG)


# RECOMENDATIONS
* The managers should sit together and the way they manage their teams should be discussed. This will help for the managers to draw insights from others' strategies.
* Wale’s team should be closely watched. While this is being done, the operators particularly under Wale should be managed by Victor as it could increase their performance.
* Based on the abnormal turnout of response time and resolution time in some times, the shift times of team members should be readjusted.
* The tickets handled by Victor's team alone is much. These tickets should be spread out across different teams but only after the other teams have been worked on to have their efficiency increased.
* The company should establish good alert systems for the channels of notification. A good case is a pop of sms instead of checking emails at intervals.



