# Data Cleaning and Manipulation Summary

To ensure reliable analysis, the raw Cyclistic data (12 monthly CSV files) underwent the following cleaning and transformation steps:

## 1. Data Consolidation
- Merged **12 monthly CSV files** (January 2023 – December 2023) into a single dataset with **X million rows** and standardized column names.

## 2. Column Standardization
- Unified column names to lowercase (e.g., `started_at`, `ended_at`, `member_casual`).
- Renamed inconsistent columns from older datasets (`start_time → started_at`, `end_time → ended_at`, `usertype → member_casual`, `trip_id → ride_id`, etc.).

## 3. Datetime Parsing
- Converted `started_at` and `ended_at` columns to proper datetime objects.
- Removed rows with missing or invalid timestamps.

## 4. Ride Duration Calculation
- Created a new column `ride_length_s` (seconds) = `ended_at - started_at`.
- Converted to minutes (`ride_length_min`) for easier interpretation.

## 5. Data Filtering
- Removed:
  - Trips with **zero or negative duration**
  - Outliers with durations over **24 hours**
- Dropped rows with missing key information (start/end time, user type).

## 6. Feature Engineering
- Added:
  - `day_of_week` (Monday–Sunday)
  - `hour` (0–23)
  - `month` (January–December)
- Standardized user categories: `subscriber → member`, `customer → casual`.

## 7. Final Dataset
- Cleaned dataset saved as:  
  `data_working/cyclistic_cleaned.csv`  
- Final row count: **X rows remaining (Y% retained)**

This process ensured the data was free from major inconsistencies, accurately represented trip durations, and was ready for meaningful analysis.
