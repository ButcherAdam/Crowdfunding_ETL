# Crowdfunding_ETL
Project 2 for UT Austin Data Visualization Bootcamp involving ETL on crowdfunding data.
Group members: Zach Hooks, Oana Wright, Brian Hart, Adam Butcher, Rogelio Cardenas

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



