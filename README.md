**STRATEGIC FORECASTING: 2027 SERVICE Parts Planning**

**Project Scope:** 5-Year Historical Fleet Analysis | Confidentiality: Anonymized Data

---


**1. The Approach: Service-to-Fleet Logic**
The objective of this study is to ensure maximum machine uptime and utilization across all global regions by ensuring we have optimal service parts in stock to service projected new machine sales and the existing Install Base. Our methodology followed a three-step data pipeline:

**Step 1: Data Acquisition and Prep :** As most of the data was fetched from databse tables, I could get data cleaned and in the format needed. This saved me the effort of re-formatting and cleansing the data.

**Step 2 : Data Anonymization & Preparation:** We utilized 5 years of historical machine sales data (Anonymized), organized by Region, Quarter, and Model Type.

**Step 3: Fleet Dynamics Modeling:** We analyzed the interplay between New Machine Sales (inflow) and the Active Installed Base (existing machines in the field) to project total machine usage hours.

**Step 4: Service Part Translation:** Using the fleet usage projections, we predicted the specific quantity of Service Parts required per machine type and region.


---


**2. Analytical Competitive Landscape (The Benchmarks)**
To identify the most reliable "Signal" in this 5-year dataset, we tested three distinct mathematical approaches:

**Random Forest (Bagging):** WINNER. Best at handling the "spiky" nature of regional machine sales. 

**HGBR (Gradient Boosting):** Tested for high-velocity patterns but showed signs of overfitting.

**ARMA (Classical Time-Series):** Used to check for linear trends in global machine usage ($AR$) and self-correcting errors ($MA$).


---


**3. Risk & Confidence ($CI$)**

Every projection for 2027 includes a 95% Confidence Interval ($CI$).

**Narrow $CI$**: Indicates stable machine models where parts can be ordered "Just-in-Time."

**Wide $CI$**: Indicates high-volatility machine lines or new regions where Safety Stock is recommended to prevent downtime
