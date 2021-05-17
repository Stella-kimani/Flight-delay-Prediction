# Flight delay Prediction

STEP I: Understanding the problem.

Flight delays not only irritate air passengers and disrupt their schedules but also cause :

a decrease in efficiency an increase in capital costs, reallocation of flight crews and aircraft an additional crew expenses As a result, on an aggregate basis, an airline's record of flight delays may have a negative impact on passenger demand.


GOAL I: This project aims to predict the estimated duration of flight delays per flight

This solution proposes to build a flight delay predictive model using Machine Learning techniques. The accurate prediction of flight delays will help all players in the air travel ecosystem to set up effective action plans to reduce the impact of the delays and avoid loss of time, capital and resources.

STEP II:Getting Data
This dataset is sourced from Zindi.
https://zindi.africa/competitions/ai-tunisia-hack-5-predictive-analytics-challenge-2

Dataset Variable definition.
Variable definitions

DATOP - Date of flight

FLTID - Flight number

DEPSTN - Departure point

ARRSTN - Arrival point

STD - Scheduled Time departure

STA - Scheduled Time arrival

STATUS - Flight status

ETD - Expected Time departure

ETA - Expected Time arrival

ATD - Actual Time of Departure

ATA - Actual Time of arrival

DELAY1 - Delay code 1

DUR1 - delay time 1

DELAY2 - Delay code 2

DUR2 - delay time 2

DELAY3 - Delay code 3

DUR3 - delay time 3

DELAY4 - Delay code 4

DUR4 - delay time 4

AC - Aircraft Code



STEP II: Clean and Prepare data
All Ideas regarding feature engineering:

Step III: Building Model
Build a predictive model (Catboost Regressor)


Some additional features like ratio of airport capacity and Tunisia's population can also be helpful

High level feature on departure time like 'early morning','morning','afternoon','evening','night' can be created.

Mean encoding of Categorical variables with smoothing can also be important where categorical values are large in number

Binning less occurring of values for some categorical variables

Flight direct or connecting

Removing Bias from dataset like some delays are unpredictable like delay eg Weather uncertainity

Hyperparameter Tuning can also be performed but as of now hardware resource (less computation power) is constraint.

Ensemble, Stacking techniques can also be experimented to improve results.


