## Group 24 Participants: Laban Kariuki, Dennis Kobia, Martin Kithome

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

## RESULTS

## Decision Tree Classifier to classify a shot outcome given some features of the shot, for a particular team
from statsbombpy import sb
We get data with the football teams players and the countries where the teams are located
We also get other statistics which includes'match_id', 'match_date', 'kick_off', 'competition', 'season',
   'home_team', 'away_team', 'home_score', 'away_score', 'match_status',
     'match_status_360', 'last_updated', 'last_updated_360', 'match_week',
     'competition_stage', 'stadium', 'referee', 'home_managers',
     'away_managers', 'data_version', 'shot_fidelity_version',
      'xy_fidelity_version'
      
## Elastic Net Model to find out the relation between shots by a player and the goals scored
Here we get to see player names and their age and countries of origin.
we also see the characteristics of shots scored by the featured players.
we will use Seaborn's pairplot to visualize the relationships between;
  '90s':which represents the number of 90-minute periods in a soccer game
  'Gls':which represents the number of goals.
  'Sh': which represents the number of shots taken.
  'SoT': which represents the number of shots on target.
  'Dist':which represents the distance of shots.
 
## Introductory football analysis (Pass maps, Shot Maps, Heat Maps) and Network Analysis
from mplsoccer.pitch import Pitch
Here we have an example of players: Karim Benzema', 'Francisco Román Alarcón Suárez',
 'Carlos Henrique Casimiro', 'Toni Kroos', 'Sergio Ramos García',
  'Marcelo Vieira da Silva Júnior', 'Raphaël Varane',
  'Daniel Carvajal Ramos', 'Vinícius José Paixão de Oliveira Júnior',
  'Lionel Andrés Messi Cuccittini', 'Frenkie de Jong',
  'Arthur Henrique Ramos de Oliveira Melo', 'Gerard Piqué Bernabéu',
  
We go ahead to demonstrate some of the happening in the football pitch. some of these
activities include: 
'Pass', 'Ball Receipt*', 'Carry', 'Pressure', 'Block',
 'Ball Recovery', 'Interception', 'Dribbled Past', 'Dribble',
 'Miscontrol', 'Foul Committed', 'Shot', 'Dispossessed', 'Foul Won'
 
## K-Means clustering to cluster shot outcomes for Barcelona
we use the KMeans class from scikit-learn's clustering module. 
the KMeans algorithm is is used for partitioning the dataset into the following distinct, non-overlapping subsets (clusters)
 'shot_body_part', 'shot_first_time', 'shot_one_on_one',
 'shot_open_goal', 'shot_statsbomb_xg', 'shot_technique',
 'shot_type', 'shot_outcome'
 
 ## Linear Regression model on football data
We use La Liga 2020-21 shot stats - Sheet1.csv" data for regression
Linear regression is a supervised learning algorithm used for predicting a 
continuous target variable based on one or more predictor features

## Logistic Regression to predict the pass outcome in a match
LogisticRegression is a class within scikit-learn which we will use for binary and multiclass classification.

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
1. [*La Liga 2020-21 shot stats - Sheet1.csv*](https://github.com/Kichimbi/DSFPT04AP4_Project_Group_24/blob/main/La%20Liga%202020-21%20shot%20stats%20-%20Sheet1.csv) exported from [**FBREF**](https://fbref.com/en/)
2. [*2020-21 La Liga player stats (per 90s) - Sheet1.csv*](https://github.com/Kichimbi/DSFPT04AP4_Project_Group_24/blob/main/2020-21%20La%20Liga%20player%20stats%20(per%2090s)%20-%20Sheet1.csv) exported from [**FBREF**.](https://fbref.com/en/)