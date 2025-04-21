🧾 Task Overview:
The objective was to clean and prepare a raw dataset for analysis. The dataset (marketing_campaign.csv) had issues like:
Missing values
Duplicate rows
Inconsistent formatting (text and dates)
Untidy column names
The goal was to make the dataset consistent, accurate, and ready for analysis using Python (Pandas).

🔧 Steps Taken (with Explanation):
Loaded the Dataset
Used pandas.read_csv() to load the file into a DataFrame for processing.

Removed Duplicates
Used drop_duplicates() to eliminate any repeated rows that could bias the analysis.

Handled Missing Values
Found that the Income column had missing values. These were filled with the median income using fillna().

Median was used instead of mean to avoid influence from outliers.

Standardized Text Values

Education and Marital_Status had inconsistent capitalization and spaces.

Used .str.title() and .str.strip() to make them uniform and clean.

Converted Date Format

The Dt_Customer column was a string; converted it to proper datetime format using pd.to_datetime().

Renamed Column Headers

Made all column names lowercase and replaced spaces with underscores to follow best practices and avoid errors in code.

Done using .str.lower().str.replace(' ', '_')

Saved the Cleaned Dataset

Used to_csv() to export the cleaned dataset as marketing_campaign_cleaned.csv.

✅ Result:
You now have a clean, consistent dataset that is:

Free from duplicates

Has no missing income values

Contains standardized and readable column names

Ready for data analysis or visualization


