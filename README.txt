This SQL project cleans data from a layoffs dataset.

First, the dataset is imported into MySQL from a CSV file named layoffs.csv.

Then, the following operations are performed:

Steps done:
1. Created a staging table to work with raw data safely.
2. Removed duplicate rows based on key columns.
3. Standardized data:
   - Fixed industry names (e.g., made 'Crypto Currency' to 'Crypto').
   - Cleaned country names (removed trailing periods).
   - Converted date column to proper DATE format.
4. Handled null values: Kept them as is since they are useful for analysis.
5. Removed rows where both total_laid_off and percentage_laid_off are null.
6. Dropped the temporary row_num column.

The cleaned data is in layoffs_staging2 table.
