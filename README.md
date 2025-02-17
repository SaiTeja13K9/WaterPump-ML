# Prediction of Water Pumps Functionality

## Overview

This project focuses on predicting the functionality of water pumps using data from the Ministry of Water of the United Republic of Tanzania. The dataset contains various attributes related to pump characteristics, location, and operational status. Multiple machine learning models have been implemented to classify whether a pump is functional, non-functional, or functional but requiring repairs.

## Technologies Used

- **Programming Languages**: Python, SAS
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Machine Learning Models**: Logistic Regression, Decision Tree, Neural Network, Random Forest
- **Tools**: Jupyter Notebook, SAS Enterprise Miner, Excel

## Project Workflow

### 1. Data Collection and Preprocessing

- The dataset consists of 47,521 records with 41 columns.
- Missing values were handled by imputing categorical variables with 'unknown' and replacing numerical zeros with mean/median values.
- Irrelevant columns such as ID, wpt_name, subvillage, and funder were removed to enhance model performance.
- Geolocation inconsistencies were corrected by replacing incorrect longitude values with their mean.

### 2. Exploratory Data Analysis (EDA)

- Conducted descriptive statistics using Pandas.
- Visualized the distribution of water pump functionality status.
- Analyzed feature importance through correlation heatmaps and bar charts.

### 3. Feature Engineering

- Selected relevant features like GPS height, region, basin, public meeting, scheme management, and permit status.
- Engineered new attributes, such as categorizing the construction year into age brackets.

### 4. Machine Learning Model Implementation

- **Logistic Regression**: Implemented default and stepwise selection models.
- **Decision Tree**: Built multiple models with different misclassification rates.
- **Neural Network**: Applied an AutoNeural approach to optimize prediction accuracy.
- **Random Forest**: Used ensemble learning to improve classification performance.

### 5. Model Evaluation and Comparison

- Evaluated models based on accuracy, misclassification rate, and mean squared error.
- **Best Performing Model**: Decision Tree 2 achieved the highest accuracy (~88.18%).
- Compared different models and discussed their trade-offs in terms of generalization and overfitting.

### 6. Key Findings and Insights

- The most influential factors affecting pump functionality were construction year, population size, waterpoint type, and location-based attributes.
- The dataset exhibited class imbalance, requiring careful handling to avoid biased predictions.
- The Decision Tree 2 model emerged as the most accurate predictor, making it a valuable tool for prioritizing maintenance efforts in Tanzania.

### 7. Future Enhancements

- **Improving Feature Selection**: Exploring more advanced dimensionality reduction techniques.
- **Deep Learning Approaches**: Implementing LSTMs or CNNs for spatial data analysis.
- **Real-time Monitoring**: Incorporating IoT-based sensors to dynamically update model predictions.

## How to Run the Project

1. Clone the repository from GitHub.
2. Install dependencies using `pip install -r requirements.txt`.
3. Open and run the Jupyter Notebook (`Prediction of Water Pumps Functionality_Sai Teja Kode.ipynb`).
4. Review the results and compare model performances.
