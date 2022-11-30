# Big Data Challenge

## Contributor: Sam Espe

### Overview

This was done as a submission for Homework #22 for Data Visualization and Analysis Boot Camp. The goal was to Extract, Transform, and Load two data sets from Amazon (customer reviews)(https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt) into a PostgreSQL database in the Amazon Web Services cloud. I chose to work with the Toys and Musical Instruments data sets. I used PySpark version 2.3.3 in a Google Colab notebook to perform the ETL process. The notebooks are located in the `Level 1` folder. The Google Colab files are also available at the following links: (Toys Data ETL)[https://colab.research.google.com/drive/1QRHL0xbpaXhElZWde3vpDfcbVemELkOd?usp=sharing] | (Musical Instruments ETL)[https://colab.research.google.com/drive/1pynUpKpLAacSrW2bHqmfBKwORtQnisC_?usp=sharing].


### To Replicate the Database:
1. Create an Amazon Web Service RDS PostgreSQL database with the same name as the `aws_database_name` parameter in the `PostgreSQL Set Up` section.
1. Populate the `aws_endpoint` and `aws_password` fields so they match the values for your AWS PostgreSQL database.
1. In PGAdmin (or similar program), create a PostgreSQL database with the same name as the `aws_database_name` parameter in the `PostgreSQL Set Up` section.
1. Copy the code from the `schema.sql` file (located in the `Resources` folder) into a query tool to create the tables in your local copy of PostgreSQL.
1. Run the Google Colab to extract, transform, and load the data.

I recommend using Google Colab to run the `.ipynb` files instead of Jupyter Notebook, since the files establish an environment in which the code will execute properly.
