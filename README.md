# PRODIGY_DS_02
Perform data cleaning and exploratory data analysis (EDA) on a dataset of your choice, such as the Titanic dataset from Kaggle. Explore the relationships between variables and identify patterns and trends in the data.

## Purpose
PRODIGY_DS_02 is a project where I have been assigned to perform data cleaning and exploratory data analysis (EDA) on a dataset of my choice. The primary goal is to explore the relationships between variables and identify patterns and trends in the data.

## Description
This repository contains the code and datasets used for performing data cleaning and EDA. The datasets have been collected from Kaggle, and software such as Jupyter notebooks along with Google Colab has been used for analysis.

## Usage
Users can explore the code and datasets provided in this repository to understand how to perform data cleaning and EDA on a dataset. The code is explained in detail, step by step, to help users understand each aspect of the analysis process.
### Process:
This section imports the necessary libraries for data manipulation and visualization also reads the three CSV files into Pandas DataFrames:
![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/e6b73474-1194-4adf-9cf4-98cc2a8da636)

This code displays the contents of the train_data DataFrame, showing the first few rows of the dataset in a tabular format.Similarly for gender_submissiondata and test_data:![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/7de1cb6c-91b9-4673-9b55-c834afe8d00d)
![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/f6eda1f1-a5d2-46b4-a811-b61a213072fd)
![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/1f2e48f2-1adf-4d65-b746-0c2a43088363)

We also used multiple method and function such as head and tail to display the first and last (by default 5) data. And info was used to display data types and other details whereas shape was used to define size. We also used groupby to sort the data accordingly.
![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/392fdff0-a467-4e17-8c1d-ff3c44412fe9)
![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/ea44eeef-4520-42c2-8d7e-d9d327f1e8a6)
![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/39fc97f9-ebbc-4c37-9e18-3b1384561cba)

We tried removing duplicates if it existed in the data by following code:
![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/e9fc4cfa-a4f0-4752-beea-f0925d60079b)

We find which columns have non-number information (like names, categories) and make a list of them.We used ".dtypes" for this.We separate columns with numbers (like ages, prices) and find missing values in them.For missing numbers, we put in the average value of each column.We look at the dataset to see what it looks like after we've filled in the missing numbers with averages.
![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/02883200-8539-4dc7-94a8-266a50aee47f)

Then we did the folloeing:
1. **Removing Outliers:**
   - We define a function called `remove_outliers` that takes a DataFrame (`df`) and a column name (`column`) as inputs.
   - Inside the function, we calculate the lower and upper bounds for outliers using the Interquartile Range (IQR) method.
  
2. **Applying Outlier Removal:**
   - We apply the `remove_outliers` function to the `train_data` DataFrame for the 'Age' and 'Fare' columns separately.
   - This removes outliers from these columns in the `train_data` DataFrame.

3. **Visualizing Relationships:**
   - Finally, we create a pair plot using Seaborn's `pairplot` function.
   - The pair plot shows the relationships between 'Age', 'Fare', and 'Survived' columns from the cleaned `train_data`.
   - The points are colored based on whether the passenger survived or not (`hue='Survived'`). 


![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/133afbc1-a8c4-4d36-a1cc-1c4a0b4dd94c)
![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/7a20bc85-aac1-41c8-9ecb-7c98c25f5d21)
![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/da6514ae-6c5d-479e-a611-119c99617c95)

We then created statistics for all the data and plotted necessary graphs:
![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/cd5ff323-6671-4dbc-8a4d-b63cbff9d5e8)
![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/4a121df1-7d39-4873-8c96-0a780db6d5fa)
![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/a6a76e0b-26d0-464f-9cc8-b441dfe849c9)
![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/79478d12-4960-4929-94cc-bb72e3baac94)
![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/b21e19fa-2eea-4dcf-bed1-bbc62fdbe169)
![image](https://github.com/aarya-09/PRODIGY_DS_02/assets/126316004/b64b749a-88a6-4c52-a978-d7845688b091)



## Contributing
Feedback and contributions are appreciated. If you have any suggestions, improvements, or find any issues with the code or analysis, please feel free to open an issue or submit a pull request.

## Reference dataset
Attached above.
