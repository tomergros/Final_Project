# User Management System 
    # Written by: Tomer Grossman & Oriel Somech 
    # Express,Node-js, HBS & MySQL

This Project was created as part of Web Development course.

## Prerequisite
We will give your some instructions in order to operate the application so please follow carefully.
Don't worry, it won't be too difficult :)

First, Lets start with our Database:

Make sure to download,install and run MySQL server & MySQL workbench with an active server running.
on your server open a new schema and call it `usermanagement_project`.
Then please run the following query (or you can run the attached SQL script 'user-schema.sql'):
CREATE TABLE `usermanagement_project`.`user` ( `id` INT NOT NULL AUTO_INCREMENT , `first_name` VARCHAR(45) NOT NULL , `last_name` VARCHAR(45) NOT NULL , `email` VARCHAR(45) NOT NULL , `phone` VARCHAR(45) NOT NULL , `comments` TEXT NOT NULL , `status` VARCHAR(10) NOT NULL DEFAULT 'active' , PRIMARY KEY (`id`)) ENGINE = InnoDB;

## Change .env file
We have created it for you so you just have to change the credentials.
.env file is for storing your database credentials
make sure to save the file in the main dir of the project!
Otherwise - it will make connection problems.
here is the format of the file:

```
DB_HOST = localhost // change to your sql server host name
DB_NAME = usermanagement_tut
DB_USER = root // change to your sql server user name if it's not root
DB_PASS = password  // change to your sql server user password
```

## Installation
Finally, in order to run the project, please install it locally using npm:

```
$ npm install
$ npm start
```


### Thats it! Now you can manage your own user managment app.
Enjoy!


