# Power_-BI-_Assignment-_1
## 📝Data Transformation &amp; Data Modeling 
## Power-BI Desktop Window ➡️ Get Data ➡️Transform ➡️Text/csv ➡️List of order
➡️next power query editor ➡️home ➡️new source ➡️text/csv➡️ order details, sales target ➡️open

**Data Transformation:**
  - 1) Restrict the "List of Orders" table to only the first 500 rows: Home tab➡️keep top rows➡️ click ➡️500 ok
  - 2)data type 'Date' :Date column header click➡️fixed Date  (using this didn't change it in the main window, change power query window, used locale too ,same result.)data view window➡️order date column click & select ➡️column tools ➡️formatting ➡️format: dd/mm/yyyy➡️ok 
  - 3)data type:Amount and Target column header click➡️fixed decimal number
  -  3)Format the "Customer Name" column into proper case: List of order table   "Customer Name" ➡️Add column ➡️Transform➡️Capitalize each word
  - 4)Merge: ctrl+ select column = "State" and "City" ➡️Add column➡️Merge column➡️ Separator :comma ➡️New column name:Location➡️ok
  - 5)Create a new custom column :Add column ➡️Profit margin ➡️[profit]/[amount]➡️ok
  - 6)Add a new conditional column named "Profit Status": Add column➡️conditional column➡️ new column name: "Profit Status"➡️condition:
     
   - if profit is less then 0 then "loss"
   - else if profit is = 0 then "Break-Even"
   -else if profit is greater than 0, then "Profit".

 **Merging Data (Joins):**
  - Merge the "List of Orders" and "Order Details" tables : Home tab➡️merge queries➡️ select tables ➡️left outer join ➡️ok


**Handling Missing Data & Duplicate Data:**

  - Identify missing values:Remove Error
  - Handle duplicates: Remove Duplicates


**Sorting and Filtering Data:**

  - Sorting :Order date column ➡️filter icon click ➡️Short Descending
  - Filtering:Order date column ➡️filter icon click ➡️Tamil Nadu-check,all-uncheck➡️ok
    
 **Grouping and Aggregating Data:**

 - “Order Details” table :Oder table right click ➡️Reference➡️select new table➡️Home➡️Transform ➡️Group By➡️
        - calculate the count of each Order ID: Basic➡️ Order ID ➡️new column name:count of Order ID,Operation: count rows
        -   average profit by Category :Oder table right click ➡️Reference➡️select new table➡️Home➡️Transform ➡️Group By➡️
              ADVANCED ➡️ Add aggregation ➡️new column name: average profit,Operation: average,column:profit
        - total amount by Sub-Category: Oder table right click ➡️Reference➡️select new table➡️Home➡️Transform ➡️Group By➡️
              ADVANCED ➡️ Add aggregation ➡️new column name: average profit,Operation: average,column:profit

- the total target amount: Sales Traget  right click ➡️Reference➡️select new table➡️Home➡️Transform ➡️Group By➡️
         Basic➡️ Month of Order Date ➡️new column name:Total Target,Operation: sum,column:target




**Data Modeling:**
 - Relationship between the “List of Orders” and “Order Details” tables: Model view ➡️List of order id table➡️ drag order id ➡️ order details table ➡️connect order id:  cardinality =many to many

-  Relationship between the “Order Details” and “Sales Target” tables :Model view ➡️“Order Details” ➡️drag category ➡️ “Sales Target” ➡️connect category .  cardinality=many to many



  


   






  
