## Dashboard Creation Steps

1. **Data Source Identification**
   - Used the `dbacademy.default.malawi_telecom_data` table containing monthly telecom KPIs for Malawi operators.
   - Verified data freshness and completeness by checking the latest available month and ensuring all operators are represented.

2. **Data Exploration**
   - Explored columns: `Month`, `Operator`, `Subscribers`, `ARPU MWK`, `Churn Rate Pct`, `Revenue MWK Millions`, `NPS Score`, `FCR Pct`.
   - Performed summary statistics (mean, median, min, max) for each KPI to understand data distribution.
   - Identified trends and outliers in subscriber counts, revenue, and customer satisfaction metrics using initial visualizations and descriptive statistics.
   - Examined correlations between KPIs, such as ARPU vs. Churn Rate and NPS vs. FCR.

3. **Data Cleaning & Preparation**
   - Checked for missing values and handled them appropriately (e.g., imputed with median for continuous variables, flagged missing categorical data).
   - Converted data types (e.g., ensured `Month` is datetime, numeric columns are correct types).
   - Aggregated data by operator and month for time series analysis, ensuring consistent granularity.
   - Created calculated fields such as monthly growth rates and rolling averages for smoother trend analysis.

4. **Visualization Development**
   - Created line charts for subscriber growth and revenue trends over time, segmented by operator.
   - Built bar charts for ARPU and churn rate comparisons across operators and months.
   - Added KPI widgets for NPS and FCR to highlight customer experience, using color coding for performance thresholds.
   - Incorporated scatter plots to visualize relationships between ARPU, churn, and satisfaction metrics.
   - Enabled drill-down capabilities for detailed operator-level analysis.

5. **Dashboard Assembly**
   - Combined visualizations into a single dashboard for holistic analysis, arranging charts for logical flow (e.g., growth, revenue, churn, satisfaction).
   - Added filters for `Operator` and `Month` to enable interactive exploration and custom views.
   - Included explanatory text and tooltips to guide users and provide context for each visualization.
   - Ensured responsive layout for usability across devices.

## Results

- **Subscriber Growth:** Showed steady increase for leading operators, with seasonal fluctuations and occasional dips linked to market events or promotions.
- **Revenue Trends:** Revenue correlated with subscriber growth, but ARPU varied by operator, indicating differences in pricing and customer value.
- **Churn Rate:** Identified periods of high churn, prompting further investigation into possible causes such as service disruptions or competitor activity.
- **Customer Satisfaction:** NPS and FCR metrics highlighted strengths and weaknesses in service quality, with some operators consistently outperforming others.

## Key Takeaways

- Market leaders maintained growth but faced occasional spikes in churn, often following price changes or network issues.
- Operators with higher FCR and NPS generally had lower churn rates, suggesting that customer experience initiatives are effective.
- ARPU differences suggest varying pricing strategies and customer segments, with some operators focusing on high-value customers.
- Dashboard enables ongoing monitoring and data-driven decision making for Malawi's telecom sector, supporting strategic planning and operational improvements.
