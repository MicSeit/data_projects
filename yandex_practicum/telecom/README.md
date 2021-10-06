# Timeline
Estimated timeline of the project:

- Data preprocessing ~ Day 1
- Exploratory data analysis ~ Day 1-2
- Testing hypotheses ~ Day 2-3
- Working with business metrics and indicators ~ Day 3-4
- Preparing a presentation ~ Day 5

# Introduction

This is an case study for the final project for the Practicum by Yandex curriculum.

**Telecom: Finding Clients With Non-Optimal Plans**
 
We work as analysts in a Telecommunication company, and we want to find customers (organizations that need to distribute large numbers of incoming calls among various operators, or make outgoing calls through their operators) that have non-optimal plans. With non-optimal plans we mean customers that either:
- Overpay for their current plans (as we do not want our customers to be unhappy and lose them to competition) or
- Need bigger plans than they already have (customers will be happier and we will have a higher and a more stable income) 

# Presentation and Dashboard

Link for the Presentation:
- https://1drv.ms/b/s!Ampl2l5jBrzugP577Uc3KGvXPbfNqQ?e=S0zWrN

Link for the Dashboard:
- https://public.tableau.com/views/TelecomDashboard_16251421231330/TelecomDashboard?:language=en-US&:display_count=n&:origin=viz_share_link

--------------------------------------------------------------------------------------------------------------------------

# Description of the data

_Pricing_ (All prices are given in generic monetary units.)

1. Basic price of plan A — 5000
2. Basic price of plan B — 2000
3. Basic price of plan C — 1000

- Incoming calls for all plans — free
- Internal calls for all plans — a limit of 2000 free minutes per month, beyond which:

1. Plan A — 0.10 units/minute
2. Plan B — 0.15 units/minute
3. Plan C — 0.30 units/minute

- Outgoing (not internal) calls:
1. Plan A — 0.4 units/minute
2. Plan B — 0.5 units/minute
3. Plan C — 0.7 units/minute

Clients pay 100 units for each operator (regardless of their plan).


`telecom_dataset_us.csv` contains the following columns:
- user_id — client account ID
- date — date the statistics were retrieved
- direction — call direction ( out for outgoing, in for incoming)
- internal — whether the call was internal (between a client's operators)
- operator_id — operator identifier
- is_missed_call — whether the call was missed
- calls_count — number of calls
- call_duration — call duration (excluding waiting time)
- total_call_duration — call duration (including waiting time)

`telecom_clients_us.csv` contains the following columns:
- user_id
- tariff_plan — client's current plan
- date_start — client's registration date

--------------------------------------------------------------------------------------------------------------------------

# Documentation

Telecom Project
Reading for the hypotheses testing, and the prediction models, choosing the right metrics and draw the right conclusions.	
- https://pandas.pydata.org/pandas-docs/stable/index.html
- https://scikit-learn.org/stable/index.html
- https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.mannwhitneyu.html
- https://machinelearningmastery.com/statistical-hypothesis-tests/
- https://www.isdscotland.org/About-ISD/Methodologies/_docs/Hypothesis-Testing-v0-4-2018-11-27.pdf	
	
--------------------------
	
SQL Project

Theory reminders
- https://www.w3schools.com/sql/default.asp
- https://sqlbolt.com/

--------------------------
	
AB Test

To decide which test to use, as the `recommender_system_test` did not meet the quality criteria. 
- https://geoffruddock.com/run-ab-test-with-unequal-sample-size/
	
Used for addressing the multiple testing problem and choosing the Bonferroni methodology.
- https://www.stat.berkeley.edu/~mgoldman/Section0402.pdf
	
Articles to be able to formulate statistical hypotheses better, choose the right tests and draw the right conclusions.	
- https://machinelearningmastery.com/statistical-hypothesis-tests/
- https://www.isdscotland.org/About-ISD/Methodologies/_docs/Hypothesis-Testing-v0-4-2018-11-27.pdf