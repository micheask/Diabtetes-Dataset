# Diabtetes-ETL Pipeline-Dataset
ETL pipeline analyzing diabetes patient records and CDC state-level prevalence data.  Created by Michas Kidane and Amon Bayu

Datasets
Source	Type	Records	Description
Mendeley Multiclass Diabetes Dataset	CSV	260+	Patient-level clinical markers (HbA1c, BMI, cholesterol, etc.) from Iraqi Medical City Hospital
CDC Diabetes State Burden Toolkit	REST API	500	State-level diabetes prevalence and incidence rates (post-2000)


Table 1: patient_records Gender, AGE, Urea, Cr, HbA1c, Chol, TG, HDL, LDL, VLDL, BMI, Class

Table 2: cdc_burden year, location, long_text_indicator, stratification_group1, data_value, lower_confidence_limit, upper_confidence_limit

Key Findings
HbA1c is the strongest diabetes classifier — averages of 4.58 (No Diabetes), 6.01 (Pre-Diabetic), and 8.84 (Diabetic)
BMI increases with diabetes classification
Gender bias present: males overrepresented in diabetic cases (79/128), females in non-diabetic (58/96)
Datasets were kept as separate tables — no shared key exists for merging
