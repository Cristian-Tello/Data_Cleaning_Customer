## STORE 1 - CUSTOMER DATA CLEANING
**Project Type: Data Cleaning** 

**Role: Data Analyst** 

**Programming Language: Python**

## Tools & Technologies
**PYTHON**

The project was developed using Python, focusing on built-in functions, string methods, list operations, data type conversion, and exception handling.
	

| Function | Purpose|
| --- | --- |
| **print()** | Display cleaned data, results, and validation outputs |
| **type()** | Check the data type of variables |
| **int()** | Convert age values into integers |
| **sum()** | Calculate the total spending across categories |
| **len()** | Count the number of registered customers |
	
## String Methods Used
| Method | Purpose|
| --- | --- |
| **.strip()** | Remove unnecessary spaces from the beginning and end of names |
| **.replace()** | Replace underscores (_) with spaces |
| **.split()** | Separate customer names into individual elements |
| **.sort()** | 	Sort customer records by user ID |
| **.append()** | Add cleaned customer records to the new usuarios_limpio list |
| **List indexing** | Access customer IDs, names, ages, categories, and spending values |

## Other Python Concepts
**Exception Handling**

Used try / except to validate age values and handle cases where a value could not be converted into an integer.

**Formatted Strings**

Used Python f-strings to dynamically generate customer summaries and business messages.

## Project Overview
Store 1, an e-commerce company, is preparing to launch a new Customer Loyalty Program. Before creating personalized campaigns and customer segments, the company needs to ensure that its customer data is complete, consistent, and properly structured.

The objective of this project was to review and transform a sample of Store 1's customer data, correcting formatting and data-type issues and preparing the information for future analysis, customer segmentation, and KPI development.

## Description
Store 1 was reviewing the quality and consistency of its customer database before launching a new Customer Loyalty Program.

The raw data contained several inconsistencies, including:

* Extra spaces in customer names
* Underscores used as name separators
* Inconsistent capitalization
* Ages stored as floating-point or string values
* Customer information stored in nested lists

These inconsistencies could affect future customer segmentation and marketing analysis.

As a Data Analyst, my task was to clean and transform the customer data so it could be used reliably for further analysis.

The main objectives were to:

* Clean customer names
* Standardize age values
* Validate data types
* Separate first and last names
* Sort customer records
* Calculate total customer spending
* Count registered customers
* Create structured customer summaries
* Prepare the dataset for future KPI and segmentation analysis

I used Python and built-in functions and methods to perform the data cleaning and transformation process.

The main steps included:

1. Removing unnecessary spaces from customer names.
2. Replacing underscores with spaces.
3. Splitting customer names into first and last names.
4. Converting customer ages into integer values.
5. Validating invalid age values using exception handling.
6. Sorting customer records by user ID.
7. Calculating total spending across product categories.
8. Counting the number of registered customers.
9. Creating formatted customer summaries.
10. Building a cleaned customer list with the transformed information.

## Result

The customer information was transformed into a more consistent and structured format, making it easier to review and prepare for future analysis.

The cleaned data provides a foundation for future business analysis such as:

Customer segmentation
Customer spending analysis
Product category preferences
Customer value analysis
Loyalty Program KPIs
Personalized marketing campaigns

The project demonstrates how data cleaning and validation are essential steps before using customer data to support business decisions.

## Data Cleaning Process
**1. Cleaning Customer Names**

Customer names contained unnecessary spaces and underscores.

Example:

" mike_reed "

After cleaning:

"mike reed"

Using:

usuario_nombre.strip()
usuario_nombre.replace("_", " ")

**2. Splitting Names**

The cleaned name was separated into individual elements:

usuario_nombre.split()

Result:

["mike", "reed"]

This structure can later support personalized customer communications and segmentation.

**3. Data Type Validation**

Customer ages were initially stored in different formats.

For example:

usuario_edad = 32.0

The value was converted to an integer:

usuario_edad = int(usuario_edad)

The resulting value was:

32

Invalid values were also tested using exception handling.

**4. Sorting Customer Records**

Customer records were sorted by user ID:

usuarios.sort(reverse=False)

This facilitates data review and the creation of organized reports.

**5. Calculating Customer Spending**

Customer spending was stored as a list of values corresponding to different product categories.

Example:

spending_by_category = [894, 213, 173]

The total spending was calculated using:

sum_total = sum(gasto_por_categoria)

Result: 1280

This creates an important customer-level metric that can be used for future segmentation and KPI analysis.

**6. Counting Registered Customers**

The number of customers was calculated using:

Registered customers = len(usuarios)

This provides a simple business metric that can be used to measure the current size of the customer database.

**7. Creating the Cleaned Dataset**

A new list called usuarios_limpio was created to store the transformed customer information:

clean_users = []

Cleaned records were then added using:

clean_users.append(...)

This created a separate structure containing the processed customer information.

## Conclusion

This project demonstrates the use of Python fundamentals for data cleaning and preparation in an e-commerce business context.

The main focus was not only to correct data-formatting issues, but to understand how data quality affects the ability to perform reliable customer analysis and generate meaningful business KPIs.
