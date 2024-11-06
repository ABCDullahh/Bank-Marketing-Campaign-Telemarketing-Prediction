## Bank Marketing Campaign Optimization with Machine Learning

---

This repository contains a comprehensive analysis and model development for a bank's marketing campaign targeting time deposits. The project utilizes machine learning techniques to predict customer interest in time deposits, thereby improving conversion rates, optimizing marketing spend, and reducing operational inefficiencies.

---

### 📌 **Project Overview**

The bank aims to enhance its marketing strategy by identifying customers with high potential interest in time deposits, a product with historically low conversion rates in previous campaigns. Given budget constraints, the bank cannot reach all customers directly, such as through phone calls, making it essential to focus on high-potential leads. This project addresses these challenges with a machine learning model prioritizing recall and optimizing precision to minimize lost revenue from false negatives.

### 📝 **Problem Statement**

The core problem is identifying the most likely customers to subscribe to time deposits while considering:
1. **Minimizing False Negatives** to capture potential revenue.
2. **Balancing Precision and Recall** to control marketing costs within budget constraints.

### 🎯 **Goals**

1. **Primary Goal**: Build a predictive model that identifies customers likely to subscribe to time deposits.
2. **Secondary Goal**: Minimize false negatives to prevent lost revenue from missing potential customers.

### 📊 **Dataset**

The dataset used for this analysis can be found on Kaggle at [Bank Marketing Campaign Dataset](https://www.kaggle.com/datasets/volodymyrgavrysh/bank-marketing-campaigns-dataset/data). The dataset includes customer demographic information, interaction history, and economic indicators that help segment customers effectively.

---

### 🔍 **Project Structure**

The project is divided into several steps:

1. **Business Understanding**: Defines the campaign challenges, constraints, and objectives.
2. **Data Understanding**: Analyzes 41,188 rows and 21 features related to customer demographics, economic indicators, and past campaign results.
3. **Data Preprocessing**: Addresses missing values, data imbalances, and outliers.
4. **Feature Engineering**: Enhances the dataset with new features like contact ratio and job categories to improve predictive power.
5. **Exploratory Data Analysis (EDA)**: Univariate, bivariate, and multivariate analyses uncover insights about customer preferences.
6. **Modeling and Evaluation**: Multiple classification models are tested, with LightGBM chosen for its performance on the F2-score (prioritizing recall).
7. **Model Constraint**: Lists constraints for model optimization, ensuring model effectiveness with minimal overfitting and redundancy.
8. **Deployment**: Implementing the final model into a pipeline for scalable predictions.

---

### 📈 **Model Evaluation**

The final LightGBM model was tuned with hyperparameter optimization. Key metrics include:

- **F2-Score**: Prioritized due to high false negative costs.
- **ROC-AUC**: Evaluates the model's ability to distinguish between potential and non-potential customers, with an AUC score of 0.80.
- **Threshold Optimization**: Ensures high recall without sacrificing precision.

---

### 🏆 **Key Insights**

1. **Customer Segmentation**: Older customers, customers with specific job types (e.g., retired, management), and customers with higher education levels showed more interest in time deposits.
2. **Contact Strategy**: Fewer contact attempts lead to better conversion rates. Over-contacting decreases effectiveness.
3. **Economic Indicators**: Lower Euribor and higher consumer price index positively impact time deposit interest, suggesting an opportunity to leverage economic conditions.

---

### 🚀 **Results**

The LightGBM model significantly outperforms the rule-based approach by:

- **Reducing False Negatives by 48.2%**: Reduces the number of missed potential customers.
- **Increasing True Positives by 105.5%**: Improves identification of customers interested in time deposits.
- **Increasing Net Profit by 149.53%**: Results in a net profit of €23,039.904 compared to the rule-based model’s loss.

---

### 🛠 **Project Setup**

#### **Requirements**

- Python 3.8+
- Pandas
- NumPy
- Scikit-learn
- LightGBM
- SHAP
- Matplotlib

#### **Installation**

Clone this repository and install the dependencies:

```bash
git clone https://github.com/ABCDullahh/Purwadhika-Final-Project-Bank-Marketing-Campaign.git
cd bank-marketing-campaign
```

#### **Run the Notebook**

Open the Jupyter notebook to explore the code and reproduce the analysis:

```bash
jupyter notebook
```

---

### 📈 **Future Enhancements**

1. **Enhanced Customer Features**: Integrate more external data, such as credit scores, for deeper customer profiling.
2. **Real-Time Predictions**: Integrate model deployment with the bank's CRM for real-time customer scoring.

---

### 👥 **Contributors**

- **Faizal Lutfi Yoga Triadi**
- **Taufiqurrahman** 

---

### 📄 **References**

1. [LightGBM Documentation](https://lightgbm.readthedocs.io/en/latest/Parameters-Tuning.html)
2. [SHAP Documentation](https://github.com/slundberg/shap)
3. Business insights referenced from customer behavior research and finance literature listed in the project notebook.


---

**NOTE**: The full documentation for each stage, including additional business insights and strategic recommendations, is available within the notebook.
