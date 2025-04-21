# Tehran-Real-Estate-Price-Estimation


House Price Prediction in Tehran
This project focuses on predicting the price of apartments in Tehran based on various features such as area, number of rooms, parking availability, and more. The dataset contains real-world data for over 4000 apartments in Tehran, and the task is to estimate the house prices in either Iranian Toman or USD using this data.

Dataset Overview
The dataset housePrice.csv contains the following columns:

Area: The area of the house in square meters.

Room: The number of rooms in the house.

Parking: Whether the house has a parking space (Yes/No).

Warehouse: Whether the house has a warehouse (Yes/No).

Elevator: Whether the house has an elevator (Yes/No).

Address: The approximate address of the house in Tehran (Some entries may have missing addresses).

Price (Toman): The price of the house in Iranian Toman.

Price (USD): The price of the house in US dollars.

Data Preprocessing
Before training a model, some preprocessing steps should be followed to clean and prepare the data:

Missing Addresses: Some houses have missing addresses. These rows should be removed from the dataset since the address information is not necessary for the price prediction task.

Outliers in Area: Some houses have an unusually large area that is likely a mistake (e.g., values far above the typical apartment sizes). These rows should be identified and removed from the dataset to avoid skewing the predictions.

Convert Categorical Variables:

The columns Parking, Warehouse, and Elevator contain categorical data in the form of "Yes" or "No". These need to be converted into numerical values (e.g., 1 for "Yes", 0 for "No") for use in machine learning models.

Feature Scaling: The features such as Area, Room, and price columns have different scales. It is recommended to scale numerical features before feeding them into models like linear regression or neural networks.

Handling Missing Values: If there are any missing values in numeric columns (like Area or Room), these should be imputed or the rows should be dropped.

Task: Price Prediction
The main objective is to predict the Price (Toman) or Price (USD) for a given apartment based on its features (Area, Room, Parking, Warehouse, Elevator)
