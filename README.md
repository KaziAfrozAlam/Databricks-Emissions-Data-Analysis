# # Databricks Emissions Data Analysis
End-to-End Data Project in Databricks

**An end-to-end data analytics project using Databricks SQL and AI/BI Dashboards to explore greenhouse gas emissions, identify major emission contributors, and uncover geographic and population-based emission patterns.**

## 📊 Interactive Dashboard

Explore the published dashboard:

### [🚀 Open Live Databricks Dashboard](https://dbc-a0ffbe41-0f59.cloud.databricks.com/dashboardsv3/01f176f1f32c19bf8813bb1cf6cef613/published?o=7474646072753747)

The dashboard provides an interactive view of the emissions analysis. Access depends on the dashboard's sharing permissions.

---

## 📌 Business Problem

Understanding greenhouse gas emissions is important for identifying major emission contributors and examining how emissions vary across geographic regions.

This project explores emissions data to answer questions such as:

- Which states have the highest total greenhouse gas emissions?
- Which counties or areas have the highest emission levels?
- Which areas have the highest emissions relative to population?
- How much do the ten highest-emitting states contribute to overall emissions?
- How are emissions geographically distributed?

## 🎯 Project Objectives

- Explore and analyze greenhouse gas emissions data.
- Perform geographic and state-level emissions analysis.
- Calculate population-adjusted emissions.
- Identify the highest-emitting states and areas.
- Calculate the contribution of leading states to overall emissions.
- Build visualizations to communicate analytical findings.
- Present the analysis through an interactive Databricks dashboard.

## 🏗️ Project Workflow

The project follows a structured analytics workflow:

```text
2023 Emissions Dataset (CSV)
           |
           ▼
   Databricks Workspace
           |
           ▼
   Data Availability
           |
           ▼
     Databricks SQL
           |
           ▼
   Analytical Queries
           |
           ├── Geographic Emissions
           |
           ├── State-Level Analysis
           |
           ├── County-Level Analysis
           |
           ├── Emissions per Person
           |
           └── State Contribution Analysis
                    |
                    ▼
          Databricks Visualizations
                    |
                    ▼
           Published AI/BI Dashboard
```

## 🗂️ Dataset

**Dataset:** `Emissions_Data_2023.csv`

**Location:** `Datasets/Emissions_Data_2023.csv`

The dataset contains emissions, population, and geographic information used to perform the analysis.

| Column | Description |
|---|---|
| `latitude` | Geographic latitude |
| `longitude` | Geographic longitude |
| `GHG emissions mtons CO2e` | Greenhouse gas emissions |
| `county_state_name` | County or area name |
| `population` | Population |
| `state_abbr` | State abbreviation |

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Databricks | Cloud data analytics environment |
| Databricks SQL | Querying and data analysis |
| SQL | Aggregations, calculations, ranking, and analysis |
| CSV | Source dataset |
| Databricks AI/BI Dashboards | Interactive data visualization |

## 🔍 Analysis & Implementation

### 1. Geographic Emissions Analysis

- Uses latitude and longitude to explore the geographic distribution of emissions.
- Prepares emission values for location-based visualization.
- Supports geographic comparisons across the available records.

### 2. State-Level Emissions Analysis

- Aggregates greenhouse gas emissions by state.
- Ranks states according to total emissions.
- Identifies the top ten states by total emissions.

### 3. County-Level Emissions Analysis

- Examines emissions across counties and areas.
- Ranks the top ten areas by total greenhouse gas emissions.
- Supports comparisons between geographic records.

### 4. Population-Adjusted Emissions Analysis

- Calculates emissions per person using emissions and population.
- Handles comma-separated numeric values through SQL conversion.
- Uses `NULLIF` to avoid division by zero.
- Identifies the top ten records by emissions per person.

### 5. Top States' Contribution Analysis

- Calculates the combined emissions of the top ten states.
- Compares their combined emissions against overall emissions.
- Calculates their percentage contribution to total emissions.

## 📈 Dashboard & Visualization

The published dashboard brings the analytical queries together into a visual interface.

**Dashboard:** [Explore the Live Dashboard](https://dbc-a0ffbe41-0f59.cloud.databricks.com/dashboardsv3/01f176f1f32c19bf8813bb1cf6cef613/published?o=7474646072753747)

The project includes geographic, state-level, county-level, and population-adjusted analysis.

## 📁 Repository Structure

```text
Databricks-Emissions-Data-Analysis/
│
├── Datasets/
│   └── Emissions_Data_2023.csv
│
├── Scripts/
│   ├── New Query 2026-07-03 20_25_10.dbquery.ipynb
│   ├── New Query 2026-07-03 20_56_28.dbquery.ipynb
│   ├── New Query 2026-07-03 21_31_25.dbquery.ipynb
│   ├── New Query 2026-07-03 22_18_54.dbquery.ipynb
│   └── New Query 2026-07-03 23_42_23.dbquery.ipynb
│
├── LICENSE
└── README.md
```

## ⚙️ Getting Started

### Prerequisites

- Databricks workspace
- Access to Databricks SQL
- Emissions dataset included in this repository

### Setup & Execution

1. Clone the repository:

   ```bash
   git clone https://github.com/KaziAfrozAlam/Databricks-Emissions-Data-Analysis.git
   ```

2. Open your Databricks workspace.

3. Upload `Datasets/Emissions_Data_2023.csv` to your workspace.

4. Create the `emissions_data` table using the uploaded dataset.

5. Import the SQL notebooks from the `Scripts/` directory.

6. Configure the catalog and schema as `emissions.default`, or update the SQL references to match your workspace.

7. Execute the queries to reproduce the analysis.

8. Create visualizations from the query results and explore the published dashboard.

## 💡 Key Project Highlights

- Hands-on experience with Databricks SQL.
- Geographic exploration of greenhouse gas emissions.
- State and county-level emissions analysis.
- Population-adjusted emissions calculations.
- SQL-based ranking and percentage contribution analysis.
- Interactive dashboard publishing and visualization.

## 👨‍💻 Author

**Kazi Afroz Alam**
- GitHub: [KaziAfrozAlam](https://github.com/KaziAfrozAlam)

---

**Built with Databricks SQL | Data Analytics | Interactive Visualization**
