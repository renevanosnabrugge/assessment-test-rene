# CricStatsBuddy  - Minimal Viable Product
>This assignment is part of the Xebia XMS Hiring process. You should have received companion documents that explains the details of the procedure and an overview of the company CricStats.

![CricStats Logo](/images/CricStats.png)

## The Assignment
The customers of CricStats are looking for a solution that can provide them with a Dashboard to gain insights in this data. As Xebia, we are asked to help to design an architecture for this application and implement a (MVP of a) Dashboard.

This repository contains the requirements for the Minimal Viable Product. 

### Your tasks

CricStats aims to provide interactive Dashboards for its customers based on the data collected from matches, practice sessions and other sources. They want to provide interactive dashboards that can be used to analyse different aspects of the game. The dashboards are accessible to authorized users only.

Since, the data comes from different sources, they are available in two different formats, namely CSV and JSON. 

Following aspects of the game of cricket are important for customers of CricStats (actually the game of cricket is complexer than the version used for this assessment):
- Two teams, each with 3 players.
- A game consists of 2 innings. 
- In each inning one team bats and the other bowls.
- The batting team tries to score runs.
- The team that scores more runs after the two innings wins.
- Each inning is of 1 over which consists of 6 balls being bowled by a bowler.


The data files present have the following information:
- Stadiums: CSV file with all the stadiums. Id, Name, Country, City. Id is unique. The file is without header information.
![Stadium CSV](/images/cricstats-stadiumscsv.png)

- Games: JSON files with team information and the information about each innings and individual balls.
![Games JSON](/images/cricstats-json.png)

We have been tasked to come up with an architecture (e.g. Medallion) of the data flow and sample implementation of a Dashboard. It is important to think about how the csv/json files will move through the archtiecture to finally be used in the dashboards.

For CricStats, this is all a big experiment, so it is crucial that the platform has very low operational cost from the start.

## User stories

Below are a few user stories that would be required to be implemented so that the data lands into the system in the format that can be used in Dashboards on the CricStats platform. 

>Note: feature completeness less important than a sound architecture, so select a few that you feel are feasible within the timeframe of the assignment.

### :memo: US01 – Import raw data files into Fabric
CricStats developers must have access to raw data in fabric.

Acceptance Criteria:
- The raw files are accessible in fabric

### :memo: US02 – Transform into tables
The data must be tranformed into tables that can be used for dashboards, or further analysis by CricStats developers.

When new files are added they are tranformed automatically at the end of the day.

Acceptance Criteria:
- Raw data transformed into fabric tables.
- Automatic tranformation of new files at the end of day.

### :memo: US03 – Winning team determination
In the raw files, there is no information about which team won the game. But it is important to have this information as well for analysis.

Acceptance Criteria:
- The winning team is determined for each game.


### :memo: US04 – Dashboard showing runs scored in different countries
For the decision makers a dashboard is needed where we can see the runs scored by a player in different countries. The Dashboard should only be accessible to authorized users.

Acceptance Criteria:
- The Dashboard shows correctly the total runs scored by each player in different countries
- The Dashboard is not accessible to unauthorized users.


### :memo: USBONUS – Surprise us!

Looking at these four use cases, is there another cool feature you can think of and you want to show off? Surprise us! 😊


## Checklist
Implement a minimum viable product that demonstrates your solution architecture. We are most interested to see how you structure your code internally. This is more important to us than feature completeness.

Also think about the setup of an automation process for movement of data through your architecture. Also think about other aspects of the Fabric that might be relevant.

> Be realistic with the limited amount of time. This part is important as we want to assess your hands-on skills. It is also a starting point for the technical discussion of architecture, technology and development practices.

‼️As stated before, do reach out if and when you have any questions. Don't assume. Ask!
