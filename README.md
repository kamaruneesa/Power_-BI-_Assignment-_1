# Power_-BI-_Assignment-_1
## 📝Data Transformation &amp; Data Modeling 
## Power-BI Desktop Window ➡️ Get Data ➡️Transform ➡️Text/csv ➡️List of order
➡️next power query editor ➡️home ➡️new source ➡️text/csv➡️ order details, sales target ➡️open
 **Data Transformation:**
  - **● Restrict the "List of Orders" table to only the first 500 rows: Home tab➡️keep top rows➡️ click ➡️500 ok
  - ** data type 'Date':  Amount and Target column header click➡️fixed decimal number
  - ** Format the "Customer Name" column into proper case: List of order table   "Customer Name" ➡️Add column ➡️Transform➡️Capitalize each word
  - **Merge: ctrl+ select column = "State" and "City" ➡️Add column➡️Merge column➡️ Separator :comma ➡️New column name:Location➡️ok
  - **Create a new custom column :Add column ➡️Profit margin ➡️[profit]/[amount]➡️ok
  - Add a new conditional column named "Profit Status": Add column➡️conditional column➡️ new column name: "Profit Status"➡️condition:
     
   - if profit is less then 0 then "loss"
   - else if profit is = 0 then "Break-Even"
   -else if profit is greater than 0, then "Profit".
 **Merging Data (Joins):** 
  
