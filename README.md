## Prodigy Infotech-Ds-Task-2
# 🛳️ Titanic Data Survival Analysis

<p align="center">
  <img src="https://github.com/ProgrammerAk55/Prodigy-Ds-Task-2/blob/main/Task-2.png" alt="Task 1 Banner" width="600" />
</p>

---

## 📌 Overview

This project performs an in-depth **Exploratory Data Analysis (EDA)** on the legendary **Titanic dataset** from Kaggle’s survival prediction challenge.  
It reveals patterns behind **who survived and why**, exploring the social, economic, and demographic dynamics aboard — a timeless case study in **data-driven human behavior**.

---

## 📥 Dataset & Sources

**Files used**
- [Train.csv(https://raw.githubusercontent.com/ProgrammerAk55/Prodigy-Ds-Task-2/refs/heads/main/Train.csv)]
- [Test.csv(https://raw.githubusercontent.com/ProgrammerAk55/Prodigy-Ds-Task-2/refs/heads/main/Test.csv)]
- [Gender_submission.csv(https://raw.githubusercontent.com/ProgrammerAk55/Prodigy-Ds-Task-2/refs/heads/main/Gender-submission.csv)]

All datasets were merged into one unified DataFrame for seamless exploration.

---

## ⚙️ Data Preparation

- Inspected dataset using `.shape`, `.info()`, `.describe()`
- Detected and imputed missing values:
  - **Categorical (mode):** `Cabin`, `Embarked`, `Survived`
  - **Numerical (mean):** `Age`, `Fare`
- Engineered new features:
  - `Family_size = SibSp + Parch + 1`
  - `AgeGroup` (binned age ranges)
  - `Family_type` (Alone / Small / Large)

✅ **Result:** Clean dataset with no missing values

---

## 🔍 Exploratory Insights & Key Findings

**1️⃣ Gender & Survival**
| Sex    | Survivors | % Survived |
| ------ | ---------- | ---------- |
| Male   | 109        | 19.0%      |
| Female | 316        | 72.7%      |

**2️⃣ Passenger Class (Pclass)**
- Survival rates decreased with class → **1st > 2nd > 3rd**  
- Male passengers in 3rd class had the lowest survival odds.

**3️⃣ Age & Survival**
- **Children and teens** had higher survival.
- **Seniors** faced minimal chances.

**4️⃣ Family Impact**
- **Small families (2–4)** had the highest survival.
- **Solo or large families** had the least.

**5️⃣ Ticket & Embarkation**
- Most sold ticket: `CA.2343` → *0 survivors*  
- Passengers from **Cherbourg (C)** had the highest survival, especially women.

---

<details>
<summary>📊 Click to view all Visualizations (Plotly)</summary>

1. Sex Distribution  
2. Age Distribution by Survival  
3. Survival Count by Age Group  
4. Age Distribution by Pclass  
5. Family Size vs Survival  
6. Survival by Siblings/Spouses (SibSp)  
7. Survival by Family Type  
8. Sex Distribution by Most Sold Ticket  
9. Embarked × Survival × Sex  

</details>

---

## 🎯 Conclusions

| Factor          | Impact          | Insight                               |
| ---------------- | --------------- | ------------------------------------- |
| **Sex**         | 🔥 High          | Females 3.8× more likely to survive   |
| **Pclass**      | 🔥 High          | Wealthier passengers fared better     |
| **Age**         | ⚡ Moderate       | Younger = higher odds                 |
| **Family Size** | ⚡ Moderate       | Small families had best outcomes      |
| **Embarked**    | ⚠️ Low/Moderate  | Cherbourg passengers had advantage    |

💡 *Survival wasn’t random — it mirrored social hierarchy, gender norms, and access to resources.*

---

## 🧠 Tools & Libraries Used

- **Python** (Jupyter / Google Colab)
- **Matplotlib**
- **Pandas** – data manipulation  
- **Plotly Express** – interactive visualization 
- **Seaborn**
  
---

## ▶️ How to Reproduce

1. Open `Task2.ipynb` in **Colab** or **Jupyter**.  
2. Upload the dataset files.  
3. Run all notebook cells to generate the same analysis and visuals.

---

## 🚀 Next Steps

- Build **predictive ML models** for survival forecasting.  
- Integrate **“What-If” simulators** for counterfactual exploration.

---

## 🏁 Acknowledgement

- Dataset: [Kaggle Titanic Challenge](https://www.kaggle.com/c/titanic)  
- Project developed under **Prodigy InfoTech Data Science Internship – Task 2 (PRODIGY_DS_02)**

---

> 💬 *“Data reveals not just what happened — but why it mattered.”*


