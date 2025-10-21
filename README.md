# 👩‍👧 Data-Driven Insights for Women & Child Development – Shirol Taluka, Kolhapur

## 📖 Project Overview

This project originates from a real-world freelance assignment for the **Department of Women and Child Development**, Shirol Taluka, District Kolhapur (Maharashtra).
The department needed assistance in **cleaning and organizing beneficiary records** collected from nearby Anganwadi centers.

The raw dataset contained **mixed Marathi and English text**, multiple inconsistencies, and unsorted regional data.
After completing the cleaning task, I extended the dataset into a **personal data analytics project**, adding an **Eligibility feature** and developing **interactive visualizations** and an **AI-generated dashboard** to demonstrate insights and analytical thinking.

---

## 🎯 Objectives

* Clean and standardize a real government dataset containing regional beneficiary details.
* Sort data **pincode-wise** and **address-wise** to improve readability and accessibility.
* Handle **bilingual entries** (Marathi + English) effectively.
* Create a new **Eligibility** column based on age criteria using Python.
* Visualize data trends and summary insights through graphs and dashboards.

---

## 🧰 Tools & Technologies Used

| Category      | Tools / Libraries             |
| ------------- | ----------------------------- |
| Data Cleaning | Python (Pandas, NumPy)        |
| Visualization | Matplotlib, Seaborn, Power BI |
| AI Dashboard  | MetricDash AI                 |
| File Handling | Excel, CSV                    |
| Environment   | Jupyter Notebook              |

---

## 🧹 Data Cleaning & Preparation Steps

1. **Loaded raw CSV file** using Pandas.
2. **Removed duplicates** and corrected null/missing values.
3. **Standardized text encoding** for bilingual (Marathi + English) fields.
4. **Sorted data** by pincode and address for region-specific reporting.
5. **Cleaned inconsistent date formats** and verified age entries
   

## 🧮 Feature Engineering – Eligibility Logic

After cleaning, a new **Eligibility** column was created to classify beneficiaries based on age.

```python
df = pd.read_excel(r"C:\Users\Prerana\OneDrive\Desktop\LadakiBahin\Shirol_with_Age.xlsx")

# Eligibility column (Age between 21 and 60 is Eligible)
df['Eligibility'] = df['Age'].apply(lambda x: 'Eligible' if 21 <= x <= 60 else 'Not Eligible')

# Check result
print(df[['Age', 'Eligibility']].head(10))
```

This helped in identifying beneficiaries meeting specific criteria (e.g., adult education, welfare benefits).

---

## 📊 Visualizations & Dashboard Insights

I used **Python**, **Power BI**, and **AI (MetricDash)** to visualize trends and insights.

### 📈 Key Visual Insights

* **Pincode-wise Beneficiary Distribution**
* **Age-wise Eligibility Breakdown**
* **Marathi vs. English Entries Count**
* **Total Records and Eligibility Ratio**

🔗 **AI Dashboard Demo**:  https://preranakamble25.github.io/Smart-Beneficiary-Insights-Shirol-Taluka-MH-Kolhapur---Data-Analysis-/

## 🧠 Key Learnings

* Worked with **real bilingual data** (Marathi + English) for a government dataset.
* Improved dataset accuracy and readability through **data cleaning automation**.
* Developed **analytical problem-solving** by creating custom eligibility criteria.
* Enhanced presentation through **AI-driven dashboard visualization**.

---

## 🏁 Final Outcome

✅ Cleaned and standardized dataset ready for official reporting.

✅ Age-based Eligibility column added using Python logic.

✅ Interactive dashboard showing key regional insights.

## 🧾 Author

**👩‍💻 Prerana Kamble**

Data Analyst | Python | SQL | Power BI

📍 Kolhapur, Maharashtra, India

 [LinkedIn](www.linkedin.com/in/prerana-kamble-234058239)
