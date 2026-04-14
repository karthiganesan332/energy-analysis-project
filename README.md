**This project explores electricity demand patterns and uses optimization to evaluate how battery storage can improve cost efficiency and grid performance.**

# Analysis Section

This project analyzes real-world electricity demand data from the American Electric Power (AEP) region to identify patterns in energy usage and build a predictive model. It explores how demand varies by hour, day, and season, and demonstrates how these patterns can be used for load forecasting.

## Key Features
- Time-series analysis of hourly energy consumption  
- Visualization of daily, weekly, and seasonal patterns  
- Comparison of summer vs winter demand behavior  
- Machine learning model to predict energy usage  
- Feature importance analysis to identify key drivers of demand  

## Key Insights
- Energy demand peaks in the afternoon and evening  
- Weekday consumption is higher than weekends  
- Summer demand shows strong afternoon peaks due to cooling  
- Winter demand peaks in morning and evening due to heating  

## Technologies Used
- Python  
- pandas  
- NumPy  
- matplotlib  
- scikit-learn  

## How to Run
1. Clone the repository:
   git clone https://github.com/karthiganesan332/energy-analysis-project.git

2. Install dependencies:
   pip install -r requirements.txt

3. Open the notebook:
   analysis.ipynb

# Optimization Section

This section builds on the demand analysis by modeling how battery storage can be optimally scheduled to reduce electricity costs and improve grid performance.

Using real AEP demand data and a simulated time-varying price signal, we formulate an optimization problem that determines when to charge and discharge a battery subject to physical and operational constraints.

The model incorporates:
- Energy balance between demand, grid supply, and battery usage  
- Battery capacity and charge/discharge limits  
- Ramp constraints to reflect realistic grid operation  
- Time-varying electricity prices  

We then perform scenario analysis across different battery sizes to evaluate the impact of storage on system performance.

## Key Features
- Optimization-based battery scheduling using cvxpy  
- Integration of real-world demand data  
- Scenario analysis across multiple battery capacities  
- Evaluation of cost, peak demand, and variability metrics  
- Visualization of system behavior under different configurations  

## Key Insights
- Battery storage reduces total operating cost  
- Storage shifts demand away from high-price periods  
- Peak demand is reduced through load shifting  
- System variability decreases, improving grid stability  
- Results depend strongly on storage capacity and ramp constraints  
- Increasing storage shows diminishing returns beyond moderate capacity  

## Technologies Used
- Python  
- pandas  
- NumPy  
- matplotlib  
- seaborn  
- cvxpy  
- OSQP solver  

## How to Run
1. Clone the repository:
   git clone https://github.com/karthiganesan332/energy-analysis-project.git

2. Install dependencies:
   pip install -r requirements.txt

3. Open the notebook:
   optimization.ipynb