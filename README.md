# Healthcare Analytics for Doctor Visits

## Project Overview
This project explores patterns in doctor visits using a healthcare dataset. It demonstrates a basic data analytics workflow: data inspection, quality checks, summary statistics, visualizations, and communication of findings.

## Problem Statement
People may differ in how often they visit a doctor. This project explores whether the number of visits varies with factors such as age, gender, income, reported illnesses, health status, chronic-condition indicators, and healthcare support.

## Objectives
- Understand the dataset structure and columns.
- Check data quality, including missing values.
- Summarize doctor visits.
- Compare visits across selected groups.
- Create visualizations and communicate descriptive findings.

## Dataset
The supplied dataset contains **5,190 records and 13 columns**.

| Column | Description |
|---|---|
| `visits` | Number of doctor visits during the period covered |
| `gender` | Gender category recorded in the dataset |
| `age` | Age value stored in numerical/decimal format |
| `income` | Income-level measure |
| `illness` | Number of reported illnesses or health problems |
| `reduced` | Days normal activities were reduced or affected by health problems |
| `health` | Numerical indicator of general health status |
| `private` | Indicator for private healthcare or insurance |
| `freepoor` | Indicator for free healthcare support based on financial need |
| `freerepat` | Indicator for special repatriation-related healthcare support |
| `nchronic` | Indicator for a chronic health condition |
| `lchronic` | Indicator for a long-term chronic health condition |
| `Unnamed: 0` | Record identifier, not a healthcare measurement |

**Data note:** The dataset guide does not specify the precise scale for decimal `age` values. Do not interpret them as years without checking the original documentation.

## Tools and Technologies
- **Python** — analysis programming language
- **pandas** — data loading and tabular analysis
- **NumPy** — numerical operations
- **Matplotlib** — visualizations
- **Jupyter Notebook** — interactive analysis environment

## Project Files
- `doctor_visits.csv` — source dataset
- `Healthcare_Analytics.ipynb` — analysis notebook
- `Healthcare_Analytics_Project_Presentation.pptx` — project presentation
- `visits_by_age_group.csv`, `visits_by_chronic_condition.csv`, `visits_by_gender.csv`, `visits_by_illness.csv` — summary tables, if included
- Chart image files — visualizations, if included

## How to Run

### 1. Install dependencies
Install Python and Jupyter Notebook, or use Anaconda. With pip, run:

```bash
pip install pandas numpy matplotlib jupyter
```

### 2. Keep the files together
Place `doctor_visits.csv` in the same folder as `Healthcare_Analytics.ipynb`.

### 3. Start Jupyter Notebook
Open a terminal in the project folder and run:

```bash
jupyter notebook
```

Open `Healthcare_Analytics.ipynb`.

### 4. Run the notebook
Run the cells from top to bottom. Review the output tables and charts. If your dataset has a different filename, update the path in the data-loading cell.

## Initial Descriptive Findings
The initial analysis reported:
- **5,190** records and **13** columns.
- Average doctor visits per record: approximately **0.302**.
- Median doctor visits: **0**.
- Approximately **79.8%** of records reported zero visits; approximately **20.2%** reported one or more visits.
- Initial group comparisons suggested that average visits differ across reported-illness groups and chronic-condition groups, and between gender groups.

These are descriptive observations from this dataset only. They do not prove causation and should not be generalized to all patients or populations.

## Limitations
- The dataset guide does not fully specify the units or scale for every numeric field.
- Indicator-field coding should be checked before detailed interpretation.
- Results describe the supplied records and may not represent other populations.
- This is an educational analytics project, not a clinical decision-support tool.

## Responsible Use
This project is for learning and demonstration only. It does not diagnose conditions or recommend treatment and does not replace advice from qualified healthcare professionals. Avoid sharing identifiable or sensitive patient information.

## Author
**Student Name:** Shiwank Singh  
**Project:** Healthcare Analytics for Doctor Visits
