# Schema to mysql for querrying  
- samples of sql querries and data modeling i have done in the past but wasnt able to upload it. My road to SQL and DATABASE.




## CREATING DATABASE

&#x1F4D9; Created the star schema for the DNS students class
https://dbdiagram.io/d/64c733e702bd1c4a5ef39145
![1](https://github.com/lois4801/Sql_database_trial/assets/96842662/46e58b2e-3e91-48e0-84e6-b8e358bc8ad3)


&#x1F4D9; Then I will now export it to mysql server workbench to populate the data.
![Untitled](https://github.com/lois4801/Sql_database_trial/assets/96842662/06700d6e-8954-43a8-a53c-c96372d0c20b)


&#x1F4D9; Upon opening the file.I have to connect it to the local instance.
![3 2](https://github.com/lois4801/Sql_database_trial/assets/96842662/ce9cd7b0-cc50-4570-85d8-bf72f054571e)


&#x1F4D9; Press ok and it should appear like this.
![4](https://github.com/lois4801/Sql_database_trial/assets/96842662/267ad00d-3559-4a10-93cf-c96a4793686e)



&#x1F4D9; After connecting. I find it interesting that I have to still create a database folder inside mysql workbench. Thus, thats what I did.  I have create a database title DNS_students, press the thunder button, then refresh the side menu and see if the database folder is now in there.

![5](https://github.com/lois4801/Sql_database_trial/assets/96842662/887f6cd4-a066-4172-8e89-11e4928ff33a)



&#x1F4D9; To create the database tables that you have created from the schema. Always direct it to the database folder that you have created.
In my case type USE DNS_Students; 

![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/d9233694-a3d7-4f47-b8b1-5fd9219ea68b)



&#x1F4D9;I can autopopulate all the data from each table first or execute in creating the table first. I find that executing all the tables should comes first just to make sure that everything is good. Once it is loaded. We can see the tables created inside dns students database
![6](https://github.com/lois4801/Sql_database_trial/assets/96842662/3dab6725-0c5e-4bdb-850d-15363e941b3c)


&#x1F4D9; I can now populate the data inside the table created.
![7](https://github.com/lois4801/Sql_database_trial/assets/96842662/aa1e468c-87f9-449b-b52b-41e03105a242)



&#x1F4D9; Checking if all the table we now successfully loaded with the data necessary by using the select syntax 
![8](https://github.com/lois4801/Sql_database_trial/assets/96842662/0f72638a-a713-441c-b7c3-d1175485c9f1)











