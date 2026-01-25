# PACC Cricket Analytics Project

## Overview
This project is a sports analytics case study built using historical match data from Port Adelaide Cricket Club (PACC).  
The aim is to demonstrate end-to-end data analytics skills — from raw data engineering to coach-oriented insights — using real, messy cricket data.

The project is designed as a **portfolio piece**, with a strong emphasis on:
- Data correctness and validation
- Cricket-specific domain understanding
- Clear analytical storytelling for non-technical stakeholders (coaches)

---

## Project Objectives
- Transform raw ball-by-ball cricket data into analysis-ready datasets
- Analyse how matches are won or lost at a team level
- Support selection and preparation decisions using player-level analytics
- Present insights in a clear, coach-friendly manner

---

## Data Sources
All data is sourced from **play.cricket.com.au**, including:
- Ball-by-ball match data
- Match results
- Batting, bowling, and fielding statistics
- Player match-level performance summaries

Raw data files are intentionally excluded from this repository.

---

## Project Structure

```text
pacc-cricket-analytics/
├── notebooks/
│   ├── 01_parse_ball_by_ball.ipynb
│   ├── 02_team_insights.ipynb
│   ├── 03_player_selection.ipynb
│   └── 05_case_study_tom_andrews_vs_adelaide.ipynb
├── data/
│   ├── raw/        # ignored (local use only)
│   └── processed/  # cleaned, analysis-ready outputs
├── powerbi/
│   └── PACC_Coach_Dashboard.pbix
├── docs/
│   └── data_dictionary.md
└── README.md

## Notebook Guide

### Notebook 01 — Ball-by-Ball Data Engineering
**Purpose:**  
Convert raw ball-by-ball CSV files into a trustworthy analytical dataset.

Key steps:
- Parse over and ball numbers correctly (not treated as decimals)
- Extract cumulative runs and wickets from score strings
- Derive runs-per-ball and wicket indicators using differencing
- Validate derived totals against official scorecards
- Apply innings-based phase logic suitable for multi-day matches

This notebook focuses on **data correctness**, not insights.

---

### Notebook 02 — Team & Innings Performance Insights
**Purpose:**  
Analyse how matches are won and lost at a team level.

Focus areas:
- Run rate patterns across an innings
- Wicket timing and collapse detection
- Momentum analysis
- Comparison of winning vs losing performances

---

### Notebook 03 — Player Contribution & Selection Support
**Purpose:**  
Support team selection decisions using player-level performance data.

Focus areas:
- Consistency vs volatility
- Recent form analysis
- Multi-skill contributions (batting, bowling, fielding)

---

### Notebook 05 — Player Case Study: Opponent-Specific Analysis
**Purpose:**  
A deep-dive analysis of an individual player’s performance against a specific opponent over multiple seasons.

This notebook is designed to support **match preparation** for players and coaches.

---

## Tools & Technologies
- Python (pandas, numpy)
- Jupyter Notebooks
- Git & GitHub
- Power BI (for dashboarding)

---

## Notes on Data Usage
- Player names are used for analytical demonstration only
- This project is non-commercial and intended purely for learning and portfolio purposes

I have copy pasted this exactly into readme. Is it fine?