# 🚢 Titanic Dataset Exploratory Data Analysis (EDA)

This project presents a comprehensive Exploratory Data Analysis (EDA) of the Titanic dataset, uncovering patterns in passenger demographics, survival rates, and socioeconomic factors. Through visualizations, statistical tests, and interpretive insights, we explore what influenced survival aboard the ill-fated voyage.

---

## 📁 Dataset Overview
The dataset contains information on 891 passengers, including:
- **Demographics**: Age, Sex, Class
- **Travel Details**: Fare, Embarkation Port, Cabin
- **Outcome**: Survival status (0 = did not survive, 1 = survived)

---

## 📊 Key Findings

### 🎯 Survival Analysis
- **Overall Survival Rate**: Only 38% of passengers survived.
- **By Sex**: 74% of females survived vs. only 19% of males.
- **By Class**: 1st class had the highest survival rate (~63%), while 3rd class had the lowest (~24%).
- **By Fare**: Survivors paid significantly higher fares (mean ≈ ₹48.40) than non-survivors (mean ≈ ₹22.12).
- **By Age**: Survivors were slightly younger (mean ≈ 28.3) than non-survivors (mean ≈ 30.6).

### 📈 Demographic Insights
- **Age Distribution**: Most passengers were adults aged 20–40 (median age = 28).
- **Sex Distribution**: Males outnumbered females (577 vs. 314).
- **Class Distribution**: Majority traveled in 3rd class (491 passengers).

### 💰 Fare & Class Dynamics
- **Fare Distribution**: Highly right-skewed, with most passengers paying low fares and a few outliers paying premium prices.
- **Class vs Fare**: Strong negative correlation (-0.55), confirming that higher-paying passengers were in 1st class.
- **Class vs Age**: Moderate negative correlation (-0.37), suggesting older passengers tended to occupy higher classes.

---

## 🧪 Statistical Tests

| Test                        | Variable(s)           | Result Summary                                                                 |
|----------------------------|------------------------|--------------------------------------------------------------------------------|
| **Chi-Square Test**        | Sex vs Survival        | p ≈ 1.19 × 10⁻⁵⁸ → Strong association between gender and survival              |
| **T-Test**                 | Fare vs Survival       | p ≈ 6.12 × 10⁻¹⁵ → Survivors paid significantly more                          |
| **T-Test**                 | Age vs Survival        | p ≈ 0.039 → Survivors were slightly younger                                   |
| **Point-Biserial Corr.**  | Fare vs Survival       | r ≈ 0.257 → Moderate positive correlation                                     |
| **Point-Biserial Corr.**  | Age vs Survival        | r ≈ -0.077 → Weak negative correlation                                        |
| **Pearson/Spearman Corr.**| Age vs Fare            | Weak but significant positive correlation (Pearson r ≈ 0.096, Spearman r ≈ 0.135) |

---

## 📉 Visualizations Included
- Boxplots for age distribution and outliers
- Bar charts for passenger count by sex and class
- Scatterplot of Age vs Fare colored by survival
- Correlation heatmap of numerical features

---

## 📌 Conclusion
The analysis reveals that survival aboard the Titanic was heavily influenced by **gender**, **class**, and **fare**, with **age** playing a modest role. Wealthier, female, and younger passengers had significantly better odds of survival, reflecting both social norms and structural inequalities of the time.

---

## 🛠️ Next Steps
- Feature engineering (e.g., FamilySize, Title extraction)
- Handling missing data (Age, Cabin)
- Building predictive models (Logistic Regression, Random Forest)
