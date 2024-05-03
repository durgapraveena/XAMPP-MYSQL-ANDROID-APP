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

 ##Testing the API Calls
For testing the API Calls here I am using POSTMAN. It is a REST API Client for Google Chrome.

 Finalizing API Calls
The below table displays our API URLs with the Parameter and Method. Remember using localhost in android side will not work. You need to find your IP. I have my IP in the below table, but in your case you need to find yours. So if you are using a windows you can use ipconfig command to find IP and for MAC or Linux use the ifconfig command. For more details you can visit this tutorial.
 

POST: http://192.168.101.1/HeroApi/v1/Api.php?apicall=createhero
GET: http://192.168.101.1/HeroApi/v1/Api.php?apicall=getheroes
POST: http://192.168.101.1/HeroApi/v1/Api.php?apicall=updatehero
GET: http://192.168.101.1/HeroApi/v1/Api.php?apicall=deletehero&id=idvalue

##Android App 
download the source code from by repo
** IMPORTANT**
Defining Internet Permission in AndroidManifest
As we need to perform network request from our Application, we need to define **internet permission** for this. And because we are working with localhost our APIs are not secured i.e. we have HTTP URLs and not HTTPS for our APIs.
And by default your application are restricted to communicate with non HTTPS URLs (For security reasons). So you need to explicitly define that your app should be allowed to communicate with HTTP URLs. And to do this you need to add **usesCleartextTraffic=”true”** inside your opening application tag. (See the below code that is AndroidManifest.xml for my project.).

**##demo**
![image](https://github.com/durgapraveena/XAMPP-MYSQL-ANDROID-APP/assets/88362905/25dfc870-d8b2-400f-a670-8cfe00f139f7)
![image](https://github.com/durgapraveena/XAMPP-MYSQL-ANDROID-APP/assets/88362905/13f49782-47e4-4c9c-adc5-e86b73a727d7)
![image](https://github.com/durgapraveena/XAMPP-MYSQL-ANDROID-APP/assets/88362905/dce7ff52-73b8-4148-8744-4605a8619d51)
![image](https://github.com/durgapraveena/XAMPP-MYSQL-ANDROID-APP/assets/88362905/9d5aafa6-d882-4c94-8402-71dc153775ae)

**REFERENCE LINKS**
https://www.simplifiedcoding.net/android-mysql-tutorial-to-perform-basic-crud-operation/



