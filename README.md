# Cleaned Sample Dataset



File Name:
cleaned_sample_data.csv

Description:
This dataset is a cleaned version of a sample data containing basic information about individuals including ID, Name, Age, Gender, and Join Date. All missing values, duplicates, and inconsistencies have been handled.

Columns:
1. ID – Unique identifier for each individual (integer)
2. Name – Name of the individual (string)
3. Age – Age of the individual (integer)
4. Gender – Gender of the individual (male or female)
5. Join_Date – Joining date of the individual (YYYY-MM-DD format)

Data Cleaning Steps:
1. Missing values in Age were filled with the mean of available ages.
2. Missing values in Join_Date were filled with the mode of available dates.
3. Duplicate rows were removed.
4. Gender values standardized (M, m → male, F, f → female).
5. Outliers in Age were detected and removed (e.g., Age > 100).
6. Data types corrected (Age → integer, Join_Date → datetime).

Usage:
- The CSV file can be used for data analysis, visualization, and machine learning practice.
- Recommended to keep a backup of the original raw dataset.
"""

# Save README as a txt file in your desired location
readme_file_path = r"C:\Users\PC\Documents\Projects\README_Cleaned_Sample_Data.txt"

with open(readme_file_path, "w") as file:
    file.write(readme_content)

print(f"README file saved at: {readme_file_path}")
