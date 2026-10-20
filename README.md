# PUBG-Python-project

A Python course project analyzing match statistics from PUBG, one of the best-known battle royale games. The work is based on a sample of 50,000 players.
 
### Dataset
 
The data comes from [Kaggle: PUBG Match Deaths](https://www.kaggle.com/datasets/skihikingkevin/pubg-match-deaths/data) and contains match and player information: `date`, `game_size`, `match_id`, `match_mode`, `party_size`, `player_assists`, and other fields.
 
### Goal
 
To find out how winners differ from losers, and how game statistics change over time and across game modes.
 
### What's inside
 
- **Daily trends in average kills** for winners and losers, with summary statistics (mean, median, standard deviation, maximum)
  ![Daily trends in average kills](/plots/Daily_Trends_Average_Kills.png)
- **Survival time distribution** as a histogram with mean markers
  ![Survival time distribution](/plots/Survival_time_distribution_in_PUBG.png)
- **Survival time trends by date**: a scatter plot and daily averages
  ![Survival time trends by date](/plots/Survival_time_distribution_in_PUBG_2.png)
- **Player distribution across game modes** (Solo, Duos, Squads)
  ![Player distribution across game modes](/plots/Distribution_teammodes.png)
### Key findings
 
- The data is heavily imbalanced: only **2.9%** of players are winners (1,445 wins vs 48,555 losses).
- Winners average **3.76 kills** vs **0.8** for losers. The median for losers is 0: more than half of them get no kills at all.
- Winners survive about **30 minutes**, losers about **12**. Many losers are eliminated as early as the 2-3 minute mark after landing.
- Daily fluctuations in winners' averages are caused by small sample size (about 16 wins per day), not by real changes in the game. There is no clear trend over the period.
- Mode distribution: Squads 49.9%, Duos 33.7%, Solo 16.4%. These are shares of players, not matches.
