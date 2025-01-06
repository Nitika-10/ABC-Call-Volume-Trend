# ABC-Call-Volume-Trend
This project analyzes call volume data to identify trends, peak periods, and patterns over time. The goal is to optimize resource allocation and improve customer service efficiency. (Trend Analysis, Peak Detection, Pattern Insights, Visualization).

Project Description :

For you final project we are providing you with a dataset of a Customer Experience (CX) Inbound calling team for 23 days. Data includes Agent_Name, Agent_ID, Queue_Time [duration for which customer have to wait before they get connected to an agent], Time [time at which call was made by customer in a day], Time_Bucket [for easiness we have also provided you with the time bucket], Duration [duration for which a customer and executives are on call, Call_Seconds [for simplicity we have also converted those time into seconds], call status (Abandon, answered, transferred).

A customer experience (CX) team consists of professionals who analyze customer feedback and data, and share insights with the rest of the organization. Typically, these teams fulfil various roles and responsibilities such as: Customer experience programs (CX programs), Digital customer experience, Design and processes, Internal communications, Voice of the customer (VoC), User experiences, Customer experience management, Journey mapping, Nurturing customer interactions, Customer success, Customer support, Handling customer data, Learning about the customer journey.

Approach :

Start with a clear and concise summary of your insights
Use clear and concise language
Use visual aids
Provide context
Highlight key findings
Consider the audience
Tech Stack Used :

MS Excel
Link to excel File :

Click Here

Calculate the average call time duration for all incoming calls received by agents (in each Time_Bucket).
Time Bucket	Average call duration (in secs)
9_10	199.01
10_11	209.15
11_12	203.35
12_13	190.76
13_14	193.60
14_15	193.20
15_16	195.49
16_17	196.54
17_18	198.71
18_19	201.09
19_20	203.94
20_21	202.55


Insights:

Time_Bucket is measured in the Rows and average of Call_Seconds is measured in the Values section. And we put Call_Status in the Filters section.
The total average of call time duration which are answered by the agents is 198.6 seconds.
The average call time duration for all incoming calls received by agents is the highest in between 10 am to 11 am and from 7 pm to 8 pm
The average call time duration for all incoming calls received by agents is the least in between 12 noon to 1 pm.
Show the total volume/ number of calls coming in via charts/ graphs [Number of calls v/s Time]. You can select time in a bucket form (i.e. 1-2, 2-3, …..)
Time Bucket	No. of calls
9_10	9588
10_11	13313
11_12	14626
12_13	12652
13_14	11561
14_15	10561
15_16	9159
16_17	8788
17_18	8534
18_19	7238
19_20	6463
20_21	5505


Insights:

We plotted Time_Bucket in the rows and took Count of Customer_Phone_No and Count of Time in the Values section.
We measured Count of Time as the percentage of Column Total.
The customers call the most in between 11 am to 12 noon.
The customers call the least in between 8 pm to 9 pm.
As you can see current abandon rate is approximately 30%. Propose a manpower plan required during each time bucket [between 9am to 9pm] to reduce the abandon rate to 10%. (i.e. You have to calculate minimum number of agents required in each time bucket so that at least 90 calls should be answered out of 100.)
Time Bucket	Number of calls	% of calls inbound	Required Agents
9_10	9588	8%	5
10_11	13313	11%	6
11_12	14626	12%	7
12_13	12652	11%	6
13_14	11561	10%	6
14_15	10561	9%	5
15_16	9159	8%	4
16_17	8788	7%	4
17_18	8534	7%	4
18_19	7238	6%	3
19_20	6463	5%	3
20_21	5505	5%	3
Grand Total	117988	100%	57
Date	abandon	answered	transfer	Grand Total
01-Jan	684	3883	77	4644
---	---	---	---	---
02-Jan	356	2935	60	3351
03-Jan	599	4079	111	4789
04-Jan	595	4404	114	5113
05-Jan	536	4140	114	4790
06-Jan	991	3875	85	4951
07-Jan	1319	3587	42	4948
08-Jan	1103	3519	50	4672
09-Jan	962	2628	62	3652
10-Jan	1212	3699	72	4983
11-Jan	856	3695	86	4637
12-Jan	1299	3297	47	4643
13-Jan	738	3326	59	4123
14-Jan	291	2832	32	3155
15-Jan	304	2730	24	3058
16-Jan	1191	3910	41	5142
17-Jan	16636	5706	5	22347
18-Jan	1738	4024	12	5774
19-Jan	974	3717	12	4703
20-Jan	833	3485	4	4322
21-Jan	566	3104	5	3675
22-Jan	239	3045	7	3291
23-Jan	381	2832	12	3225
Grand Total	34403	82452	1133	117988
Average	1496	3585	49	5130
% of calls	29%	70%	1%	
Assumptions:
Agents working Hrs
Break
Agents working Hrs on Floor
Agents Time spent on calls
| | | | | Avg Call Volume per day(9:00 AM to 9:00 PM) | 5130 | Nos | | Average call duration (9:00 AM to 9:00 PM) | 199 | Seconds | | Total call duration for 90% Calls | 255 | Hrs | | Agents required per day | 57 | Nos |



Insights

Total agents working can be calculated by average calls on a single day divided by total time spend by one man in a single day.
total agent = 187.96/5 = 37.59

If agents are working for 5 hrs a day and 60% calls are getting answered. If we want 90% of the calls to get connected, we apply unitary method to find how many more employee we want.
total agent = 90*37.59/60 = ~57 agents
First, we created pivot table. Date & Time is dragged down to Rows, Call Status to Columns, while taking count Call Duration in the Values section.

Then, we calculated the average of abandon, answered and transfer by using the average excel formula.

29% of the calls are abandoned, 1% is transferred, while 70% of the calls are answered in the daytime.

Total agents required to answer the 90% of the calls per day is 56.

The minimum number of agents required for each time bucket is calculated by 56 * count of time (calculated in the 2nd question).

Let's say customers also call this ABC insurance company in night but didn't get answer as there are no agents to answer, this creates a bad customer experience for this Insurance company. Suppose every 100 calls that customer made during 9 Am to 9 Pm, customer also made 30 calls in night between interval [9 Pm to 9 Am] and distribution of those 30 calls are as follows:

Now propose a manpower plan required during each time bucket in a day. Maximum Abandon rate assumption would be same 10%.

Assumptions:
Agents working Hrs
Break
Agents working Hrs on Floor
Agents Time spent on calls
| | | | | Avg Call Volume per day(9:00 AM to 9:00 PM) | 5130 | Nos | | Average call duration (9:00 AM to 9:00 PM) | 199 | Seconds | | Total call duration for 90% Calls | 255 | Hrs | | Agents required per day | 57 | Nos | | | | | | If support is provided from 9:00 PM to 9:00 AM) | | Avg Call Volume (9:00 PM to 9:00 AM) | 1539 | Nos | | Total Call duration (9:00 PM to 9:00AM) | 77 | Hours | | Agents required (9:00 PM to 9:00AM) | 17 | Nos |

Time_Bucket	Calls_inbound	% of calls inbound	Required agents
21_22	3	10%	2
22_23	3	10%	2
23_24	2	7%	1
00_01	2	7%	1
01_02	1	3%	1
02_03	1	3%	1
03_04	1	3%	1
04_05	1	3%	1
05_06	3	10%	2
06_07	4	13%	2
07_08	4	13%	2
08_09	5	17%	3
Total	30	100%	17
Time_Bucket	Required Agents
21_22	2
22_23	2
23_24	1
00_01	1
01_02	1
02_03	1
03_04	1
04_05	1
05_06	2
06_07	2
07_08	2
08_09	3
9_10	5
10_11	6
11_12	7
12_13	6
13_14	6
14_15	5
15_16	4
16_17	4
17_18	4
18_19	3
19_20	3
20_21	3


We first calculated the Time Distribution by dividing each calls distribution by total calls i.e., 30.
The number of agents required for each time bucket is calculated by 15 * Time Distribution
15 is calculated above by dividing the additional hours required to answer the night calls by 5 (actual working hours of agents).
Also, while calculating, the round figure is taken into consideration as there cannot be 1.5 men working.
Insights:

The customers call the least in the evening. So, the company can reduce the number of agents at that time for answering the calls.
The company can hire 15 customer support agents for the night shift work.
The company can shift some of the day workers for the night shift.
The employees who are working 9 am to 9 pm. The manager can change some of the workers shift from 5 am to 2 pm and some workers from 2 pm to 11 pm to get the most calls answered.
The company can make the employers divide into 3 parts too, so that the agents are always available 24/7.
We found there were few outliers in the data. And if we have removed that outliers, then the answers would have been different.
Results:

I learned how an analyst can make an impact in customer service department.
I learned how a company deals with the customers to give them the most satisfaction.
I got to know about the IVR Duration, which is an AI tool, who answer the calls to get to know the customer exact question and then transfer it to the right agent to get the customer's queries get answered.
This project was easy to get the answers as the data provided by the team have already calculated the time bucket and converted the calls duration into seconds, so we do not have to spend time on it to calculate.
I learned about the behavioral analytics
