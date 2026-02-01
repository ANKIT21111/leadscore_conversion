# 🎯 Lead Scoring Case Study: X Education

[![Python 3.x](https://img.shields.io/badge/python-3.x-blue.svg)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/machine--learning-scikit--learn-orange.svg)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/data--processing-pandas-ff69b4.svg)](https://pandas.pydata.org/)

## 📝 Project Overview
**X Education** is an education company that sells online courses to industry professionals. While they generate many leads, their conversion rate is relatively low. To improve efficiency, the company wants to identify the "Hot Leads"—those most likely to convert into paying customers.

This project involves building a **Logistic Regression** model to assign a **Lead Score** (0 to 100) to each lead. A higher score indicates a higher probability of conversion, allowing the sales team to focus their efforts effectively.

### 🚀 Business Goal
The CEO has set a target lead conversion rate of **80%**. The model must be flexible enough to handle changing business requirements in the future.

---

## 📊 Dataset Insights
The dataset contains approximately **9,000 leads** with various attributes such as:
- **Lead Origin/Source**: Where the lead came from (API, Landing Page, Google, etc.).
- **Engagement Metrics**: Total visits, time spent on the website, page views per visit.
- **Demographics**: Occupation, Specialization, City.
- **Activity**: Last activity, last notable activity.
- **Target Variable**: `Converted` (1 if converted, 0 otherwise).

---

## 🛠️ Methodology & Tech Stack

### 💻 Technologies Used
- **Language**: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, Statsmodels
- **Visualization**: Matplotlib, Seaborn

### 🔄 Pipeline Steps
1.  **Data Cleaning**: Handled missing values, treated 'Select' (default nulls), and filtered out low-frequency categories.
2.  **Exploratory Data Analysis (EDA)**: Analyzed conversion rates across different features to identify key drivers.
3.  **Feature Engineering**: Created dummy variables for categorical features and scaled numerical variables.
4.  **Model Building**: Built a Logistic Regression model using `Statsmodels` for detailed analysis and `Scikit-learn` for final implementation.
5.  **Model Evaluation**: Optimized the probability cutoff using **ROC Curves** and evaluated performance using:
    - Accuracy
    - Sensitivity & Specificity
    - Precision & Recall

---

## 📈 Key Results
- **Model Performance**: The final model successfully identifies leads with high conversion potential.
- **Conversion Target**: By targeting leads with a score above the optimized threshold, the company can move closer to its **80% conversion goal**.
- **Insights**: Features like "Time Spent on Website", "Lead Source (Welingak Website)", and "Last Activity (SMS Sent)" were found to be strong predictors of conversion.

---

## 📂 Project Structure
```text
├── Leads.csv                        # Raw dataset
├── Leads Data Dictionary.xlsx       # Column descriptions
├── Assignment Subjective Questions.docx # In-depth analysis & business questions
├── README.md                        # Project documentation
└── [Workings/Notebooks]             # Jupyter notebooks (if applicable)
```

---

## ⚙️ How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/[your-username]/leadscore-conversion.git
   ```
2. Install dependencies:
   ```bash
   pip install pandas numpy scikit-learn seaborn matplotlib statsmodels
   ```
3. Run the Jupyter Notebook or analysis script.

---

## 🤝 Contributing
Contributions are welcome! Feel free to open issues or submit pull requests to improve the model or documentation.

---

⭐ *If you find this project useful, please consider giving it a star!*
