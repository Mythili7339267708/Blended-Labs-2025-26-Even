# Lab 5 – Build a Database Server (AWS)

## Author

* **Name**: V MYTHILI
* **Register Number**: 212223040123


---

## Objective

The objective of this experiment is to understand how to deploy and configure a database server in AWS. This lab focuses on launching an EC2 instance, installing a database management system (DBMS), configuring basic database settings, creating a sample database, and validating connectivity to the database server.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing VPC and EC2 knowledge (from previous labs)
* Basic knowledge of Linux commands and SQL

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Security Groups
* SSH Client (Terminal / PuTTY)
* MySQL / MariaDB / PostgreSQL (any one)

---

## Tasks Performed

### Task 1: Launch EC2 Instance for Database Server

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type and configure key pair and security group.

---

### Task 2: Configure Security Group for Database Access

Modify the security group to allow:

* SSH (Port 22) for remote access
* Database port (e.g., MySQL – 3306 or PostgreSQL – 5432)

---

### Task 3: Connect to EC2 Instance

Connect to the EC2 instance using SSH from your local machine.

---

### Task 4: Install Database Server

Install a database server software such as MySQL, MariaDB, or PostgreSQL on the EC2 instance using package manager commands.

---

### Task 5: Start and Configure Database Service

Start the database service and configure basic settings such as root password and user privileges.

---

### Task 6: Create a Sample Database

Create a sample database and a table inside it. Insert a few records into the table.

---

### Task 7: Test Database Connectivity

Test the database server by connecting to it locally or remotely and performing basic SQL queries.

---

## Workflow 


1.Create a DB Security Group in VPC with MySQL/Aurora port 3306 allowed from Web Security Group.

2.Create a DB Subnet Group using subnets from us-east-1a and us-east-1b in Lab VPC.

3.Launch a MySQL Multi-AZ RDS instance named lab-db with username main and database lab.

4.Wait until the RDS status becomes Available, then copy the Endpoint from Connectivity & Security.

5.Open the WebServer IP, go to the RDS page, enter the endpoint and database credentials, then test the Address Book application.

---

## Output Screenshots 

### Screenshot 1: EC2 Instance for Database Server

<img width="1920" height="953" alt="image" src="https://github.com/user-attachments/assets/427babc6-f807-4656-b1fe-d242a249bd54" />

---

### Screenshot 2: Database Service Running

<img width="1919" height="948" alt="image" src="https://github.com/user-attachments/assets/be9c9c65-1d64-4928-9371-6c7ce963923a" />

<img width="1920" height="962" alt="image" src="https://github.com/user-attachments/assets/898e5d25-cb34-4da6-8efe-ad324fd90e78" />

---

### Screenshot 3: Sample Database and Table

<img width="1920" height="1021" alt="image" src="https://github.com/user-attachments/assets/ba1be8b4-987b-494b-9de0-a1eedd9dceac" />

<img width="1920" height="1014" alt="image" src="https://github.com/user-attachments/assets/0456f8aa-e319-4e0a-864d-2a822df44276" />

---

## Result

This experiment demonstrated how to build a database server in AWS using an EC2 instance. By installing and configuring a DBMS, creating a sample database, and testing connectivity, the fundamentals of hosting and managing a cloud-based database server were underst
