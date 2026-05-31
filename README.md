# Data Analytics Dataset Cleaning Pipeline

A lightweight Python automated data cleaning script using `pandas`. This project handles missing values, standardizes date formats, eliminates duplicate records, and exports a verified, production-ready dataset for downstream data analytics and visualization.

## 📌 Features
* **Missing Value Handling:** Automatically replaces missing values in the `CouponCode` column with a default `"NO_COUPON"` flag.
* **Date Standardization:** Parses the `Date` column into a consistent datetime format while gracefully catching and reporting corrupt or invalid date formats.
* **Deduplication:** Identifies and removes duplicate transactions based on `OrderID`, retaining only the first occurrence.
* **Data Quality Reporting:** Prints a quick terminal-based **Data Cleaning Verification Report** to confirm dataset integrity before saving.

---

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Libraries:** `pandas`, `openpyxl` (for Excel file handling)

---

## 📂 Project Structure
```text
├── Dataset for Data Analytics.xlsx         # Raw input dataset (not tracked in Git)
├── Cleaned_Data_Analytics_Dataset.xlsx     # Processed and cleaned output dataset
├── data_cleaning.py                        # Main Python cleaning script
└── README.md                               # Project documentation
