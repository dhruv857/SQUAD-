# Capwatt Desktop Documentation

- Download the zip file and unzip them. The folders required for desktop are admin, database and desktop.
> You will need Apache, PHP and MySQL server for this to run.
> - [XAMPP](https://www.apachefriends.org/download.html) is recommended if you are trying to run the application locally.
>  - If you are running on a server have Apache, MySQL and PHP set up on it and define root of the web server.


# Steps to run the app on XAMP (Apache|MySQL server|PHP)

- On MySQL Database, import the ```squad.sql``` file. It is in ```database``` folder.
	- if you installed XAMPP this can be done by starting the Apache and MySQL Servers and navigating to phpmyadmin on browser.
	- if you are on you server, use
	  ``` mysql -u username -p password < <path to squad.sql>```
- Create a user in MySQL
	- if you have PHPMyadmin, navigate to phpmyadmin user accounts section.
		- Create a user by going to ```Add User Account```
		- Create a user with ``` <username>,<password>```. Change host to ```localhost```. And give global privileges. (If you are advanced user, assign permissions accordingly).
- Once you finish importing SQL script, go to the desktop folder.
- Open ``` desktop/pages/assets/db.php ``` file.
- Edit the following ( look for the assignments/variables)
	```php
		$servername = "localhost"; //or if you defined any or are using server
        	$username = "<username>"; //whatever you created in the step earlier
        	$password = "<password>"; //whatever you created in the step earlier
   	```
