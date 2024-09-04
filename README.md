# 5G-Energy-Consumption

Working on the '5G-Energy consumption' dataset that was provided by the  international telecommunication union (ITU) in 2023 as part of a global challenge or competition for data scientists all over the world to solve the 5G energy consumption modelling using machine learning techniques.

PROBLEM STATEMENT:

Network operational expenditure (OPEX) already accounts for around 25 percent of the total telecom operator’s cost, and 90 percent of it is spent on large energy bills. More than 70 percent of this energy is estimated to be consumed by the radio access network (RAN), particularly by the base stations (BSs). Thus, the objective is to build and train a ML model to estimate the energy consumed by different 5G base stations taking into consideration the impact of various engineering configurations, traffic conditions, and energy-saving methods.

DATASET DESCRIPTION:

This dataset is derived from the original copy and simplified for learning purposes. It includes cell-level traffic statistics of 4G/5G sites collected on different days.


The dataset contains the following columns:
Time: Timestamp of the data entry.
BS: Identifier for the base station.
Energy: Energy consumption values.
load: Network load values.
ESMODE: Energy-saving mode status.
TXpower: Transmission power.

MODEL DESCRIPTION
The model is based on linear regression, selected for its simplicity and effectiveness in predicting continuous variables. Feature selection and preprocessing were done on two columns to ensure the model's accuracy; 'Time' and 'BS'. 
The dataset underwent several preprocessing steps, including handling missing values, outlier detection and removal, and feature scaling using standardization.

MODEL TRAINING AND EVALUATION:
The model was trained on 70% of the dataset, with 30% held out for testing. It was evaluated using metrics such as Mean Squared Error (MSE) and R-Squared, achieving an MSE of 58.91175942638825 and R Squared of 0.5809464925256873.

To use this model, clone the repository, install the required dependencies listed in `requirements.txt`, and run 'model.predict()' with your input data to get energy consumption predictions.
