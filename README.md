# simpleApp/simpleApp_back-spring
Import as maven project.

Start mysql.
Create the new database. Creates the user admin password admin. Gives all the privileges to the new user on the newly created database.

SQL:

create database simpleApp;

create user 'admin'@'localhost' identified by 'admin';

grant all on simpleApp.* to 'admin'@'localhost';

In application.proterties chage spring.jpa.hibernate.ddl-auto=none to spring.jpa.hibernate.ddl-auto=create-drop the first run (to generate the db tables)

start: simpleAppApplication.java > run as > Java Application
