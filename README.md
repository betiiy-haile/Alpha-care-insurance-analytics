# **Insurance Analytics and Statistical Modeling Project**

This project focuses on data analysis, version control, A/B hypothesis testing, and statistical modeling to uncover insights from insurance data and create predictive models. It is structured into multiple tasks, each addressing a specific aspect of the analytics workflow.

## **Table of Contents**
- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Tasks Breakdown](#tasks-breakdown)
  - [Task 1: Git, GitHub, and EDA](#task-1-git-github-and-eda)
  - [Task 2: Data Version Control (DVC)](#task-2-data-version-control-dvc)
  - [Task 3: A/B Hypothesis Testing](#task-3-ab-hypothesis-testing)
  - [Task 4: Statistical Modeling](#task-4-statistical-modeling)
- [Installation](#installation)
- [How to Run the Project](#how-to-run-the-project)
- [Conclusion](#conclusion)

---

## **Introduction**
This project leverages advanced data analysis techniques, including exploratory data analysis (EDA), hypothesis testing, and statistical modeling, to derive actionable insights from an insurance dataset. We also implement best practices in version control with Git and DVC and build a CI/CD pipeline using GitHub Actions for continuous integration and model deployment.

## **Project Structure**


- `data/`: Directory containing raw and cleaned datasets.
- `data_storage/`: Local storage for dataset versioning using DVC.
- `src/`: Source code folder for data processing and model building scripts.
- `shared/`: Utility functions shared across different tasks in the project.
- `notebooks/`: Jupyter notebooks used for EDA and analysis.
- `.github/`: GitHub Actions CI/CD workflows configuration.
- `README.md`: Project documentation.
- `requirements.txt`: Dependencies required to run the project.



## **Tasks Breakdown**

### **Task 1: Git, GitHub, and EDA**

**Objective**: 
- Set up a Git repository with proper version control and branching.
- Perform Exploratory Data Analysis (EDA) on the provided insurance dataset, including descriptive statistics, outlier detection, and visualization.

**Key Steps**:
1. **Repository Setup**:
   - Create a Git repository with a `task-1` branch.
   - Ensure at least 3 descriptive commits per day documenting progress.
   
2. **Exploratory Data Analysis**:
   - **Data Summarization**: Analyze key features like `TotalPremium`, `TotalClaim`, and categorical variables.
   - **Univariate and Bivariate Analysis**: Visualize data distributions and correlations.
   - **Outlier Detection**: Use box plots and statistical methods to identify outliers.
   - **Visualization**: Generate insightful visualizations highlighting trends.

### **Task 2: Data Version Control (DVC)**

**Objective**: 
- Implement DVC for data version control, allowing you to track dataset versions and manage large files efficiently.

**Key Steps**:
1. **DVC Setup**:
   - Initialize DVC and configure a local storage remote.
   - Add datasets to DVC and version them through multiple commits.
   
2. **Data Tracking**:
   - Track data with `dvc add`.
   - Push tracked data to the local remote using `dvc push`.

3. **Version Control**:
   - Commit `.dvc` files to Git and ensure smooth integration between Git and DVC.

### **Task 3: A/B Hypothesis Testing**

**Objective**: 
- Conduct hypothesis testing to evaluate risk differences and profitability across provinces, zip codes, and genders.

**Key Steps**:
1. **Metrics and Segmentation**:
   - Identify key performance indicators (KPIs) and segment data into control and test groups.

2. **Statistical Testing**:
   - Apply statistical tests (t-tests, chi-squared) to validate the null hypotheses.
   - Analyze p-values and determine if differences are statistically significant.

3. **Reporting**:
   - Document the test outcomes and provide insights into potential business impacts.

### **Task 4: Statistical Modeling**

**Objective**: 
- Build predictive models using Linear Regression, Random Forests, and Gradient Boosting (XGBoost) to predict total premiums and claims.

**Key Steps**:
1. **Data Preparation**:
   - Handle missing data and perform feature engineering.
   - Convert categorical data to numeric formats using one-hot encoding or label encoding.

2. **Modeling Techniques**:
   - Train models using Linear Regression, Decision Trees, Random Forest, and XGBoost.
   - Evaluate models with accuracy, precision, recall, and F1-score.

3. **Model Interpretation**:
   - Use SHAP or LIME to explain the model outputs and determine the impact of features.


## **Installation Steps**

Follow these steps to set up the project locally:

### 1. **Clone the repository**
Clone the project repository from GitHub to your local machine:

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
```
### 2. **Set up Python virtual environment**
Create a Python virtual environment and activate it:

```bash
# Create a virtual environment
python -m venv venv

# Activate the virtual environment (Linux/Mac)
source venv/bin/activate

# Activate the virtual environment (Windows)
.\venv\Scripts\activate
```