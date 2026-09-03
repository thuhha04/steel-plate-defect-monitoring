# Steel Plate Defect Monitoring Dashboard

A Power BI portfolio project using the **UCI Steel Plates Faults dataset** to explore defect patterns in steel plate inspection data.

The project focuses on using data preparation, basic analysis, and visualization to create a simple dashboard for monitoring defect distribution and plate characteristics.

## Project Overview

The dataset contains inspection information for steel plates, including:

* Steel Type: A300 and A400
* Fault Type
* Plates Thickness
* Pixel Area
* Other inspection-related measurements

I used Power BI to organize the data and build an interactive dashboard that makes the main patterns easier to review.

## Business Objective

The main goals of this project are to:

* Understand which fault types occur most frequently.
* Compare fault distribution between A300 and A400 steel types.
* Compare average plate thickness across fault types.
* Compare average pixel area across fault types.
* Create a simple reporting view that can be used to monitor and explore inspection data.

## Dataset

**Source:** UCI Machine Learning Repository – Steel Plates Faults Dataset

The dataset contains steel plate inspection records classified into different fault categories.

The project uses the dataset for **descriptive analysis** rather than trying to determine the actual root cause of each defect.

## Data Preparation

I used **Power Query** to prepare the dataset before building the dashboard.

Main steps included:

* Reviewing the dataset structure and available fields.
* Checking data types and relevant columns.
* Preparing the data for analysis and visualization.
* Checking key values and aggregations against the source data.

## Dashboard

The dashboard provides a one-page view of the inspection data.

### KPIs

* **Total Plates** – total number of valid records.
* **A300** – number of A300 plates.
* **A400** – number of A400 plates.
* **Most Frequent Fault** – fault category with the highest number of records.

### Defect Analysis

* **Fault Distribution** – number of plates by fault type.
* **Fault Distribution by Steel Type** – comparison of fault types between A300 and A400.

### Plate Characteristics

* **Average Plates Thickness by Fault Type**
* **Average Pixel Area by Fault Type**

### Filters

The dashboard includes interactive filters for:

* Fault Type
* Steel Type

![Steel Plate Defect Monitoring Dashboard](screenshots/dashboard.png)

## Key Findings

Some patterns observed from the dashboard include:

1. **Other Fault** is the most frequently observed fault category, while **Dirtiness** has the lowest occurrence.
2. **Other Fault** appears more frequently in A400 plates than in A300 plates.
3. Average plate thickness differs across fault categories, with **Other Fault** having the highest average and **K Scratch** the lowest.
4. Average pixel area also varies between fault categories, with **K Scratch** showing the highest average and **Stains** the lowest.

These findings describe patterns in the available dataset. They do not confirm the production root cause of the defects.

## Operational Recommendations

Based on the analysis, a few areas could be investigated further:

* Review the characteristics of **Other Fault**, as it has the highest frequency.
* Compare A300 and A400 defect patterns to identify areas that may require closer monitoring.
* If production-level data is available, compare defect patterns across batches, production periods, or process conditions.
* Use additional production information to investigate possible reasons behind differences between fault categories.

## Tools & Skills

* Power BI
* Power Query
* Microsoft Excel
* Data Preparation
* Data Validation
* KPI Reporting
* Data Analysis
* Data Visualization
* Operational Reporting
* Descriptive Analysis
* Insight Generation

## Project Structure

```text
steel-plate-defect-monitoring/
├── README.md
├── powerbi/
│   └── Steel_Plate_Defect_Monitoring_Dashboard.pbix
└── screenshots/
    └── dashboard.png
```
