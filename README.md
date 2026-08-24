# Automated Data Quality Dashboard

## Overview

A Python-based data quality automation system that detects,
classifies, cleans, and audits common data-quality problems
in customer datasets.

The system demonstrates automated data validation,
confidence scoring, safe data cleaning, error reporting,
and audit logging.

---

## Business Problem

Operational datasets often contain:

- Duplicate records
- Missing values
- Invalid email addresses
- Inconsistent formatting
- Invalid transaction amounts

Manually identifying these problems is repetitive,
time-consuming, and difficult to audit.

This project automates that workflow.

---

## Results

| Metric | Result |
|---|---:|
| Records processed | 547 |
| Clean records retained | 500 |
| Duplicates removed | 47 |
| Audit events recorded | 114 |
| Missing values remaining | 24 |
| Invalid/blank emails remaining | 34 |
| Negative amounts remaining | 5 |
| Final data-quality score | 95.8% |

### Processing Performance

The system processed the dataset automatically and measured
the actual execution time inside Google Colab.

---

## Before vs After

**Before**

547 records

↓

**Automated quality checks**

Duplicates • Missing values • Invalid emails • Invalid amounts

↓

**Cleaning**

47 duplicate records removed

↓

**After**

500 records retained

↓

**Final quality score**

95.8%

---

## How It Works

```text
Raw CSV
   |
   v
Data Quality Detection
   |
   +--> Duplicate Detection
   |
   +--> Missing Value Detection
   |
   +--> Email Validation
   |
   +--> Format Checks
   |
   +--> Transaction Validation
   |
   v
Confidence Scoring
   |
   +--> High Confidence --> Automated Action
   |
   +--> Lower Confidence --> Human Review
   |
   v
Cleaned Dataset
   +
Error Report
   +
Audit Log
