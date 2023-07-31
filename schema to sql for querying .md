# Schema to mysql for querrying  
- samples of sql querries and data modeling i have done in the past but wasnt able to upload it. My road to SQL and DATABASE.

NOTE:
This is just to add colors to the texts
```diff
- text in red
+ text in green
```diff
# text in gray
@@ text in purple (and bold)@@
```


- ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) `#1589F0`
- ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) `#f03c15`
- ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) `#c5f015`


## CREATING DATABASE

```diff + Created the star schema for the DNS students class. ```

![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/db855d7f-b166-4c51-8b55-1ea98a9d9621)



Then I will now export it to mysql server workbench to populate the data.


![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/e91ef46f-70a8-45cd-8733-baa057266a7f)



Upon opening the file.I have to connect it to the local instance.


![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/3a745592-c6bb-4695-b545-31171fc0942f)



Press ok and it should appear like this.
![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/8d3a6222-91f7-404c-8ef0-31e2a1cc3cb3)



After connecting. I find it interesting that I have to still create a database folder inside mysql workbench. Thus, thats what I did.  I have create a database title DNS_students, press the thunder button, then refresh the side menu and see if the database folder is now in there.


![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/cdea80f0-f653-4e40-a2d5-034447961871)



-To create the database tables that you have created from the schema. Always direct it to the database folder that you have created.
In my case type USE DNS_Students; 
![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/d9233694-a3d7-4f47-b8b1-5fd9219ea68b)



- We can autopopulate all the data from each table first or do it one by one. I find that executing all the tables should comes first just to make sure that everything is good. Once it is loaded. We can see the tables created inside dns students database

Use DNS_Students;
CREATE TABLE `sports` (
  `SportsID` varchar(50) PRIMARY KEY,
  `SportsName` varchar(200) UNIQUE,
  `SportsDesc` varchar(300)
);

CREATE TABLE `restaurants` (
  `RestID` varchar(50) PRIMARY KEY,
  `RestName` varchar(200) UNIQUE,
  `Rest_City` varchar(100),
  `Rest_Details` varchar(300) DEFAULT " A nice restaurant"
);

CREATE TABLE `students` (
  `StudentID` int PRIMARY KEY AUTO_INCREMENT,
  `Student_name` varchar(200),
  `City` varchar(100),
  `SportsID` varchar(50),
  `RestID` varchar(50),
  `Student_Age` int
);

ALTER TABLE `students` ADD FOREIGN KEY (`SportsID`) REFERENCES `sports` (`SportsID`);

ALTER TABLE `students` ADD FOREIGN KEY (`RestID`) REFERENCES `restaurants` (`RestID`);



![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/8a3e72b6-f594-486d-a964-b6f27b48046b)




//
INSERT INTO sports VALUES
('S1', 'Hockey', 'Our favourite sport'),
('S2', 'Soccer', '22 players chasing a ball'),
('S3', 'Personal Fitness', 'Can we classify it as sport'),
('S4', 'Rugby', 'For the tough ones')
;

INSERT INTO restaurants
VALUES
('R1', 'Almonak', 'Halifax', 'Special for Brunch'),
('R2', "John's Lunch", 'Halifax', 'Special for Lunch'),
('R3', 'Destination Dogs', 'MOncton', 'A unique name'),
('R4', 'Atelier Tony', 'Dieppe', 'Upscale restaurant')
;


INSERT INTO students (Student_name, City, SportsID, RestID, Student_Age)
VALUES
('Alex', 'Bedford', 'S1',NULL,89),
('Adan', 'Halifax', null,NULL,70),
('Kunle', 'Moncton', 'S2','R1',40),
('Chidinma', 'St Johns', 'S3','R1', null),
('Israa', 'Saint Johns', 'S3',NULL, 23),
('Luri', 'Gander', 'S4','R2', 22),
('Jena', 'Brigus', 'S1',NULL, 22),
('Nancy', 'Gander', null,'R3', 34),
('Vicky', 'Dartmouth', 'S2',NULL, 23),
('Zach', 'Fredricton', 'S3','R4', 23),
('Shadi', 'Bedford', null,'R4', 28),
('Klara', 'Fredricton', 'S1',NULL, 18),
('Divya', 'Halifax', 'S2','R1', 17),
('Emma', 'Halifax', 'S3','R2', 25),
('Marion', 'Moncton', 'S2','R1', null),
('Sophie', 'Saint Johns', 'S1',NULL, 15),
('Atikur', 'Halifax', 'S1',NULL, 25),
('Chisom', 'Bedford', 'S1',NULL, 22),
('Amir', 'Bedford', 'S1','R4', 23),
('Sophie', 'Moncton', 'S1','R2', 22),
('Gustavo', 'Gander', 'S1',NULL, 16)
;
//


