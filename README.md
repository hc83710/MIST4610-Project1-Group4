# MIST4610-Project1-Group4

## Team Name: 
61608 Group 4

## Team Members:
1. An, Ben [@benan03](https://github.com/benan03)
2. Burt, Keegan[@keeganburt24](https://github.com/keeganburt24)
3. Cheng, Hsin [@hc83710](https://github.com/hc83710)
4. Cho, Nick [@nichooo4](https://github.com/nichooo4)
5. Shields, David [@DubNation44](https://github.com/DubNation44)

## Problem Description:
Our database system is designed to support a sports betting platform where users can analyze statistics before placing wagers on teams or players. Utilizing advantages of data and information systems, we replace the uncertainty of gut feeling with objective, accurate, informative, and integrated tables for bettors to visualize waging factors. The database system has the ability to track and visualize relationships between teams, coaches, conferences, games, players, and players' statistics to better apply to winning money via sports bets. Examples of ways to achieve this function include: 1. calculates and presents betting odds based on player statistics, 2. comparisons on team performances to conclude conference standings, and 3. tailored betting (e.g. Best offensive teams)


## Data Model:
((((((((This data model showcases a grocery store's operational data, including products, inventory, sales transactions, and employee details. The Product entity is linked to both Category and Brand, allowing for the organization of products by type (e.g., dairy, beverages) and tracking of the brand of the products. The Inventory entity tracks product stock levels, restock quantities, and dates, ensuring that the store remains well-supplied. Sales data is captured through two interconnected tables: Sales Transaction, which logs overall transaction details like payment type and total price, and Sales Transaction Details, which records the specific products and quantity sold in each transaction. Lastly, the Employee entity connects staff members to the sales they process, supporting workforce management and performance tracking. The relationships between these entities ensure comprehensive data storage for managing day-to-day operations.

The Product entity serves as the foundation of the data model. It stores the product name, description, price, and expiration date. Category and Brand use the Product entity as the linking entity in a many-to-many relationship. A brand can be associated with many categories and a category can be associated with many brands. 

The Inventory entity has a one-to-one relationship with Product because this entity is used to simply connect the inventory information to each product.

When it comes to the Sales Transaction entity, this is connected to the Product entity through a one-to-many relationship. A product can be included in many sales transaction details, but when it comes to the specific sale transaction, each detail must be associated with one product. The Sales Transaction relates directly to the transaction details.

Finally, Employee has a one-to-many relationship with the Sales Transaction entity. Employees could have worked at plenty of sales transactions, but a sales transaction can only have one employee. The Employee entity and its relationships are used to track which employees are working which sales, allowing the grocery store to have input on its employees.))))))

![Data_Model](https://github.com/user-attachments/assets/a2e4bf50-2e38-4a40-92ce-d02d03172aee)


## Data Dictionary:
![Data_Dictionary](https://github.com/user-attachments/assets/47eb73a7-5864-40f7-b4e3-c04a5045aceb)
![Data_Dictionary](https://github.com/user-attachments/assets/6ee9fd21-6ef8-422a-ba4a-3fcd4a28619b)
![Data_Dictionary](https://github.com/user-attachments/assets/5f5f88e1-2fc2-4668-98f4-7bbcc1c0d9b2)
![Data_Dictionary](https://github.com/user-attachments/assets/8fa9e2f5-b76e-4c3a-9e5c-13b557bf2753)
![Data_Dictionary](https://github.com/user-attachments/assets/1fb3cbed-8150-41da-bf8c-0181117013ea)


## Queries:
1. Query 1: Heisman Odds. 
The Heisman Odds are betting odds assigned to outstanding college players who are in contention to win the annual Heisman Trophy. This query identifies top non-senior players based on total yards and touchdowns to help predict the best Heisman Trophy candidates to bet on for next season. Additionally. it highlights rising stars with standout performances.

![Query1](https://github.com/user-attachments/assets/a2d33dec-a51b-416d-b2f9-269abfadfb81)
![Query1](https://github.com/user-attachments/assets/c73c9138-037f-4c48-9a4f-c96d47387883)

2. Query #2: Potentials of Coaches.
The query ranks coaches by winning percentage, which is calculated from total number of wins divided by total number of games (wins + loses). In doing so, it identifies coaches that possess strong leadership skills and winning track records to help bettors make smarter wagers on game outcomes.

![Query2](https://github.com/user-attachments/assets/a63399bd-14b3-4bf1-be2f-92057f130f6a)
![Query2](https://github.com/user-attachments/assets/ecfe668e-10fc-4301-bfe0-5acc42ad5c78)

3. Query #3: Best Offensive Teams.
Total touchdowns are a strong indicator of offensive strength. The highest-ranked teams in total touchdowns is likely to have the most productive offenses. The query ranks teams based on the total touchdowns scored by their players to reflect which teams have standout offensive players. It also ensures that the best teams appears at the top of the query result.

![Query3](https://github.com/user-attachments/assets/c1bff08b-2828-4c19-a67c-bee631dafc36)
![Query3](https://github.com/user-attachments/assets/a8b6017e-c509-4e3f-a0fb-18dc89af5e85)

4. Query #4: Conference Championships
The query provides insight of teams that are likely to win the conference championship. This is important for bettors to accurately predict the outcomes of each conference championship. ​

![Query4](https://github.com/user-attachments/assets/b41a878d-b923-4d91-9258-aeb3d887bd9b)
![Query4](https://github.com/user-attachments/assets/8f4bc752-1b3a-44c1-9c46-b97c63b182bd)

5. Query #5: Average Yards/TDs per Position
The query ranks positions by their average yards per season. It is important for bettors to decide which position to bet on in an upcoming game, and they can use this query to make specific position-based betting decisions.

![Query5](https://github.com/user-attachments/assets/404e183e-6690-4440-bffa-0c981567f3ef)
![Query5](https://github.com/user-attachments/assets/b7cb0a07-d6b9-47c7-a5a1-d0e232978103)

6. Query #6: Best Players by Team (Based on Touchdowns)
![Query6](https://github.com/user-attachments/assets/74e3b84d-26e7-4c0c-976d-129a4a6e869b)
![Query6](https://github.com/user-attachments/assets/55e01a62-a4c8-4e2e-b52e-65970e38541f)



6. Query 6 outputs the product name of products that were sold a total of less than two times.

![query6](https://github.com/user-attachments/assets/b583f152-9b3e-4e5d-bb40-35784b32b077)

The information provided by this query can let a manager decide what products are not as popular or are not selling as well as other products within the grocery store. This can help them when they need to put in orders for new inventory and if they want to purchase the low-selling products again. This can also help managers make decisions about promotions and price cuts. 

7. Query 7 shows all brand names and the corresponding contact emails for brands that have sold a total of at least four products, ordered in descending order. 

![query7](https://github.com/user-attachments/assets/13964846-ec2d-4eb6-8684-eae34b4ee43f)

Managers have the ability to see what brands are the highest performing in the grocery store and who to contact if they want to communicate with them to place more orders with the brand. The total number of products sold are ordered from highest to lowest so managers can see the most popular brand at the top of the list. 

8. Query 8 displays the category name, the amount of revenue the category generates, and the percentage of revenue that category makes up. 

![query8](https://github.com/user-attachments/assets/36708902-deae-49e0-90d7-b3580fc34485)

By showing category revenue and its corresponding percentage, grocery store managers can identify which categories are doing the best in terms of revenue and which categories are not producing as much revenue. Managers could find which categories to work on and develop, such as ordering new products, in order to generate more revenue. Results are ordered by the amount of revenue made from highest to lowest so managers can clearly identify the top category.

9. Query 9 retrieves all products and their respective brand names. 

![query9](https://github.com/user-attachments/assets/9b29694d-db8d-4e10-b792-39e2a73f3021)

This query allows managers can get a comprehensive list of products along with their associated brand names. This information allows managers to review the current product lineup and understand which brands are most represented in the inventory.

10. Query 10 lists all sales transactions and dates with the corresponding names of the employees who processed those transactions.

![query10](https://github.com/user-attachments/assets/14ebdbc8-f3ea-4d4d-9d95-db7342f272bc)

For grocery store managers, this query is helpful in tracking which employees are handling specific transactions, making it easier to monitor sales performance, manage employee accountability, and identify transaction trends across different staff members.

## Database information:
![Queries](https://github.com/user-attachments/assets/37204bab-ca5e-4f11-bae6-e37f3c5dca67)
Name of the database: ha_group4_crn61608

All queries are bookmarked through stored procedures and can be called using this format: CALL TP_Qx(); where 'x' is the query number.
