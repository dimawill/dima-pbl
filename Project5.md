# Client -server Architecture with Mysql - Project Steps
* Created 2 Ubuntu EC2 servers on AWS namely DB-server and Client in the same AZ
* Connected to the DB-server
* Installed mysql-server
* Enabled the service
* Connected to the Client server
* Retrieved updates from the repository - sudo apt update -y
* Installed mysql-client
* Configured the security group on the DB-server to accept in-bound traffic on port 3306 from the client private IP address
* Ran mysql secure installation on the DB-Server
* Ran sudo mysql command
* Created a Remote User and password
* Created a database named test_db
* Granted privileges on the test_db to the Remote User
* Flushed the privileges
* Configured mysql server to allow connections from the remote host by making changes to the bind address in the script
* Restarted the server
* Established a remote connection from mysql client to mysql DB-server
* Displayed the database<img width="955" alt="PROJECT5 COMPLETE" src="https://user-images.githubusercontent.com/86001367/123630918-06ca6000-d80e-11eb-9039-3f5cb42e8e72.png">
