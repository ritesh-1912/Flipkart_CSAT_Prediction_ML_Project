# Flipkart Customer Satisfaction Analysis (Machine Learning Capstone)

## 📌 Project Overview
This project focuses on the e-commerce domain, specifically analyzing customer interactions and feedback for **Flipkart**. In the competitive online retail space, customer satisfaction (CSAT) is a primary driver of growth and loyalty.

The core objective of this project is to analyze customer support data to identify key drivers of satisfaction and build a **Machine Learning Classification model** capable of predicting CSAT scores. These insights aim to help optimize agent performance, streamline support channels, and improve overall service quality.

## 🚀 Business Objective
To maintain a competitive edge, the project addresses the following key business questions:
* **Performance Variability:** How do different agents, managers, and shifts perform regarding CSAT?
* **Channel Effectiveness:** Which support channels (Call vs. Chat) yield higher satisfaction?
* **Time Sensitivity:** What is the correlation between "Connected Handling Time" and customer happiness?
* **Sentiment Drivers:** Which interaction categories lead to positive or negative outcomes?

## 📂 Dataset Description
The analysis utilizes a dataset (`Customer_support_data.csv`) capturing details of customer interactions, including:
* **Interaction Details:** Channel name, Category, Sub-category.
* **Customer Feedback:** Remarks and CSAT Score (Target Variable).
* **Agent Data:** Agent Name, Supervisor, Manager, Tenure Bucket, Shift.
* **Order & Product Data:** Order timestamps, Product category, Item price.

## 🛠️ Tech Stack & Libraries
The project is implemented in **Python** using the following libraries:
* **Data Manipulation:** `pandas`, `numpy`
* **Visualization:** `matplotlib`, `seaborn`
* **Machine Learning:** `scikit-learn`
    * *Models:* Logistic Regression, Random Forest Classifier
    * *Preprocessing:* LabelEncoder, StandardScaler
    * *Model Selection:* train_test_split, cross_val_score
    * *Metrics:* accuracy_score, classification_report, confusion_matrix

## 📊 Project Workflow
1.  **Data Loading & Understanding:** Importing the dataset and inspecting structure (rows, columns, data types).
2.  **Exploratory Data Analysis (EDA):**
    * Univariate analysis of CSAT scores and agent shifts.
    * Bivariate analysis to find correlations between handling time and satisfaction.
    * Visualizing missing values and data distribution.
3.  **Data Cleaning & Preprocessing:**
    * Handling missing values (imputation for `Item_price`, `Connected_handling_time`, etc.).
    * Encoding categorical variables (Label Encoding).
    * Feature Scaling.
4.  **Model Building:**
    * Splitting data into Training and Testing sets.
    * Training baseline models (Logistic Regression).
    * Training ensemble models (Random Forest).
5.  **Evaluation:**
    * Assessing performance using Accuracy, Precision, Recall, and F1-Score.
    * Hyperparameter tuning for model optimization.

## 📈 Key Insights & Results
* **Channel Performance:** Identified specific channels that consistently outperform others in resolving queries.
* **Handling Time:** Analysis revealed the "sweet spot" for interaction duration that maximizes CSAT.
* **Agent Training:** Highlighted performance gaps in specific tenure buckets (e.g., 'On Job Training' vs. '>90 Days'), suggesting targeted training needs.

## 🔮 Future Scope
* **Advanced Modeling:** Experimenting with XGBoost or LightGBM for improved accuracy.
* **NLP Analysis:** Implementing Sentiment Analysis on the "Customer Remarks" text column to extract deeper qualitative insights.
* **Deployment:** creating a Streamlit or Flask API to serve the model for real-time CSAT prediction.

## 📝 How to Run
1.  Clone the repository:
    ```bash
    git clone [https://github.com/yourusername/flipkart-csat-analysis.git](https://github.com/yourusername/flipkart-csat-analysis.git)
    ```
2.  Install dependencies:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
3.  Run the Jupyter Notebook:
    ```bash
    jupyter notebook Flipkart_Project_Innovexis.ipynb
    ```

## 🤝 Contribution
This project was developed as an individual Machine Learning Capstone Project. Contributions and feedback are welcome!
