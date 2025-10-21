# Mario ETL Personal Projec3. 

## 📋 Project Requirements

1. **Download** Mario ETL.zip file and extract the contents
2. **Create** the Medallion Architecture Notebooks
3. **Submit** Bronze, Silver, and Gold Parquet files
4. **Complete** 3 Total Notebooks (Bronze, Silver, Gold)

---

## 🥉 Bronze Layer

**Objective:** Data Ingestion and Initial Processing

1. Combine all CSV files into one DataFrame and save in parquet format

---

## 🥈 Silver Layer

**Objective:** Data Cleaning and Transformation

### Data Cleaning Tasks

1. **Fill null values** with smart categories
2. **Remove punctuation errors** from "Kart Role" column
3. **Check misspellings** on the "Player Name" column. Output a table of all similar names with similarity % above 80% 🍄
4. **Normalize Team names** - Remove uppercase and use `capitalize()` method
5. **Correct misspelled names** for Mario only from "Player Name" column

### Data Type Formatting

| Apply the following data types: | Column Name | Data Type |
| ------------------------------- | ----------- | --------- |
| Player Name                     | `string`    |
| Team                            | `string`    |
| Kart Racing Rank                | `string`    |
| Mushroom Cup Participation      | `bool`      |
| Participation in Battle Mode    | `bool`      |
| Platforming Rank                | `string`    |
| Boss Battle Rank                | `string`    |
| Power-Ups Owned                 | `string`    |
| Power-Ups Used                  | `int32`     |
| Team Points                     | `int32`     |
| Levels Completed                | `int32`     |
| Lives Lost                      | `int32`     |
| Times Hit by Enemies            | `int32`     |
| Vehicle Type                    | `string`    |
| World                           | `string`    |
| Coins Spent in Toad Town        | `int32`     |
| Companion                       | `string`    |
| Primary Game                    | `string`    |

### Additional Cleaning Steps

7. **Clean whitespace** - Remove leading and trailing spaces from:

   - Vehicle Type
   - World
   - Primary Game

8. **Apply title case** to:
   - Companion
   - World

---

## 🥇 Gold Layer

**Objective:** Analytics and Reporting

### 📊 Create 10 Gold Reports

1. **Team Performance Summary**

   - Total team points, average rank, and total coins spent in Toad Town by team
   - _Rank scoring:_ `{'S': 5, 'A': 4, 'B': 3, 'C': 2, 'D': 1}`

2. **Player Performance**

   - Total team points earned by each player

3. **Power-Up Analytics**

   - Count and average number of power-ups used per player

4. **World Difficulty Analysis**

   - Average number of lives lost in each world

5. **Top Performers**

   - Top player per team by team points

6. **Vehicle Popularity**

   - Popularity count of each vehicle type

7. **Risk Assessment**
   - Players at highest risk (total lives lost, sorted most to least)
8. **World Completion Stats**

   - Average and total number of levels completed in each world

9. **Team Combat Analysis**

   - Total and average number of times each team was hit by enemies

10. **Spending Analysis**
    - Total coins spent in Toad Town by each team

---

## 📤 Submission Requirements

**Submit via Canvas:**

### 📁 Parquet Files

#### Core Files

- `Bronze.parquet`
- `Silver.parquet`

#### Gold Report Files

- `gold_team_summary.parquet`
- `gold_player_performance.parquet`
- `gold_powerup_player.parquet`
- `gold_world_difficulty.parquet`
- `gold_top_player_per_team.parquet`
- `gold_vehicle_counts.parquet`
- `gold_risk_assessment.parquet`
- `gold_world_completion.parquet`
- `gold_hits_team.parquet`
- `gold_spending_analysis.parquet`

### 📓 Jupyter Notebooks

- `Bronze_Mario.ipynb`
- `Silver_Mario.ipynb`
- `Gold_Mario.ipynb`

---

_Good luck with your Mario ETL project! 🎮_
