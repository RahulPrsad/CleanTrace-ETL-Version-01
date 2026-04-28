# AutoDataCleaner v1 — Dataset Cleaning & Audit Log Generator

AutoDataCleaner v1 is a browser-based ETL mini project that allows users to upload dirty datasets in CSV or Excel format and automatically performs dataset cleaning with a complete row-level audit log.

The system helps users preprocess raw data by removing duplicates, filling missing values, standardizing text, normalizing dates, and generating downloadable cleaned files with detailed tracking of every change made.

---

## Features

### Upload Support
- CSV (.csv)
- Excel (.xlsx, .xls)

### Automated Cleaning Operations
- Remove duplicate rows
- Remove fully empty rows
- Fill null values using:
  - Mean
  - Median
  - Mode
- Standardize text formatting
- Remove extra spaces and control characters
- Normalize inconsistent text casing
- Canonicalize category values
- Normalize date formats to ISO 8601 (YYYY-MM-DD)
- Detect invalid numeric values
- Type coercion for numeric columns

### Generated Outputs
- cleaned_dataset.csv
- audit_log.csv
- summary_report.txt

### Audit Log Tracking
Each change includes:
- Row ID
- Column Name
- Old Value
- New Value
- Rule Applied
- Reason
- Timestamp

---

## Project Objective

The goal of this project is to automate basic ETL preprocessing tasks for users who work with raw datasets.

Instead of manually cleaning data in Excel or Python scripts, users can simply upload a dataset and receive:
- a cleaned dataset
- a full audit report
- a cleaning summary

This improves data quality, saves time, and increases transparency in preprocessing.

---

## Tech Stack

### Frontend
- HTML5
- CSS3
- JavaScript (Vanilla JS)

### Libraries Used
- SheetJS (XLSX.js)

### Processing Type
- Fully Browser-Based (No Backend Required)

---

## How It Works

### Step 1
Upload a dirty CSV or Excel dataset

### Step 2
Select cleaning options:
- duplicates
- null handling
- text cleaning
- date normalization

### Step 3
Run the cleaning pipeline

### Step 4
System generates:
- cleaned dataset
- audit log
- summary report

### Step 5
Download all generated files

---

## Folder Structure

```bash
AutoDataCleaner-v1/
│
├── index.html
├── README.md
└── sample_dataset.csv
