# Customer Churn Prediction

## Project Overview
This project focuses on predicting customer churn using machine learning. By analyzing customer data, the project aims to identify patterns and factors that contribute to customer attrition.

## Repository Structure

```
|-- logs/fit
|-- Churn_Modelling.csv
|-- Prediction.ipynb
|-- app.py
|-- experiments.ipynb
|-- label_encode_gender.pkl
|-- model.h5
|-- onehot_encoder_geo.pkl
|-- requirements.txt
|-- scaler.pkl
```

### File Details

- **logs/fit**: Directory containing logs related to model training.
- **Churn_Modelling.csv**: Dataset used for training and testing the machine learning models.
- **Prediction.ipynb**: Jupyter notebook for making predictions and evaluating the model.
- **app.py**: Backend application for deploying the machine learning model.
- **experiments.ipynb**: Jupyter notebook for data analysis, preprocessing, and experimentation with different algorithms.
- **label_encode_gender.pkl**: Pickle file for the label encoder used to encode gender.
- **model.h5**: Trained machine learning model saved in HDF5 format.
- **onehot_encoder_geo.pkl**: Pickle file for the one-hot encoder used for geographical data.
- **requirements.txt**: List of Python dependencies required for the project.
- **scaler.pkl**: Pickle file for the scaler used to normalize the dataset.

## Getting Started

### Prerequisites
1. Python 3.7 or higher
2. Virtual environment (optional but recommended)

### Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/SHUBHAM01S2/Customer-Churn-Prediction.git
    cd Customer-Churn-Prediction
    ```
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

### Usage
1. **Run the application**:
    ```bash
    python app.py
    ```
2. **Exploring Notebooks**:
    Open `Prediction.ipynb` or `experiments.ipynb` in Jupyter Notebook to view data analysis and prediction workflows.

### Dataset
The dataset `Churn_Modelling.csv` contains the following key columns:
- Customer ID
- Credit Score
- Geography
- Gender
- Age
- Tenure
- Balance
- NumOfProducts
- IsActiveMember
- EstimatedSalary
- Exited (target variable)

### Model
The model uses features from the dataset to predict the likelihood of a customer exiting. Preprocessing steps include:
- Encoding categorical variables (gender and geography)
- Scaling numerical features
