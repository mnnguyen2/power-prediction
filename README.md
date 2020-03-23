# Predicting Your Next Electricity Bill 
## Introduction

**Why predict electricity consumption?**

The ability to forecast electricity consumption based on historical usage data is crucial to effective short-term power load allocation and better long-term infrastructure planning. In addition, prediction for electrictity consumption could also play an essential role in enabling proactive energy system planning, reducing operations cost, and enforcing accurate billing.

I'm using the Household electricity power consumption dataset from UCI Machine Learning Repository. The dataset contains measurements of electric power consumption in one household with a one-minute sampling rate over a period of almost 4 years. The dataset also contains different electrical quantities and some sub-metering values. Overall, my ultimate objective would be to answer the following question: **Can the househole electricity consumption be predicted with reasonable accuracy?**

## About the dataset:
This archive contains 2075259 measurements gathered in a house located in Sceaux (7km of Paris, France) between December 2006 and November 2010 (47 months).

![TS png](https://github.com/mnnguyen2/power-prediction/blob/master/power%20TS.png)

**Attributes info:** <br>

1.date: Date in format dd/mm/yyyy <br>
2.time: time in format hh:mm:ss <br>
3.global_active_power: household global minute-averaged active power (in kilowatt) <br>
4.global_reactive_power: household global minute-averaged reactive power (in kilowatt) <br>
5.voltage: minute-averaged voltage (in volt) <br>
6.global_intensity: household global minute-averaged current intensity (in ampere) <br>
7.sub_metering_1: energy sub-metering No. 1 (in watt-hour of active energy). It corresponds to the kitchen, containing mainly a dishwasher, an oven and a microwave (hot plates are not electric but gas powered). <br>
8.sub_metering_2: energy sub-metering No. 2 (in watt-hour of active energy). It corresponds to the laundry room, containing a washing-machine, a tumble-drier, a refrigerator and a light. <br>
9.sub_metering_3: energy sub-metering No. 3 (in watt-hour of active energy). It corresponds to an electric water-heater and an air-conditioner. 

**Notes:**
1. (global_active_power * 1000/60 - sub_metering_1 - sub_metering_2 - sub_metering_3) represents the active energy consumed every minute (in watt hour) in the household by electrical equipment not measured in sub-meterings 1, 2 and 3.
2. The dataset contains some missing values in the measurements (nearly 1,25% of the rows). All calendar timestamps are present in the dataset but for some timestamps, the measurement values are missing: a missing value is represented by the absence of value between two consecutive semi-colon attribute separators. For instance, the dataset shows missing values on April 28, 2007.
3. The active energy is the real power consumed by the household, whereas the reactive energy is the unused power in the lines.

## About this repository: 
In this repository, you should find the following files:
1. **Power Prediction Presentation (PDF)**. This file should give you a good overview of the project (bonus pretty visualizations), and a summary for the models performances.
2. **Predicting your next electricity bill Python notebook**. This notebook contains the models that I built, tuned, and evaluated to predict power usage. I also went through data cleaning, pre-processing, EDA, feature engineering, model preparation, and discussed about the evaluation metrics I used for all models.  
3. **power_consumption_data.zip** This folder contains the dataset that I used. Data source: https://archive.ics.uci.edu/ml/datasets/
