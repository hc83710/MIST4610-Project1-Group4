# MIST4610-Project1-Arjmandi'sAssailants

## Team Name: 
61608 Arjmandi's Assailants

## Team Members:
1. An, Ben [@benan03](https://github.com/benan03)
2. Burt, Keegan[@keeganburt24](https://github.com/keeganburt24)
3. Cheng, Hsin [@hc83710](https://github.com/hc83710)
4. Cho, Nick [@nichooo4](https://github.com/nichooo4)
5. Shields, David [@DubNation44](https://github.com/DubNation44)


## Problem Description:
Our database system is designed to support a sports betting platform where users can analyze statistics before placing wagers on teams or players. Utilizing advantages of data and information systems, we replace the uncertainty of gut feeling with objective, accurate, informative, and integrated tables for bettors to visualize waging factors. The database system has the ability to track and visualize relationships between teams, coaches, conferences, games, players, and players' statistics to better apply to winning money via sports bets. Examples of ways to achieve this function include: 1. calculates and presents betting odds based on player statistics, 2. comparisons on team performances to conclude conference standings, and 3. tailored betting (e.g. Best offensive teams)


## Data Model:
This data model represents a college football database, capturing data related to teams, players, coaches, conferences, and player statistics. It is designed to support the organization and management of college football team information, tracking team performance, player attributes, coaching assignments, and conference affiliations. The team entity serves as the core of the model, linking to other entities such as coach, player, and conference. Each team has a unique identifier and stores attributes like mascot, city, stadium name, and win/loss records. The model enables the efficient retrieval of player rosters, team standings, and individual performance metrics, making it useful for sports analysts, team managers, and recruiters. By structuring the data this way, the system can track player development, compare team performance within conferences, and maintain historical records of team successes and personnel changes.

The conference entity groups multiple teams based on their region and competition structure. A conference can have multiple teams, but each team belongs to only one conference, forming a one-to-many relationship.

The coach entity stores information about team coaches, including their first and last names. Each coach is associated with one team, but a team can have multiple coaches, creating a one-to-many relationship between teams and coaches.

The player entity records detailed player information, including position, physical attributes (height and weight), class standing, GPA, and the team they play for. A team can have multiple players, but each player belongs to only one team, forming another one-to-many relationship.

The playerstats entity tracks individual player performance metrics, such as total yards and touchdowns. Each player has one set of performance statistics, creating a one-to-one relationship between player and playerstats.

![Data_Model](https://github.com/user-attachments/assets/a2e4bf50-2e38-4a40-92ce-d02d03172aee)


## Data Dictionary:
![Data_Dictionary](https://github.com/user-attachments/assets/47eb73a7-5864-40f7-b4e3-c04a5045aceb)
![Data_Dictionary](https://github.com/user-attachments/assets/6ee9fd21-6ef8-422a-ba4a-3fcd4a28619b)
![Data_Dictionary](https://github.com/user-attachments/assets/5f5f88e1-2fc2-4668-98f4-7bbcc1c0d9b2)
![Data_Dictionary](https://github.com/user-attachments/assets/8fa9e2f5-b76e-4c3a-9e5c-13b557bf2753)
![Data_Dictionary](https://github.com/user-attachments/assets/1fb3cbed-8150-41da-bf8c-0181117013ea)


## Queries:
1. Query 1: Heisman Odds. 
The Heisman Odds are betting odds assigned to outstanding college players who are in contention to win the annual Heisman Trophy. This query identifies top non-senior players based on total yards and touchdowns to help predict the best Heisman Trophy candidates to bet on for next season. Additionally, it highlights rising stars with standout performances.

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

4. Query #4: Conference Championships. 
The query provides insight of teams that are likely to win the conference championship. This is important for bettors to accurately predict the outcomes of each conference championship. ​

![Query4](https://github.com/user-attachments/assets/b41a878d-b923-4d91-9258-aeb3d887bd9b)
![Query4](https://github.com/user-attachments/assets/8f4bc752-1b3a-44c1-9c46-b97c63b182bd)

5. Query #5: Average Yards/TDs per Position. 
The query ranks positions by their average yards per season. It is important for bettors to decide which position to bet on in an upcoming game, and they can use this query to make specific position-based betting decisions.

![Query5](https://github.com/user-attachments/assets/404e183e-6690-4440-bffa-0c981567f3ef)
![Query5](https://github.com/user-attachments/assets/b7cb0a07-d6b9-47c7-a5a1-d0e232978103)

6. Query #6: Best Players by Team (Based on Touchdowns). This query helps managers, coaches, and analysts identify the best-performing player (highest touchdowns) from each team. This is crucial for awards, player evaluations, and strategy planning.

![Query6](https://github.com/user-attachments/assets/55e01a62-a4c8-4e2e-b52e-65970e38541f)
![Query6](https://github.com/user-attachments/assets/74e3b84d-26e7-4c0c-976d-129a4a6e869b)


7. Query #7: Get the Total Wins and Losses for Each Team. 
The query returns the total wins and losses for every team in the last season, ranked by wins. This query provides quick access to top-performing teams, which is useful for moneyline bets made at the last minute.

![Query7](https://github.com/user-attachments/assets/82372654-6d63-4414-b0e9-8b5b603a2e9f)
![Query7](https://github.com/user-attachments/assets/e52ae8f2-efd8-4150-a3ae-f36d8f052cc3)


8. Query #8: Finding Conferences with the Most Total Wins Across All Teams. 
The query calculates the total number of wins per conference by summing up the wins of all teams in each conference. Teams from high-win conferences typically face tougher competition, affecting point spreads and totals.


![Query8](https://github.com/user-attachments/assets/c63b2a06-21ad-416d-a4a6-96a55ed50859)
![Query8](https://github.com/user-attachments/assets/a4e58a12-bf88-490d-9342-88ee43330cc4)



9. Query #9: List of Players and Their Positions.
This query lists all players along with their positions. This gives a quick reference for identifying players and their roles in the team.

![Query9](https://github.com/user-attachments/assets/3d9f7e4f-e12a-49f6-9d1a-771ff178c754)
![Query9](https://github.com/user-attachments/assets/019d99c8-9552-4ad4-95e9-147bdbcc0536)


10. Query #10: Heaviest Teams (Average Player Weight by Team). 
This query finds teams with the heaviest average player weight, which can be useful for betting on games where size and strength might be a factor—like in run-heavy offenses or defensive battles.

![Query10](https://github.com/user-attachments/assets/087b0c0c-7a87-4f0f-919a-55fc8c98f8b3)
![Query10](https://github.com/user-attachments/assets/e4664a1c-eee8-459c-b09a-91ec40e411b9)




   

## Database information:
![Queries](https://github.com/user-attachments/assets/bd33b760-d115-4961-997b-85f931a547bf)

Name of the database: ha_group4_crn61608

All queries are bookmarked through stored procedures and can be called using this format: CALL TP_Qx(); where 'x' is the query number.
