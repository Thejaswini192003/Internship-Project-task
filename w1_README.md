 # Week 1 - Task 1
This repository contains the work I've done on cleaning and normalizing on datasets, transforming it into meaningful insights, and structuring it into proper **fact** and **dimension** tables. 

# Tool Used:
  1) Power Bi   
  2) excel
     
 # Task 1 - Data Cleaning:
  
 The task involved cleaning an HR dataset **(attendance_data.csv)**, focusing on the following:

# Removing Duplicates:

I identified and removed duplicate records in the dataset using Power Bi Remove Duplicates feature.

**Steps:** Data > Tramform data > home (Remove Dulipcates) 

# Standardizing Date Formats:

Standardized the date format to **YYYY-MM-DD** and extracted the month name and day type for analysis.

**Steps:** Data > Power Bi > Data View > type the format.


# Cleaning Employee IDs:

Removed any extra characters, like the "@" symbol, from employee IDs using Power Bi's function.

**Steps:** Data > Tramform data > Replace

# Standardizing Name Capitalization:

Employee names were standardized to Title Case, ensuring the first letter of each word is capitalized for consistency.

**Steps:** Data > Tramform data > format > Title Case.

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

 # Week 1 - Task 2
# Data Normalization
                
 Denormalizated table:
![image](https://github.com/user-attachments/assets/bcee5245-c1b2-42ab-9a74-6f3afef68de6)


→ I am doing normalization using Excel.

Steps:
First create 4 another sheets (fact_orders, dim_customers, dim_poducts, dim_date)
In fact_orders sheet, paste data from main sheet and delete irrelevant columns as per output preview.
Then extract unique customer_id from main sheet using UNIQUE() function and paste as value in dim_customer sheet and named column as "customer_id".
After that extract customer name and city in dim_customer table using INDEX and MATCH function from main sheet.
The above same steps are followed for dim_date and dim_products as per output preview mentioned below.
![image](https://github.com/user-attachments/assets/6137da57-611a-48d1-8521-ca7039429571)

After normalization, here you can see normalized output file.
![image](https://github.com/user-attachments/assets/affc4f4b-b13e-4106-9dcb-d1c4b5c95e84)

