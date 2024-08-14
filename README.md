# V Profile Project - Kubernetes Deployment
In this project, I deployed a multi-tier web application called V Profile onto a Kubernetes cluster. The application was previously containerized and tested in earlier projects.

# Key Steps:
-Kubernetes Cluster Setup: I used Kops to set up a production-grade Kubernetes cluster.
-Containerized Application: The V Profile application, which includes components like MySQL, was containerized and is now ready for deployment.
-Persistent Storage: I created an EBS volume for MySQL to ensure data persistence and configured Kubernetes to manage this storage.
-Node Labeling: Nodes in the cluster were labeled based on availability zones to ensure that the database pod runs in the correct zone.
-Kubernetes Definition Files: I wrote Kubernetes YAML files to define and deploy the necessary resources, including deployments, services, secrets, and volumes.
This project showcases the process of taking a containerized application and running it in a production environment using Kubernetes, ensuring it meets the requirements for high availability, fault tolerance, and scalability.
# Prerequisites
#####
- JDK 11
- Maven 3
- MySQL 8 

# Technologies 
- Spring MVC
- Spring Security
- Spring Data JPA
- Maven
- JSP
- MySQL
# Database
Here,we used Mysql DB 
MSQL DB Installation Steps for Linux ubuntu 14.04:
- $ sudo apt-get update
- $ sudo apt-get install mysql-server

Then look for the file :
- /src/main/resources/db_backup.sql
- db_backup.sql file is a mysql dump file.we have to import this dump to mysql db server
- > mysql -u <user_name> -p accounts < db_backup.sql
