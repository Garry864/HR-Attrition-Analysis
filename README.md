# 🧑‍💼 HR Attrition Analysis

Welcome to the **HR Attrition Analysis** project repository! This project aims to understand the key factors influencing employee attrition, with the goal of helping organizations develop strategies to reduce turnover. Through comprehensive data exploration, feature engineering, and machine learning, we dive deep into employee demographics, satisfaction levels, job roles, and more.

📄 **Profile Report**:  
[Explore the Full Report](https://garry864.github.io/HR-Attrition-Analysis/)

---

## 📖 Project Overview

The dataset used in this analysis contains **1,470 employee records**, each with **35 features** related to various aspects of employees, including job roles, work experience, and satisfaction levels. This analysis aims to explore the reasons behind employee attrition and develop predictive models that can help HR departments proactively manage turnover.

---

## ✨ Key Insights

### 1️⃣ **Attrition Rate**
- **16.12%** of employees in the dataset left the company, setting the context for understanding which factors contribute to attrition.

### 2️⃣ **Data Exploration & Visualization**
- **Distribution Analysis**: Visualized distributions for numerical features like age, daily rate, income, and distance from home using histograms and kernel density estimations.
- **Bar Plots**: Used to explore attrition rates across job roles, departments, and marital statuses.
- **Pie Charts**: Displayed the proportion of attrition and non-attrition categories for various features.

### 3️⃣ **Feature Engineering**
- Several new features were created to capture potential predictors of attrition:
  - **SalesDpt**: Identifies employees in the Sales department.
  - **JobInvCut**: Flags employees with low job involvement.
  - **MiddleTraining**: Flags employees with moderate training.
  - **MoovingPeople**: Identifies employees with frequent job changes.
  - **TotalSatisfaction_mean**: Average satisfaction across various aspects of work life.
  - Other engineered features include **NotSatif**, **LongDisWL1**, **Engaged**, and **Income_YearsComp**, all aimed at better capturing patterns in attrition.

### 4️⃣ **Feature Selection**
- **Correlation Analysis**: A correlation matrix identified and removed highly correlated features to reduce multicollinearity and improve model performance.
- Seven features were dropped, including those related to departments, job involvement, and training frequency.

### 5️⃣ **Model Building & Evaluation**
- **XGBoost Classifier**: Used to predict attrition, with preprocessing steps like label encoding, one-hot encoding, and feature scaling applied to the data.
- **Hyperparameter Optimization**: RandomizedSearchCV was used to find the best combination of hyperparameters for optimal model performance.
- **Model Performance**:
  - **Accuracy**: The XGBoost model achieved an accuracy of **88.64%**.
  - **Evaluation Metrics**: The model was evaluated using a confusion matrix, ROC curve, AUC, precision-recall curve, and feature importance analysis.
  - **Top Features**: Key factors influencing attrition include **OverTime**, **TotalWorkingYears**, **JobLevel**, and **StockOptionLevel**.

### 6️⃣ **Key Findings**
- **High Impact Features**: Features like **OverTime**, **TotalWorkingYears**, **JobLevel**, and **StockOptionLevel** were found to be most important in predicting attrition.
- The model’s ability to predict attrition can help organizations take preventive measures to reduce turnover and improve retention.

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/garry864/HR-Attrition-Analysis.git
cd HR-Attrition-Analysis
```

### 2️⃣ Install Dependencies
Ensure Python is installed and set up the required environment:
```bash
pip install -r requirements.txt
```

### 3️⃣ Explore the Data
- Open the **hosted report**: [HR Attrition Analysis Report](https://garry864.github.io/HR-Attrition-Analysis/).
- Run the scripts in the `/src/` folder to reproduce or extend the analysis.

---

## 🌟 Future Exploration Opportunities

- **Employee Engagement**: Investigate deeper into engagement-related factors that influence attrition.
- **Sentiment Analysis**: Integrate employee surveys or feedback data to further analyze the reasons behind attrition.
- **Retention Strategies**: Develop and test HR strategies based on the findings to increase employee retention.
- **AI/ML Enhancement**: Explore other machine learning algorithms, such as Random Forest or Neural Networks, to compare model performance.

---

## 🤝 Contributions

Contributions are highly welcome! If you have ideas to improve the analysis, add new features, or suggest new exploration techniques, please fork the repository and submit a pull request.

---

## 📧 Contact

For inquiries or collaboration opportunities, reach out via the [GitHub profile](https://github.com/garry864).

---

🎉 **Thank you for exploring this project! Let’s work together to improve HR practices and employee retention.**

