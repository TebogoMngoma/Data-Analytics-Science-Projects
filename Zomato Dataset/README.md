# Zomato Dataset
## About Dataset
This dataset is a collection of restaurants that are registered on Zomato in Bengaluru City. In this dataset, we have more than 50000 rows and 17 columns, a fairly large dataset
### Our Goals and Objectives of this dataset are :
- Handling Missing Values
- Explore numerical features.
- Explore categorical features.
- Finding relations between features.
### Data Cleaning
- Deleting redundant columns.
- Renaming the columns.
- Dropping duplicates.
- Cleaning individual columns.
- Remove the NaN values from the dataset
- Check for some more Transformations
### Data Visualization
- Restaurants delivering Online or not
- Restaurants allowing table booking or not
- Table booking Rate vs Rate
- Best Location
- Relation between Location and Rating
- Restaurant Type
- Gaussian Rest type and Rating
- Types of Services
- Relation between Type and Rating
- Cost of Restaurant
- No. of restaurants in a Location
- Restaurant type
- Most famous restaurant chains in Bengaluru

### Packages and Libraries used for the project
- Matplotlib
- Pandas
-  Seaborn
-  Numpy 

## Exploratory Data Analysis
Exploratory data analysis (EDA) is a method of analyzing and summarizing a dataset in order to understand its main characteristics and relationships between variables. EDA is typically the first step in the data analysis process, and it involves visualizing and summarizing data in various ways to get a feel for the data and uncover patterns and trends. EDA is important because it helps to identify potential issues with the data, such as missing values or outliers, and it helps to guide the next steps in the data analysis process.
- Using the **shape** command , we can observe that our dataset has 51717 rows and 17 columns
- the **isnull()** commands shows our dataset has 37700 missing(null) values
- the **info()** command shows us that the data consists of a single numerical column(feature) **Votes** while the remaining 16 are catagorical.(later in data cleaning we will transform some of the features to numerical)
our dataset is mostly straighfoward and hence why our EDA is not that long 
## Data Cleaning
Data cleaning is the process of identifying and correcting errors, inconsistencies, and missing values in a dataset. It is an important step in the data analysis process because dirty or incomplete data can lead to incorrect or misleading results. Data cleaning typically involves a combination of automated procedures and manual inspection and correction of the data.
- First step is to remove **redundant** features as they have little to no impact in our dataset
- The removed features are namely **[phone, url,reviews_list,menu_item,address,dish_liked,cuisines]**
- Second step is two drop all null(missing) values in our data as null values Null values can affect the accuracy of data analysis: If a null value is included in a calculation, it can produce an incorrect result. For example, if you are trying to calculate the mean of a set of values and one of the values is null, the result of the calculation will be affected.
- the third step is to transform the **approx_cost** feature from catagorical to numerical as it a string and will give us issues when plot visual later and so it has to be numerical to perform calculations.
- the fourth step is to also transform the rate feature from catagorical to numerical with the same explanation as the third step
- the fifth and last step is to rename some of the feature names to make them more readable and understandable e.g we rename the **'name'** feature to **'restuarant_name'**





