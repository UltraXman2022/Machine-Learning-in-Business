<h1>Project description</h1>
You work for the OilyGiant mining company. Your task is to find the best place for a new well.

<h2>Steps to choose the location:</h2>
<ul><li>Collect the oil well parameters in the selected region: oil quality and volume of reserves;</li>
<li>Build a model for predicting the volume of reserves in the new wells;</li>
<li>Pick the oil wells with the highest estimated values;</li>
<li>Pick the region with the highest total profit for the selected oil wells.</li>
<li>You have data on oil samples from three regions. Parameters of each oil well in the region are already known. Build a model that will help to pick the region with the highest profit margin. Analyze potential profit and risks using the Bootstrapping technique.

<h2>Project instructions</h2>
1.Download and prepare the data. Explain the procedure
   
2.Train and test the model for each region:<br>
<ul><li>Split the data into a training set and validation set at a ratio of 75:25</li>
   <li>Train the model and make predictions for the validation set</li>
   <li>Save the predictions and correct answers for the validation set</li>
   <li>Print the average volume of predicted reserves and model RMSE</li>
   <li>Analyze the results</ul></li><br>
   
3.Prepare for profit calculation:<br>
<ul><li>Store all key values for calculations in separate variables</li>
   <li>Calculate the volume of reserves sufficient for developing a new well without losses. Compare the obtained value with the average volume of reserves in each region</li>
   <li>Provide the findings about the preparation for profit calculation step</ul></li>
<br>

4.Write a function to calculate profit from a set of selected oil wells and model predictions:<br>
 <ul><li>Pick the wells with the highest values of predictions</li>
 <li>Summarize the target volume of reserves in accordance with these predictions</li>
 <li>Provide findings: suggest a region for oil wells' development and justify the choice. Calculate the profit for the obtained volume of reserves</ul></li>
<br>   

5.Calculate risks and profit for each region:<br>
<ul><li>Use the bootstrapping technique with 1000 samples to find the distribution of profit</li>
<li>Find average profit, 95% confidence interval and risk of losses. Loss is negative profit, calculate it as a probability and then express as a percentage</li>
<li>Provide findings: suggest a region for development of oil wells and justify the choice</ul></li>
<br> 

Data description
Geological exploration data for the three regions are stored in files:<br>
geo_data_0.csv. download dataset<br>
geo_data_1.csv. download dataset<br>
geo_data_2.csv. download dataset<br>
id — unique oil well identifier
f0, f1, f2 — three features of points (their specific meaning is unimportant, but the features themselves are significant)
product — volume of reserves in the oil well (thousand barrels).
Conditions:
Only linear regression is suitable for model training (the rest are not sufficiently predictable).
When exploring the region, a study of 500 points is carried with picking the best 200 points for the profit calculation.
The budget for development of 200 oil wells is 100 USD million.
One barrel of raw materials brings 4.5 USD of revenue The revenue from one unit of product is 4,500 dollars (volume of reserves is in thousand barrels).
After the risk evaluation, keep only the regions with the risk of losses lower than 2.5%. From the ones that fit the criteria, the region with the highest average profit should be selected.
The data is synthetic: contract details and well characteristics are not disclosed.
