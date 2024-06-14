# Alzheimer's Disease Prediction through Transfer Learning

This personal project aims to develop a predictive model for Alzheimer's disease using transfer learning techniques. The model is designed to analyze patient data and predict the likelihood of Alzheimer's disease, enabling early detection and intervention.

## Project Overview

Alzheimer's disease is a progressive neurological disorder that leads to memory loss, cognitive decline, and ultimately, the inability to carry out simple tasks. Early detection is crucial as it can help in managing symptoms, planning for the future, and slowing the progression of the disease. This project leverages the power of transfer learning to build a robust predictive model.

## Methodology

### Data Collection and Preprocessing

1. **Data Collection**: The dataset includes images and labels for different stages of Alzheimer's disease (Very Mild Demented, Mild Demented, Moderate Demented, and Non-Demented).
2. **Data Cleaning**: Handling missing values, outlier detection, and data normalization to prepare the dataset for analysis.
3. **Data Splitting**: Splitting the dataset into training and testing sets to evaluate the model's performance.

### Exploratory Data Analysis (EDA)

1. **Visualization**: Using plots and charts to understand the distribution of data and the relationships between different features.
2. **Statistical Analysis**: Summary statistics to gain insights into the dataset and identify important features for the model.

### Feature Engineering

1. **Feature Creation**: Generating new features that can improve the model's predictive power.
2. **Feature Selection**: Identifying the most relevant features to reduce dimensionality and improve model performance.

### Model Building

1. **Transfer Learning**: Utilizing pre-trained neural networks to leverage existing knowledge and apply it to the Alzheimer's disease dataset.
2. **Model Training**: Training various machine learning models and fine-tuning hyperparameters to achieve the best performance.
3. **Model Evaluation**: Assessing the models using metrics such as accuracy, precision, recall, F1 score, and ROC-AUC.

### Model Deployment

1. **Exporting the Model**: Saving the trained model for future use.
2. **API Development**: Creating an API to serve the model and make predictions on new data.
3. **Web Application**: Building a user-friendly web interface to interact with the model and visualize predictions.

## Repository Structure

```
.
├── data                                # Data folder
│   ├── Dataset                         # Image dataset for Alzheimer's stages
├── reference                           # Project reference files
├── images                              # Project image/graph files
├── models                              # Final regression models
├── results                             # Model predicted file location
├── Alzheimers_sample.ipynb             # Project notebook with EDA and model creation
└── README.md
```

## Installation

To run the notebooks and reproduce the results, you need to set up a Python environment with the required libraries. You can use the following steps to set up the environment:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Saibalajinikki/Alzheimers-Disease-Prediction-through-Transfer-Learning.git
   cd Alzheimers-Disease-Prediction-through-Transfer-Learning
   ```

2. **Create a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install the dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

5. **Open the `Alzheimers_sample.ipynb` notebook** and run the cells in sequence to preprocess the data, perform exploratory data analysis, engineer features, build the models, and evaluate their performance.

## Business Problem

Accurate early detection of Alzheimer's disease can significantly improve patient care and management. This project aims to develop a predictive model to assist in early diagnosis using transfer learning techniques. This model can help healthcare professionals identify Alzheimer's disease at an earlier stage, leading to better patient outcomes.

## Approach

1. **Check for data completeness and integrity.**
2. **Perform EDA** with statistical analysis to determine significant features.
3. **Visualize significant features** using plots and charts.
4. **Engineer new features** based on statistical findings.
5. **Model linear regression models** and evaluate each model for final implementation.
6. **Implement feature engineering** and final model to the dataset.

## Analysis

Initial findings suggest that certain features, such as cognitive test results and medical history, play a significant role in predicting Alzheimer's disease. Visualizations and statistical analyses highlight the importance of these features in the model.

## Modeling

Using Scikit-learn and transfer learning techniques, various models were created:
- **Basic Linear Regression**
- **Recursive Feature Elimination (RFE)**
- **RFE with Cross Validation (RFECV)**

It was determined that the Linear Regression model with Recursive Feature Elimination performed the best and was utilized for the final implementation.

## Summary

The Alzheimer's disease prediction data was analyzed, tested, and modeled. Key factors influencing the predictions were identified, including cognitive test scores and medical history. The transfer learning model showed significant improvement in prediction accuracy. Future work includes enhancing the model with additional features and exploring different neural network architectures.

## Future Work

- Create additional features using interaction terms.
- Explore other transfer learning models and neural network architectures.
- Improve the dataset by including more diverse patient data.

## Contributing

If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

## License

This project is licensed under The Unlicense. See the [LICENSE](LICENSE) file for details.
