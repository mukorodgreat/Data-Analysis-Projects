# Superstore Sales Analysis
I will be carrying out Exploratory Data Analysis of a notable dataset, the Superstore Dataset from Kaggle.com

## Superstore Sales Analysis
This is an exploratory data analysis I performed on the Superstore Sales Data available on Kaggle website [Link]. 
The purpose of this project is to get insights into the Superstore sales data to uncover trends in sales patterns, profit and Customers demography. 
This project is going to be in 5 Phases  
1.	Superstore Sale Data Analysis using Excel
2.	Superstore Sale Data Analysis using SQL
3.	Superstore Sale Data Analysis Python
4.	Superstore Sale Data Analysis using Power BI
5.	Superstore Sale Data Analysis using Tableau

# 1.	Superstore Sale Data Analysis using Excel
![Dashboard](https://github.com/user-attachments/assets/9ba1b4f3-ff8d-4a65-b88f-ffeb1dcee09c)
*Superstore Dashboard with Excel*

In this phase I will be carry out an exploratory data analysis on the Superstore Sales Dataset using the traditional 
Ms. Excel tools and the Ms. Excel Power Query Tools in which produce the above Dashboard  
- A.	Data cleaning and preprocessing
  1. Load the Dataset to Excel:
  2. Inspect and Understand the Data:
  3. Handle Missing Values (If any):
  4. Calculate Summary Statistics:
  5. Data Modelling/Normalization: 
- B.	Data Visualization:
- C.	Hypothesis Testing/ Statistical analysis:
- D.	Documentation:

## A.	Data cleaning and preprocessing
   ### i.	Load the Dataset to Excel:
The downloaded dataset came in csv. (Comma Separated Values) format and I will be using 
**Data Tab > Get External Data > From Text** to load the data to excel worksheet or

![Import1](https://github.com/user-attachments/assets/0f31429f-406f-406d-ba1f-c54c1940363b)

Load and Transform the Data using Power Query Editor

![import3](https://github.com/user-attachments/assets/56a2758a-6d9e-4c1e-8a53-d1bd10c2a106)
**Data Tab > Get and Transform > New Query**

The data will be loaded into the Power Query Editor where we will easily cleanup the data, create new tables among others 
to completely transform the data and Load the transform data into Excel Data Model Environment as shown below.   
![Import4](https://github.com/user-attachments/assets/cba6bbc0-f753-4abc-8138-85777ea24f3f)

   ###  ii.	Inspect and Understand the Data:
        After loading the data, I used Data Tab > Filter to review the dataset to understand its structure, contents and 
        check the column headers and data types to ensure they are correctly interpreted by Excel. The dataset has the following headers/Columns

- Row ID => which contain Unique ID for each row (Each Product in the Order).
- Order ID => Order ID for each Customer Order 
- Order Date => Order Date of the product.
- Ship Date => Shipping Date of the Product.
- Ship Mode=> Shipping Mode specified by the Customer.
- Customer ID => Customer ID of the Customer that Placed the Order.
- Customer Name => Name of the Customer.
- Segment => The segment where the Customer belongs.
- Country => Customer Country of residence.
- City => Customer City of residence.
- State => Customer State of residence.
- Postal Code => Postal Code of every Customer.
- Region => Region where the Customer belong.
- Product ID => Unique ID of the Product.
- Category => Category of the product ordered.
- Sub-Category => Sub-Category of the product ordered.
- Product Name => Name of the Product
- Sales => Sales of the Product.
- Quantity => Quantity of the Product.
- Discount => Discount Allowed.
- Profit => Profit/Loss from the Product.

Note: The data is clean but for the purpose of Feature Engineering and performance, there will be need for Normalization of the 
Dataset because it contains a lot of redundant data which I did using both the traditional Excel tools and the Excel Power Query Tools as shown above.

**Order ID** 
        : A total of 9,994 Products were sold in 5,009 Unique Orders (The Order ID is not Unique in this Column) Multiple Products in each Unique 
        Order ID as shown in the figure below. 
        
![Orderid](https://github.com/user-attachments/assets/2e72b2c1-6b7e-4898-9316-cd1225733fc3)

### iii.	Identifying Unique Values / Handling duplication Values in Excel
In this section I will be fletching unique values that we will need to population the tables we will be creating for this project using 
the “Remove Duplication Function” in Ms. Excel which include 
- Customers
- Products 
- Location 
- Orders
- Sales Table

![Remove Duplicate](https://github.com/user-attachments/assets/db800d51-c4c5-4261-b902-31aeaf6d8e24)

### iv.	Handle Missing Values (If any):
The data in this dataset are clean and did not contain any missing values. However, it is important to note that Ms. Excel can handle missing values (If any) 


### v.	Calculate Summary Statistics:
I will use Descriptive statistics in Microsoft Excel which provide a summary of the main features of Quantity of product Ordered in the Superstory dataset, offering insights into the product order through measures of central tendency, dispersion, and distribution shape. Common descriptive statistics include mean, median, mode, standard deviation, variance, range, minimum, maximum, and more. Below is the result from Ms. Excel which shows the calculations and interpretation these statistics using Excel.
![Statistic Summary](https://github.com/user-attachments/assets/5385eb38-4f8e-42ca-8159-e8919b959b5f)

- Mean: The average quantity every Customer ordered 3.79.
- Standard Error: How much the average order would vary if you picked different groups of orders from the Sales table 0.02.
- Median: The quantity ordered right in the middle when all the ordered quantities are lined up 3.
- Mode: The quantity that the most customers ordered 3.
- Standard Deviation: How much Customers' order vary from the average order 2.23.
- Sample Variance: Another way to show how much Customers' orders vary 4.95.
- Kurtosis: Shows if there were many Customers with very high or very low quantity orders 1.99.
- Skewness: Indicates if more Customers placed lower quantity orders and a few placed really high orders, or vice versa 1.28.
- Range: The gap between the highest and lowest quantity ordered 13.
- Minimum: The lowest quantity ordered in the dataset 1.
- Maximum: The highest quantity ordered in the dataset 14.
- Sum: The total of all the Customers' quantity ordered added together 37873.
- Count: The number of transaction that took place in the dataset 9994.


### vi.	Data Modelling/Normalization 
In this section I will be organizing the data in a database efficiently, which involves creating tables and establishing relationships between these tables based on rules designed to protect the data and make the database more flexible by eliminating redundancy and inconsistent dependency.

The Superstore data can be analysis as it is now, but for the purpose of improve performance in Ms. Excel you can use the **Traditional Excel Tool** or the **Excel Power Query Engine** to create the following tables from this dataset.

1.	**Order Table** (Order ID, Customer ID, Location ID, Order Date, Shipping Date, Segment)
2.	**Product Table** (Product ID, Product Name, Category ID)
3.	**Category Table** (Category ID, Cat Name)
4.	**Subcategory Table** (SubCat ID, SubCat Name)
5.	**Customers Table** (Customer ID, Customer Name, Segment)
6.	**Location Table** (Location ID, City, State, Region, County)
7.	**Fact Sales Table** (Row ID, Order ID, Customer ID, Location ID, Product ID, Sales, Quantity, Discount, Profit) as shown below.

![Org Table](https://github.com/user-attachments/assets/012681bf-fe3a-4fa9-8e7c-43c70e92d93b)


### a.	Creating Table Relationship in Excel.
![Relationship in Excel](https://github.com/user-attachments/assets/208196b4-b445-4de3-b654-7aa99c2fa433)

After creating all the above mentioned tables, I created Relationships to relate all the tables in the Data Model using the Relationship button in Excel **Data Tab** which can also be done by using Click and drag in **Diagram View** of the **Manage Data Model** Window as shown above. And below is the **Diagram View** of the Data Model in the **Manage Data Model** Window of Excel.

![Data Model](https://github.com/user-attachments/assets/e039bc93-6e12-48b8-938a-640e3c70af13)

#### i.	Outcome of Data Modelling/Normalization 
After carrying out this step, each of the tables was well organized by pulling all the related columns into their individual tables as shown above.
After creating the tables and fletching the Unique data into the individual tables, the data shows that 
1.	Orders: There are 5,009 Unique Orders (Multiple items in an order)
2.	Customers: There are 793 Unique Customers
3.	Products: There are 1,862 Unique Products
4.	Location: There are 531 Unique Locations

#### ii. Calendar Table
In addition to the above created tables, I created a Calendar table which is simply a table of all the consecutive dates between the selected start and end date. Each row contains one date and is thus unique. Beside the date the table usually contains attributes like year, quarter, month, day, day of week, week of year etc.  which is an essential part of every data modelling and analysis. One of its major advantage is that as the data grows, the Calendar table is automatically update.



## B.	Data Visualization:
Here we will use various visualization techniques, such as histograms, scatter plots, box plots, and heat-maps to visually explore the data and identify patterns or trends that may not be immediately apparent from the summary statistics alone. 

In this section I took advertage of the **Ms Excel Power Pivot** to create carry out my analysis before creating the Dashboard as show below

![Dashboard](https://github.com/user-attachments/assets/cb979e7a-3674-47a0-a7e6-14bd5d0b9f6a)

## C.	Hypothesis Testing/ Statistical Analysis:
Hypothesis Testing: 
Here we will test hypotheses or assumptions about the data. This may involve comparing different groups or categories within the data to see if there are significant differences or correlations.

Below are some of the analysis done us Power Pivot
### 1. Profitability 

#### A. Profit By Region	
![image](https://github.com/user-attachments/assets/2db65d4f-b43a-4fd3-b818-0afd1dd79877)

#### B. Profit By Sub-Category		
![image](https://github.com/user-attachments/assets/34462649-a688-4f91-87d7-9ba047253360)

#### C. Profitable Months	
![image](https://github.com/user-attachments/assets/2ad69c69-250f-49d4-b857-5fd90f15e210)

#### D. Top 5 Profitable States	
![image](https://github.com/user-attachments/assets/bcbde224-3929-4327-8761-013524d2beee)

#### E. Least 3 Profitable Products	
![image](https://github.com/user-attachments/assets/4cfea6d6-dd3c-467a-a888-42d543de72a5)


### 2. Customers Distribution/Demography

#### F. Least 5 States with the Lowest Number of Customers and Sales		
![image](https://github.com/user-attachments/assets/a0df5cfc-4186-482c-b301-b3bbe49679af)












