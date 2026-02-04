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
│
├── notebooks/
│   ├── Notebook 01 — Ball-by-Ball Data Engineering.ipynb
│   ├── Notebook 02 — PACC 1st grade team analysis.ipynb
│   └── Notebook 03 — Player Case Study: Anshul Sethi.ipynb
│
├── data/
│   ├── raw/        # ignored (local use only)
│   └── processed/ # cleaned, analysis-ready outputs (not committed)
│
├── docs/
│   └── data_dictionary.md
│
├── reports/
│   └── README.md  # player / coach-facing summaries
│
├── .gitignore
├── LICENSE
└── README.md
```
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

### Notebook 02 —  PACC 1st grade team analysis
**Purpose:**  
Analyse how matches are won and lost at a team level.

Focus areas:
- Run rate patterns across an innings
- Wicket timing 
- Collapse detection
- Partnership analysis

---

### Notebook 03 — Player Case Study: Anshul Sethi

**Purpose:**  
Analyse Anshul Sethi’s batting performance to identify patterns related to
time at the crease, conversion of starts, and dismissal behaviour.

**Focus areas:**
- Time at the crease and its relationship to scoring output
- Conversion of starts into higher scores (e.g. 30+ to 50+)
- Dismissal modes across different run brackets

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
