# Missouri Care Gap Market Analysis

Healthcare analytics project analyzing Missouri care coordination gaps, SDOH vulnerability, FQHC access, and avoidable cost risk using Python, Power BI, and public health datasets.

## Project Overview

This project identifies Missouri counties and St. Louis ZIP codes where health burden, social vulnerability, and healthcare resource gaps may create higher care coordination risk. It combines public population health data, Federally Qualified Health Center (FQHC) access indicators, geospatial analysis, and cost modeling into an employer-ready analytics case study.

The final deliverable includes cleaned dashboard datasets, Python notebooks, visual outputs, methodology documentation, and a Power BI dashboard designed to help decision-makers prioritize outreach, care management, and intervention planning.

## Business Problem

Healthcare organizations, public health teams, and population health leaders often need to decide where limited care coordination resources should be deployed first. The challenge is that risk is not driven by one factor alone. Communities with high chronic disease burden may also face limited access to primary care, higher social vulnerability, transportation barriers, or other structural challenges.

This analysis answers the question:

> Where in Missouri are care coordination gaps likely to be most severe, and where could targeted interventions produce the greatest avoidable cost reduction?

## Dashboard Screenshots

### Missouri County-Level Dashboard

![Missouri Care Coordination Gap Analytics Dashboard](images/Screenshot%202026-05-09%20224431.png)

This dashboard summarizes county-level vulnerability, avoidable cost, potential savings, risk tier distribution, and geographic concentration of care coordination burden across Missouri.

### St. Louis ZIP-Level Dashboard

![St. Louis ZIP-Level Population Health Intelligence Dashboard](images/Screenshot%202026-05-09%20224538.png)

This dashboard provides a more granular St. Louis ZIP-code view, highlighting intervention priority, vulnerability, estimated avoidable cost, and potential savings.

## Key Findings and Expected Insights

- Missouri care coordination risk is not evenly distributed. Higher SDOH vulnerability and care coordination burden appear concentrated in southeastern and rural Missouri counties.
- The statewide dashboard estimates approximately `$774.9M` in avoidable healthcare cost and `$155.0M` in potential savings opportunity across Missouri counties.
- St. Louis ZIP-level analysis estimates approximately `$78.2M` in avoidable cost and `$15.6M` in potential savings across 45 ZIP areas.
- Risk tiering helps separate counties and ZIP codes into clearer intervention groups instead of treating all high-need areas the same.
- Combining health burden, SDOH vulnerability, and FQHC access creates a more actionable prioritization model than using disease prevalence or cost alone.

## Data Sources

This project uses public and derived datasets related to:

- CDC PLACES health burden indicators
- HRSA health center and FQHC site availability
- Missouri county and ZIP-level geography
- Social determinants of health and vulnerability indicators
- Derived care gap, risk tier, estimated avoidable cost, and potential savings measures

Prepared dashboard datasets are available in the `data/` folder:

- `data/missouri_county_final_dashboard_dataset.xlsx`
- `data/powerbi_county_dashboard_dataset.xlsx`
- `data/powerbi_zip_dashboard_dataset.xlsx`

## Methodology

The analysis follows a three-part workflow:

1. Data collection and cleaning

   The first notebook prepares Missouri county-level public health, SDOH, and healthcare resource data. It creates derived scores for SDOH vulnerability, resource gaps, and care coordination gap severity.

2. St. Louis ZIP-level deep dive

   The second notebook applies a more localized analysis to St. Louis ZIP codes, creating intervention priority categories and ZIP-level estimates for vulnerability, avoidable cost, and potential savings.

3. Cost quantification and impact analysis

   The third notebook estimates avoidable cost exposure and potential savings from targeted care coordination interventions. Outputs are exported as charts and dashboard-ready datasets.

## Core Outputs

### Missouri Care Gap Map

![Missouri care gap map](outputs/missouri_care_gap_map_final.png)

### Missouri Risk Tier Map

![Missouri risk tier map](outputs/missouri_risk_tier_map_final.png)

### SDOH Vulnerability Map

![Missouri SDOH vulnerability map](outputs/missouri_sdoh_vulnerability_map_final.png)

### Potential Intervention Savings

![Potential intervention savings](outputs/potential_intervention_savings.png)

## Repository Structure

```text
.
|-- dashboards/
|   `-- missouri_care_gap_dashboard.pbix
|-- data/
|   |-- missouri_county_final_dashboard_dataset.xlsx
|   |-- powerbi_county_dashboard_dataset.xlsx
|   `-- powerbi_zip_dashboard_dataset.xlsx
|-- docs/
|   |-- Missouri_Care_Gap_Methodology.docx
|   `-- Missouri_Care_Gap_Project_Report.docx
|-- images/
|-- notebooks/
|   |-- 01_data_collection_cleaning.ipynb
|   |-- 02_st_louis_zip_deep_dive.ipynb
|   `-- 03_cost_quantification_impact_analysis.ipynb
|-- outputs/
|-- README.md
`-- requirements.txt
```

## Power BI Dashboard

The Power BI dashboard is included here:

```text
dashboards/missouri_care_gap_dashboard.pbix
```

It supports county and ZIP-level exploration of care gap risk, SDOH vulnerability, resource gaps, intervention priority, and estimated financial impact.

## Reports

Supporting documentation is available in the `docs/` folder:

- `docs/Missouri_Care_Gap_Methodology.docx`
- `docs/Missouri_Care_Gap_Project_Report.docx`

## No PHI Used

This project does not use protected health information (PHI), patient-level records, claims-level records, or personally identifiable health data. The analysis is based on public, aggregate, and derived population health datasets intended for portfolio, education, and decision-support demonstration purposes.

## Getting Started

Clone the repository:

```bash
git clone https://github.com/BrightonSibs/missouri-care-gap-market-analysis.git
cd missouri-care-gap-market-analysis
```

Create and activate a virtual environment on Windows:

```powershell
python -m venv .venv
.venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Open the notebooks:

```bash
jupyter notebook
```

## Technologies Used

- Python
- pandas
- GeoPandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- scikit-learn
- Jupyter Notebook
- Power BI

## Project Status

This repository contains the completed analysis artifacts, dashboard-ready datasets, visual outputs, methodology documentation, and Power BI dashboard for the Missouri care gap market analysis.
