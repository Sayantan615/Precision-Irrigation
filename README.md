# Precision Irrigation: From Data to Prediction

## Project Overview
This project aims to optimize agricultural water usage by predicting crop irrigation needs using Machine Learning. By analyzing environmental and soil sensor data, the system determines the optimal amount of water required (Low, Medium, or High), helping to reduce water waste and ensure optimal crop health.

## Dataset Information
The dataset consists of 19 input features covering soil characteristics, weather conditions, and crop details:

- **Soil Data:** Type, pH, Moisture, Organic Carbon, Electrical Conductivity.
- **Weather Data:** Temperature (°C), Humidity, Rainfall (mm), Sunlight Hours, Wind Speed (km/h).
- **Crop Data:** Type (e.g., Cotton, Rice, Wheat), Growth Stage, Season.
- **Management Data:** Irrigation Type, Water Source, Field Area (hectares), Mulching Usage, Previous Irrigation (mm), Region.
- **Target Feature:** `Irrigation_Need` (Categories: Low, Medium, High).

## Methodology
The project follows a standard data science lifecycle:
1. **Data Inspection & Cleaning:** Handling missing values and verifying data types.
2. **Exploratory Data Analysis (EDA):** Visualizing feature distributions and correlations.
3. **Preprocessing:** Encoding categorical variables using Label Encoding and scaling numerical features.
4. **Model Training:** Implementing and comparing multiple classifiers, including:
   - Random Forest
   - XGBoost
   - K-Nearest Neighbors (KNN)
5. **Evaluation:** Assessing models using Accuracy, F1-Score, and Recall (with a focus on safety/minimizing under-irrigation).
6. **IoT Simulation:** A script to simulate real-time sensor data and provide predictions based on a consensus of models.

## Key Results
- **Random Forest:** Achieved high accuracy (~98%) and robust performance across classes.
- **XGBoost:** Delivered top-tier results (~99% accuracy) with excellent handling of complex feature interactions.

## Installation & Usage
1. **Clone the repository:**
   ```bash
   git clone https://github.com/Sayantan615/Precision-Irrigation.git
   ```
2. **Install dependencies:**
   You can install all required modules using the following command:
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Notebook:**
   Open `precision_irrigation.ipynb` in Jupyter Lab or Notebook to view the full analysis and model training process.

## Repository Structure
- `Datasets/`: Contains the training, validation, and blind test datasets.
- `precision_irrigation.ipynb`: The main research and implementation notebook.
- `README.md`: Project documentation.
