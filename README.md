# SQL_Data_Cleaning_Project

#Cleaning Nashville Housing Data in SQL

This project involves cleaning and preprocessing the Nashville Housing dataset using SQL queries. The dataset is stored in a table named NashvilleHousing in the PortfolioProject database.

#Steps:

* Date Format: Convert the SaleDate column to a standard date format using the CONVERT function.
* Populate Property Address Data: Fill in missing PropertyAddress values by joining the table with itself on ParcelID and using the ISNULL function.
* Break out Address into Individual Columns: Split the PropertyAddress column into separate columns for Address, City, and State using the SUBSTRING and PARSENAME functions.
* Change Y and N to Yes and No in "Sold as Vacant" field: Use a CASE statement to replace 'Y' and 'N' values with 'Yes' and 'No' in the SoldAsVacant column.
* Remove Duplicates: Use a ROW_NUMBER function to identify duplicate rows and remove them.
* Delete Unused Columns: Drop unnecessary columns from the table to reduce clutter and improve data quality.
  
#Queries:

The SQL queries used to perform these steps are included in the code file. Each section is separated by a line of dashes for readability.

#Output:

The cleaned and preprocessed dataset is stored in the NashvilleHousing table. The final output can be viewed by running a SELECT * query on the table.
