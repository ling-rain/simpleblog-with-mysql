# simpleblog-with-mysql

This is a sample blog project which uses Spring MVC 3 framework and MySQL for persistance.

#Prepare two service
First Create a mysql service using mysql image, with a database named "blog" which have excuted the project.properties/blog.sql script. 
That should set up the database.

Then Create a blogweb service using the build image.

#Linked the blogweb and mysql
Method 1st:
On resource/jdbc.properties file, write up the jdbc.username and jdbc.password. 
That should be username and password for your MySQL database.

Method 2nd:
i.e, linked the two via setting ENV as follow:

DB_HOST  //mysql service IP or NAME
DB_PORT  //i.e. 3306
DB_NAME  //i.e. blog
DB_USERNAME //mysql username
DB_PASSWORD //mysql password

ps: Related to hcpaas/springmvc-mysql-blog



