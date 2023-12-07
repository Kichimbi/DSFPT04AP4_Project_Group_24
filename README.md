# An Introduction to Football (Soccer) Data Analysis with Python
This is a repository introducing hands-on football (soccer) data analyses to those who want to start working with football data and perform analyses on the same.

# Summary:

---

This project introduces the following concepts:
1. How to access open event data from [*statsbomb* api](https://github.com/statsbomb/open-data#:~:text=StatsBomb%20Open%20Data%20Welcome%20to%20the%20StatsBomb%20Open,encourage%20new%20research%20and%20analysis%20at%20all%20levels.) using [`statsbombpy`](https://github.com/statsbomb/statsbombpy),
2. How to draw and visualize a soccer pitch using [*mplsoccer*](https://mplsoccer.readthedocs.io/en/latest/index.html), 
3. How to visualize a pass network map for a particular team in a particular game,
4. How to use [*NetworkX*](https://networkx.org/) module to analyse the pass network (eg. finding out degree distribution of passes, clustering coefficient, centrality, etc.), 
5. How to implement computational geometric concepts like Convex Hulls, Voronoi diagrams and Delaunay triangulations to understand and visualize football tracking data (using [*scipy.spatial*](https://docs.scipy.org/doc/scipy/reference/spatial.html) and *mplsoccer*),
6. How to analyse *Expected Goals (xG)* using open data from *statsbomb*,
7. How to use *Radar Charts* for comparing and evaluating players' per 90s stats using [*soccerplots*](https://github.com/Slothfulwave612/soccerplots/blob/master/docs/radar_chart.md) package,
8. How to use *Linear Regression* on football data, with the help of [*scikit learn*](https://scikit-learn.org/stable/index.html) module, to predict correlation betweeen *Goals scored* and *Shots on goals*,
9. How to make use of *Elastic Net* to find the relationship between number of shots taken vs the number of goals scored,  
10. How to use *Logistic Regression* to predict whether a pass is a successful pass or not (given some features of the pass), 
11. How to use a *Decision Tree Classifier* to build a model for predicting a shot outcome from a particular team, 
12. How to use *Random Forest* to predict whether a pass is a successful pass or not,
13. How to use *Naive Bayes Classifier* to predict a pass outcome,
14. How to use *K-means clustering* to cluster shot outcomes for Barcelona in La Liga
---

# References:

---
Resources that helped me start with football data analysis:
1. [**Friends of Tracking**](https://www.youtube.com/channel/UCUBFJYcag8j2rm_9HkrrA7w) youtube channel usually hosted and maintained by [**Dr. David Sumpter**](https://www.david-sumpter.com/),
2. Book [**Soccermatics**](https://www.amazon.co.uk/Soccermatics-Mathematical-Adventures-Pro-Bloomsbury/dp/1472924142/ref=tmm_pap_swatch_0?_encoding=UTF8&qid=&sr=) by Dr. Sumpter,
3. Youtube channel maintained by [**McKay Johns**](https://www.youtube.com/channel/UCmqincDKps3syxvD4hbODSg),
4. [**FC Python**](https://fcpython.com/) blog,
5. [**Graph Theory and Complex Network: An Introduction**](https://www.amazon.com/Graph-Theory-Complex-Networks-Introduction/dp/9081540610) by **Dr. Maarten Van Steen**,
6. [**Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow: Concepts, Tools, and Techniques to Build Intelligent Systems**](https://www.amazon.com/Hands-Machine-Learning-Scikit-Learn-TensorFlow/dp/1492032646/ref=sr_1_1?crid=2SIYCCF7IMD9K&dchild=1&keywords=hands+on+machine+learning+with+scikit-learn+and+tensorflow&qid=1619017819&sprefix=Hands+on+mach%2Caps%2C411&sr=8-1) by **Aurélien Géron**.
---

# Miscellaneous data files:

---
1. [*La Liga 2020-21 shot stats - Sheet1.csv*] exported from [**FBREF**](https://github.com/Kichimbi/DSFPT04AP4_Project_Group_24/blob/main/La Liga 2020-21 shot stats - Sheet1.csv)
2. [*2020-21 La Liga player stats (per 90s) - Sheet1.csv*] exported from [**FBREF**.](https://github.com/Kichimbi/DSFPT04AP4_Project_Group_24/blob/main/2020-21 La Liga player stats (per 90s) - Sheet1.csv). (https://github.com/Kichimbi/DSFPT04AP4_Project_Group_24/football-analysis-project#miscellaneous-data-files/2020-21 La Liga player stats (per 90s) - Sheet1.csv).

---
