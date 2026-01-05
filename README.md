# COVID-19 Data Analysis Using Pandas (Johns Hopkins CSSE)

## Project Overview
This project analyzes global and regional **COVID-19 daily reports** using Python and the Pandas library.  
The goal is to demonstrate practical **data wrangling, aggregation, and visualization skills** on a real-world public health dataset.

The analysis focuses on understanding trends in **confirmed cases, deaths, recoveries, and active cases** across countries and U.S. states.

---

## Data Source
- Johns Hopkins University – CSSE COVID-19 Dataset  
- Daily reports repository:  
  https://github.com/CSSEGISandData/COVID-19

**File format:** `MM-DD-YYYY.csv` (UTC)

---

## Dataset Description
Key fields used in this analysis:
- `Country_Region`
- `Province_State`
- `Confirmed`
- `Deaths`
- `Recovered`
- `Active`
- `Incident_Rate`
- `Case_Fatality_Ratio`

The dataset contains missing values and mixed data types, requiring preprocessing before analysis.

---

## Data Preparation
- Loaded daily report CSV files directly from GitHub
- Inspected dataset structure using `.head()` and `.info()`
- Identified and quantified missing values
- Handled missing values using logical assumptions (e.g., replacing NaN with 0 where appropriate)
- Created derived features such as **Active Cases**
- Grouped and aggregated data by country and U.S. state

---

## Analysis Performed

### Global Analysis
- Total confirmed cases by country
- Total deaths by country
- Total recovered cases by country
- Active cases by country
- Identification of countries with:
  - No confirmed cases
  - No deaths
  - No recovered cases
- Top 10 countries by:
  - Confirmed cases
  - Active cases

### United States Analysis
- State-wise COVID-19 deaths
- State-wise active cases
- State-wise confirmed cases

### Temporal Analysis
- Worldwide confirmed cases trend over time (Jan 3–9, 2021)

---

## Visualizations
The project includes multiple visualizations to support insights:
- Line plots for global trends
- Bar charts for country-wise and state-wise comparisons
- Interactive visualizations using **Plotly**
- Clear labeling and formatting for interpretability

---

## Key Insights
- COVID-19 impact varies significantly by country and region
- Some countries report confirmed cases but no recoveries due to reporting differences
- The United States shows large variation across states in confirmed, active, and death counts
- Active case calculation highlights ongoing disease burden more clearly than confirmed cases alone
- Time-series aggregation reveals rapid global growth patterns over short periods

---

## Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Plotly

---

## Skills Demonstrated
- Real-world data acquisition from public repositories
- Data cleaning and missing value handling
- Group-by aggregation and summarization
- Exploratory data analysis (EDA)
- Data visualization and storytelling
- Working with time-series data

---

## Conclusion
This project demonstrates the application of **core data analysis techniques** on a large, real-world public health dataset.  
It highlights the ability to extract meaningful insights from raw data and present results clearly through visualizations, making it suitable for analytical reporting and decision support.

---

## Future Enhancements
- Extend analysis to longer time ranges
- Normalize metrics by population
- Add rolling averages and growth rates
- Integrate predictive modeling for trend forecasting
