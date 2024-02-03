# Sales Data Analysis

## Power BI Dashboard
You can view my interactive Power BI Report [here](https://app.powerbi.com/groups/me/reports/911d94a9-64f4-4143-a1fc-d740c55f23bc/ReportSection?experience=power-bi).
![Sales Analysis](https://github.com/NouraAlgohary/Sales-Analysis/assets/103903785/3c05a35d-db81-4543-8650-d03a9b125c96)

## Project Overview:
This project involves analyzing sales data from an Excel spreadsheet. The primary objective is to create a Power BI report with meaningful visualizations to understand key metrics such as the number of orders, total line total, total tax amount, total freight amount, and total due amount. The project aims to provide insights into sales performance using descriptive statistics and well-designed visuals.

## Project Steps:
### 1. Data Extraction:
Extract data from the provided Excel spreadsheet and model it in a "Star Schema".

![image](https://github.com/NouraAlgohary/Sales-Analysis/assets/103903785/a8c86df9-d7a3-489a-a787-72a0150dff30)

![image](https://github.com/NouraAlgohary/Sales-Analysis/assets/103903785/1570375e-1ec0-4762-9bf6-3a0b35badd0e)

### 2. Data Profiling:
#### 1. Overview:
Dataset Description:
The dataset contains information about sales transactions, including details about the territory, ship method, product, order quantity, unit price, line total, tax amount, freight, and total due.
#### 2. Measures:
- Order Quantity (OrderQty):</br>
Data Type: Numeric</br>
Description: Represents the quantity of products ordered in each transaction.</br>

- Unit Price:</br>
Data Type: Numeric</br>
Description: Indicates the price of a single unit of the product.</br>

- Line Total:</br>
Data Type: Numeric</br>
Description: Represents the total amount for each line item in the order, calculated as the product of order quantity and unit price.</br>

- Tax Amount (TaxAmt):</br>
Data Type: Numeric</br>
Description: Signifies the tax amount associated with the transaction.</br>

- Freight:</br>
Data Type: Numeric</br>
Description: Denotes the cost of shipping for the order.</br>

- Total Due:</br>
Data Type: Numeric</br>
Description: Represents the total amount due for the entire order, including line total, tax amount, and freight.</br>
#### 3. Categorical Columns:
- Territory:</br>
Data Type: Categorical</br>
Description: Specifies the territory associated with each sales transaction.</br>

- TerritoryGroup:</br>
Data Type: Categorical</br>
Description: Indicates the group to which the territory belongs.</br>

- Ship Method ID:</br>
Data Type: Numeric</br>
Description: Unique identifier for the shipping method used in the transaction.</br>

- Ship Method:</br>
Data Type: Categorical</br>
Description: Describe the shipping method employed for the order.</br>

- Product ID:</br>
Data Type: Numeric</br>
Description: Unique identifier for each product.</br>

- Product:</br>
Data Type: Categorical</br>
Description: Specifies the product involved in the sales transaction.</br>

- Product SubCategory:</br>
Data Type: Categorical</br>
Description: Categorizes the product under a specific subcategory.</br>

- Product Category:</br>
Data Type: Categorical</br>
Description: Classifies the product into a broader category.</br>

### 3. Data Cleaning and ETL:
- Profile and clean the extracted data.
- Perform Extract, Transform, and Load (ETL) operations to structure the data for analysis.
- Load the following fields:</br>
DimDate

![image](https://github.com/NouraAlgohary/Sales-Analysis/assets/103903785/aaf64b73-20f4-486c-8121-d6364ffc32c2)

DimProduct

![image](https://github.com/NouraAlgohary/Sales-Analysis/assets/103903785/d60353eb-3f67-4759-a416-5f8e37eba401)

DimShipMethod

![image](https://github.com/NouraAlgohary/Sales-Analysis/assets/103903785/2a708c4c-101b-44ca-9655-7e882022446e)

DimStatus

![image](https://github.com/NouraAlgohary/Sales-Analysis/assets/103903785/56d0a655-286e-471b-b347-781c1b6c9cf1)

DimTerritory

![image](https://github.com/NouraAlgohary/Sales-Analysis/assets/103903785/6abd1eca-1d51-45cf-a902-ebc220e377aa)

FactSales

![image](https://github.com/NouraAlgohary/Sales-Analysis/assets/103903785/1bd7b89e-3049-4e0a-a0c9-d9c4917def6c)
![image](https://github.com/NouraAlgohary/Sales-Analysis/assets/103903785/40233be1-6192-49fc-b006-cf95b57e9b70)


### 4. Create Measures and Visualizations:
#### 1. Measures:
- No. of Orders:
Calculation: Count of unique order IDs.</br>
Purpose: Quantifies the total number of orders.</br>

- Total Line Total:
Calculation: Sum of the Line Total for all orders.</br>
Purpose: Represents the cumulative value of all line items in the orders.</br>

- Total Tax Amount:
Calculation: Sum of the Tax Amount for all orders.</br>
Purpose: Illustrates the total tax incurred across all transactions.</br>

- Total Freight Amount:
Calculation: Sum of the Freight Amount for all orders.</br>
Purpose: Captures the overall cost of shipping for all orders.</br>

- Total Due Amount:
Calculation: Sum of the Total Due Amount for all orders.</br>
Purpose: Provides the total amount due, inclusive of line total, tax amount, and freight.</br>

#### 2. Visualizations:
- No. of Orders by Order Date:
Visualization Type: Line Chart or Bar Chart</br>
Description: Displays the trend in the number of orders over time, allowing identification of peak periods and trends.</br>

- No. of Orders by Status:
Visualization Type: Pie Chart or Stacked Bar Chart</br>
Description: Represents the distribution of orders based on their status, such as 'Pending,' 'Shipped,' or 'Delivered'.</br>

- No. of Orders by Category, Subcategory, and Product:
Visualization Type: Nested Bar Chart or Treemap</br>
Description: Hierarchically showcases the breakdown of orders by product categories, subcategories, and specific products.</br>

- No. of Orders and Total Due Amount by Territory:
Visualization Type: Dual-Axis Bar Chart or Map</br>
Description: Provides a comparison of the number of orders and the total due amount across different territories. This helps identify regions contributing most to sales.</br>

_This documentation serves as a guide for project execution, ensuring a systematic approach to extracting, processing, and visualizing sales data for meaningful insights._

