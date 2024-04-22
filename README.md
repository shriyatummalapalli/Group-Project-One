# Group Project One


## Problem Description
The task at hand involves building a relational database to manage the operations of a basketball club. The key entities in this model are the member profiles and teams. The member profiles represent individuals who are part of the basketball club, and they are associated with payment records, member statistics, and the teams they belong to. Teams contribute to member statistics, and each team has coaches assigned to them. These teams also participate in games. The objective is to effectively model these various relationships, generate sample data, and use this data to populate all entities and their attributes. Furthermore, the aim is to develop functional queries on this data to gain valuable insights into the club's operations from a managerial perspective.

## Data Model
The purpose of the data model depicted is to effectively show the relationships between the various entities that make up the hypothetical basketball club. 

The memberProfiles entity holds vital member details for the basketball club. It is an entity that stores important information about individuals who comprise the club such as, the members name and contact info. There is a one-to-many relationship between memberProfiles and Teams, as multiple members can belong to a single team. Additionally, there is a one-to-one relationship between members and payment records, as each member has a single payment record.

The memberStats entity serves as an associative entity between member profiles and teams within the basketball club database. It contains a unique playerStatsID along with references to the member and team associated with it. Additionally, there is an attribute for points, representing the number of points scored by each player. This entity facilitates the tracking of individual player statistics within the context of their respective teams.

The team's entity is another important entity. It includes attributes such as the team name, the number of players, and the memberIDs associated with each team. Additionally, it stores information about the coaches who oversee each team. There is a one-to-many relationship with games, as each team can participate in multiple games throughout the season.

The coaches entity contains essential details about each coach, including their name and contact information. It also includes a rating attribute, allowing individuals to assess the quality of each coach before making a selection. Additionally, there is a one-to-many relationship between coaches and teams, as a single coach may oversee multiple teams within the basketball club.

The games entity stores crucial details about each basketball game. It is linked to teams through a one-to-many relationship, as each team plays many games.The information recorded includes the date, location, and duration of each game, all associated with a specific team.

The payment records entity stores important information regarding the financial transactions of each member. It includes details such as the billing date, amount owed, payment type, and payment status. This entity is associated with member profiles through a one-to-one relationship, as each member is linked to a specific payment record.

## Data Dictionary





