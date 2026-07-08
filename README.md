# Synthetic Healthcare Patient Dataset Analysis

## Project Overview

This project focuses on generating, inspecting, cleaning, validating, and visualizing a synthetic healthcare dataset containing information from **100 patients**. The dataset simulates real-world IoMT (Internet of Medical Things) healthcare monitoring data, including patient demographics, diseases, vital signs, and healthcare alert indicators.

The objective of this project is to demonstrate a complete healthcare data analytics workflow, starting from raw synthetic data generation to data quality assessment and exploratory data analysis (EDA).

---

# Dataset Description

The synthetic dataset contains **100 patient records** with **19 attributes** representing patient information, medical conditions, sensor readings, and health alerts.

## Dataset Features

| Column Name | Description |
|-------------|-------------|
| patient_id | Unique identifier for each patient |
| patient_name | Synthetic patient name |
| age | Patient age |
| gender | Patient gender |
| disease | Diagnosed medical condition |
| heart_rate | Heart rate measurement (beats per minute) |
| spO2_level | Blood oxygen saturation percentage |
| systolic_blood_pressure | Systolic blood pressure reading |
| diastolic_blood_pressure | Diastolic blood pressure reading |
| body_temperature | Body temperature in Celsius |
| respiratory_rate | Breathing rate per minute |
| bmi | Body Mass Index |
| fall_detection | Indicates whether patient experienced a fall |
| data_accuracy | Sensor data accuracy percentage |
| heart_rate_alert | Heart rate abnormality indicator |
| spO2_level_alert | Oxygen saturation alert indicator |
| blood_pressure_alert | Blood pressure alert indicator |
| temperature_alert | Fever/normal temperature indicator |
| timestamp | Time of patient measurement |

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Faker Library
- Google Colab / Jupyter Notebook

---

# 1. Synthetic Dataset Generation

A synthetic healthcare dataset was generated using Python and the Faker library.

The dataset includes:

- Patient demographics
- Medical diagnoses
- Physiological measurements
- Sensor accuracy information
- Healthcare alert labels
- Timestamp-based monitoring data

The generated dataset consists of:

- **100 unique patients**
- **19 healthcare attributes**
- Multiple disease categories
- Realistic medical parameter ranges

---

# 2. Data Inspection

The initial dataset inspection was performed to understand the structure and quality of the data.

## Inspection Activities

Performed:

- Dataset shape analysis
- Column identification
- Data type verification
- Statistical summary generation
- Missing value analysis
- Duplicate record detection

### Inspection Checks

| Check | Purpose |
|------|---------|
| Dataset shape | Determine number of records and attributes |
| Data types | Verify numerical and categorical columns |
| Statistical summary | Understand data distribution |
| Missing values | Identify incomplete records |
| Duplicate detection | Ensure unique patient records |

---

# 3. Data Cleaning

Data cleaning was performed to improve data quality and prepare the dataset for analysis.

## Cleaning Steps

### Duplicate Removal

Duplicate patient records were identified and removed to maintain data consistency.

### Missing Value Handling

- Numerical columns:
  - Missing values replaced using median imputation

- Categorical columns:
  - Missing values replaced with `"Unknown"`

### Timestamp Conversion

Timestamp columns were converted into proper datetime format for time-based analysis.

### Data Formatting

- Verified patient IDs
- Ensured consistent column formats
- Removed invalid records

---

# 4. Data Validation

Healthcare datasets require validation against realistic medical ranges.

The following validation rules were applied:

| Attribute | Validation Range |
|-----------|-----------------|
| Age | 18 - 100 years |
| Heart Rate | 40 - 200 bpm |
| SpO2 Level | 70 - 100 % |
| Temperature | 30 - 45 °C |
| Blood Pressure | Systolic should be greater than diastolic |

Validation checks ensured that:

- Patient information was realistic
- Sensor readings were within acceptable ranges
- Invalid records were identified

---

# 5. Exploratory Data Analysis (EDA)

EDA was performed to identify patterns and relationships within the healthcare data.

## Visualizations Created

### Disease Distribution

Analyzed the number of patients affected by each disease category.

Purpose:
- Understand disease prevalence
- Identify common medical conditions

---

### Patient Age Distribution

Visualization of patient age groups using histograms.

Purpose:
- Analyze demographic distribution
- Identify age-related trends

---

### Gender Distribution

Analyzed the distribution of male and female patients.

Purpose:
- Understand demographic balance

---

### Heart Rate Analysis

Examined heart rate patterns using:

- Histograms
- Density plots
- Threshold analysis

Purpose:
- Identify patients with elevated heart rates
- Analyze cardiac risk indicators

---

### SpO2 Level Analysis

Used boxplots to analyze oxygen saturation levels.

Purpose:
- Identify low oxygen saturation cases
- Detect possible respiratory concerns

---

### Vital Sign Correlation Analysis

Generated a correlation heatmap to analyze relationships between:

- Heart rate
- SpO2 levels
- Blood pressure
- Temperature
- BMI

Purpose:
- Identify relationships among healthcare parameters
- Support future predictive modeling

---

### Disease vs Heart Rate Analysis

Compared heart rate variation across different disease categories.

Purpose:

- Identify disease-related physiological changes
- Understand patient health patterns

---

### Healthcare Alert Analysis

Analyzed:

- Heart rate alerts
- SpO2 alerts
- Blood pressure alerts
- Temperature alerts

Purpose:

- Identify potentially critical patients
- Evaluate healthcare monitoring indicators

---

# Data Quality Report

After preprocessing:

| Quality Metric | Result |
|---------------|--------|
| Total Records | 100 |
| Total Features | 19 |
| Missing Values | 0 |
| Duplicate Records | 0 |
| Unique Patients | 100 |

---

# Key Insights

The analysis provided the following observations:

- The dataset successfully simulates real-world healthcare monitoring scenarios.
- Vital signs such as heart rate, oxygen saturation, and blood pressure provide important indicators for patient health assessment.
- Alert columns help identify abnormal physiological conditions.
- Correlation analysis highlights relationships between healthcare measurements.
- The cleaned dataset can be used for:
  - Machine learning models
  - Predictive healthcare analytics
  - IoMT applications
  - Real-time monitoring systems

---

# Future Enhancements

Possible improvements:

- Generate larger patient datasets (10K+ records)
- Add real-time streaming simulation using Apache Spark
- Build patient risk prediction models
- Develop healthcare dashboards using Streamlit/Power BI
- Implement anomaly detection for early disease prediction

---

# Conclusion

This project demonstrates an end-to-end healthcare data analytics workflow, including synthetic data generation, data preprocessing, validation, and visualization. The resulting dataset provides a foundation for advanced analytics, machine learning, and IoMT healthcare monitoring applications.


