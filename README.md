# 📊 Student Stress Analysis Using Python: EDA & Insights  

<img width="275" height="183" alt="image" src="https://github.com/user-attachments/assets/af48c29a-cdf0-4dbb-af3c-441940360b21" />

## 📌 Project Overview  
Stress is a common challenge among students, often driven by academic workload, personal responsibilities, and lifestyle factors. While stress can be harmful when unmanaged, it can also act as a motivating force that pushes students to achieve their goals.  

This project explores a dataset of student stress responses to uncover patterns across **age, gender, and stress types**. Using Python for **data cleaning, exploratory data analysis (EDA), and visualization**, the study aims to:  

- Identify the dominant age ranges represented in the dataset.  
- Understand how different groups (Teens, Young Adults, Adults, Older Adults) experience stress.  
- Examine the balance between **Positive Stress**, **Negative Stress**, and **No Stress** among students.  
- Investigate correlations between key stress factors such as **workload, sleep, and anxiety**.  

By analyzing these patterns, the project provides insights into how academic institutions and educators can better support students, while also highlighting the limitations of the dataset (e.g., imbalance toward positive stress).  

Ultimately, this analysis is a step toward understanding the complexity of student stress and promoting healthier learning environments.  


The project was carried out in **3 phases**:  
1. **Data Cleaning & Preparation**  
2. **Exploratory Data Analysis (EDA)**  
3. **Insights & Interpretation**  

---

## 📂 Dataset  
- **File:** `Stress_Dataset.csv`  
- **Size:** ~840 student records  
- **Key Features:**  
  - `Age` → numerical (student age)  
  - `Gender` → categorical (Male/Female)  
  - `Stress Type` → categorical (Positive, Negative, No Stress)  
  - Other factors → workload, sleep, anxiety, etc.  

---

## ⚙️ Phase 1: Data Cleaning & Preparation  
- Removed outliers (e.g., invalid ages like `100`).  
- Created **Age Groups**: Teen, Young Adult, Adult, Older Adult.  
- Encoded categorical variables (`Gender`, `Stress Type`).  
- Verified missing values and ensured dataset consistency.  

---

## 🔎 Phase 2 – Exploratory Data Analysis (EDA)

The goal of this phase was to uncover hidden trends and patterns in the student stress dataset. Multiple exploratory techniques were applied using **Pandas, Matplotlib, and Seaborn** to understand distributions, group behaviors, and factor relationships.  

### 1️⃣ Univariate Analysis  
- **Age Distribution:**  
  - Most students fall within **18–21 years**.  
  - Very few students are below 16 or above 25.  
  - Outliers (like age = 100) were removed.  

- **Gender Distribution:**  
  - The dataset is almost evenly split between **male** and **female** students.  
  - Gender encoding was performed for analysis (Male=0, Female=1).  

- **Stress Type Distribution:**  
  - **Positive Stress** dominates, accounting for more than 80% of responses.  
  - Very few records show **Negative Stress** or **No Stress**.  

---

### 2️⃣ Bivariate Analysis  
- **Age vs Stress Type:**  
  - **Young Adults** (18–25) overwhelmingly report Positive Stress (>600 students).  
  - Teens (15–17) also report Positive Stress but at lower counts (~120–140).  
  - Adults and Older Adults have almost no representation.  

- **Gender vs Stress Type:**  
  - Both males and females lean toward **Positive Stress**, though females show slightly higher stress in academic-related factors.  

---

### 3️⃣ Correlation Analysis  
A **heatmap** was generated to check how different numerical factors interact.  

- Strong associations were noticed between:  
  - **Workload and Anxiety** → suggesting heavy workload increases stress levels.  
  - **Sleep Duration and Stress** → students with reduced sleep tended to report higher stress.  
- Weak or negligible correlation between gender and stress type.

  <img width="1150" height="514" alt="image" src="https://github.com/user-attachments/assets/999643bf-bc23-43c0-9e3e-faeb23f699cb" />


---

### Key Observations from Phase 2  
1. The dataset is **imbalanced** toward Positive Stress.  
2. **Young Adults** form the core of the dataset, making it primarily representative of undergraduates.  
3. Gender differences exist but are subtle; academic workload seems to impact both groups.  
4. Lifestyle factors like **sleep and workload** are central to stress patterns.  


## 🔑 Phase 3: Insights & Interpretation  

1. **Demographics**  
   - The dataset mainly represents **undergraduate students (18–21)**.  
   - Teens form a smaller segment; Adults and Older Adults are almost absent.  

2. **Stress Profile**  
   - Students overwhelmingly report **Positive Stress** (goal-oriented/motivational).  
   - Negative/No Stress are underrepresented → dataset is imbalanced.  

3. **Gender Differences**  
   - Female students report slightly higher levels of stress compared to males.  

4. **Stress Factors**  
   - Workload, lack of sleep, and anxiety are **strongly correlated**, showing that academic pressure often manifests in multiple ways.  

5. **Key Takeaway**  
   - The dataset reflects a population of mostly **young students experiencing positive stress**.  
   - However, the lack of balance across stress types limits the ability to study negative stress in depth.  

---

## 📌 Conclusion & Recommendations  
- **Conclusion:** Most students experience **positive academic stress**, especially Young Adults.

  
- **Recommendation:**  
  - Future studies should collect **balanced datasets** that capture negative stress.  
  - Universities should focus on **stress management programs**, targeting workload, sleep, and mental health.  

---



## 🛠️ Tools & Libraries  
- Python (Pandas, NumPy)  
- Matplotlib & Seaborn (Visualizations)  
- Jupyter Notebook  

---
