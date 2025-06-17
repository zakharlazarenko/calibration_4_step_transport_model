# Project: Calibration of a Four-Step Transportation Model

## 1. Project Goal

The main goal of this project is to demonstrate how a classical four-step transportation model can be calibrated using data science tools.  
We simulate a simplified transport network and use synthetic Origin-Destination (OD) matrices, route assignment logic, and observed traffic counts to calibrate the model and improve its predictive accuracy.

This project combines my background in Transport Systems Engineering with my data science training and aims to provide a practical, portfolio-ready case study. It is particularly relevant for short- and medium-term transport planning tasks where accurate demand estimation is essential.

## 2. What is the Four-Step Transportation Model?

The four-step model is a well-established framework used in urban and regional transportation planning to estimate and assign travel demand within a transportation network. The steps are:

### Step 1: Trip Generation  
Estimates the number of trips produced and attracted by each zone based on land use, population, employment, etc.

### Step 2: Trip Distribution  
Distributes the generated trips between origin and destination zones, forming an OD matrix.

### Step 3: Mode Choice  
Determines the proportion of trips by each mode of transport (e.g., car, public transport, walking).  
*(Note: In this project, we simplify the model by using a single mode.)*

### Step 4: Route Assignment  
Assigns trips from the OD matrix to specific routes or links in the network based on route costs, typically travel time or distance.

The result is a prediction of traffic volumes on individual road segments, which can then be compared tl-world traffic counts.

## 3. Why is Calibration Important?

The reliability of any transportation model depends on how well it replicates real-world conditions.  
Even a correctly structured model can produce inaccurate forecasts if the OD matrix or behavioral parameters are not well calibrated.

Calibration adjusts the model inputs — particularly the OD matrix — so that the model's output (simulated traffic flows) better matches observed traffic counts.  
This process helps ensure that the model can be used for practical decision-making, such as infrastructure planning, traffic management, or evaluating policy scenarios.

In this project, we demonstrate a simple calibration procedure using synthetic data. We measure model performance before and after calibration using std error metrics (e.g., MAPE, RMSE).

By the end of the project, we will have:
- Built a basic four-step transport model using Python and synthetic data
- Estimated traffic flows before calibration
- Applied a simple calibration approach
- Evaluated the improvement in model accuracy
