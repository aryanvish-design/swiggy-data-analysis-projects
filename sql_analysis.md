1. Overall Average Price & Delivery Time Query
   
### 1. Overall Average Price & Delivery Time Query

```sql
SELECT 
    ROUND(AVG(Price), 2) AS Avg_Price, 
    ROUND(AVG(`Delivery time`), 1) AS Avg_Delivery_Time 
FROM swiggy.swiggy;

<img width="382" height="125" alt="image" src="https://github.com/user-attachments/assets/ed7f6f7b-3aad-489e-95d6-229d167263a6" />
