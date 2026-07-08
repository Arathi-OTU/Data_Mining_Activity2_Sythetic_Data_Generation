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

# Project Workflow

The project follows a complete healthcare data analytics pipeline:
