# Data Cleaning & Preprocessing – Project Summary (Task1)
📁 **Objective**:
The goal of this project was to clean and standardize a raw dataset containing order, shipping, and transaction information in preparation for analysis. This included handling missing values, renaming columns for clarity and consistency, converting data types, and exporting the final cleaned version to a CSV file.
**Steps Performed**:    
1. Loading the Dataset  
Loaded the dataset into a Pandas DataFrame using Jupyter Notebook.    
2. Handling Null Values    
Identified missing (null / NaN) values in multiple columns.    
Replaced null values in specific shipping-related columns (ship-city, ship-state, ship-postal-code, ship-country, fulfilled-by) with 0.  
Dropped rows with null values in critical financial columns currency and amount.  
3. Renaming Columns  
Renamed all columns to a consistent snake_case format (lowercase with underscores and no spaces) for better readability and code compatibility.  
4. Data Type Conversions  
Converted ship_postal_code column to integer (int) for numeric operations.  
Converted date column to Pandas datetime format.  
****⚠️ Challenges Encountered****  
**🛑 Warning on Date Conversion**  
Encountered a warning.  
UserWarning: Could not infer format, so each element will be parsed individually...  
This happened because Pandas couldn’t automatically detect the date format.  
**Solution:** It's recommended to specify the format explicitly using the format argument in pd.to_datetime() for consistency and better performance.  
****✅ Final Outcome****  
Cleaned, consistent, and analysis-ready dataset.  
All nulls handled, types converted, and column names standardized.  
Dataset now ready for use in reporting, visualization, or machine learning workflows.  



