- Unzip Race_Code.zip contents and move the **race** folder to htdocs directory.
- Run XAMPP **(You need to use PHP 5.6 or 5.4, OSTickets is buggy with PHP7.0 and higher, make sure you use XAMPP with supported PHP versions)**, and navigate to **phpmyadmin**.
- On PHPMyadmin, navigate to phpmyadmin user accounts section.
  - Create a user by going to ``` Add User Account ```
  - Create two users:
      - one with ``` username:livechat, password:SqUaD1 ```. Change host as ```localhost```. And give global privileges. (If you are advanced user, assign permissions accordingly).This is for enodlffm_connect database(for LiveHelperChat) which is in ```chat.sql``` file in ```race_sql``` folder.If you want to change it, you can change it in file ```race/connect/settings/settings.inc.php```.
      - one with ``` username:race, password:SqUaD1 ```. Change host as ```localhost```. And give global privileges. (If you are advanced user, assign permissions accordingly).This is for enodlffm_ticket database(for OSTickets) which is in ```tickets.sql``` file in ```race_sql``` folder.If you want to change it, you can change it in file ```race/include/ost-config.php```.
- Local mysql executable and cd to that folder.
  ```sh
    cd <path-to-mysql-executable>
  ```

  For XAMPP, usually it is at
  ```sh
  <installation directory of XAMPP>/mysql/bin/
  ```
  For MAMP, usually it is at
  ```sh
  /Applications/MAMP/Library/bin
  ```
  On server,  use
  ```sh
       which mysql
  ```
  to get the path of mysql executable.

- Command once mysql executable
  ```sh
    mysql -u <username> -p  < <path-to-tickets.sql>
    mysql -u <username> -p  < <path-to-chat.sql>
  ```
  *Enter the password for mysql user when prompted*
  *tickets.sql and chat.sql are located inside the sql folder which is provided with code.*
- Once sql is uploaded, run XAMPP Apache and MySQL server.
- The application urls are:
  - RaceConnect Client Login URL: ``` <web-path-to-race-folder>```, if using XAMPP, it is ```http://localhost:<port>/race```
  - RaceConnect Admin/Agent Login URL: ``` <web-path-to-race-folder>/scp```, if using XAMPP, it is ```http://localhost:<port>/race/scp```
  - Live helper chat agent/admin login: ```<web-path-to-race-folder>/connect/index.php/site_admin/user/login```, if using XAMPP, it is located at ```http://localhost:<port>/race/connect/index.php/site_admin/user/login```


## Default Credentials:
    - For RaceConnect Admin located at ``` <web-path-to-racefolder>/scp```, if using XAMPP, it is ```http://localhost:<port>/race/scp```,
      - username: ```raceadmin```
      - password: ```racesquad2017123```
    - For RaceConnect Client located at ``` <web-path-to-racefolder>```, if using XAMPP, it is ```http://localhost:<port>/race/```
      - username: ```md81586n```
      - password: ```123456```
    - For Live Helper Chat located at ```web-path-to-race-folder>/connect/index.php/site_admin/user/login```, if using XAMPP, it is located at ```http://localhost:<port>/race/connect/index.php/site_admin/user/login```
      - username: ```raceadmin```
      - password: ```racesquad2017123```
      - **If you see weird characters, click on ```Settings``` option on the left sidebar once you login to admin, on settings page, click on  ```Clean Cache``` under ```System``` Tab**


## Simple Application Architecture

  - LiveHelperChat Activty Diagram
    ![LiveHelperChat Activity Diagram](https://livehelperchat.com/var/media/images/lhc%281%29.png)

## Technologies Used

  - PHP
  - MYSQL
  - HTML
  - CSS  
  - Bootstrap  
  - jQuery
  - Angular
  - OSTickets
  - LiveHelperChat

## Links to refer
  - [LiveHelperChat Forum](https://forum.livehelperchat.com/)
  - [OSticket Forum](http://osticket.com/forum/)
  - [Apache Forum](https://www.apache.org/foundation/getinvolved.html)
  - [PHP](http://php.net/get-involved.php)
  - [MYSQL Forum](https://forums.mysql.com/)
  - [Host on DigitalOcean](https://www.digitalocean.com/community/)

## Brand Guidelines
    - Link and file to be inserted here
