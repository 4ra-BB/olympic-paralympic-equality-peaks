# Olympic & Paralympic Equality Peaks

**What drove the biggest leaps in gender equality and Paralympic participation in Olympic history?** A data-driven analysis of six country case studies — from Algeria's feminist movement to Ukraine's grassroots Paralympic schools.

---

## Overview

This project identifies statistically meaningful increases in:

1. **Gender equality** (% female athletes) in Olympic delegations
2. **Paralympic participation growth** (total delegation size)
3. **Gender equality within Paralympic delegations** (intersectional analysis: gender × disability)

For each dimension, we detect the countries with the most significant sustained growth, and investigate the policies, social movements, and infrastructure behind those peaks.

## Methodology

- **Metric for gender equality**: edition-to-edition change in percentage points of female athletes per delegation
- **Metric for Paralympic growth**: edition-to-edition change in total delegation size
- **Filters**: minimum 10 athletes per delegation, maximum 8-year gap between editions (to ensure comparability)
- **Peak detection**: both single-edition spikes and sustained multi-edition trends (3+ consecutive increases)
- **Summer and Winter Games** analysed separately (4-year cycles)
- **Context analysis**: review of policies, legislation, and social factors in the 10 years preceding each growth period

### Data corrections

- **Nagano 1988 → 1998**: the Paralympic dataset contained Nagano entries labelled as 1988. Countries such as Armenia, Belarus, Czech Republic, and Estonia — which did not exist as independent nations until 1991 — confirmed this was a mislabelling. The year 1998 was entirely missing from the dataset.

## Selected Case Studies

### Olympic Gender Equality

| Country | Period | Consecutive editions | Total increase |
|---|---|---|---|
| 🇩🇿 Algeria | 1988–2012 | 7 | +44.7 pp |
| 🇧🇷 Brazil | 1976–2004 | 8 | +45.3 pp |
| 🇲🇾 Malaysia | 1996–2020 | 7 | +60.0 pp |

### Paralympic Participation

| Country | Period | Type | Growth |
|---|---|---|---|
| 🇰🇷 South Korea | 1984–1988 | Spike (host effect) | 18 → 226 athletes |
| 🇪🇸 Spain | 1972–1992 | Sustained (6 editions) | 11 → 233 athletes |
| 🇺🇦 Ukraine | 2000–2016 | Sustained (5 editions) | 30 → 168 athletes |

### Paralympic Gender Equality (Intersectional)

| Country | Period | Type | Change |
|---|---|---|---|
| 🇷🇼 Rwanda | 2012–2016 | Spike | 0% → 92.3% female |
| 🇸🇮 Slovenia | 2000–2012 | Sustained (4 editions) | +61.0 pp |
| 🇹🇼 Taiwan (Chinese Taipei) | 2000–2016 | Sustained (5 editions) | +54.4 pp |

## Key Finding

None of the six cases analysed can be explained by a single factor. Sustained growth was always the product of the intersection of at least three elements:

- A **political-institutional change** (a new constitution, a law, a democratic transition, independence)
- An **investment in sports infrastructure** (schools, federations, funding programmes)
- A **human or symbolic catalyst** (a social movement, a landmark athlete, a visionary leader, or a major sporting event)

Laws alone did not generate participation. Events alone inflated numbers that later deflated. Individuals alone could not scale without structure. The contrast between South Korea and Spain illustrates this clearly: both hosted Paralympic Games, but only in Spain did the growth endure, because it had two decades of institutional building behind it.

> Data does not measure intentions or political will; it measures outcomes. And the outcomes show that structural change in sports participation — whether in gender or inclusion — is not decreed: it is built.

## Repository Structure

```
olympic-paralympic-equality-peaks/
│
├── README.md
├── data/
│   ├── olympics.xlsx                  # Raw Olympic athlete-level data (1896–2026)
│   └── paralympics.xlsx               # Raw Paralympic delegation data (1960–2026)
│
├── notebooks/
   └── Olympic_&_Paralympic_Gender_Equality_and_Participation_Analysis.ipynb                             

## Data Sources

- **Olympic athletes (1896–2016)**: [120 years of Olympic history: athletes and results](https://www.kaggle.com/datasets/heesoo37/120-years-of-olympic-history-athletes-and-results) — individual athlete-level data scraped from sports-reference.com (rgriffin, 2018)
- **Olympic delegations (2020–2026)**: Delegation totals (men/women) compiled from official Olympic records and Wikipedia country pages
- **Paralympic delegations (1960–2026)**: Country-level delegation data (men/women/total) compiled from IPC records and Wikipedia country pages
- **IOC Continental Associations**: Official IOC regional groupings

## Tools

Python · pandas · NumPy · Plotly · Matplotlib · Seaborn · Google Colab


## Author

**Laura Benkel Brander**
Sociologist & Data Scientist | Sport × Social Impact × Data

[LinkedIn](https://www.linkedin.com/in/laurabenkelbrander)

## License

This project is licensed under the MIT License. Data sources retain their original licensing terms.
