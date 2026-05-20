# Lab 6 – Scale and Load Balance Your Architecture

## Title Scale and Load Balance Your Architecture


Author : V MYTHILI   
Reg no : 212223040123

---

## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.

---

## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch

---

## Tasks Performed

### Task 1: Review Existing Architecture

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.

---

## Workflow 

1.Create an AMI named WebServerAMI from Web Server 1 after the instance status becomes 2/2 checks passed.

2.Create a Target Group (LabGroup) and an Application Load Balancer (LabELB) using Lab VPC, Public Subnets, and Web Security Group.

3.Create a Launch Template (LabConfig) using the AMI, then create an Auto Scaling Group with:
   Desired: 2
   Min: 2
   Max: 6
   CPU target tracking: 60%

4.Verify load balancing by checking that two Lab Instance targets become healthy, then open the Load Balancer DNS name in a browser.

5.Test Auto Scaling using Load Test in the web app, confirm new instances launch automatically, then terminate Web Server 1 and submit the lab.

---

## Output Screenshots 

### Screenshot-1: Creating an AMI for Auto Scaling

<img width="1920" height="954" alt="image" src="https://github.com/user-attachments/assets/9475e751-ca74-4f20-9dcf-92db98b0f55d" />


### Screenshot-2: Creating a Load Balancer

<img width="1920" height="952" alt="image" src="https://github.com/user-attachments/assets/3480054e-9a8d-45ac-b801-344c98e6e4a7" />


<img width="1917" height="946" alt="image" src="https://github.com/user-attachments/assets/ecd71bf9-2e8a-4e84-a4d0-97deee65378a" />


### Screenshot-3: Creating a Launch Template and an Auto Scaling Group

<img width="1920" height="956" alt="image" src="https://github.com/user-attachments/assets/c0cf7da9-4352-4714-ae2b-c348d8200146" />

<img width="1920" height="952" alt="image" src="https://github.com/user-attachments/assets/37ad2714-7fc6-4f3b-9ba0-351eae5f4d65" />


### Screenshot-4: Testing Auto Scaling


<img width="1920" height="967" alt="image" src="https://github.com/user-attachments/assets/25f001ff-ddf7-4c35-abe6-2ab7a0b23fa1" />


<img width="1920" height="562" alt="image" src="https://github.com/user-attachments/assets/f79b6770-2d2d-4581-b17b-b74f8b4af6c9" />

<img width="1920" height="951" alt="image" src="https://github.com/user-attachments/assets/a59eb739-b2fb-4d5a-a486-3bc36ecd4591" />


<img width="1920" height="956" alt="image" src="https://github.com/user-attachments/assets/a326b024-e417-429f-b8dc-d8daac111150" />


### Screenshot-5: Terminating Web Server 1

<img width="1920" height="953" alt="image" src="https://github.com/user-attachments/assets/5a5a27ea-7ff8-402c-917b-d07be964f4a0" />

---


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
