# Credit Scoring Model

This repository contains a credit scoring model project built using a comprehensive financial dataset. The project demonstrates data exploration, preprocessing, feature engineering, and model development to predict credit risk based on historical credit behavior and trade line information.

## Model Performance

- Training Accuracy (~84.7%): This indicates that the model performs well on the training data, correctly predicting outcomes for about 84.7% of the training samples.
- Test Accuracy (~82.8%): The model maintains strong performance on unseen data, correctly predicting about 82.8% of test samples.
 

## Overview

The project leverages a dataset with 3,000 records and 30 features that capture various aspects of credit history. Key features include:

- **TARGET**: A binary indicator (0/1) representing the creditworthiness of an individual where 0 indicates Good Loan and 1 indicates Bad Loan.
### Identifiers
- **ID**: Unique identifier for each record.

### Credit Behavior and History
- **DerogCnt**: The count of derogatory marks on a credit record.
- **CollectCnt**: Number of collections accounts.
- **BanruptcyInd**: Indicator for bankruptcy (0/1), where 15.3% of records indicate bankruptcy.
- **InqCnt06**: Number of credit inquiries in the last 6 months.
- **InqTimeLast**: Time (possibly in months) since the last inquiry.
- **InqFinanceCnt24**: Financial inquiries count over the past 24 months.

### Trade Line (TL) Information
- **TLTimeFirst** & **TLTimeLast**: These indicate the time since the first and most recent trade line activity.
- **TLCnt03, TLCnt12, TLCnt24, TLCnt**: These columns represent the count of trade lines over different time windows (3, 12, 24 months, and overall).
- **TLSum & TLMaxSum**: These represent the sum of trade line amounts or credit limits and the maximum among them.
- **TLSatCnt & TLSatPct**: is indicative of satisfactory accounts and the corresponding percentage.
- **TLDel60Cnt, TLDel3060Cnt24, TLDel90Cnt24, TLDel60CntAll**: These columns measure the count of delinquent trade lines. The “60” refers to 60-day delinquencies and similar logic applies to the other columns.
- **TLBadCnt24 & TLBadDerogCnt**: indicates counts of bad or derogatory accounts within a 24-month period.
- **TLOpenPct & TLOpen24Pct**: Percentages representing open trade lines overall and within the last 24 months.
- **TL75UtilCnt & TL50UtilCnt**: Utilization counts, measuring the number of accounts with at least 75% or 50% utilization.
- **TLBalHCPct**: the percentage of high-credit balance on trade lines.

The dataset, combined with the notebook implementation, offers a robust foundation for credit risk assessment, ideal for educational purposes or further research in predictive modeling.


## Getting Started

### Prerequisites

To run the notebook locally, ensure you have the following installed:
- Python 3.x
- Jupyter Notebook or JupyterLab
- Required Python packages:
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `matplotlib` / `seaborn` (for data visualization)
  - Any other libraries listed in the notebook

You can install the required packages using pip:
```bash
pip install -r requirements.txt
```
or manually install the packages

### Running the Project

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Killua2026/machineLearningprojects/credit-scoring.git
   cd credit-scoring
   ```

2. **Open the Notebook:**
   Launch Jupyter Notebook or JupyterLab in the repository directory:
   ```bash
   jupyter notebook
   ```
   Then, open the `Credit_scoring_model.ipynb` file to explore the code and analysis.

3. **Explore and Modify:**
    Run the notebook cells, experiment with different model parameters, or extend the analysis as needed.

## Project Workflow

The notebook covers the following steps:
- **Data Loading and Exploration:**  
  Load the Excel dataset and perform an initial analysis to understand data structure and quality.
  
- **Data Preprocessing:**  
  Handle missing values, outliers, and perform necessary transformations on numerical and categorical data.
  
- **Feature Engineering:**  
  Extract and create meaningful features from the credit history and trade line metrics.
  
- **Model Building:**  
  Implement machine learning algorithms to predict the `TARGET` variable, evaluate performance, and compare models.
  
- **Results and Insights:**  
  Present findings on feature importance and the model’s predictive performance, providing insights into credit risk factors.


## Contributions

Contributions to improve this project are welcome. Please fork the repository and submit pull requests for any enhancements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

## Contact
**Email:**
 iobi.2301688.stu.cu.edu.ng
