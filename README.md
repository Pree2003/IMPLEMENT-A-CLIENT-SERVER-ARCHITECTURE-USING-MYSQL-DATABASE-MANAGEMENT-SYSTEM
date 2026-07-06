<img width="554" height="69" alt="image" src="https://github.com/user-attachments/assets/8cab9760-9b32-4b41-9717-a737a628a82a" />
The screenshot shows the Amazon EC2 Instances dashboard with two running virtual machines. 
The first instance is named My SQL Server, and the second is named My client server. 
Both instances are running on the t3.micro instance type with the Linux/UNIX platform in the Europe (Stockholm) Region (eu-north-1a). The screenshot also shows that both instances have passed all three AWS status checks, indicating they are operating normally. In addition, the public IPv4 addresses, public DNS names, security groups, key pair names, and launch times for each instance are displayed, 
confirming that both servers have been successfully created and are available for use

<img width="553" height="395" alt="image" src="https://github.com/user-attachments/assets/d243c781-c327-47aa-a36f-cefd1b34c96e" />
The screenshot shows a successful Secure Shell (SSH) connection from the local Windows computer to the MySQL server hosted on an Amazon EC2 instance. 
The connection was established using the server's private key (sql server.key.pem) and the server's public IP address. 
After authentication, the Ubuntu 26.04 LTS welcome message is displayed, confirming that the login was successful. 
The terminal also provides system information, including memory usage, disk usage, the server's private IPv4 address, 
available software updates, and a notification that a system restart is required. 
The command prompt (ubuntu@ip-172-31-31-73:~$) indicates that the user is logged into the remote MySQL server and is ready to continue with the server configuration and database installation.

<img width="554" height="146" alt="image" src="https://github.com/user-attachments/assets/782c2278-6f1c-4d9b-8f8e-65a48bc738e1" />
The screenshot shows the execution of the sudo apt update command on the MySQL server after successfully logging in via SSH. 
This command updates the server's package index by retrieving the latest information about available software packages and security updates from the Ubuntu repositories. 
The output confirms that the package lists were successfully downloaded from the official Ubuntu repositories for the Europe (Stockholm) region. 
At the end of the process, the system reports that 19 packages are available for upgrade, indicating that the server is up to date with the latest package information and is ready for the installation of MySQL and other required software.

<img width="554" height="262" alt="image" src="https://github.com/user-attachments/assets/8efb47d1-d9d4-48ae-87d5-8127b36e5709" />
The screenshot shows the installation of the MySQL Server on the Ubuntu EC2 instance using the sudo apt install mysql-server -y command. 
During the installation, the package manager downloads and installs the MySQL server along with its required dependencies, including the MySQL client, server core, and supporting libraries. The output also displays the total download size, required disk space, and the software repositories from which the packages are retrieved. This step prepares the server to function as the database management system for the project, 
enabling it to store, manage, and provide access to application data within the client-server architecture.

<img width="554" height="179" alt="image" src="https://github.com/user-attachments/assets/d78874b1-66d3-4090-a85f-b0d0ca694e53" />
The screenshot shows the output of the sudo systemctl status mysql command, which is used to verify the status of the MySQL service after installation. 
The output confirms that the MySQL Community Server has been successfully installed and is currently active (running). 
It also shows that the service is enabled to start automatically during system boot and that the server is operational. 
Additional information, such as the service's process ID (PID), memory usage, CPU usage, and startup logs, is displayed, confirming that the MySQL database server is running correctly and is ready to accept database connections for the client-server application.

<img width="554" height="259" alt="image" src="https://github.com/user-attachments/assets/4ff7bc53-7306-41b3-abe4-f5c69b2fa4e8" />
The screenshot shows the verification of the installed MySQL version and a successful login to the MySQL server. 
The mysql --version command confirms that MySQL version 8.4.10 is installed on the Ubuntu server. 
The sudo mysql command then opens the MySQL monitor, displaying the server version and a welcome message, which confirms that the database server is functioning correctly and is accessible. 
After verifying the installation, the session is closed using the exit command, returning to the Ubuntu terminal. This step confirms that MySQL has been installed successfully and is ready for database configuration and use in the client-server architecture. 

<img width="553" height="337" alt="image" src="https://github.com/user-attachments/assets/d51cc87e-6897-46d2-90ae-9052fd48515e" />
The screenshot shows a successful SSH connection from the local Windows computer to the client server hosted on an Amazon EC2 instance. 
The connection is established using the client's private key (client server.key.pem) and the server's public IP address. After authentication, the Ubuntu 26.04 LTS welcome message is displayed, confirming that the login was successful. 
The terminal provides system information, including memory usage, disk usage, the server's private IPv4 address, and the number of available software updates. 
A notification indicating that a system restart is required is also displayed. 

<img width="554" height="240" alt="image" src="https://github.com/user-attachments/assets/3830b1de-e8fc-469c-b963-278199362977" />
The screenshot shows a successful SSH connection from the local Windows computer to the client server hosted on an Amazon EC2 instance. 
The connection is established using the client's private key (client server.key.pem) and the server's public IP address. After authentication, the Ubuntu 26.04 LTS welcome message is displayed, confirming that the login was successful. 
The terminal provides system information, including memory usage, disk usage, the server's private IPv4 address, and the number of available software updates. 
A notification indicating that a system restart is required is also displayed. 

<img width="554" height="240" alt="image" src="https://github.com/user-attachments/assets/e4b37841-213c-44dc-b436-6b3a19be82be" />
The screenshot shows the execution of the sudo apt update command on the client server after establishing an SSH connection. 
This command refreshes the package index by downloading the latest information about available software packages and security updates from the Ubuntu repositories. 
The output confirms that the package lists were successfully retrieved and updated without errors. 
At the end of the process, the system indicates that 19 packages are available for upgrade, showing that the package information is current. 
Updating the package repository ensures that the latest software versions and dependencies are available before installing the applications required for the client-server architecture.

<img width="553" height="275" alt="image" src="https://github.com/user-attachments/assets/c8959109-a074-43fe-a8e4-0321fd87af66" />
The screenshot shows the installation of the MySQL client on the client EC2 server using the sudo apt install mysql-client -y command. 
During the installation process, the package manager downloads and installs the MySQL client along with the required dependencies, including mysql-client-core, mysql-common, and supporting libraries. 
The output also displays the total download size, required disk space, and the Ubuntu repositories used to obtain the packages. 
Installing the MySQL client enables the client server to connect to and communicate with the remote MySQL database server, allowing it to send database queries and retrieve data as part of the client-server architecture.

<img width="554" height="59" alt="image" src="https://github.com/user-attachments/assets/d5277f5c-0dc4-4637-80c6-7104de2dadf9" />
The screenshot shows the verification of the MySQL client installation on the client EC2 server using the mysql --version command. 
The output confirms that MySQL Client version 8.4.10 is installed successfully on the Ubuntu operating system.

<img width="568" height="158" alt="image" src="https://github.com/user-attachments/assets/6579f8ef-9f39-4ca1-ab1b-5adfba4d7b29" />
To enable communication between the mysql-client and mysql-server EC2 instances,the inbound rules of the mysql-server Security Group were updated. 
Since MySQL uses TCP port 3306* by default, a new inbound rule was created to allow the client instance to establish a connection with the MySQL Server. 
Using the client's private IP address with the `/32` CIDR notation restricts access to a single host. 
This is a security best practice because it prevents unauthorized devices from accessing the MySQL database.
The source was not configured as `0.0.0.0/0`,which would allow connections from any IP address on the internet. 
Restricting access to the client instance satisfies the principle of least privilege and improves the overall security of the client-server architecture. 
The mysql-server Security Group was successfully configured to accept MySQL connections only from the mysql-client EC2 instance over TCP port 3306.  
This allows secure communication between the two instances within the same Amazon Virtual Private Cloud (VPC) while preventing unauthorized access from external sources.
Verifying the installed version ensures that the MySQL client is available and ready to establish connections with the remote MySQL database server. This step confirms that the client server has been configured with the necessary software to communicate with the database server as part of the client-server architecture.
This confirms that the client server is accessible and ready for the installation and configuration of the software required to communicate with the MySQL database server.

<img width="553" height="408" alt="image" src="https://github.com/user-attachments/assets/3b2f8a17-a8cb-48d3-895e-627b74e33041" />
The MySQL Server configuration file (mysqld.cnf) was reviewed using the sudo cat /etc/mysql/mysql.conf.d/mysqld.cnf command to examine the server's default configuration settings. 
Alternatively, the file can be opened with a text editor such as vi for modification. 
The configuration file contains important settings that control the operation of the MySQL server, including the service user, default port (3306), data directory, network configuration, logging options, and performance parameters. 
During the review, particular attention was given to the bind-address parameter, which determines the network interfaces on which the MySQL server listens for incoming connections. 
The default configuration showed that the server was configured to accept only local connections, indicating that this setting would need to be modified to allow secure communication with the MySQL client EC2 instance.

<img width="554" height="433" alt="image" src="https://github.com/user-attachments/assets/23747502-0002-4b23-a02d-ebc36b2c2308" />
After configuring the MySQL server to allow remote connections, a dedicated remote user was created to enable secure communication from the MySQL client EC2 instance. 
The MySQL interactive shell was accessed using the sudo mysql command, allowing administrative access as the root user.
A new user named remote_user was created and restricted to connections from the client server's private IP address (172.31.18.229) to improve security. 
An incorrect user entry was removed, and the correct remote user was granted full privileges on the MySQL server using the GRANT ALL PRIVILEGES command. 
The changes were applied using FLUSH PRIVILEGES, and the MySQL session was closed with the exit command. 
This configuration completed the authentication and authorization setup, allowing the client EC2 instance to securely connect to the remote MySQL database server.

<img width="554" height="408" alt="image" src="https://github.com/user-attachments/assets/f459b424-8166-40ce-9b6c-7170add6d810" />
After configuring the MySQL server, creating a remote user, and updating the AWS Security Group rules, the MySQL client EC2 instance was used to test the remote database connection. 
The connection was established using the MySQL command-line utility with the command mysql -u remote_user -p -h 172.31.31.73, where the remote username, password authentication, and private IP address of the MySQL server were specified. 
The successful display of the MySQL monitor confirmed that the client server was able to communicate with the database server, that remote authentication was correctly configured, and that communication through TCP port 3306 was allowed. 
After connecting, the SHOW DATABASES; SQL query was executed to verify database access, displaying the default MySQL databases. 
This successful test confirmed that the MySQL client-server architecture was implemented correctly, allowing secure remote database connections over the AWS private network.
