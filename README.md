# Big-Data with AWS (Amazon Web Services)
[![0179d-SC1-Aqa-Ty8-Dbc-TJMDYE-7-fit-scale-size-1028x578-v1569472044.jpg](https://i.postimg.cc/wMYmzkdQ/0179d-SC1-Aqa-Ty8-Dbc-TJMDYE-7-fit-scale-size-1028x578-v1569472044.jpg)](https://postimg.cc/JDKncZ0s)

## Background
In this assignment, you will put your ETL skills to the test. Many of Amazon's shoppers depend on product reviews to make a purchase. Amazon makes these datasets publicly available. They are quite large and can exceed the capacity of local machines. One dataset alone contains over 1.5 million rows; with over 40 datasets, data analysis can be very demanding on the average local computer. Your first goal for this assignment will be to perform the ETL process completely in the cloud and upload a DataFrame to an RDS instance. The second goal will be to use PySpark or SQL to perform a statistical analysis of selected data.

This homework assignment contains two levels. The second level is optional but highly recommended.
  1. Create DataFrames to match production-ready tables from two big Amazon customer review datasets.
  2. Analyze whether reviews from Amazon's Vine program are trustworthy.

**DISCLAIMER: I have ONLY done Level 1. Level 2 attempted but not complete in another Git hub Repo. Instructions for Level 2 is located in Instructions folder.**

## Data Source
  - https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt

## Application / Technologies Used
  - Google Colaboratory 
  - AWS (RDS and S3)
  - SQL 

## Instructions for Level 1
  - Use the provided schema to create tables in your RDS database.
  - Create two separate Google Colab notebooks and extract any two datasets from the list at review dataset. Put each dataset into its own notebook.
    - **Note:** You could ETL both data sources in a single Colab notebook, but it will be easier to work with these large S3 data sources in separate notebooks.
- Be sure to handle the header correctly. If you read the file without the header parameter, you may find that the column headers are included in the table rows.
- Complete the following steps for each notebook (one dataset per notebook).
	- Count the number of records (rows) in the dataset.
	- Transform the dataset to fit the tables in the schema file. Be sure that the DataFrames match in data type and in column name.
	- Load the DataFrames that correspond to tables into an RDS instance. Note: This process can take up to 10 minutes for each. Ensure that everything is correct before uploading.

## Hints and Considerations 
	- Included in the Instructions Folder. 
	
## Output
	- pgAdmin output
[![pg-Admin-4-Output.jpg](https://i.postimg.cc/brmDtYs3/pg-Admin-4-Output.jpg)](https://postimg.cc/gL629WyZ)
