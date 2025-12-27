# IPL Match Analysis and Outcome Prediction

## Introduction
This project performs an exploratory and predictive analysis of Indian Premier League (IPL) match data to understand how team performance, toss decisions, venue advantages, and seasonal trends influence match outcomes. Using structured data analysis and visualization, the project extracts meaningful insights from historical IPL matches and applies them to predict likely winning scenarios.

---

## Dataset
The dataset contains match-level IPL data, where each row represents a single match played across multiple seasons.

**Dataset characteristics:**
- Match-level historical IPL data
- Multiple IPL seasons covered
- Structured tabular format

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
The dataset was preprocessed to ensure consistency and correctness before analysis. The following steps were performed:

- Standardized team names across seasons to avoid duplicate representations  
- Handled missing values in outcome-related columns such as `winner`  
- Converted season and win margin columns into numerical format  
- Ensured categorical consistency in toss decisions and venue names  
- Filtered matches with valid results for outcome-based analysis  

These steps ensured accurate aggregation and comparison across teams, venues, and seasons.

---

## Data Visualization and Analysis

### Team-wise Wins Across Seasons
![Team-wise Wins](docs/image.png)

This chart shows cumulative wins by each team across IPL seasons. **Mumbai Indians and Chennai Super Kings clearly lead in total wins**, demonstrating sustained dominance over multiple seasons. Teams with consistently lower win counts reflect either shorter participation periods or unstable team performance, highlighting the importance of continuity and squad strength in long-term success.

---

### City-wise Team Distribution and Home-Ground Impact
![City-wise Distribution](docs/image%20copy.png)

This visualization shows that teams associated with cities such as **Mumbai, Chennai, Bangalore, and Kolkata** not only play more matches but also record proportionally higher win counts. The direct relationship between match volume and wins indicates a strong **home-ground advantage**, where familiarity with pitch conditions, crowd support, and reduced travel contribute to improved performance. Teams with stable home venues accumulate wins faster than those with fewer or changing home locations.

---

### Toss Decision Preference by Teams
![Toss Decision Preference](docs/image%20copy%202.png)

The chart shows that most teams, particularly **Mumbai Indians, Chennai Super Kings, and Kolkata Knight Riders**, prefer to **field after winning the toss**. This consistent preference suggests a strategic inclination toward chasing targets, likely due to pitch behavior, dew factor, and score-awareness advantages in limited-overs cricket.

---

### Distribution of Winning Margins by Teams
![Winning Margin Distribution](docs/image%20copy%203.png)

This visualization highlights that dominant teams such as **Mumbai Indians and Chennai Super Kings** achieve both frequent and larger-margin victories. Their distributions show wider spreads, indicating the ability to secure convincing wins, while teams with narrower distributions tend to win closer contests, reflecting less consistent dominance.

---

### Player Consistency Across Seasons
![Player Consistency](docs/image%20copy%204.png)

The chart identifies a small set of players who deliver strong performances across multiple seasons. Performance peaks vary by season, suggesting that while individual consistency exists, overall player impact is influenced by team composition, role changes, and seasonal form.

---

### Probability of Winning After Winning the Toss
![Toss Win Probability](docs/image%20copy%205.png)

This chart shows that **winning the toss alone does not significantly increase winning probability**, as most teams hover close to a 50% success rate after winning the toss. While some teams show marginal improvements, match outcomes are more strongly driven by team strength and execution rather than toss advantage.

---

### Head-to-Head Dominance Heatmap
![Head-to-Head Heatmap](docs/image%20copy%206.png)

The heatmap reveals clear dominance patterns among teams. **Mumbai Indians show repeated dominance over several opponents**, while **Chennai Super Kings maintain balanced performance across teams**. Darker cells indicate frequent victories in head-to-head matchups, reflecting tactical advantages and psychological edges developed over time.

---

### Team-wise Monthly Win Probability
![Monthly Win Probability](docs/image%20copy%207.png)

This chart shows that teams like **Mumbai Indians and Chennai Super Kings exhibit higher win probabilities during later months of the tournament**, particularly April and May. This indicates strong adaptability as the season progresses and suggests that form, fitness, and tactical stability improve toward critical stages of the competition.

---

## Prediction Based on Observed Trends
Based on historical patterns in the dataset, teams with consistent long-term performance—especially **Mumbai Indians and Chennai Super Kings**—are more likely to win matches regardless of toss outcome. Teams choosing to field after winning the toss show slightly improved success rates, indicating a marginal chasing advantage. Additionally, teams with higher win probabilities in later months are more likely to perform well in playoff scenarios, suggesting momentum and adaptability as key success factors.

---

## Conclusion
This project demonstrates how IPL match data can be systematically analyzed to uncover performance patterns, strategic trends, and outcome determinants. The analysis highlights the dominance of consistent teams, the limited but notable influence of toss decisions, and the strong impact of home-ground advantage. Overall, the project shows how data-driven insights can enhance understanding and prediction of outcomes in competitive sports tournaments like the IPL.

---

## Author
**Pritika Mediboina**  
Data Analytics | Python | SQL | Data Visualization
