# Medical Appointment No-Shows – Data Cleaning & Preprocessing

# DataSet Explaination
This project is part of my Data Analyst Internship Task 1.
The dataset is from Kaggle’s Medical Appointment No Shows, containing information about patients, their medical appointments, and whether they showed up or not.
The objective of this task is to clean and preprocess the dataset so it’s ready for further analysis.

# 🎯 Objectives
1. Handle missing values.
2. Remove duplicate rows.
3. Standardize and clean categorical/text columns (e.g., gender, neighbourhood).
4. Convert date columns into proper datetime formats.
5. Ensure numeric columns have the correct datatypes.
6. Identify and handle outliers 

# Tools & Libraries
Python- Pandas, NumPy

# Data Cleaning workflow
Import the Python Libraries - Pandas and Numpy
Loaded the dataset into Pandas and stored it in a DataFrame called df.
Exploring the data
Checked for missing values
Removed duplicates (if any)
Standardized categorical values (e.g., Gender → F/M, Neighbourhood → title case like Jardim Da Penha).
Converted date columns → ScheduledDay and AppointmentDay into datetime.
Renamed columns for clarity and consistency 
Fixed data types → PatientId as string
Handled outliers in Age → removed negative ages (-1), and unrealistic age (115).

# Final DataSet Format

| Column           | Type       | Description                              |
| ---------------- | ---------- | --------------------------------------   |
| PatientID        | object     | Unique patient identifier                |
| AppointmentID    | int64      | Appointment identifier                   |
| Gender           | object     | `M` or `F`                               |
| ScheduledDay     | datetime64 | Date & time when appointment was made    |
| AppointmentDay	 | datetime64 | Actual appointment date                  |
| Age              | int64      | Patient’s age (0–100)                    |
| Neighbourhood    | object     | Patient’s neighbourhood                  |
| Scholarship      | int64      | Whether patient is enrolled in welfare   |
| Hypertension     | int64      | Hypertension indicator (0/1)             |
| Diabetes         | int64      | Diabetes indicator (0/1)                 |
| Alcoholism       | int64      | Alcoholism indicator (0/1)               |
| Handicap         | int64      | Handicap indicator (0/1)                 |
| SMS_received     | int64      | Whether SMS reminder was sent (0/1)      |
| Attended         | object     | `Yes/No` → Did patient attend?           |

# Deliverables
Cleaned dataset1(.csv).
This README.md file with cleaning steps summary.
