 # Week 1 - Task 1
This repository contains the work I've done on cleaning and normalizing an HR dataset, transforming it into meaningful insights, and structuring it into proper fact and dimension tables. The project includes using various tools like Excel, Power BI, MySQL, Python, and Power Query to achieve the required data transformation.

# Tool Used:
  1) Power Bi   and
  2) excel
     
 # Task 1 - Data Cleaning:
  
 The task involved cleaning an HR dataset (attendance_data.csv), focusing on the following:

# Removing Duplicates:

I identified and removed duplicate records in the dataset using Power Bi Remove Duplicates feature.

Steps: Data > Tramform data > home (Remove Dulipcates) 

# Standardizing Date Formats:

Standardized the date format to YYYY-MM-DD and extracted the month name and day type for analysis.

Steps: Data > Tramform data >


# Cleaning Employee IDs:

Removed any extra characters, like the "@" symbol, from employee IDs using Power Bi's function.

Steps: Data > Tramform data >

# Standardizing Name Capitalization:

Employee names were standardized to Title Case, ensuring the first letter of each word is capitalized for consistency.

Steps: Data > Tramform data > format > Title Case.

# Mapping Status Values:

Mapped status values to abbreviations as follows:

Work From Office → WFO

Work From Home → WFH

Birthday Leave → BL

Menstrual Leave → ML

Paid Leave → PL

Sick Leave → SL

Weekly Off → WO

Power Query was used to replace the values: Data > Transform > Replace Values

# Data Insights Extracted
From the cleaned dataset, I extracted the following insights:
1) Unique employee names.
2) WFH percentage for May.
3) Day of the week with the highest attendance in June.
4) Employees with WFH > 10% in April
