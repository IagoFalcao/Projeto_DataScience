# 📊 Social Media Impact on Teen Mental Health & Academic Performance

## 🧩 Problem Statement

This project investigates **when and under what conditions social media usage becomes harmful**, using a dataset of 1,200 teenagers.

The main objective is to explore whether social media usage has measurable effects on **mental health (stress, anxiety, depression)** and **academic performance**, and to understand if these effects emerge under specific behavioral or contextual conditions.

---

## 📁 Dataset Overview

- **Source:** Kaggle  
- **Size:** 1,200 teenagers  
- **Age Range:** 13–19 years old  

The dataset includes behavioral, lifestyle, and mental health indicators related to social media usage.

### 🔑 Key Features

- `age` – Age of the student  
- `gender` – Gender  
- `daily_social_media_hours` – Daily time spent on social media  
- `platform_usage` – Most used platform  
- `sleep_hours` – Daily sleep duration  
- `screen_time_before_sleep` – Device usage before bedtime  
- `academic_performance` – Academic score/performance  
- `physical_activity` – Daily exercise level  
- `social_interaction_level` – Real-life social interaction  
- `stress_level` – Stress level  
- `anxiety_level` – Anxiety level  
- `addiction_level` – Social media addiction level  
- `depression_label` – Depression indicator  

---

## 🔍 Exploratory Data Analysis (EDA)

The initial step focused on:

- Understanding data structure (`.info()`, `.describe()`)
- Checking for missing and duplicate values
- Visualizing categorical distributions (gender, platform usage)
- Analyzing behavioral patterns

### ✅ Key Findings

- No missing or duplicate values were found  
- Balanced categorical distributions  
- No obvious anomalies in data structure  

---

## 📈 Statistical Analysis

### 🧪 Hypothesis Testing (Pearson Correlation)

Several hypotheses were tested to evaluate linear relationships:

#### 1. Screen Time Before Sleep vs Sleep Hours
- ❌ No significant correlation  
- Fail to reject H₀  

#### 2. Social Media Usage vs Anxiety
- r ≈ 0.028 (negligible)  
- p-value > 0.05  
- ❌ No significant relationship  

#### 3. Social Media Usage vs Academic Performance
- r ≈ 0.013 (negligible)  
- ❌ No significant relationship  

#### 4. Academic Performance vs Anxiety
- Slight negative relationship observed  
- However, not linked to social media usage  

---

## 🔥 Correlation Matrix Insights

A full correlation matrix confirmed:

- Most variables have **coefficients close to zero**
- No strong linear relationships detected

### Notable (but weak) patterns:
- Depression vs Sleep → (-0.19)
- Depression vs Social Media Usage → (0.18)

---

## 📊 Grouped Analysis

### Stress Level by Social Interaction & Gender

- Uniform distribution across all groups  
- Median stress = 5 for all categories  
- Identical variance across segments  

👉 Suggests **no influence of gender or social interaction on stress levels**

---

## 🔍 Deep Analysis

Although no **linear relationships** were found, this does **not** imply absence of impact.

Instead, it suggests:

- 📌 Effects may be **non-linear**
- 📌 Impact may depend on **combined behavioral factors**

### Central Question:
> *Under what conditions does social media become harmful?*

---

## 🤖 Machine Learning Approach

### Model: Random Forest Regressor

Two prediction tasks were performed:

---

### 📘 1. Predicting Academic Performance

- Features: All variables except target  
- Result: ❌ Negative R²  

👉 Model performs worse than baseline → no predictive power

---

### 📱 2. Predicting Addiction Level

- Same approach  
- Result: ❌ Negative R²  

👉 Again, no meaningful patterns detected

---

### 📊 Feature Importance

- No feature showed strong predictive influence  
- Importance distribution was relatively flat  

---

## ⚠️ Key Insight

The dataset shows:

- Lack of correlation  
- Lack of predictive patterns  
- Uniform distributions  

### 🚨 Interpretation:

This strongly suggests that:

- The dataset may contain **synthetic or randomly generated data**, OR  
- There are **methodological issues in data collection**

---

## 📌 Conclusion

This project successfully applied:

- Descriptive Statistics  
- Hypothesis Testing  
- Correlation Analysis  
- Machine Learning (Random Forest)  

Even though no significant relationships were found, this is a **valid and important result in Data Science**.

> Proving the absence of patterns is just as valuable as finding them.

---

## 🚀 Next Steps

Future improvements may include:

- Applying **unsupervised learning (K-Means)** for clustering  
- Testing **non-linear models more deeply**
- Using a **more reliable and real-world dataset**
- Feature engineering (interaction terms, transformations)

---

## 🛠️ Tech Stack

- Python  
- Pandas  
- NumPy  
- Matplotlib / Seaborn  
- SciPy  
- Scikit-learn  

---

## 🎯 Learning Outcomes

- Practical understanding of correlation vs causation  
- Hands-on experience with hypothesis testing  
- Model evaluation using R²  
- Identifying limitations of datasets  
- Thinking critically about data quality  

---

## 📎 Author

Developed as a hands-on Data Science project focused on applying statistical reasoning and machine learning techniques in a real-world context.
