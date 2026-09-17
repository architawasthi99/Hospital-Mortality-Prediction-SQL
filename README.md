# 🏥 Hospital Mortality Analysis

<p align="center">
  <img src="https://media.istockphoto.com/id/1194838627/vector/patient-in-hospital.jpg?s=612x612&w=0&k=20&c=LqhY8qXr1IgGA0PjGLwqEyVJL-MBTFBU5rf3Dcg4DWo=" width="600">
</p>

<p align="center">
  <b>Exploring the factors associated with in-hospital mortality using SQL, Excel, and PowerBI.</b>
</p>

---

## 📌 Project Overview

Hospital mortality is influenced by a combination of demographic characteristics, existing medical conditions, physiological indicators, and the circumstances surrounding ICU admission.

This project analyzes a dataset of **10,000 hospitalized patients** to identify patterns and factors associated with in-hospital mortality. The analysis focuses on variables such as **age, ethnicity, gender, BMI, weight, heart rate, ICU admission source, ICU type, length of stay, and comorbidities**.

The project combines **Excel for data cleaning, MySQL for data analysis, and Tableau for data visualization** to transform raw healthcare data into meaningful insights.

> **Note:** This project focuses on exploratory data analysis and identifying associations in the dataset. The findings should not be interpreted as clinical predictions or medical recommendations.

---

## 🎯 Business Problem

Healthcare professionals need to understand which patient characteristics and hospital-related factors are associated with higher in-hospital mortality.

By identifying meaningful patterns in historical patient data, healthcare organizations can better understand:

- Which age groups have higher mortality rates?
- Which ICU admission sources are associated with more deaths?
- How do comorbidities relate to mortality?
- Does ICU length of stay differ between survivors and non-survivors?
- Are BMI, weight, and heart rate associated with patient outcomes?
- Which patient groups require closer attention from a data-analysis perspective?

The goal of this project is to use data to uncover these patterns and present them through an interactive dashboard.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Excel** | Data cleaning and preparation |
| **MySQL** | Data querying and exploratory analysis |
| **PowerBI** | Interactive dashboard and visualization |
| **SQL** | Aggregation, filtering, grouping, and analysis |

---

## 📂 Dataset

The dataset contains information about hospitalized ICU patients, including demographic, physiological, and clinical attributes.

🔗 **[Dataset Used](https://www.kaggle.com/datasets/mitishaagarwal/patient)**

---

## 🔗 Project Resources

- 💻 **[SQL Analysis](https://github.com/SharifAthar/Hospital-Mortality-Prediction-SQL/blob/main/Hospital_Mortality_SQL_Analysis.sql)**
- 📁 **[Dataset](https://www.kaggle.com/datasets/mitishaagarwal/patient)**

---

# 🔄 Project Workflow

```text
Raw Dataset
     ↓
Data Cleaning in Excel
     ↓
Import Data into MySQL
     ↓
Exploratory Data Analysis using SQL
     ↓
Identify Patterns & Trends
     ↓
Build Tableau Visualizations
     ↓
Interactive Hospital Mortality Dashboard
     ↓
Insights & Recommendations

🔍 Analysis Approach

The analysis was divided into several key areas:

1. Patient Demographics

I analyzed:

Age
Gender
Ethnicity
Weight
BMI

This helped identify demographic patterns among patients who survived and those who died during hospitalization.

2. ICU Analysis

The analysis explored:

ICU admission source
ICU type
ICU length of stay
Number of deaths and survivors
Average age of deceased patients
3. Comorbidity Analysis

The dataset included several comorbidities, including:

AIDS
Cirrhosis
Diabetes Mellitus
Hepatic Failure
Immunosuppression
Leukemia
Lymphoma
Solid Tumor with Metastasis

These were analyzed to understand their relationship with hospital mortality.

4. Physiological Indicators

I also examined:

BMI
Weight
Maximum heart rate
APACHE hospital death probability

These variables helped provide additional context around patient outcomes.

📊 Key Findings
1. Overall Hospital Mortality

Out of 10,000 admitted patients, 634 patients died, resulting in an overall mortality rate of 6.34%.

This provided the baseline for examining which patient and hospital characteristics were associated with mortality.

2. Age and Mortality

Age showed one of the clearest patterns in the analysis.

A large proportion of patients were between 50 and 89 years old, and mortality generally increased across the older age groups.

Patients aged 70 years and above experienced substantially higher mortality compared with many younger age groups.

This suggests that advanced age was an important factor associated with hospital mortality in this dataset.

3. ICU Admission Source

The Accident & Emergency department accounted for the largest number of ICU admissions and consequently had the highest absolute number of deaths.

However, looking at mortality as a percentage provides a different perspective.

The Floor admission source recorded a mortality rate of approximately 11.76% in the analysis, while "Other ICU" was excluded from some comparisons because of its very small sample size.

This highlights why both patient volume and mortality rate should be considered when analyzing healthcare data.

4. ICU Type

The analysis showed noticeable differences in mortality across ICU types.

The Med-Surg ICU represented a notable outlier in the number of deaths.

However, differences in ICU populations and patient severity should be considered when interpreting these results.

5. Weight, BMI & Heart Rate

Among patients who died:

Average Weight: 67.57 kg
Average BMI: 23.3
Average Maximum Heart Rate: 115.1 bpm

The average BMI was within the normal BMI range, suggesting that mortality was not simply concentrated among patients with high BMI.

The average maximum heart rate was also relatively high, providing an additional physiological variable worth investigating.

These observations describe patterns in the dataset and do not establish that BMI or heart rate directly caused mortality.

6. Comorbidities

The analysis examined eight major comorbidities.

Among the analyzed conditions, Diabetes Mellitus, Immunosuppression, and Solid Tumor with Metastasis showed comparatively high mortality percentages.

Diabetes had the highest observed mortality percentage at approximately 24.45%.

This highlights the importance of considering underlying medical conditions when studying hospital outcomes.

7. ICU Length of Stay

ICU length of stay was also compared between patients who survived and those who died.

Across several ICU types, patients who died generally had a higher average ICU length of stay than survivors.

Longer ICU stays may reflect greater illness severity and increased exposure to complications. However, length of stay should be interpreted as an associated factor rather than proof of causation.

📈 Tableau Dashboard

The analysis was transformed into an interactive Tableau dashboard to make the findings easier to explore.

Dashboard includes:
📊 Patient distribution by age
🏥 Deaths vs. survivors by ICU admission source
⚖️ BMI category distribution
⏱️ Average ICU length of stay
🩺 Comorbidity mortality rates
👥 Ethnicity-based mortality analysis
📋 Death percentage by age group
🏥 Deaths and average age by ICU type
📌 Overall hospital mortality statistics
Dashboard Preview
<p align="center"> <img src="https://i.ibb.co/SV4r1Rt/Screen-Shot-2023-06-29-at-4-52-19-PM.png" width="700"> </p>

🔗 View Interactive Tableau Dashboard

💡 Major Takeaways

Based on the exploratory analysis, several patterns stood out:

👴 Age

Older patients generally showed higher mortality percentages in the dataset.

🩺 Comorbidities

Certain underlying conditions, particularly diabetes, were associated with higher observed mortality percentages.

❤️ Heart Rate

Patients who died had an average maximum heart rate of 115.1 bpm, suggesting that physiological indicators may provide useful signals for further analysis.

🏥 ICU Stay

Longer ICU stays were generally associated with the non-survivor group across several ICU types.

🚑 ICU Admission

Accident & Emergency accounted for the largest number of admissions and deaths, while mortality percentages varied considerably across admission sources.

📌 Limitations

Although the dataset provides several useful insights, there are important limitations to consider.

The dataset does not capture every factor that may influence patient outcomes. For example, it does not provide a complete picture of:

Specific treatments received
Medication history
Detailed surgical interventions
Additional vital signs
Socioeconomic factors
Healthcare accessibility
Mental health and psychosocial factors
Patient preferences
Detailed clinical decision-making

Therefore, the relationships identified in this project should be considered observational associations within the dataset rather than causal relationships.

🚀 Future Improvements

Future versions of this project could be extended by:

🤖 Building a machine-learning mortality prediction model
📊 Adding more clinical variables
🧠 Comparing multiple ML classification algorithms
📈 Creating a real-time healthcare analytics dashboard
🔍 Performing feature importance analysis
⚕️ Incorporating treatment and medication information
🏥 Adding hospital-level comparisons
📉 Evaluating model performance using precision, recall, F1-score, and ROC-AUC

A future ML component could transform this project from an exploratory analytics project into an end-to-end healthcare analytics and prediction system.

🧠 Conclusion

This project demonstrates how healthcare data can be transformed into actionable analytical insights using Excel, SQL, and Tableau.

The analysis identified several important patterns associated with hospital mortality, particularly around age, comorbidities, ICU characteristics, physiological indicators, and length of stay.

Among these, age and certain comorbidities showed particularly noticeable differences in mortality across patient groups.

Most importantly, the project demonstrates an end-to-end data analytics workflow:

Data Cleaning → SQL Analysis → Visualization → Insights → Recommendations

👨‍💻 Author

Archit Awasthi

B.Tech — Computer Science & Engineering

Skills Demonstrated

SQL MySQL Excel Tableau Data Analysis Data Cleaning Data Visualization
