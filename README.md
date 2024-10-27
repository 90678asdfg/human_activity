# human_activity
This project focuses on Human Activity Recognition (HAR) using smartphone sensor data and machine learning techniques to classify different physical activities based on accelerometer and gyroscope data. The data was collected from a group of volunteers performing six distinct activities. The primary goal is to build machine learning models that can accurately predict which activity is being performed based on the sensor readings.

DATASET OVERVIEW:

Participants: 30 volunteers aged 19-48 years.
Activities:
WALKING
WALKING UPSTAIRS
WALKING DOWNSTAIRS
SITTING
STANDING
LAYING
Device: Samsung Galaxy S II, placed on the waist of each volunteer.
Data Collected:
3-axial linear acceleration
3-axial angular velocity (gyroscope) at 50Hz.
The dataset was split into:

Training Set: 70% of the data
Test Set: 30% of the data
The dataset can be found here (UCI HAR Dataset).

PREPROCESSING:

Several pre-processing steps were performed on the raw sensor data to prepare it for machine learning:

Noise Filtering: Applied filters to clean the sensor data.
Segmentation: Data was segmented into fixed-width sliding windows of 2.56 seconds with 50% overlap (128 readings per window).
Signal Decomposition: Used a Butterworth low-pass filter to separate body acceleration from gravity. A 0.3 Hz cutoff was applied for gravitational force.
Preprocessing Tasks:
Checking for duplicates
Removing NULL/missing values
Addressing any class imbalance issues
Exploratory Data Analysis (EDA)
EDA was carried out to better understand the data:

Histograms and Box Plots: Used to visualize the distribution of features for each activity.
Scatter Plots: Created to examine the relationships between different features.
Time Series Plots: Helped analyze the variation in sensor readings over time.
These visualizations and statistics provided insight into how the sensor data corresponds to different physical activities.

MACHINE LEARNING MODELS:

The pre-processed data was used to train and evaluate several machine learning models:

Decision Tree
Random Forest
Support Vector Machine (SVM)
Neural Networks

KEY STEPS:

Feature Extraction: Extracted time-domain and frequency-domain features from the sensor data to distinguish activities.
Model Training: The training set (70% of the data) was used to train the models.
Evaluation: The performance of the models was evaluated on the test set (30% of the data) using metrics like accuracy, precision, recall, and F1-score.
Hyperparameter Tuning: Performed to improve model performance.

RESULTS:

The model performance is evaluated based on its ability to generalize well to new data. Cross-validation and hyperparameter tuning were conducted to ensure the best possible performance of each model. The final results demonstrate the accuracy and effectiveness of different models in predicting human activities.

TECHNOLOGIES USED:

Programming Language: Python

LIBRARIES:

Pandas, NumPy for data manipulation
Scikit-learn for machine learning algorithms
Seaborn, Matplotlib for data visualization
