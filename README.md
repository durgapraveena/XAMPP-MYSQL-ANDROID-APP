# Android MySQL Tutorial to Perform Basic CRUD Operation

In this project we will learn the basic CRUD operation in MySQL database from Android Application. 

## What is CRUD?
Creating a Record -> In the database we insert a record.

Reading Stored Records -> No point of saving data when we can’t read it back  So the second operation is reading the stored data back.

Updating Stored Records -> We may also need to update the existing data. So the third operation is update.

Deleting Records -> Lastly we may also need to delete the existing data from the database.

So basically in any database we perform the above mentioned operations. In this tutorial I am going to use MySQL and PHP.
## Building Web APIs
The first step is building the required Web APIs. This is because from the android application, to communicate with our web server we need an interface called API.

So our android device will send a request to our API,  then our API will perform the requested task and it will give us the response related to the task. You can see the below diagram for more clarification.
![Screenshot from 2024-05-03 12-13-01](https://github.com/durgapraveena/XAMPP-MYSQL-ANDROID-APP/assets/88362905/3fa8a0a8-429f-4a4d-bbc8-48a53ad8bc6c)
## Installations
 Androdid studion installation Link (Application)
 https://developer.android.com/studio/
 
 Xampp installation Link(DATABASE,PHP WEBSERVER)
 https://www.geeksforgeeks.org/how-to-install-xampp-in-linux/
 
 Postman installation(API TESTING)
 https://www.geeksforgeeks.org/how-to-install-postman-on-ubuntu/
 ## Create database 
 So here I am using XAMPP (You can go with wamp or lamp as well). So first create the following database.
![image](https://github.com/durgapraveena/XAMPP-MYSQL-ANDROID-APP/assets/88362905/049fe1e5-efe3-48f7-984b-31db3496e3ab)
mysql database
So open localhost/phpmyadmin and run the following query to create the above table.
##Creating PHP Project
So inside htdocs (c:/xampp/htdocs) create a new folder (You can also use an IDE like PHP Storm to create project but remember create the project inside c:/xampp/htdocs only). 
I have given the name HeroApi to my project. 
Inside the project create two more folders named includes and Api. You can see the below screenshot for the directory structure that I am using. (I am using Sublime Text for coding server part).

 ![image](https://github.com/durgapraveena/XAMPP-MYSQL-ANDROID-APP/assets/88362905/6bd50f99-a62b-4ddc-a20f-5941113fc88d)
 


