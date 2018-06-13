- Unzip Race.zip contents and move the **race** folder to htdocs directory.
- Run XAMPP and navigate to **phpmyadmin**.
- On PHPMyadmin, navigate to phpmyadmin user accounts section.
  - Create a user by going to ``` Add User Account ```
  - Create two users:
      - one with ``` username:enodlffm_livechat ,password:SqUaD1 ```. Change host as ```localhost```. And give global privileges. (If you are advanced user, assign permissions accordingly).
      - one with ``` username:enodlffm_race ,password:SqUaD1 ```. Change host as ```localhost```. And give global privileges. (If you are advanced user, assign permissions accordingly).
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
- Command once you locate mysql executable
  ```sh
    mysql -u <username> -p  < <path-to-tickets.sql>
    mysql -u <username> -p  < <path-to-chat.sql>
  ```
  *Enter the password for mysql user when prompted*
-






## Default Credentials:

## Database Diagram


## Simple Application Architecture


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
  -
  -
  -

## Brand Guidelines
    - Link and file to be inserted here
