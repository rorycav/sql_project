#
# sql_project
Group NAME:
61608 Group 3
|
Database name: ha_group_crn61608
## Team Members
1. Cavanaugh, Rory
2. Chadha, Jasmine
3. McNally, Owen
4. Mulnix, Hayden
5. Nguyen, Timmy
## Problem Discription
Our Starbucks Database is designed to enhance the quality and efficiency of service at our local college coffee shop. It provides a comprehensive view of key operations, including ingredients used in food and beverages, menu offerings, sales transactions, and employee performance. This database enables us to generate valuable insights for improving sales revenue, tracking employee performance, and implementing targeted marketing strategies. With this system, Starbucks management can optimize operations, streamline service, and maximize overall efficiency.
## Data Model
This database models Starbucks' operational efficiency by tracking food and drink sales, ingredient usage, and employee performance. Ingredients are linked to both food and drink entities through a many-to-many relationship, as a single ingredient in inventory can be used in multiple food and drink items. This relationship forms the weak entities food_ingredients and drinks_ingredients, which associate each food or drink item with its corresponding ingredients.

For example, both a Caramel Cold Brew and a Caramel Frappuccino contain sugar and caramel. By structuring the database this way, we enable inventory tracking and supply chain analysis, allowing Starbucks to optimize ingredient management.

Similarly, the receipt entity records food and drink transactions, creating a many-to-many relationship between food and drink items and their sales. The weak entities food_sold and drink_sold capture the food or drink ID and the corresponding receipt(s), enabling the analysis of sales frequency and item demand.

Additionally, the receipt entity is linked to employees through a one-to-many relationship, as one employee can handle multiple sales, but each sale is attributed to a single employee. This structure supports performance evaluation by tracking individual employee contributions to sales. This performance data can be used by Starbucks to see which employees are operating most efficiently at certain times of the day. Employee data, including tenure and position, can further be used for workforce analysis.

By leveraging SQL queries from data being stored within this data model, key business insights can be extracted, such as best-selling items, peak sales times, and ingredient consumption patterns, all of which help Starbucks streamline operations and maximize efficiency.

<img width="876" alt="Screenshot 2025-03-14 at 11 59 38 AM" src="https://github.com/user-attachments/assets/423f405d-1a30-483e-8bd2-983bf4f3bbe9" />
## Data Dictionary
<img width="478" alt="Screenshot 2025-03-14 at 12 01 19 PM" src="https://github.com/user-attachments/assets/18fcbf02-11f1-404f-ad27-ab435bee11ee" />
<img width="476" alt="Screenshot 2025-03-14 at 12 01 44 PM" src="https://github.com/user-attachments/assets/71a2013d-9eaf-4855-b22e-10ccf94fcd6b" />
<img width="489" alt="Screenshot 2025-03-14 at 12 02 05 PM" src="https://github.com/user-attachments/assets/1c3e0556-266e-439f-bfef-ab8649d1035e" />
## Queries
Simple Query 1: Query 1 displays the receipt IDs, total sale value, date of transaction, time of transaction, and employee IDs
<img width="790" alt="Screenshot 2025-03-14 at 12 07 48 PM" src="https://github.com/user-attachments/assets/97a2d4dc-17cd-4d3a-9d23-d073646ff0fa" />
This query provides management insight on transactions during a specified date. Management can analyze how sale price fluctuates throughout the day, as well as the success or failure of certain employees during the day.
Simple Query 2:
This query displays the total revenue of the Starbucks
<img width="793" alt="Screenshot 2025-03-14 at 12 08 42 PM" src="https://github.com/user-attachments/assets/358d94d7-2629-4be1-9e31-e3995830630e" />
Management is able to use this query as a flat numerical value to judge their performance, which can be useful on a broad scale. 
Simple Query 3:
This query lists the foods Starbucks has to offer, order by price in descending order.
<img width="790" alt="Screenshot 2025-03-14 at 12 09 32 PM" src="https://github.com/user-attachments/assets/86be0b3f-744b-489a-b412-f14097cb752b" />
This is helpful to management as they are able to identify which products would generate the most revenue. This allows managers to create target promotions to push high priced item.
Simple Query 4:
This query lists each food item offered, and the ingredients included in that food.
<img width="792" alt="Screenshot 2025-03-14 at 12 10 18 PM" src="https://github.com/user-attachments/assets/064e6670-aa94-4b59-ad8e-23cdd13dd74c" />
Managers will be able to use this information to track ingredient usage, and ultimately reduce waste. This could also be used to forecast supply needs, as some ingredients may belong to 10+ items versus another ingredient might only belong to 1 or 2.
Query 5:
This query displays the highest sold food item with the most ingredients.
<img width="787" alt="Screenshot 2025-03-14 at 12 11 08 PM" src="https://github.com/user-attachments/assets/39049e05-0428-4ab3-bc17-a836fea5f075" />
This can be useful for management as they are able to clearly identify which food item is their best seller, but is costing them the most in terms of ingredients usage. This could lead management to search for alternative ingredient options that would allow for less waste and a greater profit margin.
Query 6:
This query displays side by side the food versus drink revenue.
<img width="786" alt="Screenshot 2025-03-14 at 12 11 53 PM" src="https://github.com/user-attachments/assets/b2aa43b8-8028-4ac3-8575-aa5418034efe" />
By breaking down revenue into food sales and drink sales, it allows management to compare performance between these categories.This query is a simple yet powerful tool for Starbucks management to track sales performance, optimize inventory, and improve marketing strategies by analyzing the contribution of food and drinks to overall revenue.
Query 7:
This query displays the drink name and the corresponding total time it has sold
<img width="791" alt="Screenshot 2025-03-14 at 12 12 55 PM" src="https://github.com/user-attachments/assets/8531efec-ce04-4076-89d5-48009d14c8cb" />
By counting the number of times each drink has been sold and organizing the results in descending order, management can quickly identify the most and least popular beverages. This insight helps in menu optimization, allowing decision-makers to determine which drinks should be promoted, discounted, or potentially removed from the menu
Query 8:
This query displays the employees name and id as well as how long they have worked at the starbucks and the total sales they have generated.
<img width="788" alt="Screenshot 2025-03-14 at 12 14 07 PM" src="https://github.com/user-attachments/assets/9180c130-ea13-48af-b038-8f2a9028eb88" />
This query would prove to be beneficial to Starbucks management as it provides valuable insights into employee performance and experience. By displaying each employee's total sales alongside their tenure, managers can assess how experience correlates with sales performance. Employees with longer tenure may be expected to generate higher sales due to their familiarity with products and customer service skills. However, if newer employees are performing equally well or better, it could indicate strong training programs or highlight high-performing individuals who may be suited for leadership roles.
Query 9: This query specifically retrieves the total revenue generated by each employee from food sales on March 10, 2024 and ranks them in descending order.
<img width="791" alt="Screenshot 2025-03-14 at 12 15 10 PM" src="https://github.com/user-attachments/assets/0394c72d-0a65-4d89-8004-1295df3de2d8" />
While this specific example is limited to March 10, 2024 the query can be edited to pull up any date of operations. The query also identifies the maximum revenue earned by an employee on a given day, making it a clear easy process to highlight top performers and optimize staffing decisions based on revenue contribution.
Query 10: This query shows the total number of hours worked, sales made, revenue acquired, and average revenue per sale for each hour in a given day.
<img width="789" alt="Screenshot 2025-03-14 at 12 15 56 PM" src="https://github.com/user-attachments/assets/59f5a6c8-927b-4744-acf2-2ccc69793f5d" />
This query would help Starbucks identify peak and slower hours, allowing them to prepare for better staffing and inventory management. By identifying and understanding hourly sales trends, the Starbucks on Alps can optimize scheduling and promotions to maximize revenue. 
## Database Information
<img width="989" alt="Screenshot 2025-03-14 at 12 17 17 PM" src="https://github.com/user-attachments/assets/d590c8da-d6da-4bbc-848e-c67e6614e7cd" />
















