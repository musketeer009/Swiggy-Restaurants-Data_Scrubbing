# Swiggy-Restaurants-Data_Scrubbing
This project involves cleaning swiggy restaurants dataset by handling missing values, duplicates, and inconsistencies to improve data quality for accurate analysis. 

Here's a summary of the data in both files:

Swiggy Raw Data Includes:
id (restaurant ID)
name (restaurant name)
city (location)
rating ( rating by users)
rating_count (number of ratings)
cost (price range)
cuisine (types of food offered)
lic_no (license number)
link (restaurant URL)
address (physical address)
menu (JSON file link to menu)


Restaurants Includes:
id (restaurant ID)
name (restaurant name)
city (location)
rating (numeric rating)
rating_count (numeric value of ratings)
cuisine (type of food)
cost (numeric cost)
revenue (calculated revenue)
link (restaurant URL)


Cleaning Plan:

Check and Standardize Data Types: Ensure all columns have the correct type

Handle Missing Values: Identify and clean null or inconsistent entries.

Validate Numeric Ranges: Ensure ratings, costs, and revenues fall within logical ranges.

Clean Text Fields: Remove whitespace, standardize case, and validate URLs.

Duplicate Check: Identify and remove duplicate rows based on unique identifiers.


Cleaning Summary – Restaurants Dataset
Data Types: All columns are now in the correct formats:

id, rating_count, cost, revenue → Integer
rating → Float (between 0 and 5)
name, city, cuisine, link → String


Range Validations:
Ratings: Between 0 and 5.
Cost: Positive values only.
Revenue: Positive values (including zero).



Text Cleaning:
Standardized name, city, and cuisine columns to title case.
Ensured all URLs in the link column are valid Swiggy links.

Duplicates:
Removed duplicate entries based on the id column.
Record Count: 61425 rows
