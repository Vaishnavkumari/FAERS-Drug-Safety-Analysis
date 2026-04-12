# FDA FAERS — Adverse Drug Reaction Analysis

**Vaishnavi Kumari** | B.Pharm Final Year | [LinkedIn](https://linkedin.com/in/vaishPV)

**Tools:** Python (Pandas) · Power BI
**Data:** FDA FAERS Public Dataset — Q4 2025
**Scale:** 10 million+ raw records

---

## Why I Built This

FAERS is the FDA's real-world adverse event database — the same data
that pharmacovigilance teams use for post-marketing safety surveillance.

I wanted to work with real data, not mock datasets. So I downloaded the
raw FAERS files, cleaned and merged them in Python, and built a Power BI
dashboard that surfaces drug safety insights the way a safety analyst would.

---

## What I Did

**In Python:**
- Loaded 4 relational FAERS tables — demographics, drugs, reactions,
  and outcomes — and merged them at patient level
- Classified each case as serious or non-serious using ICH E2A criteria
- Generated every 2-drug combination per patient to identify
  co-prescribed drug patterns linked to serious outcomes
- Cleaned the full dataset down to 500,000 analysis-ready records

**In Power BI:**
## 📊 Dashboard
📄 [View FAERS Dashboard (PDF)](Dashboard/FAERS_ADR_Analysis_VaishnaviKumari%20(1).pdf)

- Built a 6-panel interactive dashboard with slicers for outcome,
  gender, and age group
- Surfaces serious ADR rate, top drugs, top reaction terms,
  and patient risk breakdown at a glance

---

## What I Found

- **77% of reports had a serious outcome** — reflecting how FAERS
  skews toward serious cases by design
- **Acetaminophen, Prednisone, and Rituximab** were the most
  frequently reported drugs in serious ADR cases
- **Females made up 67% of all reports** — consistent with known
  gender differences in ADR reporting behaviour
- **18–45 year olds** showed the highest serious ADR rate —
  likely driven by off-label use and drug interaction patterns
- **"Drug ineffective"** was a top MedDRA PT term — showing
  that FAERS captures more than just safety signals

---

## What's in This Repo

- **notebooks** — full Python analysis script
- **outputs** — cleaned CSV files used in Power BI
- **dashboard** — Power BI dashboard screenshot
- **data** — instructions to download raw FAERS files

---

## How to Reproduce

1. Download FAERS Q4 2025 from the FDA website
2. Place raw files in `data/raw/`
3. Run `notebooks/faers_analysis.py`
4. Open Power BI and connect to `outputs/faers_cleaned.csv`

---

*All analysis performed on publicly available FDA data.
No proprietary or patient-identifiable information used.*
