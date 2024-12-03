# W2U Group Data Cleaning Using MS Excel Power-Query

<br>

### Overview
This project involved cleaning and transforming a sales text format file for W2U Group using Power Query in Microsoft Excel. The raw dataset contained inconsistencies, blank rows, unnecessary columns, and formatting issues that were addressed systematically.

The cleaned dataset is now structured and ready for further analysis or reporting.

<BR>

### Objective
To utilize Power Query to:

- Standardize and clean the raw dataset.
- Ensure proper structure and formatting for easy analysis.
- Remove redundant or irrelevant data while maintaining data integrity.

<br>
  
### Dataset
- Source: [Unclean File](https://drive.google.com/file/d/1OvxqjlIN0tCLduibVk2YEs5vnPAGAQPc/view?usp=sharing) Contains unclean text file from W2U Group.
- Clean Data: [W2U Clean Dataset](https://docs.google.com/spreadsheets/d/15sPaC9LjVSF1BoKvpwemtXbiqDOKsnPm/edit?usp=sharing&ouid=100554781607807743501&rtpof=true&sd=true)

<BR>

### Steps in Data Cleaning
#### 1. Remove Unnecessary Rows
- Removed the top three rows, which contained irrelevant information unrelated to the dataset.
#### 2. Filter Frist Column
- Filtered out the column containing long dashes (|--|--|) to exclude non-data entries.
#### 3. Eliminate Blank Rows
- Identified and removed all blank rows to ensure a cleaner dataset.
#### 4. Split First Row
- Split the current first row of the first column, into separate columns using the "|" delimiter.
#### 5. Rename Columns and Remove Empty Columns
- Renamed the columns with dataset to their appropriate names to reflect the actual data accurately.
- Deleted columns containing no data to streamline the dataset.
#### 6. Merge Columns
- Combined the last two columns into a single column to consolidate related data.
- Renamed the merged column as "Total" to reflect its purpose.
#### 7. Remove Top Header Row
- Removed the first row after the initial transformations, which was no longer necessary.
#### 8. Split Product-Category Column
- Split the Product-Category column into two separate columns using the "-" delimiter to differentiate product details and categories.
#### 9. Rename Columns
- Renamed the newly split Product-Category columns to meaningful names:
  - Product Name
  - Category
#### 10. Standardize Text Fields
- Applied the Trim function across all columns to remove unnecessary spaces.
#### 11. Data Type Conversion
- Converted columns to appropriate data types:
  - Whole Number data type: Order number and Quantity column.
  - Currency data type: Price per unit and Total column.
  - Text data type: Product and Category column.
  - Date data type: Order date column.

<br>

### Tools Used
- Power Query: For data transformation and cleaning.
- Microsoft Excel: To handle the raw and cleaned datasets.
