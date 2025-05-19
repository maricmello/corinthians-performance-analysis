# ⚽ Corinthians Performance Analysis (Brasileirão)

## Description

This project analyzes matches played by the Corinthians football team using match data to explore statistics such as goals scored, game locations (home/away), and other relevant performance metrics. The goal is to clean, transform, and analyze the data to generate insights about the team’s performance. This project was carried out for the discipline Produção de Textos Acadêmicos at FATEC de Jundiaí.

---

## Data Source

The data was obtained from [Base dos Dados](https://basedosdados.org/dataset/c861330e-bca2-474d-9073-bc70744a1b23?table=18835b0d-233e-4857-b454-1fa34a81b4fa).

---

## Data Structure

- `season_year`: Championship year  
- `date`: Match date  
- `home_team`: Home team  
- `away_team`: Away team  
- `home_goals`: Goals scored by the home team  
- `away_goals`: Goals scored by the away team  
- `attendance`: Match attendance  
- `max_attendance`: Stadium maximum capacity  

Auxiliary columns created during processing:

- `home`: Whether Corinthians played at home (True/False)  
- `corinthians_goals`: Goals scored by Corinthians  
- `opponent_goals`: Goals scored by the opponent  
- `goal_difference`: Goal difference (Corinthians - opponent)  
- `location`: Match location ("Home" or "Away")  

---

### 🔎 Methods

- Data filtering and transformation using **pandas**
- Visualizations with **seaborn** and **matplotlib**
- Normality check: **Shapiro-Wilk test**
- Comparison test: **Mann-Whitney U test** (non-parametric)

### 📊 Outputs

- Frequency tables for goals and goal differences
- KDE, boxplot, and violin plots
- Statistical evidence on whether location impacts performance

### 🧰 Requirements

```bash
pip install pandas matplotlib seaborn scipy
