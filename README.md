# Yard_Management_Solution
A predictive yard optimisation model that consider dwell time uncertainty as well as re-allocation of blocking containers

My algorithm considers the yard optimisation problem as a two-part problem:
1. Predicting the dwell time of incoming containers accurately
2. Matching empty slots with incoming containers to minimize the number of moves per container

### Historical Data Required:
For a minimum of one calendar year, the following data points are required
1. Consignee Name	
2. Container Size (in TEUs)	
3. Cargo Description	
4. Gate in Date (DD/MM/YYYY format)
5. Gate out Date/Delivery Date (DD/MM/YYYY format)

### User-given Inputs:
1. Height-wise slots
2. Length-wise slots
3. Breadth-wise slots
4. Post Date
5. Forecast Window

### Data Transformation Pipeline:
1. Categorical data is converted to label data
2. Dwell Time = Gate Out Date - Gate In Date

## Solution Steps:
1. Dwell Time prediction of incoming containers
2. Heuristic for Container-Slot Matching with Location suggestion for Blocking Containers



