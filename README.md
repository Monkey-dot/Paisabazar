# 🏦 Paisabazaar Banking Fraud & Credit Score Analysis

**An Exploratory Data Analysis (EDA) & Machine Learning Classification Project**


**Project Overview & Business Context**
Paisabazaar is a financial services company that assists customers in finding and applying for banking and credit products. An integral part of their service is assessing the creditworthiness of individuals, which is crucial for loan approval and risk management. 

Accurate classification of credit scores helps Paisabazaar enhance credit assessment processes, reduce the risk of loan defaults, and offer personalized financial advice. This project aims to develop a predictive model that classifies individual credit scores based on features like income, credit card usage, and payment behavior.

**Dataset Access**
*Note: The original dataset contains over 100,000 records across 28 features. Because the file exceeds GitHub's standard upload limits, it is hosted externally.*
* **[Click Here to Download/View the Paisabazaar Dataset](https://drive.google.com/file/d/1PUzj3s8nGueR42CO3AKfJmJ7fadiMrnn/view?usp=drive_link)**

**Tech Stack**
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (Logistic Regression, Decision Tree, K-Nearest Neighbors)[cite: 20]

**Key Exploratory Data Analysis (EDA) Insights**
* **Data Health:** Checked via `.isnull().sum()` and `.duplicated().sum()`, confirming 0 missing values and 0 duplicate rows, allowing for clean analysis without statistical imputation.
* **Class Balance:** The `Standard` credit score tier is the largest customer segment, followed by `Poor` and `Good`.
* **Income Distribution:** Customers in the `Good` credit score tier earn a significantly higher median annual income than those in the `Standard` and `Poor` tiers.
* **Banking Trends:** Higher outstanding debt strongly correlates with holding a higher number of loans and experiencing payment delays. Conversely, a longer credit history age strongly reduces outstanding debt.

**Machine Learning Workflow & Results**
To build a solid mathematical baseline for automatically classifying credit scores, the numerical financial features were normalized using `StandardScaler`. The data was split into 80% training data (80,000 records) and 20% testing data (20,000 records). 

Three foundational models were evaluated:
1. **Decision Tree Classifier** (Best Performer) 
2. **K-Nearest Neighbors (KNN)** 
3. **Logistic Regression** (Baseline)

**How to Run This Project**
1. Clone the repository: `git clone https://github.com/Monkey-dot/Paisabazar.git`
2. Download the dataset from the link provided above and place the `dataset-2.csv` file in the root directory.
3. Open `Paisabazar.ipynb` in Google Colab or Jupyter Notebook and run all cells.
