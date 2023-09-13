# Black-Friday-Sales-Analysis

## Introduction
This project aims to analyze the Black Friday sales data to gain insights into customer behavior, popular products, and purchase trends during the Black Friday sale. The dataset used for this analysis contains information about customer demographics, product categories, and purchase amounts.

## Link to Sales Dashboard
https://sales-analysis-dashboard.streamlit.app/

## Data Source
The dataset used for this analysis is sourced from Kaggle. It contains the following columns:
User_ID	
Product_ID	
Gender	
Age	
Occupation	
City_Category	
Stay_In_Current_City_Years	
Marital_Status	
Product_Category_1	
Product_Category_2	
Product_Category_3	
Purchase


## Steps to replicate
1.	Explore Kaggle Datasets:
Go to the Kaggle Datasets page (https://www.kaggle.com/datasets) to explore the available datasets. You can search for specific datasets using keywords or browse through various categories.

2.	Select a Black Friday Sales Dataset:
Look for a dataset that interests you or aligns with your analysis objectives.Click on a dataset to access its details, including a description, file format, size, and any associated kernels or notebooks.
3.	 https://www.kaggle.com/datasets/pranavuikey/black-friday-sales-eda
Using the above dataset for current project.

4.	Download the Dataset:
If the dataset is available for download, click the "Download" button to save it to your local machine. Make sure to note the file path where you downloaded the dataset.

5.	To load a dataset using Python in Google Colab, follow these steps:
Access Google Colab:
Go to https://colab.research.google.com/ and sign in with your Google account.
If you don't have a Google account, you can create one for free.
Create a New Colab Notebook:
Click on the "New Notebook" button to create a new Colab notebook.

6.	Upload the Dataset to Google Colab:
In google colab, you can upload a CSV file using this line of Code.
from google.colab import files
upload=files.upload()
When you run this cell, you will receive a prompt to “browse” your files and upload the file that you want to upload.

7.	After you have uploaded the CSV file, now it is time to read the CSV file. 

8.	Let's walk through a basic Black Friday sales data analysis using Python and some popular data analysis libraries like Pandas and Matplotlib. 
9.	Explore the data: Display the first few rows of the dataset; Get a summary of the dataset; Check for missing values; Describe the numerical columns

10.	Exploratory Data Analysis (EDA)
Countplot for ‘gender’
![image](https://github.com/ahanadasg/Black-Friday-Sales-Analysis/assets/113302918/c3c20d31-fe80-478f-b930-0300492fce03)


Bar plot of purchase by city category
![image](https://github.com/ahanadasg/Black-Friday-Sales-Analysis/assets/113302918/26bb2f45-4f40-4a96-8ea7-2f074ec3cff0)


Box plot of purchase by gender
![image](https://github.com/ahanadasg/Black-Friday-Sales-Analysis/assets/113302918/8bd621aa-c849-4925-a91a-31b4c517fbca)

Bar plot of purchase by City Category
![image](https://github.com/ahanadasg/Black-Friday-Sales-Analysis/assets/113302918/a8f3389e-daa4-4b4e-ae69-da561ba89220)

11.	Product Analysis: Top 10 products by sales
  
12. Analyzing Columns: Check the basic structure of the dataset, including column names, data types, and missing values. Get summary statistics of the numerical features to understand the data distribution.

    
13.	Multi Column Analysis: Explore relationships between multiple columns using scatter plots, box plots, or other suitable visualizations.

    ![image](https://github.com/ahanadasg/Black-Friday-Sales-Analysis/assets/113302918/5f42ba4f-13ed-41e9-9244-bb1aa96552ff)

14. Steps to create visualization dashboard using Streamlit
  i.	Install Streamlit in your machine.

  ii.	Create a .py file which contains the necessary code in python to visualize the dataset in Streamlit.
  
  iii.	Open cmd. Type cd<space>“Name of directory in which your .py file is located”
  Example: cd Downloads
  
  iv.	Next, let us assume the name of the python file is excel_dashboard.py.
  
  v.	In cmd type “streamlit run excel_dashboard.py”
  
  vi.	Make sure you have the .py file and the csv/excel dataset in the same folder.
  
  vii.	Link to dashboard: http://192.168.100.5:8501


## Conclusion
The Black Friday Sale Analysis project provides valuable insights into customer behavior, product preferences, and purchase trends during the Black Friday sale. The findings can be used to optimize marketing strategies, product offerings, and customer targeting for future sales events.


 




