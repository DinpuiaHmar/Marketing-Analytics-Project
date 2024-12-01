# Marketing-Analytics-Project

---

#### **Project Title:**  
**Marketing Dataset Project**  
**Group 8 Members:**  
LaldinPuia Hmar, Isha, Kushal Shahi, Shruti, Adarsh Tiwari  

---

#### **Purpose:**  
This project analyzes a marketing dataset containing customer-level data to identify patterns, predict behaviors, and provide actionable insights for enhanced marketing strategies.  

---

### **Contents**  
1. [Introduction](#introduction)  
2. [Dataset Overview](#dataset-overview)  
3. [Methodology](#methodology)  
4. [Findings](#findings)  
5. [Recommendations](#recommendations)  
6. [Limitations](#limitations)  
7. [Future Directions](#future-directions)  

---

### **Introduction**  
The project leverages AI and data analytics techniques to analyze customer demographic, behavioral, and transactional data. Clustering, regression, and classification models were implemented to understand customer segments and provide actionable marketing recommendations.  

---

### **Dataset Overview**  

- **Dataset Information:**  
  - Customer profiles: 10,000 individuals  
  - Variables: Age (18–70 years), Gender, Income, Spending Score (1–100), Preferred Shopping Channel (Online, In-Store, Both), etc.  

- **Preliminary Observations:**  
  - Positive correlation between income and spending score.  
  - Males tend to shop more, have higher satisfaction, and return more products.  
  - High correlation between spending score and online shopping frequency.  

---

### **Methodology**  

#### **Data Preprocessing:**  
- Checked for null values: None found.  
- Removed duplicates: No duplicates were present.  
- Outlier detection: Addressed using IQR and box plots.  
- Scaled data: MinMax Scaler was applied.  
- Categorical variables: Encoded using LabelEncoder and OneHotEncoder.  

#### **Models Implemented:**  
1. **KMeans Clustering:**  
   - Clustered customers into 4 segments based on income, spending score, and online shopping frequency.  
   - Marketing strategies were tailored for each cluster.  

2. **ANOVA Analysis:**  
   - Tested if spending scores differed by shopping channels (Online, In-Store, Both).  

3. **Regression Analysis:**  
   - Identified income and online shopping frequency as significant predictors of spending score.  

4. **Classification Models:**  
   - Logistic Regression, KNN, Naive Bayes, and CART were implemented to predict loyalty program membership.  

---

### **Findings**  

#### **KMeans Clustering:**  
- Cluster 0: High-income & high-spending → Luxury products.  
- Cluster 1: Low-income & high online shopping frequency → Affordable items.  
- Cluster 2: Low-income & low-spending → Minimal marketing focus.  
- Cluster 3: High-income & low online shopping → Campaigns to influence spending.  

#### **Regression Analysis:**  
- Spending Score increases with income (0.2609 units per increase).  
- Online Shopping Frequency significantly predicts spending score (0.6706 units per increase).  

#### **ANOVA Analysis:**  
- Spending scores are equal across shopping channels, suggesting uniform marketing campaigns.  

---

### **Recommendations**  

1. **Customer Segmentation:**  
   - Focus on high-income, high-spending customers with luxury products.  
   - Target low-income, high online shoppers with promotions and affordable pricing.  

2. **Omnichannel Strategies:**  
   - Promote cross-channel experiences like "shop online, pick up in-store."  
   - Ensure consistent offers across channels.  

3. **Data-Driven Marketing:**  
   - Prioritize marketing resources on high-income, frequent online shoppers.  
   - Deprioritize segments with low spending potential.  

4. **Loyalty Program:**  
   - Address barriers for frequent online shoppers to increase loyalty adoption.  

---

### **Limitations**  

1. **Model Accuracy Issues:**  
   - Poor performance in predicting loyalty program membership.  
   - Naive Bayes model highly biased toward non-members.  

2. **Data Quality Concerns:**  
   - Existing data may lack sufficient granularity or detail.  

3. **Hyperparameter Optimization:**  
   - Limited improvements despite GridSearchCV tuning.  

---

### **Future Directions**  

- Acquire higher-quality, detailed datasets for improved modeling performance.  
- Experiment with advanced algorithms like deep learning for loyalty prediction.  
- Incorporate external data sources (e.g., economic indicators, customer reviews) for richer insights.  

---

### **How to Use This Repository**  

1. **Preprocessing Script:**  
   - Load and preprocess the dataset using `data_preprocessing.py`.  

2. **Clustering:**  
   - Run `kmeans_clustering.py` to generate customer segments.  

3. **ANOVA & Regression:**  
   - Use `analysis.py` for statistical testing and regression insights.  

4. **Classification Models:**  
   - Run `classification_models.py` to predict loyalty membership.  

---

### **Contact Information**  

For queries or contributions, reach out to:  
**Group Lead:** LaldinPuia Hmar  
**Email:** laldinpuia.hmar_asp25@ashoka.edu.in  

---  
