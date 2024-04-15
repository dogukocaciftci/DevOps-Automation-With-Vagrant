# DevOps Automation for Java Application with Vagrant

This repository houses the automation scripts and configurations necessary to setup a full-stack Java application environment using Vagrant, Bash, and various services such as MySQL, Memcached, RabbitMQ, Tomcat, and Nginx.

## Project Structure

- `Vagrantfile` - Configurations for the VMs.
- `backend.sh` - Script for backend setup including database and message broker.
- `memcache.sh` - Installation and setup of Memcached.
- `mysql.sh` - Setup for MySQL database, including schema and user privileges.
- `rabbitmq.sh` - Setup for RabbitMQ message broker.
- `tomcat.sh`, `tomcat_ubuntu.sh` - Setup scripts for Tomcat server.
- `application.properties` - Configuration properties for the Java application.

## Setup Instructions

1. **Prerequisites**: Ensure you have Vagrant and VirtualBox installed on your system.
2. **Clone the Repository**: Clone this repository to your local machine.
3. **Start Vagrant**: Navigate to the directory containing `Vagrantfile` and run the following command to start and provision the virtual machines:
   ```
   vagrant up
   ```
4. **SSH into VM**: Once the VMs are up, you can SSH into them using:
   ```
   vagrant ssh [vm_name]
   ```
5. **Manual Steps**: Some steps may require manual intervention as described in the script comments.

## Services Setup

The setup scripts included in this repository automate the installation and configuration of the following services:
- **MySQL**: Database service setup with initial configurations for user and database creation.
- **Memcached**: A distributed memory object caching system.
- **RabbitMQ**: A message broker setup with initial user configuration.
- **Tomcat**: Java application server setup, deployment configurations, and optimizations.
- **Nginx**: (Assuming it's part of the setup based on the initial description, though no script provided)

## Validation

After the setup is complete, validate the services by accessing the configured ports via the browser or command line tools to ensure they are running as expected.

## Contributing

Contributions to this project are welcome! Please fork the repository and submit pull requests with your enhancements. For major changes, please open an issue first to discuss what you would like to change.


# Prerequisites
#
- JDK 11 
- Maven 3 
- MySQL 8

# Technologies 
- Spring MVC
- Spring Security
- Spring Data JPA
- Maven
- JSP
- Tomcat
- MySQL
- Memcached
- Rabbitmq
- ElasticSearch
# Database
Here,we used Mysql DB 
sql dump file:
- /src/main/resources/db_backup.sql
- db_backup.sql file is a mysql dump file.we have to import this dump to mysql db server
- > mysql -u <user_name> -p accounts < db_backup.sql


