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


### 3. Top Rated Restaurants

```sql
SELECT 
    Restaurant, 
    City, 
    AvgRating, 
    `Total ratings` 
FROM swiggy.swiggy 
ORDER BY AvgRating DESC, `Total ratings` DESC 
LIMIT 5;
```
<img width="552" height="167" alt="image" src="https://github.com/user-attachments/assets/54b6835c-c2de-4084-9be0-83047c5a2db4" />

### 4. City-wise Restaurant Distribution

```sql
SELECT 
    City, 
    COUNT(*) AS Total_Restaurants 
FROM swiggy.swiggy 
GROUP BY City 
ORDER BY Total_Restaurants DESC 
LIMIT 5;
```
<img width="271" height="141" alt="image" src="https://github.com/user-attachments/assets/87a81558-8a02-44fc-a5de-2e611dbeec98" />
