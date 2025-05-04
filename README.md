# 📊 Medical Appointment No-Show Analysis & ETL Pipeline

This project analyzes real hospital data from Brazil to understand patterns in **patient no-shows**. It includes an ETL (Extract, Transform, Load) pipeline, exploratory data analysis (EDA), and insights derived from feature exploration.

---

## 🧠 Problem Statement

Hospitals face challenges with patients missing their appointments, leading to lost resources and scheduling inefficiencies. This project investigates factors that influence no-show behavior and prepares the data for possible downstream tasks like modeling or dashboarding.

---

## 🔁 ETL Pipeline

- ✅ **Extract**: Load raw dataset from Kaggle (`noshowappointments.csv`)
- ✅ **Transform**:
  - Cleaned column names
  - Removed invalid age entries
  - Converted date columns
  - Calculated `waiting_days` (appointment day - scheduled day)
  - Encoded the target variable `No-show` (Yes → 1, No → 0)
- ✅ **Load**: Saved cleaned dataset to `cleaned_noshow.csv`

📄 Script: [`scripts/etl_pipeline.py`](scripts/etl_pipeline.py)

Run the pipeline:
```bash
python scripts/etl_pipeline.py
