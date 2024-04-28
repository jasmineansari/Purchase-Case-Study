# Purchase-Case-Study
Spearheaded the refinement of data, intertwining it with an intricate analysis. Deployed visually engaging graphical representations for  astute data comprehension. Applied the One Sample Test for Mean &amp; Proportion and Two Sample Test for Proportion &amp; Mean to distill  discerning conclusions.

### Dataset Description
The provided Jupyter notebook analyzes a dataset related to customer purchases. The dataset contains the following columns:

1. **User_ID**: A unique identifier for each customer.
2. **Product_ID**: A unique identifier for each product.
3. **Gender**: The gender of the customer (F or M).
4. **Age**: The age group of the customer (0-17, 18-25, 26-35, 36-45, 46-50, 51-55, 55+).
5. **Occupation**: The occupation of the customer (represented by an integer value).
6. **City_Category**: The category of the city the customer lives in (A, B, or C).
7. **Stay_In_Current_City_Years**: The number of years the customer has stayed in the current city (2, 3, 4, or 4+).
8. **Marital_Status**: The marital status of the customer (0 or 1).
9. **Product_Category_1**: The primary product category purchased by the customer.
10. **Product_Category_2**: The secondary product category purchased by the customer (some values are missing).
11. **Product_Category_3**: The tertiary product category purchased by the customer (many values are missing).
12. **Purchase**: The total purchase amount by the customer.

### Data Preprocessing
1. **Data Cleaning**: The notebook starts by importing the necessary libraries (numpy, pandas, matplotlib, and seaborn).
2. **Data Loading**: The dataset is loaded from a CSV file named "train.csv".
3. **Data Exploration**: The `data.info()` function is used to explore the dataset, revealing the data types and the number of non-null values for each column.
4. **Handling Missing Values**: The notebook identifies that some columns (Product_Category_2 and Product_Category_3) have missing values. To address this, the rows with missing values are dropped using `data.dropna()`.
5. **Feature Engineering**: The categorical features (User_ID, Product_ID, Gender, Age, City_Category) are encoded using the LabelEncoder from the scikit-learn library.

### Data Analysis
1. **Unique Values**: The unique values for various columns are explored, such as the unique User_ID, Product_ID, Age, and City_Category.
2. **Null Value Analysis**: The number of null values in each column is checked using `data.isnull().sum()`.

### Potential Next Steps
The notebook provides a solid foundation for further analysis and modeling on the customer purchase data. Some potential next steps could include:

1. Exploratory Data Analysis (EDA): Perform more in-depth analysis and visualization to understand the relationships between different features and the target variable (Purchase).
2. Feature Engineering: Create additional derived features from the existing ones to potentially improve the predictive power of the model.
3. Model Building and Evaluation: Implement various machine learning algorithms (e.g., regression, classification) to predict the purchase amount or whether a customer will make a purchase.
4. Hyperparameter Tuning: Optimize the performance of the chosen models by tuning their hyperparameters.
5. Model Deployment: Deploy the trained model to make predictions on new, unseen data.

By building upon the foundation laid in this notebook, we can further explore the customer purchase data and develop insights that can inform business decisions.
