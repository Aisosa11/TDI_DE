# TDI_DE
The aim of the project was to focus on data exploration, cleaning, and analysing datasets with Pandas. The dataset used was titanic dataset.
Started by importing all the libraries that would be needed such as Pandas, Numpy, seaborn and matplotlib for charts.
Dataset was downloaded from kaggle https://www.kaggle.com/datasets/brendan45774/test-file and using google colab, I had to first write a line of code allowing me upload file from my local drive into google colab.
After importing the file the data was read into a dataframe called *df* and to display the first few rows of the data I use the *.head()* function.
When working on a dataset the first step is checking and eliminating null values, We can simply do this by finding null and replacing with average of each columns. Also, we can remove columns which are not needed such as the Names, etc.To perform this i used the *drop function* to drop columns not needed and I looped through columns to check for missing values and replace with median values and missing columns in Embarked columns to "U" to signify Unknown routes.
I used the "describe" function to  check column arrangement  and df.info() to check the data type of each columns.
I created two  dataframe from an existing dataframe *(df_num and df_cat)* to separate categorical data from numerical data.
After which I looped through the created dataframe df_num which then creates a series of histograms visualizing the distribution of numerical values within a single column which allows exploration of the spread, central tendency, and potential outliers in the numerical data.
I also performed the same for the categorical columns in DataFrame named df_cat and created separate bar charts for each column visualizing the distribution of values within a single categorical column of the DataFrame df_cat. It allows you to quickly visualize the data distribution across different categorical variables.
I grouped the data by Survivors and non-survivors for each Pclass,Sex and Embarked which was helpful to provide insights on how survival rates were affected by passenger class, gender, and embarkation port on the Titanic.
To get surviaval and non survival by age group I created a list called age_bins,and created a dataframe called Age Group which is used to calculate survival across different age brackets.
I also created a grouped data using the *groupby function* and the *mean function*,I was able to get the average survival rates based on gender and passenger class, a Bar chart was used for visualization.
