# Why-Teams-Lost-in-The-SEC-2024
What stats indicated a loss in the SEC, in 2024-25 season

# SEC Loss Correlation Analysis
Which team-level stats most strongly associate with losses in SEC football?

## Motivation
Conference wide, the SEC does not lack talent for football. The question becomes what specific facets of the game can differentiate between teams who evenly talented.

## Data
- Source:
  - https://cfbstats.com/2024/leader/911/team/offense/split01/category09/sort01.html
  - https://247sports.com/season/2023-football/compositeteamrankings/
  - https://247sports.com/season/2024-football/compositeteamrankings/
- Seasons/Teams: 2024 SEC teams, except UGA & Texas (played 9 conference games, to everyone else's 8)
- Variables: 30 statistical categories, ranging from passing rating to allowed yards per attempt  
- Exclusions/Notes: UGA and Texas removed from analysis because they played an additional conference game (SEC Championship Game). Time of Possesion converted to "Minutes.Percent of minute" (30 minutes and 30 seconds = 30.50 minutes)

## Methods
- Cleaned data
- Correlation of each stat to "Losses"
- t-stats and p-values (two-tailed)
- Visuals: sorted correlation bar chart with significance cueing

## Key Findings
- Most Significant Stats (descending order):
  1) Allowed yards per pass attempt
  2) Loser points per game scored
  3) Opponent QB rating
- Non-drivers (No order)
  - Loser time of possession
  - Sacks allowed per game
  - Loser chunk plays gained
- **Takeaway**: Stout defense is crucial in the SEC, specifically pass defense. 2 of the 3 most significant stats above are passing defensive stats. Defenses who struggle to defend the pass play into the hand of SEC high-level recruiting, as the SEC rakes in explosive perimeter talent year after year (in 2023 and 2024, SEC had 6 teams in the top 10 for recruiting class ranking). Passing the ball effeciently allows for higher yardage gain on average, which enables an offense to quickly get into scoring position. Couple a high count of scoring opportunities for your opponent, with offensive woes for your team, and its a recipe for a loss.

## How to Reproduce
git clone https://github.com/jonathangandrews22-art/Why-Teams-Lost-in-The-SEC-2024.git
cd Why-Teams-Lost-in-The-SEC-2024
pip install -r requirements.txt
jupyter notebook notebooks/SEC_Loss_Corr.ipynb
