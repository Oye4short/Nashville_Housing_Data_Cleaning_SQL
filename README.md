# Nashville_Housing_Data_Cleaning_SQL
This SQL script focuses on cleaning and enhancing data in the "NashvilleHousing" table within my "PortfolioProject" database. (Nashville Housing Data included in this repository) Here's a concise summary of the key tasks performed:

**View Data** <br>
        Retrieves all columns from "NashvilleHousing" for initial inspection.

**Standardize Date Format.** <br>
        Converts the "SaleDate" column to a consistent date format.

**Populate Property Address Data.** <br>
        Fills null values in the "PropertyAddress" column by updating them with non-null values from other records with the same "ParcelID."

**Break Out Address into Individual Columns**<br>
        Splits the "PropertyAddress" column into separate columns for "PropertySplitAddress" and "Property_City."

**Break Out Owner Address into Individual Columns**<br>
        Divides the "OwnerAddress" column into separate columns for "OwnerSplitAddress," "Owner_City," and "Owner_State."

**Change Y and N to Yes and No**<br>
        Converts values in the "SoldAsVacant" column from 'Y' to 'Yes' and 'N' to 'No.'

**Remove Duplicates**<br>
         Uses a Common Table Expression (CTE) with a ROW_NUMBER() function to identify and display duplicate records based on specific columns.

**Delete Unused Columns**<br>
        Drops columns "OwnerAddress," "TaxDistrict," "PropertyAddress," "SaleDate" from the table.

The script showcases a systematic approach to address data quality issues, including date standardization, handling null values, splitting addresses, converting values for better representation, and managing duplicate records.
