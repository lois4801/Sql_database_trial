NOTE:
This is just to add colors to the texts
```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```


- ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) `#1589F0`
- ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) `#f03c15`
- ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) `#c5f015`

RED APPLE (&#x1F34E;): 🍎
GREEN APPLE (&#x1F34F;): 🍏
BLUE HEART (&#x1F499;): 💙
GREEN HEART (&#x1F49A;): 💚
YELLOW HEART (&#x1F49B;): 💛
PURPLE HEART (&#x1F49C;): 💜
GREEN BOOK (&#x1F4D7;): 📗
BLUE BOOK (&#x1F4D8;): 📘
ORANGE BOOK (&#x1F4D9;): 📙
LARGE RED CIRCLE (&#x1F534;): 🔴
LARGE BLUE CIRCLE (&#x1F535;): 🔵
LARGE ORANGE DIAMOND (&#x1F536;): 🔶
LARGE BLUE DIAMOND (&#x1F537;): 🔷
SMALL ORANGE DIAMOND (&#x1F538;): 🔸
SMALL BLUE DIAMOND (&#x1F539;): 🔹
UP-POINTING RED TRIANGLE (&#x1F53A;): 🔺
DOWN-POINTING RED TRIANGLE (&#x1F53B;): 🔻
UP-POINTING SMALL RED TRIANGLE (&#x1F53C;): 🔼
DOWN-POINTING SMALL RED TRIANGLE (&#x1F53D;): 🔽



# Schema to mysql for querrying  
- samples of sql querries and data modeling i have done in the past but wasnt able to upload it. My road to SQL and DATABASE.




## CREATING DATABASE

&#x1F4D9; Created the star schema for the DNS students class
![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/db855d7f-b166-4c51-8b55-1ea98a9d9621)

&#x1F4D9; Then I will now export it to mysql server workbench to populate the data.
![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/e91ef46f-70a8-45cd-8733-baa057266a7f)



&#x1F4D9; Upon opening the file.I have to connect it to the local instance.

![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/3a745592-c6bb-4695-b545-31171fc0942f)



&#x1F4D9; Press ok and it should appear like this.

![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/8d3a6222-91f7-404c-8ef0-31e2a1cc3cb3)



&#x1F4D9; After connecting. I find it interesting that I have to still create a database folder inside mysql workbench. Thus, thats what I did.  I have create a database title DNS_students, press the thunder button, then refresh the side menu and see if the database folder is now in there.

![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/cdea80f0-f653-4e40-a2d5-034447961871)



&#x1F4D9; To create the database tables that you have created from the schema. Always direct it to the database folder that you have created.
In my case type USE DNS_Students; 

![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/d9233694-a3d7-4f47-b8b1-5fd9219ea68b)



&#x1F4D9;I can autopopulate all the data from each table first or execute in creating the table first. I find that executing all the tables should comes first just to make sure that everything is good. Once it is loaded. We can see the tables created inside dns students database

![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/553bd269-533f-4b0e-bf2c-121c9abfc35b)













&#x1F4D9; I can now populate the data inside the table created.
![image](https://github.com/lois4801/Sql_database_trial/assets/96842662/6fa72581-de16-4241-bc1c-0ce7244fc039)





