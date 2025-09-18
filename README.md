# Ladaki-Bahin-Yojna-MH-Kolhapur---Data-Analysis-
Data cleaning and analysis of "Ladaki Bahin Yojna beneficiary dataset (Kolhapur 2025)" using Python &amp; Excel.
##  Project Overview
This repository contains analysis of the **Ladaki Bahin Yojana data (Kolhapur, 2025)**.  
I originally worked as an **Anganwadi helper (freelance support)**, assisting workers with **data cleaning**.  
Later, I extended the dataset into a **practice and learning project**, where I added eligibility checks, duplicate detection, and visualizations.

---

##  Real-World Freelance Contribution
- Helped **Anganwadi workers** clean raw Excel data containing **mixed Marathi + English addresses**  
- Standardized **pincode** and **address fields** for reporting  
- Delivered a cleaned Excel dataset that could be used for their **official records**  

---

##  Practice & Learning Extension
For my **own learning as a data analyst**, I extended this project beyond the freelance cleaning task:  

-  Analyzed **applications by pincode**  
-  Visualized **age distribution of applicants**  
-  Implemented a **practice eligibility filter (60 years)**  
  *(Note: the official scheme uses 65 years; this adjustment was made only for practice)*  
-  Detected **family-wise duplicates** using surname + address  
-  Built visualizations using **Python (Pandas, Matplotlib, Seaborn)**  

---

##  Dataset
- **Source**: Raw application data provided to Anganwadi workers (anonymized for privacy)  
- **Format**: Excel (`.xlsx`)  
- **Size**: ~6170 rows, 10 columns  

---

## 🛠️ Tools & Libraries
- **Excel** → cleaning, sorting, filtering, pivot tables  
- **Python** →  
  - `pandas` for cleaning & manipulation  
  - `matplotlib` & `seaborn` for visualizations  

---

## 📊 Key Analysis & Sample Code

### 🔹 Applications by Pincode
```python
plt.figure(figsize=(10,6))
sns.countplot(y="Pincode", data=df, order=df["Pincode"].value_counts().index)
plt.title("Applications by Pincode")
plt.show()
