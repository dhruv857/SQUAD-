
# Capwatt Desktop Documentation

- Download the zip file and unzip them. The folders required for web app are Capwatt and the squad.sql file.
> You will need Apache, PHP and MySQL server for this to run.
> - [XAMPP](https://www.apachefriends.org/download.html) is recommended if you are trying to run the application locally.
>  - If you are running on a server have Apache, MySQL and PHP set up on it and define root of the web server.


# Steps to run the app on XAMP (Apache|MySQL server|PHP)

- On MySQL Database, import the ```squad.sql``` file. It is in ```database``` folder.
	- if you installed XAMPP this can be done by starting the Apache and MySQL Servers and navigating to phpmyadmin on browser.
	- if you are on you server, use
	  ```sh
		 		mysql -u <username> -p < <path to squad.sql>
		```
		*Enter the password for mysql user when prompted*
	- Create a user in MySQL
	- if you have PHPMyadmin, navigate to phpmyadmin user accounts section.
		- Create a user by going to ``` Add User Account ```
		- Create a user with ``` <username>,<password>```. Change host as ```localhost```. And give global privileges. (If you are advanced user, assign permissions accordingly).
- Once you finish importing SQL script, unzip and copy **Capwatt** folder to the root directory of your web server. If you are using **XAMPP**, it is ```htdocs```.
- Open ``` desktop/pages/assets/db.php ``` file in the **Capwatt** folder.
- Edit the following ( look for the assignments/variables)
	 ```php
	   		$servername = "localhost"; //or if you defined any or are using server
        $username = "<username>"; //whatever you created in the step earlier
        $password = "<password>"; //whatever you created in the step earlier
   ```
- Open ```desktop/pages/assets/session_check.php``` in **Capwatt** folder.
- Edit the following:
   ```php
	 		$root_url = "<web-location of Capwatt folder>/desktop/pages/";
	 ```
   For e.g., if location of your Capwatt when you open it in browser through XAMPP is ``` http://localhost:8888/Capwatt``` then
   ```php
	 		$root_url = "http://localhost:8888/Capwatt/desktop/pages";
	 ```
- Open ``` admin/assets/db.php ``` file in the **Capwatt** folder.
- Edit the following ( look for the assignments/variables)
	 ```php  
	 			$servername = "localhost"; //or if you defined any or are using server
        $username = "<username>"; //whatever you created in the step earlier
        $password = "<password>"; //whatever you created in the step earlier
   ```
- Open ```admin/session_check.php``` in **Capwatt** folder.
- Edit the following:
   ```php
	   $root_url = "<web-location of Capwatt folder>/admin/";
	 ```
   For e.g., if **Capwatt** folder is located in your web-directory root i.e. hotdogs, then the path through XAMPP is
	 ```
	 http://localhost:8888/Capwatt
	 ```
	 hence
   ```php
	 		$root_url = "http://localhost:8888/Capwatt/admin";
	 ```
- Run Apache and MySQL server through XAMPP.
- Navigate to
	```
 			http://localhost:<port-if-any>/Capwatt/
	```
	- For Client login, the url is
	 ```
	 		http://localhost:<port-if-any>/capwatt/desktop
	 ```
	- For Admin login, the url is
	```
		 http://localhost:<port-if-any>/capwatt/admin
	```


## Default Credentials:

 - For Client Login:
	 - username: ```test@capwatt.com```
	 - password: ```123456```
 - For Admin Login:
	 - username: ```admin@capwatt.com```
	 - password: ```squad@capwatt```

## Database Diagram
![database diagram](https://raw.githubusercontent.com/dhruv857/SQUAD-/master/Capwatt/DB.png)

## Simple Application Architecture
![Architecture <host can be Linux or Windows or anything you use.>](https://raw.githubusercontent.com/dhruv857/SQUAD-/master/Capwatt/Archi.png)

## Technologies Used

 - PHP
 - MYSQL
 - HTML
 - CSS  
 - Bootstrap  
 - jQuery
 - jQuery Knob
 - Highcharts

## Links to refer
   - TBD

## Brand Guidelines
	   - Link and file to be inserted here
