**Healthcare Predictive Modelling**_
Forecasting Hospital Admissions & Staffing Shortages Using Advanced Machine Learning.

**The website** — healthdata.gov 

**Who published it** — the U.S. Department of Health and Human Services

"During COVID-19, hospitals didn't fail because of a lack of effort-they failed because they couldn't see what was coming."
This project builds the early warning system they needed.


**The Story Behind This Project**
When COVID-19 swept the world, hospitals faced an invisible enemy on two fronts: the virus itself, and the chaos of not knowing what tomorrow would bring. How many patients would arrive? Would there be enough nurses? Enough ICU beds?
Traditional forecasting tools — built for stable, predictable times — crumbled under the pressure of a pandemic. They couldn't adapt to sudden surges, couldn't handle complex multi-variable data, and couldn't tell clinicians why they were making a prediction.
This project was built to change that.
Using three years of real U.S. hospital data (2020–2023), two advanced machine learning models were developed, tested, and compared — each designed to give hospitals the foresight they need to act before a crisis hits, not after.

**What This Project Does**
**Goal Description** 
1. Forecast Admissions Predict daily hospital patient inflows with high accuracy
2. Detect Staffing Shortages Classify periods of likely staff shortages before they occur
3. Explain Predictions Show why the model made each prediction, not just what it predicted
4. Support PlanningGive hospital administrators actionable, data-driven intelligence

**The Two Models**
**Model 1 — Hybrid LightGBM-LSTM**

"The Fast, Efficient Workhorse"

A two-stage pipeline that combines the best of two worlds:

LightGBM handles 
1. Structured, tabular features (demographics, bed counts, test positivity) 
2. Fast, interpretable, and robust
3. LSTM takes over for the sequential,
4. Time-dependent patterns — learning the lagged relationships between infection waves and ICU demand

Best for: Resource-constrained environments,short-term planning, clinics without GPU infrastructure.

**Model 2 — Temporal Fusion Transformer (TFT)**

"The Powerful, Interpretable Oracle"

A state-of-the-art attention-based deep learning architecture that:

1.Jointly processes static hospital features (size, location, capacity).
2. Dynamic time-series signals (daily admissions, ICU occupancy, staff absence)
3. Uses multi-head attention to focus on the most relevant past time steps
4. Produces visual attention heatmaps and variable selection weights — so you can see exactly what the model is thinking

Best for: High-stakes forecasting, data-rich environments, strategic planning at scale.

