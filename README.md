# Deep Learning Challenge

This project is designed to create a binary classifier that predicts the success of applicants receiving funding from Alphabet Soup, a nonprofit foundation.

## Project Overview

Alphabet Soup wants a tool to help identify the applicants most likely to succeed in their ventures. Using a dataset of over 34,000 records, this project implements a deep learning model to achieve this goal.

## Dataset

The dataset contains metadata about organizations, including:

- **EIN and NAME**: Identification columns
- **APPLICATION_TYPE**: Alphabet Soup application type
- **AFFILIATION**: Affiliated sector of industry
- **CLASSIFICATION**: Government organization classification
- **USE_CASE**: Use case for funding
- **ORGANIZATION**: Organization type
- **STATUS**: Active status
- **INCOME_AMT**: Income classification
- **SPECIAL_CONSIDERATIONS**: Special considerations for application
- **ASK_AMT**: Funding amount requested
- **IS_SUCCESSFUL**: Target variable indicating success

## Project Steps

1. Data preprocessing:
   - Dropped non-beneficial columns (`EIN` and `NAME`).
   - Encoded categorical data using `pd.get_dummies`.
   - Standardized numerical data using `StandardScaler`.

2. Splitting the data:
   - Split the dataset into training and testing sets.

3. Model design:
   - Built a deep neural network with two hidden layers:
     - **Layer 1**: 80 neurons, ReLU activation
     - **Layer 2**: 30 neurons, ReLU activation
     - **Output**: 1 neuron, Sigmoid activation

4. Model training:
   - Trained the model for 50 epochs with a batch size of 32.

5. Evaluation:
   - Evaluated the model's accuracy and loss on the testing set.

## Dependencies

- Python 3.7+
- TensorFlow
- Scikit-learn
- Pandas
- Numpy

## Usage

To run this project:

1. Clone the repository:
   ```bash
   git clone https://github.com/criswait/deep-learning-challenge.git
