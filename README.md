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
* Name - The name of a player
* pos - The position of a player (PG - point guard, SG - shooting guard, SF - small forward, PF - power forward, C - center)
* team_id - The name of the team the player plays for (there are 30 NBA teams)

Quantative Features:
* season - The year of the basketball season of play. A value 2023 would refer to the 2022-2023 season.
* age - The age of the player
* g - The number of games played
* gs - The number of games the player started (was one of the starting 5 players)
* mp_per_g - The average number of minutes played per game

* fg_per_g - The average number of field goals (made) per game 
* fga_per_g - The average number of field goals attempted (misses & makes) per game
* fg_pct - Field goal percentage (fg_per_g / fga_per_g)

* fg3_per_g - The average number of three-point field goals (made) per game
* fg3a_per_g - The average number of three-point field goals attempted (misses & makes) per game
* fg3_pct - Three-point field goal percentage (fg3_per_g / fg3a_per_g)

* fg2_per_g - The average number of two-point field goals (made) per game
* fg2a_per_g - The average number of two-point field goals attempted (misses & makes) per game
* fg2_pct - Two-point field goal percentage (fg2_per_g / fg2a_per_g)

* efg_pct - The average effective field goal percentage per game

* ft_per_g - The average number of free throws (made) per game 
* fta_per_g - The average number of free throws attempted (misses & makes) per game
* ft_pct - Free throws percentage (ft_per_g / fta_per_g)

* orb_per_g - Average offensive rebounds per game
* drb_per_g - Average defensive rebounds per game
* trb_per_g - Average rebounds (offensive + defensive) per game

* ast_per_g - Average assists per game

* stl_per_g - Average steals per game
* blk_per_g - Average blocks per game
* tov_per_g - Average turnovers per game
* pf_per_g - Average personal fouls per game
* pts_per_game - Average points per game

* mp - Total minutes played

* ts_pct - True Shooting Percentage (calculation: https://www.breakthroughbasketball.com/stats/tsp_calc.html)
* fg3a_per_fga_pct - Three-point shots attempted per field goal shot attempted percentage (of the field goals you shot, what percentage were three-point shots?)
* fta_per_fga_pct - Free throw shot percentage per field goal shot percentage
* drb_pct - Defensive rebound percentage
* orb_pct - Offensive rebound percentage
* trb_pct - Total rebound percentage
* ast_pct - Assist percentage
* blk_pct - Block percentage
* tov_pct - Turnover percentage
* usg_pct - Usage percentage

* ows - Offensive win shares
* dws - Defensive win shares
* ws - Win shares
* ws_per_48 - Win shares per 48 minutes
* obpm - Offensive box plus/minus
* dbpm - Defensive box plus/minus
* vrop - Value over replacement percentage
* award_share - MVP voting win share percentage
* mov - Average margin of victory during the season
* mov_adj - Average margin of victory adjusted for difficulty of opponent during the season
* win_loss_pct - Win percentage for the season
