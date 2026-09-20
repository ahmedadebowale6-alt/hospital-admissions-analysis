# Hospital Admissions Analysis | Power BI, Power Query, DAX & MySQL

An internship project analysing hospital-admission data to help management monitor workload, 30-day readmissions, treatment costs and patient outcomes.

The project uses a 1,000-record hospital admissions dataset and an interactive Power BI dashboard to turn operational data into clear performance reporting. It was completed as part of the **Tech Studio Academy Power BI Internship Project**.

> **Important:** This repository contains an anonymised training dataset with patient IDs only. It should not be treated as real clinical data or used for patient-care decisions.

## Dashboard Preview

![Hospital admissions dashboard preview](dashboard_preview.png)

This static preview is calculated from the project CSV. Open `Dashboard.pbix` in Power BI Desktop to explore the interactive report.

## Project Objective

To provide hospital management with an accessible dashboard that answers four operational questions:

- Where are patient admissions concentrated?
- Which departments, months and age groups have higher 30-day readmission rates?
- How do treatment costs vary across departments and outcomes?
- What trends can support better discharge planning, follow-up care and resource monitoring?

## Dashboard Scope

The Power BI report includes three analysis areas:

1. **Hospital overview** - KPI cards, admissions by department, and filters for department and discharge month.
2. **Readmission analysis** - monthly trends, readmission rate by department and age group, and departmental comparison.
3. **Cost and outcome analysis** - patient outcome distribution, treatment cost by outcome, department cost comparison, and length-of-stay versus treatment-cost analysis.

## Data Preparation

The CSV was prepared in Power Query before reporting:

- Confirmed data types for admission date, discharge date, treatment cost and length of stay.
- Checked for blank diagnosis values and inconsistent department names.
- Checked for duplicates and missing values.
- Created **Discharge Month** from the discharge date.
- Created a numeric **Readmission Flag** where `Yes = 1` and `No = 0`.
- Created age groups: `0-18`, `19-40`, `41-60` and `61+`.

## DAX Measures

The dashboard uses DAX measures for:

- Total Patients
- Average Length of Stay
- Average Treatment Cost
- Overall 30-Day Readmission Rate

## Key Findings

| Finding | Result |
| --- | ---: |
| Total patient admissions | 1,000 |
| Average length of stay | 7.46 days |
| Average treatment cost | 330,277.84 |
| Overall 30-day readmission rate | 21.0% |
| Department with the highest admission volume | Emergency (192 admissions) |
| Department with the highest readmission rate | Cardiology (27.7%) |
| Age group with the highest readmission rate | 61+ (37.7%) |
| Month with the highest readmission rate | October (26.7%) |
| Department with the highest average treatment cost | ICU (627,742.96) |
| Most common patient outcome | Recovered (698 patients) |

## Recommendations

- Review discharge planning and post-discharge follow-up for patients aged 61 and over.
- Investigate Cardiology readmissions to identify avoidable causes and improve follow-up care.
- Monitor ICU and Oncology costs alongside patient outcomes to support efficient resource allocation.
- Use the department and month filters in Power BI to support regular performance reviews.

## Tools Used

| Tool | Purpose |
| --- | --- |
| Microsoft Power BI | Interactive dashboard and visual analysis |
| Power Query | Data cleaning and transformation |
| DAX | KPI and readmission-rate calculations |
| MySQL | Data analysis and project workflow |
| Microsoft Excel / CSV | Source-data review |

## Skills Demonstrated

- Data cleaning and quality checks
- Power Query transformations
- DAX measure creation
- Healthcare operations reporting
- KPI design and dashboard development
- Readmission and patient-outcome analysis
- Cost analysis and insight communication

## Repository Structure

```text
hospital-admissions-analysis/
├── README.md
├── dashboard_preview.png
├── hospital_admissions.csv
├── Dashboard.pbix
├── Hospital admission dash.pbix
├── Hospital_Admissions_Summary_Report.pdf
├── Power BI Hospital Internship Project PDF DATA.pdf
└── Hospital Admission Data Project.pptx
```

## How to Explore the Project

1. Review `hospital_admissions.csv` to understand the source fields.
2. Open `Dashboard.pbix` in Power BI Desktop.
3. Use the department and discharge-month filters to explore the dashboard.
4. Read the project report or presentation for methodology, findings and recommendations.

## Author

**Ahmed Adebowale Akeeb**  
Data & Operations Analyst | MSc Logistics & Supply Chain Management  
[GitHub profile](https://github.com/ahmedadebowale6-alt)

---

*Portfolio project demonstrating Power BI, Power Query, DAX, MySQL and healthcare operations analysis.*
