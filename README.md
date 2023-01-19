# MVP-Prediction
Data Science Project analyzing NBA Data in hopes of potentially predicting the MVP (Most Valuable Player) of the league.

dataset: https://www.kaggle.com/datasets/robertsunderhaft/nba-player-season-statistics-with-mvp-win-share?resource=download
# Context:

## Questions to be answered:
How are players that are traded across teams represented in the dataset?
Are there MVPS that played for different teams throughout the duration of a single season?


# Feature Engineering:

## EDA:

### Features:
The dataset contains 55 columns and 17697 rows/entries. The rows represent the performance of a player during that season. Regarding the columns, there exist the following:

Three Categorical features:
Name - The name of a player
pos - The position of a player (PG - point guard, SG - shooting guard, SF - small forward, PF - power forward, C - center)
team_id - The name of the team the player plays for (there are 30 NBA teams)

Quantative Features:
season - The year of the basketball season of play. A value 2023 would refer to the 2022-2023 season.
age - The age of the player
g - The number of games played
gs - The number of games the player started (was one of the starting 5 players)
mp_per_g - The average number of minutes played per game

fg_per_g - The average number of field goals (made) per game 
fga_per_g - The average number of field goals attempted (misses & makes) per game
fg_pct - Field goal percentage (fg_per_g / fga_per_g)

fg3_per_g - The average number of three-point field goals (made) per game
fg3a_per_g - The average number of three-point field goals attempted (misses & makes) per game
fg3_pct - Three-point field goal percentage (fg3_per_g / fg3a_per_g)

fg2_per_g - The average number of two-point field goals (made) per game
fg2a_per_g - The average number of two-point field goals attempted (misses & makes) per game
fg2_pct - Two-point field goal percentage (fg2_per_g / fg2a_per_g)

efg_pct - The average effective field goal percentage per game

ft_per_g - The average number of free throws (made) per game 
fta_per_g - The average number of free throws attempted (misses & makes) per game
ft_pct - Free throws percentage (ft_per_g / fta_per_g)
