
# UPI Transactions Analysis

This repository contains an in-depth analysis of a UPI (Unified Payments Interface) Transactions dataset. The analysis covers various aspects including data cleaning, descriptive statistics, transaction patterns, predictive modeling, anomaly detection, feature importance analysis, and clustering analysis.

## Dataset Description

### Overview
This dataset contains simulated data of UPI transactions, which are a popular method of transferring funds between bank accounts in India. UPI allows users to send and receive money using virtual payment addresses (VPAs) linked to their bank accounts.

### Content
- **Transaction ID**: Unique identifier for each transaction.
- **Timestamp**: Date and time when the transaction occurred.
- **Sender Name**: Name of the sender initiating the transaction.
- **Sender UPI ID**: Virtual Payment Address (VPA) of the sender, including bank identifier (e.g., @okaxis, @oksbi).
- **Receiver Name**: Name of the recipient receiving the transaction.
- **Receiver UPI ID**: Virtual Payment Address (VPA) of the receiver, including bank identifier (e.g., @okaxis, @oksbi).
- **Amount (INR)**: Amount transferred in Indian Rupees (INR) for each transaction.
- **Status**: Status of the transaction (SUCCESS, FAILED).

### Dataset Size
- Total rows: 1000

## Analysis Overview

The analysis is performed in a Jupyter Notebook and includes the following sections:

1. **Data Overview and Cleaning**: Initial data exploration and cleaning steps.
2. **Feature Engineering**: Creation of new features such as `DayOfWeek` and `Hour` extracted from the `Timestamp`.
3. **Descriptive Statistics**: Summary of the dataset’s central tendency, dispersion, and shape.
4. **Transaction Patterns and Trends**: Visualization of daily transaction counts and amounts.
5. **Time Series Analysis**: Decomposition of transaction amount time series to observe its trend, seasonality, and residual components.
6. **Predictive Modeling**: Building a Random Forest Classifier to predict the success or failure of transactions.
7. **Feature Importance Analysis**: Analysis of the importance of each feature in predicting transaction success using the trained Random Forest model.
8. **Fraud Detection Analysis**: Examination of transaction amounts by their status and application of Isolation Forest for anomaly detection.
9. **Clustering Analysis**: Application of PCA for dimensionality reduction and KMeans clustering to segment transactions into different groups.
10. **Advanced Visualizations**: Creation of a correlation heatmap to visualize the relationships between different features in the dataset.
11. **Conclusion**: Summary of key insights and suggestions for further analysis.

## Requirements

The following Python libraries are required to run the analysis:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- statsmodels

You can install the required libraries using pip:
```sh
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
```

## Usage

1. **Clone the Repository**:
   ```sh
   git clone https://github.com/debjit-mandal/upi-transaction-analysis.git
   cd upi-transaction-analysis
   ```

2. **Open the Notebook**:
   Open the `UPI_Transactions_Analysis.ipynb` notebook using Jupyter Notebook or Jupyter Lab:
   ```sh
   jupyter notebook UPI_Transactions_Analysis.ipynb
   ```

3. **Run the Cells**:
   Execute the cells in the notebook to perform the analysis.

## Conclusion

In this analysis, various techniques are explored to gain insights from the UPI Transactions dataset. The results include identifying daily transaction patterns, building a predictive model for transaction success, detecting anomalies, and clustering transactions into distinct groups. Further analysis could involve more sophisticated models for predictive analytics and deeper investigation into anomalies for fraud prevention.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome. If you would like to contribute to this project, please fork the repository and submit a pull request. For major changes, please open an issue first to discuss what you would like to change.

----------------------------------------------------------------