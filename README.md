# Crowdfunding_ETL
 Project 2 for UT Austin Data Visualization Bootcamp involving ETL on crowdfunding data.
## Group 4 members: Zach Hooks, Oana Wright, Brian Hart, Adam Butcher, Rogelio Cardenas

For the ETL mini project, you will work with a partner to practice building an ETL pipeline using Python, Pandas, and either Python dictionary methods or regular expressions to extract and transform the data. After you transform the data, you'll create four CSV files and use the CSV file data to create an ERD and a table schema. Finally, you’ll upload the CSV file data into a Postgres database.
Since this is a one-week project, make sure that you have done at least half of your project before the third day of class to stay on track.
Although you and your partner will divide the work, it’s essential to collaborate and communicate while working on different parts of the project. Be sure to check in with your partner regularly and offer support

## Create the Category and Subcategory DataFrames

1. Extract and transform the crowdfunding.xlsx Excel data to create a category DataFrame that has the following columns:
  - A "category_id" column that has entries going sequentially from "cat1" to "catn", where n is the number of unique categories
  - A "category" column that contains only the category titles
The following image shows this category DataFrame:
https://static.bc-edx.com/data/dl-1-2/m13/lms/img/category_DataFrame.png![image](https://github.com/user-attachments/assets/f96119f6-973c-464a-900f-1ed294109eca)
2. Export the category DataFrame as category.csv and save it to your GitHub repository.
3. Extract and transform the crowdfunding.xlsx Excel data to create a subcategory DataFrame that has the following columns:
  - A "subcategory_id" column that has entries going sequentially from "subcat1" to "subcatn", where n is the number of unique subcategories
  - A "subcategory" column that contains only the subcategory titles
The following image shows this subcategory DataFrame:
https://static.bc-edx.com/data/dl-1-2/m13/lms/img/subcategory_DataFrame.png![image](https://github.com/user-attachments/assets/efcbd5d9-abf3-4397-a768-aca67a638f05)
4. Export the subcategory DataFrame as subcategory.csv and save it to your GitHub repository.

## Create the Campaign DataFrame

1. Extract and transform the crowdfunding.xlsx Excel data to create a campaign DataFrame has the following columns:
 - The "cf_id" column
 - The "contact_id" column
 - The "company_name" column
 - The "blurb" column, renamed to "description"
 - The "goal" column, converted to the float data type
 - The "pledged" column, converted to the float data type
 - The "outcome" column
 - The "backers_count" column
 - The "country" column
 - The "currency" column
 - The "launched_at" column, renamed to "launch_date" and with the UTC times converted to the datetime format
 - The "deadline" column, renamed to "end_date" and with the UTC times converted to the datetime format
 - The "category_id" column, with unique identification numbers matching those in the "category_id" column of the category DataFrame
 - The "subcategory_id" column, with the unique identification numbers matching those in the "subcategory_id" column of the subcategory DataFrame
 - The following image shows this campaign DataFrame:
 - https://static.bc-edx.com/data/dl-1-2/m13/lms/img/campaign_DataFrame.png![image](https://github.com/user-attachments/assets/aaeb506f-fb21-447f-bfc1-d7342ff4b80b)
2. Export the campaign DataFrame as campaign.csv and save it to your GitHub repository.

## Create the Contacts DataFrame

1. Choose one of the following two options for extracting and transforming the data from the contacts.xlsx Excel data:
  - Option 1: Use Python dictionary methods.
  - Option 2: Use regular expressions.
2. If you chose Option 1, complete the following steps:
  - Import the contacts.xlsx file into a DataFrame.
  - Iterate through the DataFrame, converting each row to a dictionary.
  - Iterate through each dictionary, doing the following:
    - Extract the dictionary values from the keys by using a Python list comprehension.
    - Add the values for each row to a new list.
  - Create a new DataFrame that contains the extracted data.
  - Split each "name" column value into a first and last name, and place each in a new column.
  - Clean and export the DataFrame as contacts.csv and save it to your GitHub repository.
3. If you chose Option 2, complete the following steps:
  - Import the contacts.xlsx file into a DataFrame.
  - Extract the "contact_id", "name", and "email" columns by using regular expressions.
  - Create a new DataFrame with the extracted data.
  - Convert the "contact_id" column to the integer type.
  - Split each "name" column value into a first and a last name, and place each in a new column.
  - Clean and then export the DataFrame as contacts.csv and save it to your GitHub repository.
4. Check that your final DataFrame resembles the one in the following image:
https://static.bc-edx.com/data/dl-1-2/m13/lms/img/contact_DataFrame_final.png![image](https://github.com/user-attachments/assets/5f1af02a-6382-4d74-9266-c63fa3519e7e)

## Create the Crowdfunding Database

1. Inspect the four CSV files, and then sketch an ERD of the tables by using QuickDBD Links to an external site..
2. Use the information from the ERD to create a table schema for each CSV file.
Note: Remember to specify the data types, primary keys, foreign keys, and other constraints.
3. Save the database schema as a Postgres file named crowdfunding_db_schema.sql, and save it to your GitHub repository.
4. Create a new Postgres database, named crowdfunding_db.
5. Using the database schema, create the tables in the correct order to handle the foreign keys.
6. Verify the table creation by running a SELECT statement for each table.
7. Import each CSV file into its corresponding SQL table.
8. Verify that each table has the correct data by running a SELECT statement for each.







