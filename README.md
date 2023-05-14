# NBA-Players-2022-2023-Analysis

## Data Scraping
I scraped my data from https://www.basketball-reference.com/, a website dedicated to basketball statistics. I wrangled the data to remove filler rows that did not contain player data and rows that repeated players. The columns of the dataframe defined on the basketball reference website that can be accessed here: https://www.basketball-reference.com/leagues/NBA_2023_totals.html

## Data Processing
I processed the data in different ways with the goal of identify patterns and outliers. Specifically, I implemented the following:
* Aggregated data based on positions to determine positions that score the most points
* Aggregated data based on age to determine if age affects points scored
* Identify which player has the highest points per game average
* Aggregate data by teams

Based on this, I came to the following conclusions:
* Shooting guards (SG) scored the most points this season, with a total of 71116 points
* The most common age in the NBA is 23, although the the player with the most points is 38 years old (Lebron James with 1590 points
* Joel Embiid of the Philadelphia 76ers has the highest ppg (points per game) with an average of 33.1 points per game.

## Data Visualization
Using tidyverse's ggplot, I graphed 
