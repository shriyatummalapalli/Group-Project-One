# Group Project One


## Problem Description
The task at hand involves building a relational database to manage the operations of a basketball club. The key entities in this model are the member profiles and teams. The member profiles represent individuals who are part of the basketball club, and they are associated with payment records, member statistics, and the teams they belong to. Teams contribute to member statistics, and each team has coaches assigned to them. These teams also participate in games. The objective is to effectively model these various relationships, generate sample data, and use this data to populate all entities and their attributes. Furthermore, the aim is to develop functional queries on this data to gain valuable insights into the club's operations from a managerial perspective.

## Data Model
The purpose of the data model depicted is to effectively show the relationships between the various entities that make up the hypothetical basketball club. 

The memberProfiles entity holds vital member details for the basketball club. It is an entity that stores important information about individuals who comprise the club such as, the members name and contact info. There is a one-to-many relationship between memberProfiles and Teams, a single member can be part of many teams. Additionally, there is a one-to-one relationship between members and payment records, as each member has a single payment record.

The memberStats entity serves as an associative entity between member profiles and teams within the basketball club database. It contains a unique playerStatsID along with references to the member and team associated with it. Additionally, there is an attribute for points, representing the number of points scored by each player. This entity facilitates the tracking of individual player statistics within the context of their respective teams.

The team's entity is another important entity. It includes attributes such as the team name, the number of players, and the memberIDs associated with each team. Additionally, it stores information about the coaches who oversee each team. There is a one-to-many relationship with games, as each team can participate in multiple games throughout the season.

The coaches entity contains essential details about each coach, including their name and contact information. It also includes a rating attribute, allowing individuals to assess the quality of each coach before making a selection. Additionally, there is a one-to-many relationship between coaches and teams, as a single coach may oversee multiple teams within the basketball club.

The games entity stores crucial details about each basketball game. It is linked to teams through a one-to-many relationship, as each team plays many games.The information recorded includes the date, location, and duration of each game, all associated with a specific team.

The payment records entity stores important information regarding the financial transactions of each member. It includes details such as the billing date, amount owed, payment type, and payment status. This entity is associated with member profiles through a one-to-one relationship, as each member is linked to a specific payment record.
<img width="941" alt="Screenshot 2024-04-22 at 2 49 57 PM" src="https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/12c2a3a3-a08e-42a7-9043-5ccce81ea550">


## Data Dictionary
![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/35beb05a-10c6-4910-8c21-084d05ef091c)

![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/00169132-8d1a-4b07-856b-2832cde069d2)

![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/c2610644-1046-4e6a-8188-2a53527e25f2)

![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/cdc1806b-d701-4b84-85c3-3e9b632ea2f2)

![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/ca8b74df-3c31-4da9-b1ed-7eb421432f7e)

![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/291e0e8f-c07f-48d7-8543-b4d214186096)


## Queries
![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/b0897067-8086-4ba0-bb35-6147d10e21f1)

1) Query one shows the details of the game and which team will be playing. It includes the date of the game, the location of the game, and the team that will be playing at each respective game and location.

![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/710d61b3-29f3-46b9-a135-d8d6ad4a6fc7)
![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/a60dbd86-9710-44b7-b55d-96b2e13edad9)

Query one allows coaches to access information about the date, location, and participating teams of upcoming games. This data is valuable as it helps coaches stay well-prepared for their upcoming events. It provides them with an easy means to identify important details and plan accordingly.

2) Query two shows the income made by the establishment. 
![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/cc1447bd-ca87-4b23-9b09-75f8e6cb41f7)

![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/8c8976db-06bb-4807-9ab5-3d9f83a3120f)

Query two enables owners to view their total income, providing them with a quick overview of their profits. This information helps owners in making decisions regarding potential price adjustments to maximize profitability. Additionally, it allows them to evaluate their satisfaction with the current outcomes.

3) Query three shows the names of the members, the team they are on, and the average points scored by each member. 
![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/d9d2420d-bc11-49e4-8f46-6f2b7d120bd1)
![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/e07f7272-44e4-44ce-94f4-02ed410f0440)

Query three provides coaches and members with the ability to identify standout performers among other players. This functionality helps coaches in assessing which players are consistently scoring above the average. Using this data coaches can not only identify exceptional talent but also tailor their training and support to further enhance individual and team performance.

4) Query 4 shows the member names and the coaches associated with these members. It specifically shows the coaches whose first name starts with the letter N. 
![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/8ce953c5-7e55-4107-8c27-7f3bf61053cb)
![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/3a1efdee-3bd5-480d-9a37-868419d004b1)

Query four enables members to identify their coaches and coaches to identify their assigned members. The results specifically display members associated with coaches whose names start with the letter 'N'. This feature facilitates coaches in quickly identifying the members they are supposed to coach.

5) Query five displays teams along with their number of players and the average points scored by teams with more players than the overall average. The results are sorted in descending order based on the number of players.
![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/4208ac42-9418-4c24-b679-aa8436a71777)
![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/e7acded5-c1f4-4737-babd-25c69a8c2884)

Query five allows both members and coaches to not only track the performance of their own team but also monitor the performance of other teams with a larger number of players. This data helps members and coaches in gaining insights into potential opponents they might face in future competitions. By providing a clear overview of the performance of various teams, this information assists in strategic planning and preparation for upcoming matches.

6) Query six displays the first names of members, along with their phone numbers and certain payment details. It focuses on displaying names, phone numbers, and amounts due for members who paid using a credit card and have a payment status of 'processed'.
![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/53ff6b17-6936-46c9-a175-47ff8a867c02)
![image](https://github.com/shriyatummalapalli/Group-Project-One/assets/167737199/3350648e-def0-4345-ba36-813cf8d71e11)

Query six provides members and owners with access to specific payment details. It presents the names of individuals who have made payments using a credit card, ensuring that their transactions were successfully processed. This information serves as a reliable reference point for tracking successful payments. By offering transparency into payment processes, it facilitates efficient management and accountability for both members and owners.

## Database Information
Name of the database: ns_st85764





















