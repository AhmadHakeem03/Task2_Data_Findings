# NeoRx - Task 2

NeoRx Task 2 is a healthcare data analytics project focused on **prescription data quality investigation and patient safety risk detection**.

The work analyzes a prescription dataset (816 records) to identify critical data issues, assess their severity, and propose validation rules to improve clinical data reliability.

## Project focus

This investigation checks prescription records for issues that can impact clinical decisions, including:

- Invalid or inconsistent patient demographics (age, date of birth, patient type)
- Duplicate prescription records and conflicting timestamps
- Invalid medication dosage forms
- Potentially unsafe prescriptions for children under 5
- Logical timeline errors (for example, prescription date before birth date)
- Inconsistent dose-strength, dose-unit, quantity, and frequency relationships

## Repository structure (Task 2)

- `Task2/`
  - `code/Prescription_Data_Quality_Investigation.ipynb`  
    Main notebook for data profiling, rule-based checks, severity classification, and findings.
  - `code/Prescription Data Analysis and Quality Assessment.docx`  
    Written report of analysis and conclusions.

## Key outcomes

The Task 2 analysis identifies high-impact data quality risks and provides actionable controls, such as:

- Enforcing strict input formats and ID validation rules
- Automatically deriving age from date of birth
- Blocking future birth dates and impossible clinical timelines
- Applying age-based medication and dosage-form restrictions
- Strengthening duplicate detection and timestamp consistency checks
- Standardizing dosage and frequency entry logic

## Tools used

- Python (Jupyter Notebook)
- Pandas / NumPy for data processing
- Word documents for reporting

