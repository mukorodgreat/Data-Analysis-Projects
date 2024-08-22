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
        - I.	 Load the Dataset to Excel:
        - II.	 Inspect and Understand the Data:
        - III. Handle Missing Values (If any):
        - IV.	 Calculate Summary Statistics:
        - V.	 Data Modelling/Normalization: 
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





