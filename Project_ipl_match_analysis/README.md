# IPL Match Analysis and Outcome Prediction

## Introduction
This project analyzes historical Indian Premier League (IPL) match data to understand team performance, toss impact, venue dominance, seasonal consistency, and winning probabilities. Using exploratory data analysis and visualization, the project identifies patterns that influence match outcomes and uses these trends to make data-driven predictions.

---

## Dataset
The dataset contains match-level IPL data where each record represents one match played across multiple seasons.

**Dataset structure:**
- Each row corresponds to a single IPL match
- Includes match conditions, team details, and results

**Key columns and data types:**
- `season` (numerical): IPL season year  
- `team1`, `team2` (categorical): Competing teams  
- `winner` (categorical): Match-winning team  
- `toss_winner` (categorical): Team that won the toss  
- `toss_decision` (categorical): Bat or field  
- `venue` (categorical): Match venue  
- `win_by_runs`, `win_by_wickets` (numerical): Margin of victory  

---

## Data Cleaning
The following preprocessing steps were performed based on the dataset and analysis notebooks:

- Standardized team names to ensure consistency across seasons  
- Handled missing values in result-related columns such as `winner`  
- Converted season and win margin columns to numerical format  
- Filtered matches with valid results for outcome-based analysis  
- Ensured categorical columns (toss decision, teams, venues) had consistent labels  

These steps ensured accurate aggregation and comparison across teams and seasons.

---

## Data Visualization and Analysis

### Team-wise Wins by Season
![Team-wise Wins](docs/image.png)

This chart compares the number of matches won by each team across multiple seasons. Teams such as **Mumbai Indians and Chennai Super Kings consistently record higher win counts**, indicating long-term dominance. In contrast, newer or less stable franchises show fewer wins, highlighting the impact of squad continuity and team strategy on sustained success.

---

### City-wise Team Distribution
![City-wise Distribution](docs/image%20copy.png)

The chart shows that teams based in cities like **Mumbai, Chennai, Bangalore, and Kolkata** have played significantly more matches compared to others. This reflects franchise longevity and league structure, where older teams naturally accumulate more matches and opportunities to build strong home-ground advantages.

---

### Toss Decision Preference by Teams
![Toss Decision Preference](docs/image%20copy%202.png)

This visualization shows that **most teams prefer fielding after winning the toss**, particularly teams like Mumbai Indians, Chennai Super Kings, and Kolkata Knight Riders. The consistent preference for chasing suggests that teams believe second-innings conditions and score awareness provide a tactical advantage.

---

### Distribution of Win Margins by Team
![Win Margin Distribution](docs/image%20copy%203.png)

The violin plot highlights that dominant teams such as **Mumbai Indians and Chennai Super Kings** not only win more matches but also record **larger and more frequent winning margins**, both by runs and wickets. Teams with narrower distributions tend to win closer matches, indicating less consistent dominance.

---

### Top 5 Most Consistent Players Across Seasons
![Player Consistency](docs/image%20copy%204.png)

This chart shows that a small group of players maintain strong performance across multiple seasons, with peaks occurring in specific years. The fluctuation in performance indicates that while consistency exists, player impact is often season-dependent and influenced by team composition and form.

---

### Probability of Winning Match After Winning Toss
![Toss Win Probability](docs/image%20copy%205.png)

The chart shows that **winning the toss does not guarantee winning the match**, as probabilities remain close to the 50% reference line for most teams. Some teams show marginally higher success rates after winning the toss, but overall match outcomes are more strongly influenced by team strength than toss advantage.

---

### Head-to-Head Dominance Matrix Among Teams
![Head-to-Head Heatmap](docs/image%20copy%206.png)

The heatmap highlights strong rivalries and dominance patterns. For example, **Mumbai Indians show consistent dominance over several teams**, while **Chennai Super Kings display balanced performance across opponents**. Darker cells indicate repeated success in head-to-head encounters, revealing psychological and strategic advantages.

---

### Team-wise Win Probability by Month
![Monthly Win Probability](docs/image%20copy%207.png)

This chart shows that certain teams perform better during specific months. For instance, teams like **Mumbai Indians and Chennai Super Kings show higher win probabilities in April and May**, indicating strong adaptability as the tournament progresses. Variations suggest that form, pitch conditions, and scheduling influence seasonal performance.

---

## Prediction Based on Observed Trends
Based on the dataset, teams with historically high win counts and strong head-to-head dominance—particularly **Mumbai Indians and Chennai Super Kings**—are more likely to win matches regardless of toss outcome. Teams that prefer fielding after winning the toss show slightly improved success rates, suggesting that chasing remains a marginal advantage. Additionally, teams with higher win probabilities in later months are more likely to perform well in playoff stages, indicating that momentum and adaptability play a critical role in tournament success.

---

## Conclusion
This analysis demonstrates how IPL match data reveals consistent patterns in team dominance, toss strategy, and seasonal performance. While toss decisions influence match strategy, long-term team strength and adaptability are the primary drivers of success. The project highlights the value of data-driven analysis in understanding competitive sports outcomes and predicting future match behavior.

---

## Author
**Pritika Mediboina**  
Data Analytics | Python | SQL | Data Visualization

