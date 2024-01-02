
Project work

TKO_7093
Preface

This project is framed as a hypothetical scenario in order to give the analysis some context and flavour. The tasks you need to do are clearly indicated by the maximum points you can get, but remember to also take the surrounding scenario into account while performing your analysis and writing your report.

See the instructions in Moodle regarding how and when to submit your project report.

Your project report will be marked out of 40 points. In each step of the project, partial points can be obtained for an incomplete solution if the approach is correct. It is therefore recommended that you show your best attempt even if you know it is not fully correct. In your report, show your code and its output as well as describe your findings and conclusions. Remember to interpret your results and address the questions and tasks given to you in the scenario.
Instructions

Dear Data Scientist,

As you know we launched a rental service of electric bikes this year. Now it is time to prepare for the next year, and I need you to analyse the data we have collected. I got the file bikes.data (see attached) from our maintenance team. They said it contains all the data recorded by our bikes. Since there is no information about who rented the bikes, you can assume that each trip was made by a different person. The maintenance team also supplied me with some descriptions of the variables (see below).

Variable 	Description
ticket 	- ticket type
cost 	- paid fee in euros
month 	-  calendar month during which the trip was made
location_from 	-  start location of the trip
location_to - 	end location of the trip
duration 	- travel time in seconds
distance 	-  travel distance in meters
assistance 	-  status of electric assistance (0 = disabled, 1 = enabled)
energy_used  - 	energy consumed by the bike in watt-hours
energy_collected  - 	energy collected by the bike in watt-hours


There are several questions we would like to get answered in order to optimise our operations for the next year. I have already outlined the structure of the statistical analysis (see the sections below) to address our needs and concerns. Please plan the details and execute the analysis. I will then present your discoveries in a board meeting and also forward them to the other teams. For this purpose, please write a clear and nicely-formatted report. It must be a complete and standalone report such that the reader does not have to run code in order to understand the analysis. Make sure that all (and only) relevant information is clearly stated throughout the report.

Looking forward to receiving your report!

Yours, Head of Transportation



(2p) Write a clear and nicely-formatted report that includes all the relevant information for the reader to understand your analysis and its results. The quality of the report is worth some points by itself.
Data preparation

The file bikes.data contains data that was collected directly from the recording devices of the bikes. No preprocessing or filtering has been done. The data may therefore contain irrelevant records, such as customers only trying out how bikes can be rented with our Android app and cancelling the transaction without actually riding the bike. Furthermore, the maintenance team reported that they had quite a few technical problems with the bikes, which may have resulted in invalid values in the data. So, you need to load and clean up the data before you can perform the statistical analysis.

(2p) Load the data from the file bikes.data. Check that the variables match the documentation above.

(6p) Use both visualisations and numerical summaries to explore the variables. Filter out irrelevant records and process invalid values, if any. Explain why the records are irrelevant or the values invalid. Also explain how the modifications you made to the data fix the problems.




Data exploration

It is vital to know what our customers are like and how they use our bikes. We are particularly interested in characterising the users of the three ticket types (single, season and savonia). Explore the data to discover how the rental bikes were used during the time period at which the data was collected. Remember to examine your results, summarise your findings and point out any interesting discoveries in your report.

The marketing team is interested in knowing how much the bikes were used under each ticket type. They believe that they can use the information to improve our advertisement campaigns and consequently increase our revenue.

(4p) For each ticket type, calculate the number of trips made, the total distance travelled, the total time travelled and the total amount of fees paid. Examine your results and make comments about the customers.

(4p) For each ticket type, visualise the monthly rental activity in terms of the total distance travelled. Examine your results and make comments about the development of the rental activity over time.

The logistics team transported bikes between renting stations in order to balance their availability, but they struggled to maintain a decent number of bikes available at each station. To optimise the transport operation, the logistics team needs to know which stations tend to get depleted of bikes and which stations tend to accumulate bikes. While transporting bikes, they also noticed that quite often the bikes had fully discharged batteries. We need to upgrade our charging stations to keep them charged. For that, we need to know how much battery levels tend to change during trips.

(4p) Find the three stations that have the highest total deficit of bikes (i.e. the largest negative difference between the number of arrived bikes and the number of departured bikes) and the three stations that have the highest total surplus of bikes (i.e. the largest positive difference). Examine your results and make suggestions about how bikes could be relocated.

(4p) For each trip in the data set, calculate its net energy gain, which is defined as the difference between the energy collected and consumed during a trip. Visualise the distribution of this new variable. Make comments about how much battery levels tend to change during trips.



Hypothesis testing

There are a few hypotheses that we want to study about our customers and the trips they make. You need to examine whether the data has statistical evidence to support them. The tasks are detailed below. The other teams will want to double-check your analysis, so in your report remember to justify your choices of statistical tests, interpret the p-values, and make conclusions about the customers and their trips.

The marketing team has made a hypothesis that trip durations tend to be different between the customers who have a season ticket and the customers who buy single tickets. They also believe that the longer the trip, the higher the rate of electricity consumption tends to be. If we can find evidence for these hypotheses, the marketing team could use the information in the future advertisement campaigns.

(4p) Is there statistical evidence to claim that the travel times tend to be shorter or longer for the single than for the season ticket type. Justify your design choices, interpret the results and use your discoveries to make conclusions about customers.

(4p) Is there statistical evidence to claim that the travel distance positively correlates with the average rate at which electricity is consumed during the trip? Justify your design choices, interpret the results and use your discoveries to make conclusions about customers.

We will acquire some non-electric bikes for the next year to supplement our fleet. We need to offer them to those customers who are less likely to need electric assistance. The logistics team has a hypothesis that the Savonia students differ from the other customers with this respect.

(4p) Is there statistical evidence to claim that the savonia ticket type differs from the others with respect to how often the electric assistance is used? Justify your design choices, interpret the results and use your discoveries to make conclusions about customers.
Future directions



The statistical analysis outlined above is definitely not perfect. There must be plenty of other hypotheses that could be examined to improve our rental operations, and the questions we ask above could perhaps be tweaked to better address the needs we have. Since the marketing, logistics and maintenance teams could not come up with other hypotheses or further adjustments, it is up to you to propose improvements to the analysis.

(2p) Choose either (A) or (B) below.

(A) Formulate your own hypothesis about the use of rental electric bikes. Explain why your hypothesis would be important to explore. Describe how the hypothesis could be tested. (You do not have to perform the analysis.)

(B) Point out one or more problems in the questions asked or the approaches used above. Propose changes to address the problem(s). Explain how the changes would improve the statistical analysis.
