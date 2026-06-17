# ENEM Microdata Analysis

![Python](https://img.shields.io/badge/Python-3.12-blue)
![Status](https://img.shields.io/badge/status-in%20progress-yellow)
![License](https://img.shields.io/badge/license-MIT-green)

An exploratory data analysis of Brazil's ENEM - the largest educational exam in the country - microdata to identify performance patterns across regions, income level, and school types - using open data from INEP.

---

## About

ENEM (Brazil's National High School Exam) releases annual microdata containing information from millions of participants. This project uses those datasets to answer questions such as:
 
- What is the impact of school type (public vs. private) on scores?
- How does household income influence student performance?
- Which regions concentrate the best and worst results?

---

## Planned Analysis

- Score distribution by region
- Score distribution by school type
- Income vs. performance
- Correlation between socioeconomic indicators and scores
- Regional inequality analysis

---

## Tech Stack

- Python 3.12
- Pandas
- DuckDB
- Jupyter Notebook

---

## Data

Microdata is provided by INEP and is **not included in this repository** due to size and licensing constraints.

Download at: https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/microdados/enem

---

## Getting Started

```bash
git clone https://github.com/luismanfredi/enem-analysis.git
cd enem-analysis
pip install .
```

### Loading the data

1. Access the INEP link above
2. Download the dataset for the desired year
3. Extract the content inside the data folder into 'data/raw/'

---

## Project Structure

```
enem-analysis/
├── data/
│   ├── raw/          # original data (not versioned)
│   └── processed/    # cleaned data
├── notebooks/        # Jupyter analysis notebooks
├── src/              # data processing and utility modules
├── reports/          # charts and final outputs
├── pyproject.toml
├── CHANGELOG.md
└── README.md
```

---

## Status

| Version | Description |
|---------|-------------|
| v0.1.0  | Initial project structure |
 
**Upcoming:**
 
- [ ] Data download and initial inspection
- [ ] Data cleaning and preprocessing
- [ ] Exploratory data analysis (EDA)
- [ ] Regional performance analysis
- [ ] Income and school type analysis
- [ ] Final visualizations

---
 
## License
 
MIT License — see [LICENSE](LICENSE) for details.