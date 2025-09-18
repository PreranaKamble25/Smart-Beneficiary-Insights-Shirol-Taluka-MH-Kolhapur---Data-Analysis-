# Ladaki-Bahin-Yojna-MH-Kolhapur---Data-Analysis-
Data cleaning and analysis of "Ladaki Bahin Yojna beneficiary dataset (Kolhapur 2025)" using Python &amp; Excel.
##  Project Overview
This repository contains analysis of the **Ladaki Bahin Yojana data (Kolhapur, 2025)**.  
I originally worked as an **Anganwadi helper (freelance support)**, assisting workers with **data cleaning**.  
Later, I extended the dataset into a **practice and learning project**, where I added eligibility checks, duplicate detection, and visualizations.

##  Real-World Freelance Contribution
- Helped **Anganwadi workers** clean raw Excel data containing **mixed Marathi + English addresses**  
- Standardized **pincode** and **address fields** for reporting  
- Delivered a cleaned Excel dataset that could be used for their **official records**  

##  Practice & Learning Extension
For my **own learning as a data analyst**, I extended this project beyond the freelance cleaning task:  

-  Analyzed **applications by pincode**  
-  Visualized **age distribution of applicants**  
-  Implemented a **practice eligibility filter (60 years)**  
  *(Note: the official scheme uses 65 years; this adjustment was made only for practice)*  
-  Detected **family-wise duplicates** using surname + address  
-  Built visualizations using **Python (Pandas, Matplotlib, Seaborn)**  
   **Note:** This project is for **learning purposes only** and is **not an official government report**.  
---
### Eligibility Column Creation  
To simulate government eligibility checks, I created an **`Eligibility` column** in the dataset using Python:  
- Applicants **≥ 60 years** → Marked as **Eligible**  
- Applicants **< 60 years** → Marked as **Not Eligible**  

The updated dataset was then **exported to Excel** for further use:  

python
## Create Eligibility column
df['Eligibility'] = df['Age'].apply(lambda x: 'Eligible' if x >= 60 else 'Not Eligible')]  ```


##  Dataset
- **Source**: Raw application data provided to Anganwadi workers (anonymized for privacy)  
- **Format**: Excel (`.xlsx`)  
- **Size**: ~6170 rows, 10 columns  

---

##  Tools & Libraries
- **Excel** → cleaning, sorting, filtering, pivot tables  
- **Python** →  
  - `pandas` for cleaning & manipulation  
  - `matplotlib` & `seaborn` for visualizations  

---

## Key Insights
-Majority of applicants are in the 35–50 years age group.

-Median applicant age ~40 years.

-Youngest applicant ~18 years, oldest ~65 years.

-Pincodes with lower average age show higher eligibility rates.

-Some duplicate household entries exist (same surname + address).

-Eligibility filter (set at 60 years for practice) reduces a large share of applicants.
