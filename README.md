## TASK – Implement a Client Server Architecture using MySQL Database Management System (DBMS).

Client-Server architecture describe the relationship between two or more connectecd computer sharing data across the network. The computer that request for data is known as the client while the one that processes the request is known as the server.

To demonstrate Client-Server architecture we will be using two Ec2 instance with mysql-server and mysql-client respectively.

- Create and configure two Linux-based virtual servers (EC2 instances in AWS).

- Name one instance Mysql-server the other Mysql-client

- On mysql server Linux Server install MySQL Server software.

- On mysql client Linux Server install MySQL Client software.

- Open port 3306 on Mysql-server allow for connection. Both server can communicate using private IPs since they belong to the same subnet

- Change bind-address on Mysql-server to allow for connection from any IP address. Set the bind-address to 0.0.0.0 using the command below:

  `sudo vi /etc/mysql/mysql.conf.d/mysqld.cnf`
  
- On the mysql server, create a USER, CLIENT and grant ALL permission to the User

     ![7 rows created](https://user-images.githubusercontent.com/65022146/194963905-3f91006c-aa2c-4754-9f9c-6e0f827171c3.png)

- From mysql client Linux Server connect remotely to mysql server Database Engine without using SSH. You must use the mysql utility to perform this action.

 - Check that you have successfully connected to a remote MySQL server and can perform SQL queries. You should something similar to the screenshot below:

     ![Coonected from the client server](https://user-images.githubusercontent.com/65022146/194962720-c2a099ab-5097-4dc4-83d3-40ee0a627543.png)
  



