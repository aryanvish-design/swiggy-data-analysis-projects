1. Overall Average Price & Delivery Time Query
   
### 1. Overall Average Price & Delivery Time Query

```sql
SELECT 
    ROUND(AVG(Price), 2) AS Avg_Price, 
    ROUND(AVG(`Delivery time`), 1) AS Avg_Delivery_Time 
FROM swiggy.swiggy;
 ```
Result
<img width="382" height="125" alt="image" src="https://github.com/user-attachments/assets/ba435964-0b1a-4ac5-add0-1ee1f2f157f8" />


### 2. Top 5 Food Types / Cuisines
```sql
SELECT 
    `Food type`, 
    COUNT(*) AS Total_Restaurants,
    ROUND(AVG(Price), 2) AS Average_Price
FROM swiggy.swiggy 
GROUP BY `Food type` 
ORDER BY Total_Restaurants DESC 
LIMIT 5;
```
<img width="407" height="167" alt="image" src="https://github.com/user-attachments/assets/0818a9e7-abac-496f-9ca1-eec645c4f2dc" />
