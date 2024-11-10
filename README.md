# EV Charging Infrastructure Analysis for EnBW in Germany

Udacity Capstone Project (Data Science)

---

## Project Overview

This project aims to analyze and predict Electric Vehicle (EV) charging infrastructure accessibility across Germany, with a particular focus on EnBW charging stations. The analysis combines Google Trends data with charging station density to identify areas with accessibility gaps, especially in rural regions. By classifying regions into urban and rural categories and normalizing metrics for comparison, this project highlights where infrastructure expansion could meet growing demand more effectively.

## Project Structure

- `EV EnBW submission.html` - A rendered HTML report detailing the analysis and results.
- `EV EnBW submission.ipynb` - Jupyter Notebook containing the code for data processing, analysis, and visualizations.
- `EV_Charging_Infrastructure_Analysis_for_EnBW.pdf` - PDF write-up documenting the project methodology, analysis, and conclusions.
- `README.md` - Project documentation file.
- `germany_charging_stations.csv` - Dataset containing locations of EV charging stations across Germany.
- `germany_enbw_ev_charging_trends.csv` - Google Trends data representing search interest in EnBW EV charging stations.
- `germany_ev_charging_keywords_trends.csv` - Additional trends data for EV-related keywords.
- `kontur_population_DE_20231101.gpkg.zip` - Geopackage file with population data for Germany, used for geospatial analysis.

## Project Workflow

1. **Data Preprocessing**
   - Loading and cleaning trends and station data.
   - Handling missing values.
   - Resampling Google Trends data to monthly averages for temporal alignment.

2. **Exploratory Data Analysis (EDA)**
   - Visualizing monthly search interest to understand demand trends.
   - Classifying regions as urban or rural using population density thresholds.
   - Calculating station density per 1,000 people to identify potential supply gaps.

3. **Demand-Supply Gap Analysis**
   - Identifying regions with high demand and low charging infrastructure.
   - Calculating demand and supply averages for urban and rural classifications.
   - Merging classification data with monthly trends to compare demand across different regions.

4. **Geospatial Analysis**
   - Visualizing demand-supply gaps on a map.
   - Analyzing infrastructure needs in high-demand urban areas (e.g., Berlin) and low-density rural areas.
   - Identifying underserved areas that could benefit from additional charging stations.

5. **Visualization**
   - Comparison of normalized demand and station density across urban and rural regions.
   - Hexbin and geospatial plotting for station density across Germany.
   - Highlighting potential locations for new fast-charging stations.

## Key Findings

- **Infrastructure Gaps**: There is a noticeable gap in EV charging infrastructure in rural areas, especially for fast-charging stations, which are crucial for EV users in less densely populated regions.
- **Urban Saturation**: Urban areas show relatively high station density, indicating a saturated market. Future investments might be more impactful in underserved rural areas.
- **Region-Specific Needs**: Rural regions exhibit a higher demand for fast charging, likely due to longer travel distances. This suggests that EnBW could prioritize fast-charging infrastructure in these areas to better serve rural EV users.

## How to Use

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/ev_enbw_charging.git
   cd ev_enbw_charging
