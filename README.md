# CloudComputing
Deployment of a MySQL-based application on Azure cloud with NodeJS

1) The Database:
• it is a relational database management system that stores a database consisting of one
or more tables.
• There is a firewall that only allows the Data Server to have access to it.
(2) The Data Server:
• It is a virtual machine, provisioned in the cloud, running Windows 10 operating system
(version 20H2), with one virtual CPU, and a minimum of 4 GB of memory.
• It runs an NodeJS/Express server with an API to for fetching data from the database.
• It receives all its requests from the Application Server.
(3) The Application Server:
• It is a real physical computer (e.g., your laptop)
• It has a Windows (or Linux) operating system
• It runs a Node/JS Express server with an API that allows it to take requests from users on the Internet


How the system operates: 
• The user sends a request for data through the client agent to the Express server on the
Application Server.
• The Express server on the Application Server initiates a request to the Express server on
the Data Server to get some data.
• The Express server on the Virtual machine sends a query to the database to fetch data
based on the user’s request.
• This server may perform some processing on the data before sending it to the user.
