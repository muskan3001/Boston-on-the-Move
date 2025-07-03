# Boston-on-the-Move
🚖 Uber and Lyft Dataset Analysis – Boston, MA

📌 Overview

This project presents an in-depth analysis of Uber and Lyft rides in Boston, MA, using a dataset of 693,071 rides from November 26, 2018, to December 18, 2018. With 57 features covering ride type, distance, pricing, weather conditions, and timestamps, this dataset provides a robust foundation for business intelligence and modeling.

📊 Goal: Explore ride-sharing dynamics using dimensional modeling and answer key business questions around surge pricing, ride type distribution, and revenue potential across platforms.

⸻

🗃️ Dataset Description
	•	Size: 367.38 MB
	•	Records: 693,071
	•	Features: 57
	•	Source: Kaggle – Uber & Lyft Boston Dataset
	•	Author: Bikram Maharjan, Data Science Master’s Student

🔑 Key Variables:
	•	Ride type (UberPool, WAV, Lux, etc.)
	•	Fare and distance
	•	Timestamps
	•	Weather during ride
	•	Pickup and drop-off locations

⸻

⚙️ ETL Process

🧼 1. Data Cleaning
	•	Removed missing and irrelevant records
	•	Standardized time and date formats
	•	Filtered extreme outliers in fare/distance
	•	Harmonized categorical labels

🔄 2. Data Transformation
	•	Fact Table:
	•	fact_rides: Contains the core metrics of each ride
	•	Dimension Tables:
	•	dim_time: Extracted day, hour, weekday
	•	dim_location: Source and destination zones
	•	dim_ride_type: Categorization by service and platform
	•	dim_weather: Captured weather features during ride

📥 3. Data Loading

Data was loaded into a star-schema format to allow fast, flexible querying using SQL.

⸻

💡 Business Questions & Insights

❓ Q1: Where and when is surge pricing highest?

Insights:
	•	⏰ Peak surge windows:
	•	11 PM–1 AM
	•	8 AM–9 AM
	•	1 PM
	•	📍 High-surge locations:
	•	Fenway: Surge peaks at Hour 0 (midnight)
	•	Theatre District: Hour 8 (morning rush)
	•	Back Bay: Surge at Hours 9 and 13
	•	Northeastern University: Peaks at 1 AM and 11 AM

💡 Recommendation: Incentivize drivers in high-demand zones during these windows (e.g., Fenway during game nights). Consider guaranteed earning schemes to reduce unmet ride demand.

⸻

❓ Q2: Which ride types are most in-demand by location?

Insights:
	- **Back Bay:**
  - **Uber:** WAV (wheelchair-accessible)
  - **Lyft:** Lux (premium)

- **Fenway:**
  - **Uber:** WAV (accessibility need)
  - **Lyft:** Lux (premium rides)

- **Financial District:**
  - **Uber:** UberPool (budget-conscious commuters)
  - **Lyft:** Lux Black (executive-level)

💡 Recommendation:
Boost availability of accessible rides in residential/academic areas. Promote premium rides in business districts with location-targeted campaigns.

⸻

❓ Q3: Which platform offers better revenue and user volume?

Insights:
	•	💸 Lyft: Higher fare per mile → better driver earnings
	•	📈 Uber: More ride volume → stronger user base

💡 Recommendation:
	•	Lyft: Emphasize service quality and higher driver income in premium locations
	•	Uber: Maintain dominance through pricing strategies and coverage in high-density areas

⸻

✅ Conclusion

This project showcases how data-driven insights can empower ride-sharing platforms to:
	•	Balance demand and supply
	•	Optimize pricing
	•	Target the right customer segments

By leveraging dimensional modeling, SQL, and Python analytics, we provided actionable strategies for improved service delivery and business performance.
🧰 Technologies Used
	•	Languages: Python (Pandas, NumPy, Matplotlib, Seaborn)
	•	Database: PostgreSQL (via ipython-sql)
	•	Notebook: Jupyter
	•	Dataset: Kaggle – Boston Uber & Lyft Dataset
	•	Tools: SQL, Dimensional Modeling, EDA

⸻

🚀 Future Enhancements
	•	Integrate real-time surge data (if available)
	•	Perform geospatial analysis using Folium or Plotly
	•	Train a predictive model to forecast surge pricing zones

⸻

🙌 Let’s Connect!

If you liked this project or have suggestions for improvements, feel free to ⭐ the repo or connect with me on [LinkedIn](https://www.linkedin.com/in/muskan-gulati30/)!
