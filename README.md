## NHL Shootout Optimization & Financial Impact Analysis
This repository contains the machine learning models developed in Google Colab for my Master of Business Analytics (MSBA) Capstone Project. The project investigates how data-driven tactical optimization in NHL shootouts can mitigate secure critical standing points for "bubble" teams (+-5 pts within the playoff threshold) and generate millions in post-season revenue.
# Project Overview
NHL shootouts are entertaining for fans yet often viewed as a "coin flip" to determine the winner. However, for teams on the playoff bubble, a single shootout point can be the difference between a $26M deep playoff run and a premature off-season. Data from 5 NHL regular seasons (2020-21 to 2024-25) was pulled from the NHL Web API: [gamecenter play-by-play], [playerlanding], [club-schedule-season], and [standings[date]]. This project analyzed 440 shootout games and n=3,115 attempts.  
# Models
sxG Model: sxG = P(Y = 1 | X_1, X_2, …, Xn), where Y is the goal predicitor, 1 = goal, 0 = no goal. The X’s represent the independent features. In this study, the independent features consist of: “distance_from_net”, “angle_from_net”, “shooter_handedness”, “goalie_handedness”, “shot_type”, and “is_off_wing”, while the target feature is “is_goal”. 
Clustering: Used K-Means and  Gaussian Mixture Modeling (GMM) to identify high-probability "Sweet Spots" on the ice. utilized the Elbow and Silhouette Methods for optimal k value. 
Monte Carlo Simulation: 10,000 iterations comparing randomized lineups against data-optimized rosters, yielding a 73.4% win probability.
Financial Impact: Quantified the ROI of shootout optimization, identifying potential revenue gains from $4M to $26M per team through the playoffs. 
# Technologies Used:
Google Colab
Python (Pandas, NumPy, Scikit-Learn, XGBoost)
Matplotlib/Seaborn (Data Visualization)
NHL Web API
# Special thanks to:
Jeremy Sylvain (NHL)
Northwood University and the MSBA faculty 
Dr. Scott Morrissette (advisor) 

