# IPL Matches Data Analysis (2008–2024)

An end-to-end Exploratory Data Analysis (EDA) and data preprocessing workflow for the Indian Premier League (IPL) matches dataset (2008–2024) using Python and Pandas.

---

## Overview

This repository demonstrates the initial exploratory analysis, inspection, and cleaning of historical IPL match records. The pipeline handles raw data loading, structural diagnostics, null-value remediation, and summary statistics to prepare the dataset for downstream machine learning and analytical models.

---

## Dataset Profile

- **Source File:** `matches.csv`
- **Original Dimensions:** 1,095 rows × 20 columns
- **Cleaned Dimensions:** 1,028 rows × 19 columns
- **Timeframe:** IPL Seasons 2007/08 through 2024[cite: 8]
- **Key Attributes:** `id`, `season`, `city`, `date`, `match_type`, `player_of_match`, `venue`, `team1`, `team2`, `toss_winner`, `toss_decision`, `winner`, `result`, `result_margin`, `target_runs`, `target_overs`, `super_over`, `umpire1`, `umpire2`[cite: 8]

---

## Workflow & Methodology

### 1. Environment Setup & Data Ingestion
- Configured environment with `pandas`[cite: 8].
- Ingested raw match metadata into a Pandas DataFrame[cite: 8].

```python
import pandas as pd

df = pd.read_csv("matches.csv")
