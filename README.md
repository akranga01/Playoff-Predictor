# Playoff-Predictor Project 

Goal: Classify an NBA Team as playoff bound or not using specific Team Analytics collected from stats.NBA.com

Disclaimer: The reason we use team statistics is because there are many biases when looking at individual player stats as great player stats may not translate to overall team success, as can be seen by Bradley Beal and the Washington Wizards, Devin Booker and the Phoenix Suns, 


Step 1: First identify the baseline year to start collecting data based on when the three point frequency increased the most to make the model have less bias and more accuracy.
We are in a 3 point shooting era, so identifying when the overall league started shifting towards this is essential. 2016-2017 is the year where there was a major jump in three point shooting compared to other years in this decade. 
We need to take stats from a season that fits within this era to accurately predict future possibilities because of its context.
Stats from the 2019-2020 regular season to predict who makes playoffs, versus who actually made it.

Step 2: Identify Team factors that allow teams to make the playoffs. 
1) TS %  - takes into account three pointers and free throws on top of conventional twos
2) Net Rating - takes into account team’s offense and defense per 100 possessions, great indicator of overall success.
3) OPP EFG% - Holding teams to lower field goal percentages is a great indicator of great team defense
4) PTS Paint
5) OPP Pts Paint - The easiest place to score in basketball is in the paint, and minimizing these shots makes it harder for the opponent to score, increasing the defensive versatility and potential success. 

Step 3: Drop data accordingly to prevent collinearity and start training our models to test compiled data: 
1) Logistic Regression
2) Random Forest

Step 4: Test accuracy of the models: 
- Concluded that Logistic Regression model predicted more accurately compared to Random Forest Model, with an overall accuracy of 90%.
