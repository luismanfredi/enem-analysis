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
- What is the performance gap between public and private school students?
- How do demographic factors (race and gender) intersect with educational outcomes?

---

## Planned Analysis

- Score distribution by school type
- Income vs. performance
- Correlation between socioeconomic indicators and scores
- Demographic Disparities

---

## Tech Stack

- **Python 3.12**: Core Language
- **Pandas**: Data manipulation and transformation
- **DuckDB**: Fast, in-memory analytical SQL processing (crucial for handling ENEM's millions of rows efficiently)
- **Jupyter Notebook**: Interactive environment for Exploratory Data Analysis (EDA)

---

## Data

Microdata is provided by INEP and is **not included in this repository** due to size and licensing constraints.

Download at: https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/microdados/enem

---

## Getting Started

1. Clone the repository and navigate to the directory:
```bash
git clone https://github.com/luismanfredi/enem-analysis.git
cd enem-analysis
```
2. Create a virtual environment and activate it: 
```bash
python -m venv venv
# On Windows: venv\Scripts\activate
# On Linux/Mac: source venv/bin/activate
```
3. Install the project with development dependencies (to run notebooks):
```bash
pip install -e ".[dev]"
```

### Loading the data

1. Access the INEP link above
2. Download the dataset for the desired year 
3. Extract the content inside the "DADOS" folder into 'data/raw/'

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
├── LICENSE
└── README.md
```

---

## Status

| Version | Description |
|---------|-------------|
| v0.1.0  | Initial project structure |
| v0.2.0  | Add pyproject.toml, LICENSE, CHANGELOG and documentation |
| v0.3.0  | Initial notebook for data ingestion and structural inspection |
| v0.4.0  | Reorganized notebook workflow to better reflect the data analysis process |
 
**Upcoming:**
 
- [x] Data download and initial inspection
- [ ] Data cleaning and preprocessing
- [ ] Exploratory data analysis (EDA)
- [ ] Socioeconomic and digital inclusion analysis (Income, PC, Internet)
- [ ] Final visualizations

---
 
## License
 
MIT License — see [LICENSE](LICENSE) for details.