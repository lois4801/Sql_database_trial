# Schema to mysql for querrying  
- samples of sql querries and data modeling i have done in the past but wasnt able to upload it. My road to SQL and DATABASE.




## CREATING DATABASE

&#x1F4D9; Created the star schema for the DNS students class
https://dbdiagram.io/d/64c733e702bd1c4a5ef39145
![1](https://github.com/lois4801/Sql_database_trial/assets/96842662/46e58b2e-3e91-48e0-84e6-b8e358bc8ad3)


&#x1F4D9; Then I will now export it to mysql server workbench to populate the data.
![Untitled](https://github.com/lois4801/Sql_database_trial/assets/96842662/06700d6e-8954-43a8-a53c-c96372d0c20b)


&#x1F4D9; Upon opening the file.I have to connect it to the local instance.
![3](https://github.com/lois4801/Sql_database_trial/assets/96842662/cf10d9f2-21ed-43da-9408-7b3d56659906)


&#x1F4D9; Press ok and it should appear like this.
![4](https://github.com/lois4801/Sql_database_trial/assets/96842662/ad4087b9-a8f5-4db8-9501-77c77aaec3fb)





&#x1F4D9; After connecting. I find it interesting that I have to still create a database folder inside mysql workbench. Thus, thats what I did.  I have create a database title DNS_students, press the thunder button, then refresh the side menu and see if the database folder is now in there.

![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/cdea80f0-f653-4e40-a2d5-034447961871)



&#x1F4D9; To create the database tables that you have created from the schema. Always direct it to the database folder that you have created.
In my case type USE DNS_Students; 

![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/d9233694-a3d7-4f47-b8b1-5fd9219ea68b)



&#x1F4D9;I can autopopulate all the data from each table first or execute in creating the table first. I find that executing all the tables should comes first just to make sure that everything is good. Once it is loaded. We can see the tables created inside dns students database

![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/553bd269-533f-4b0e-bf2c-121c9abfc35b)



&#x1F4D9; I can now populate the data inside the table created.

![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/6fa72581-de16-4241-bc1c-0ce7244fc039)


&#x1F4D9; Checking if all the table we now successfully loaded with the data necessary by using the select syntax 
![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/8dfc9678-39cb-4fd8-8548-d1d1223b2aa2)





&#x1F4D9; I wanted to see if how much data do I have if I pull the whole database record just by those three tables alone.

![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/8b1e33bc-25bf-4dbe-b7f6-6c45f4d205c2)







