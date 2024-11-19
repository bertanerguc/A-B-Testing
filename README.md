# 🌟 A/B Testing for Bidding Methods

This project analyzes the results of an A/B test comparing **Maximum Bidding** and **Average Bidding** methods to determine which generates higher **purchase conversions**.

---

## 🚀 Project Overview

### 📝 Problem Statement
Facebook recently introduced a new bidding method called **Average Bidding**, which is being tested against the existing **Maximum Bidding**. A client, **bombabomba.com**, conducted an A/B test over one month to evaluate the effectiveness of the new method in increasing purchases.

The ultimate success metric is **Purchase**, and this project focuses on analyzing the A/B test results and providing actionable insights.

---

## 📂 Dataset Description

The dataset consists of two groups:
- **Control Group**: Used the Maximum Bidding method.
- **Test Group**: Used the Average Bidding method.

| Feature      | Description                                      |
|--------------|--------------------------------------------------|
| `Impression` | Number of times the ad was shown                |
| `Click`      | Number of clicks on the displayed ad            |
| `Purchase`   | Number of products purchased after clicking ads |
| `Earning`    | Revenue generated from purchased products       |

---

## 🔧 Key Features

### 🛠 Tasks

1. **Data Preparation**:
   - Load and inspect data for control and test groups.
   - Merge the datasets for analysis.
2. **Define Hypothesis**:
   - Null Hypothesis (H₀): No difference in average purchases between the groups.
   - Alternative Hypothesis (H₁): A difference exists in average purchases.
3. **Perform Statistical Tests**:
   - Test assumptions of normality and variance homogeneity.
   - Conduct an appropriate statistical test based on assumptions.
4. **Interpret Results**:
   - Evaluate statistical significance and provide actionable recommendations.

---

## 📈 Project Workflow

### 1️⃣ Data Understanding and Preparation
- Load control and test group data from an Excel file.
- Inspect data for missing values and outliers.
- Merge datasets for comparative analysis.

### 2️⃣ Hypothesis Definition
- **H₀**: Average purchases for the two groups are equal.  
- **H₁**: Average purchases for the two groups are not equal.  

### 3️⃣ Statistical Testing
- Perform **normality tests** using the Shapiro-Wilk test.
- Check **variance homogeneity** using Levene’s test.
- Conduct an **Independent Two-Sample T-Test** if assumptions are met.

### 4️⃣ Results Interpretation
- Analyze p-values to determine whether to reject or fail to reject the null hypothesis.
- Provide recommendations based on test results.

---

## 📊 Results

### 🎯 Key Findings

| Metric                  | Control Group | Test Group |
|-------------------------|---------------|------------|
| **Mean Purchase**       | 550.89       | 582.11     |
| **p-value (T-Test)**    | 0.3493       |            |

- **Conclusion**: The p-value (0.3493) indicates no statistically significant difference in average purchases between the two groups.

### 🛠 Recommendations
- Based on the analysis, there is no evidence to suggest that Average Bidding performs better than Maximum Bidding.  
- Further testing or other metrics (e.g., cost per acquisition) could be evaluated to make a more informed decision.

---

## 🛠 Tools and Libraries

- **Python**  
- **Pandas**  
- **NumPy**  
- **Matplotlib**  
- **SciPy**  

---

## 🌟 Contribution

Contributions are welcome!  
Feel free to fork this repository, create issues, or submit pull requests for improvements.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---
