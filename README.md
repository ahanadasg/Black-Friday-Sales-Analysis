# Black-Friday-Sales-Analysis

## Introduction
This project aims to analyze the Black Friday sales data to gain insights into customer behavior, popular products, and purchase trends during the Black Friday sale. The dataset used for this analysis contains information about customer demographics, product categories, and purchase amounts.

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


## Steps to replicate.
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
Output:
Product_Category_2  Product_Category_3  Purchase  
0                 NaN                 NaN      8370  
1                 6.0                14.0     15200  
2                 NaN                 NaN      1422  
3                14.0                 NaN      1057  
4                 NaN                 NaN      7969  
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 550068 entries, 0 to 550067
Data columns (total 12 columns):
     Column                      Non-Null Count   Dtype  
---  ------                      --------------   -----  
 0   User_ID                     550068 non-null  int64  
 1   Product_ID                  550068 non-null  object 
 2   Gender                      550068 non-null  object 
 3   Age                         550068 non-null  object 
 4   Occupation                  550068 non-null  int64  
 5   City_Category               550068 non-null  object 
 6   Stay_In_Current_City_Years  550068 non-null  object 
 7   Marital_Status              550068 non-null  int64  
 8   Product_Category_1          550068 non-null  int64  
 9   Product_Category_2          376430 non-null  float64
 10  Product_Category_3          166821 non-null  float64
 11  Purchase                    550068 non-null  int64  
dtypes: float64(2), int64(5), object(5)
memory usage: 50.4+ MB
None
User_ID                            0
Product_ID                         0
Gender                             0
Age                                0
Occupation                         0
City_Category                      0
Stay_In_Current_City_Years         0
Marital_Status                     0
Product_Category_1                 0
Product_Category_2            173638
Product_Category_3            383247
Purchase                           0
dtype: int64
            User_ID     Occupation  Marital_Status  Product_Category_1  \
count  5.500680e+05  550068.000000   550068.000000       550068.000000   
mean   1.003029e+06       8.076707        0.409653            5.404270   
std    1.727592e+03       6.522660        0.491770            3.936211   
min    1.000001e+06       0.000000        0.000000            1.000000   
25%    1.001516e+06       2.000000        0.000000            1.000000   
50%    1.003077e+06       7.000000        0.000000            5.000000   
75%    1.004478e+06      14.000000        1.000000            8.000000   
max    1.006040e+06      20.000000        1.000000           20.000000   

       Product_Category_2  Product_Category_3       Purchase  
count       376430.000000       166821.000000  550068.000000  
mean             9.842329           12.668243    9263.968713  
std              5.086590            4.125338    5023.065394  
min              2.000000            3.000000      12.000000  
25%              5.000000            9.000000    5823.000000  
50%              9.000000           14.000000    8047.000000  
75%             15.000000           16.000000   12054.000000  
max             18.000000           18.000000   23961.000000  



10.	Exploratory Data Analysis (EDA)
Countplot for ‘gender’
![image](https://github.com/ahanadasg/Black-Friday-Sales-Analysis/assets/113302918/0637a17f-d567-4887-ad34-7e426d47a514)

Bar plot of purchase by city category
![image](https://github.com/ahanadasg/Black-Friday-Sales-Analysis/assets/113302918/dfd32aa7-30f6-4ebc-8f04-4ebd62d827bf)

Box plot of purchase by gender
![image](https://github.com/ahanadasg/Black-Friday-Sales-Analysis/assets/113302918/8bd621aa-c849-4925-a91a-31b4c517fbca)

Bar plot of purchase by City Category
![image](https://github.com/ahanadasg/Black-Friday-Sales-Analysis/assets/113302918/a8f3389e-daa4-4b4e-ae69-da561ba89220)

11.	Product Analysis: Top 10 products by sales
    Output:
Product_Category_1
1     1910013754
5      941835229
8      854318799
6      324150302
2      268516186
3      204084713
16     145120612
11     113791115
10     100837301
15      92969042
Name: Purchase, dtype: int64

    
12. Analyzing Columns: Check the basic structure of the dataset, including column names, data types, and missing values.
    Output:
Data columns (total 12 columns):
 #   Column                      Non-Null Count   Dtype  
---  ------                      --------------   -----  
 0   User_ID                     550068 non-null  int64  
 1   Product_ID                  550068 non-null  object 
 2   Gender                      550068 non-null  object 
 3   Age                         550068 non-null  object 
 4   Occupation                  550068 non-null  int64  
 5   City_Category               550068 non-null  object 
 6   Stay_In_Current_City_Years  550068 non-null  object 
 7   Marital_Status              550068 non-null  int64  
 8   Product_Category_1          550068 non-null  int64  
 9   Product_Category_2          376430 non-null  float64
 10  Product_Category_3          166821 non-null  float64
 11  Purchase                    550068 non-null  int64  
dtypes: float64(2), int64(5), object(5)

Get summary statistics of the numerical features to understand the data distribution.

Output:
           User_ID     Occupation  Marital_Status  Product_Category_1  \
count  5.500680e+05  550068.000000   550068.000000       550068.000000   
mean   1.003029e+06       8.076707        0.409653            5.404270   
std    1.727592e+03       6.522660        0.491770            3.936211   
min    1.000001e+06       0.000000        0.000000            1.000000   
25%    1.001516e+06       2.000000        0.000000            1.000000   
50%    1.003077e+06       7.000000        0.000000            5.000000   
75%    1.004478e+06      14.000000        1.000000            8.000000   
max    1.006040e+06      20.000000        1.000000           20.000000   

       Product_Category_2  Product_Category_3       Purchase  
count       376430.000000       166821.000000  550068.000000  
mean             9.842329           12.668243    9263.968713  
std              5.086590            4.125338    5023.065394  
min              2.000000            3.000000      12.000000  
25%              5.000000            9.000000    5823.000000  
50%              9.000000           14.000000    8047.000000  
75%             15.000000           16.000000   12054.000000  
max             18.000000           18.000000   23961.000000


    
13.	Multi Column Analysis: Explore relationships between multiple columns using scatter plots, box plots, or other suitable visualizations.

    ![image](https://github.com/ahanadasg/Black-Friday-Sales-Analysis/assets/113302918/5f42ba4f-13ed-41e9-9244-bb1aa96552ff)


 




