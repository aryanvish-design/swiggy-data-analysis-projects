1. Overall Average Price & Delivery Time Query
   
### 1. Overall Average Price & Delivery Time Query

```sql
SELECT 
    ROUND(AVG(Price), 2) AS Avg_Price, 
    ROUND(AVG(`Delivery time`), 1) AS Avg_Delivery_Time 
FROM swiggy.swiggy;
 
Result
<img width="382" height="125" alt="image" src="https://github.com/user-attachments/assets/ba435964-0b1a-4ac5-add0-1ee1f2f157f8" />
