# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**: V MYTHILI
* **Register Number**: 212223040123


---

## Objective

The objective of this experiment is to understand the fundamentals of Amazon Elastic Compute Cloud (EC2). This lab focuses on launching and managing a virtual server, understanding instance types and AMIs, connecting to an EC2 instance, monitoring its status, and performing basic instance operations such as start, stop, and terminate.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* Web browser with internet connectivity
* Basic knowledge of Linux commands (optional)

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Key Pair
* Security Group
* SSH Client (PuTTY / Terminal)

---

## Tasks Performed

### Task 1: Explore Amazon EC2 Dashboard

Explore the EC2 service dashboard in the AWS Management Console. Observe the different sections such as Instances, AMIs, Instance Types, Key Pairs, Security Groups, and Elastic IPs.

---

### Task 2: Launch an EC2 Instance

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type (t2.micro) under the free tier. Configure basic settings such as instance name, key pair, and security group.

---

### Task 3: Configure Security Group

Configure a security group to allow inbound access:

* SSH (Port 22) from your IP address
* HTTP (Port 80) from anywhere (0.0.0.0/0)

This security group acts as a firewall for the instance.

---

### Task 4: Connect to EC2 Instance

Connect to the running EC2 instance using SSH. Use the downloaded key pair and connect via terminal or PuTTY.

For Amazon Linux:

```
ssh -i "keyname.pem" ec2-user@<Public-IP>
```

---

### Task 5: Perform Basic Instance Operations

Perform the following operations from the EC2 console:

* Stop the instance
* Start the instance
* Reboot the instance

Observe the state changes of the instance.

---

### Task 6: Monitor EC2 Instance

Monitor the EC2 instance using the Monitoring tab. Observe metrics such as CPU utilization, network in/out, and instance status checks.

---

### Task 7: Terminate EC2 Instance

Terminate the EC2 instance after completing the experiment to avoid unnecessary AWS charges.

---

## Workflow (Student Explanation)

1.Launch an Amazon Web Services EC2 instance named Web Server using Amazon Linux 2023, t2.micro, Lab VPC, and vockey key pair.

2.Enable termination protection and add User Data script to install and run the Apache web server automatically.

3.Monitor the instance using Status Checks, Monitoring, System Logs, and Instance Screenshot after it reaches the Running state.

4.Update the security group by allowing HTTP (Port 80) traffic from Anywhere-IPv4 and access the web page using the Public IPv4 address.

5.Stop and resize the instance to t2.small, increase EBS storage from 8 GiB to 10 GiB, test stop protection, then stop the instance successfully.


---

## Output Screenshots 

### Screenshot 1: EC2 Dashboard / Instance List

<img width="1920" height="954" alt="image" src="https://github.com/user-attachments/assets/bc3455b6-d803-43d0-b068-78bffe485353" />


<img width="1920" height="948" alt="image" src="https://github.com/user-attachments/assets/0da3d56c-ae3b-43b0-8d2e-5d75e88486af" />


<img width="1920" height="939" alt="image" src="https://github.com/user-attachments/assets/b9cd39b0-7b0d-4b4d-8bad-2c6bd40d0dd1" />


---

### Screenshot 2: SSH Connection to Instance


<img width="1920" height="953" alt="image" src="https://github.com/user-attachments/assets/639b146f-ddc8-4d92-aca8-e51f83da2752" />


<img width="1920" height="951" alt="image" src="https://github.com/user-attachments/assets/cc6cb7c2-ec9c-4ae6-9212-ead922aee00e" />


<img width="1920" height="956" alt="image" src="https://github.com/user-attachments/assets/7e8e925f-08d3-4a9e-9535-025bf809146a" />



---

### Screenshot 3: Instance Monitoring / Status

<img width="1920" height="946" alt="image" src="https://github.com/user-attachments/assets/af3cf386-c1e1-4914-a77e-fd15a042285d" />


<img width="1920" height="948" alt="image" src="https://github.com/user-attachments/assets/5ee3f06c-7605-4966-81f5-b6cb5761b413" />


<img width="1917" height="949" alt="image" src="https://github.com/user-attachments/assets/4a29865b-bbf9-42c3-8381-c2171e4e5e0c" />


<img width="1920" height="959" alt="image" src="https://github.com/user-attachments/assets/1658445c-9f24-4fd6-9ca5-953efffc83dd" />

---

## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.
