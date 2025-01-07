# Crowdfunding_ETL
Chad Hillman  
Mini Project 2  
January 2025.  

## Overview
This project focuses on extracting, transforming, and loading (ETL) crowdfunding data to clean and analyze the data. The goal is to create a well-structured database from the provided excel spreadsheets based on Module1 homework. We will be using jupyter notebook, QuickDBD to create the schema from our csv outputs and then to create the 4 tables usign SQL via PgAdmin4.

## Starter File
ETL_Mini_Project_C_Hillman.ipynb  
crowdfunding_db_schema.png  
crowdfunding_db_schema.sql  

## Resources Folder
contacts.xlsx  
crowdfunding.xlsx.  
campaign.csv  
category.csv  
contacts.csv  
subcategory.csv  

## Project Structure
Crowdfunding_ETL/
│
├── data/
│   ├── contacts.xlsx
│   ├── crowdfunding.xlsx
│   └── ...
│
├── notebooks/
│   └── ETL_Mini_Project_C_Hillman.ipynb
│
├── output/
│   ├── campaign.csv
│   ├── category.csv
│   ├── contacts.csv
│   └── subcategory.csv
│
└── schema/
    ├── crowdfunding_db_schema.png
    └── crowdfunding_db_schema.sql

## Process Steps
1. Load in the `crowdfunding.xlsx` file and create the `category` and `subcategory` DataFrames.
2. Amend the crowdfunding data to create the `campaign` DataFrame.
3. Remove unwanted columns and merge the the `category` & `subcategory` DataFrames with the newly created `campaign` DataFrame.
4. Rename the date columns and update data types to `datetime`.
5. Change data types for `goal` and `pledged` from `integer` to `float`.
6. Load in the `contacts.xlsx` file to create the `contact` DataFrame.
7. Print out the dictionary of contacts and create columns, split the `name` column into `first` and `last`, and reorder as instructed using option 1.
8. Save each DataFrame as a CSV and store them in the `resource` folder.
9. Using the DataFrame names and column headers, create the schema for the SQL database.
10. Use [Quick Database Diagrams](https://app.quickdatabasediagrams.com) to save a copy of the schema and the `crowdfunding_db_schema.sql` file.
11. Create the `crowdfunding_db` database and the 4 tables using the schema.
12. Load each CSV into the SQL database to complete the database creation.

## License
This project is licensed under the terms of the GNU General Public License v3.0. For more details, see the [LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) file.
