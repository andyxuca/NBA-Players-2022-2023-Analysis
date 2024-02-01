# NBA-Players-2022-2023-Analysis

## Data Scraping
For this analysis, I used the individual player data for all players of the 2022-2023 NBA season. I scraped my data from https://www.basketball-reference.com/, a website dedicated to basketball statistics. I wrangled the data to remove filler rows that did not contain player data and rows that repeated players. The columns of the dataframe are defined on the basketball reference website, which can be accessed here: https://www.basketball-reference.com/leagues/NBA_2023_totals.html

## Data Processing
I processed the data in different ways with the goal of identify patterns and outliers. Specifically, I implemented the following:
* Aggregated data based on positions to determine positions that score the most points
* Aggregated data based on age to determine if age affects points scored
* Identify which player has the highest points per game average
* Aggregate data by teams

After analyzing the results, I came to the following conclusions:
* Shooting guards (SG) scored the most points this season, with a total of 71116 points
* The most common age in the NBA is 23, although the the player with the most points is 38 years old (Lebron James with 1590 points
* Joel Embiid of the Philadelphia 76ers has the highest ppg (points per game) with an average of 33.1 points per game.

## Data Visualization
Using tidyverse's ggplot, I graphed the points scored by players of each team, the positions that scored the most points on each team, the points scored by Warrios players, and the points scored by Lakers players. Seeing these visualizations gave me a broader understanding of the data that I was working with. 

## Statistical Analysis
For statistical analysis, I decided to focus on two attributes, total rebounds and personal fouls. My goal was to see if there was a relationship between these two variables that could be used to describe the aggressiveness of a player. I calculated the Pearson and Spearman coefficients, which were both positive and close to one, indicating that there was a strong direct relationship between total rebounds and personal fouls.

## Machine Learning
Following statistical analysis, I performed K-means clustering on the total rebounds and personal fouls of players. I used the sum of squared error and the elbow method to determine the optimal number of clusters as 3. Then, I plotted my results and filtered the original data into three datasets based on the clusters. I analyzed the clusters using the average rebounds and personal fouls in each cluster, interpreting the three groups below. Additionally, I sorted the players in each cluster by the number of points they scored to easily identify notable players. 

Group 1: Less rebounds and less fouls
* Notable players:
  * Cory Joseph (DET)
  * Jaden Hardy (DAL)
  * Gary Harris (ORL)

Group 2: More rebounds and less fouls
* Notable Players
  * Jayson Tatum (BOS)
  * Joel Embiid (PHI)
  * Luka Doncic (DAL)

Group 3: More rebounds and more fouls
* Notable Players:
  * Dillon Brooks (MEM)
  * Malik Monk (SAC)
  * De'Andre Hunter (ATL)


