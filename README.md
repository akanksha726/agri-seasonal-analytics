# agri-seasonal-analytics

## 📈 Project Methodology
This project follows a structured approach to analyze agricultural seasonal performance:

1.  **Data Loading and Initial Inspection:** The `seasonal_agriculture_performance_dataset.csv` was loaded into a pandas DataFrame. Initial checks were performed using `df.head()` and `df.info()` to understand its structure, data types, and identify missing values.
2.  **Data Preprocessing:** Missing values in `Rainfall_mm`, `Soil_Moisture_pct`, and `Yield_Tonnes_Ha` were imputed using the mean of their respective columns.
3.  **Exploratory Data Analysis (EDA):**
    *   **Seasonal Yield and Production:** Analyzed average yield and production across Kharif, Rabi, and Zaid seasons, visualizing the results with bar plots.
    *   **Seasonal Economic Performance:** Examined average profit, revenue, and market price per season to understand financial variations, also presented through bar plots.
    *   **Seasonal Environmental Conditions:** Investigated average rainfall, temperature, humidity, and sunlight hours per season to identify environmental drivers, visualized using bar plots.
    *   **Seasonal Resource Usage:** Evaluated average water used, fertilizer, and pesticide application rates across seasons, displayed with bar plots.
    *   **Crop Distribution and Performance by Season:** Grouped data by crop and season to understand yield and profit trends for different crops in various seasons, visualized using grouped bar plots.
    *   **Regional Seasonal Performance Analysis:** Performed a detailed analysis for a specific state (e.g., Maharashtra) to showcase regional variations in yield and profit per season.
4.  **Correlation Analysis:** Calculated and visualized the correlation matrix between key environmental factors (Rainfall, Temperature, Humidity, Sunlight) and performance metrics (Yield, Profit) using a heatmap to identify relationships.
5.  **Outlier Detection:** Implemented an IQR-based method to identify and visualize unusual patterns or outliers in `Profit_INR` across different crops and seasons.
6.  **Risk-vs-Reward Frontier:** Developed a scatter plot to visualize the trade-off between `Disease_Pest_Risk_pct` and `Profit_INR` for each crop and season, using `Yield_Tonnes_Ha` as bubble size.
7.  **Water-Profit Efficiency Trade-off:** Created a scatter plot comparing `Water_Efficiency_t_per_1000m3` against `Profit_INR` to assess sustainability, with `Yield_Tonnes_Ha` as bubble size.
8.  **Executive Summary Dashboard:** Consolidated key findings into a dashboard visualizing financial viability, yield efficiency, and pest/disease risk by season.
