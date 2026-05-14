# Lab 1 - Introduction to AWS Identity and Access Management (IAM)

## Title
Introduction to AWS Identity and Access Management (IAM)


## Objective
The objective of this lab is to understand how AWS Identity and Access Management (IAM) controls authentication and authorization in AWS. The lab focuses on exploring IAM users and groups, analyzing attached policies, assigning users to appropriate groups based on organizational roles, and validating permissions by testing service access.


## Prerequisites
- Basic understanding of cloud computing concepts  
- AWS Academy Lab access  
- Web browser with internet connectivity  


## Tools Used
- AWS Management Console  
- AWS Identity and Access Management (IAM)  
- Amazon EC2  
- Amazon S3  


## Tasks Performed

### Task 1: Explore IAM Users and Groups
- Reviewed pre-created IAM users: user-1, user-2, user-3  
- Explored IAM groups: EC2-Admin, EC2-Support, S3-Support  
- Inspected managed and inline policies attached to groups  
**Screenshot:**

  <img width="1920" height="951" alt="image" src="https://github.com/user-attachments/assets/0d603aff-041d-48cc-b339-b0c00bec338d" />


<img width="1920" height="947" alt="image" src="https://github.com/user-attachments/assets/cd693dc8-71ee-4778-b507-04d5bfc5edd5" />

(Add screenshot here)

### Task 2: Add Users to Groups
- Added user-1 to the S3-Support group  
- Added user-2 to the EC2-Support group  
- Added user-3 to the EC2-Admin group  
**Screenshot:**  
(Add screenshot here)
<img width="1917" height="952" alt="image" src="https://github.com/user-attachments/assets/841200da-f252-4415-a2ea-9cb7036983be" />


<img width="1920" height="948" alt="image" src="https://github.com/user-attachments/assets/25d69b22-7b64-4ccb-9e63-967c2461764f" />


<img width="1920" height="958" alt="image" src="https://github.com/user-attachments/assets/fdbed719-cd24-4b7d-9593-f57e16ff7bfa" />

### Task 3: Test IAM User Permissions
- Logged in using IAM sign-in URL  
- Verified S3 access for user-1  
- Verified EC2 read-only access for user-2  
- Verified EC2 administrative access for user-3  
**Screenshot:**  
(Add screenshot here)


<img width="1920" height="955" alt="image" src="https://github.com/user-attachments/assets/71490d4f-a7a9-4b32-be31-7aa88a2f6e12" />



<img width="1920" height="957" alt="image" src="https://github.com/user-attachments/assets/c0098db6-abd1-4e99-b63f-f6ee111cea30" />



<img width="1920" height="949" alt="image" src="https://github.com/user-attachments/assets/ee12dca1-8d50-445b-99ff-8fd94c000faf" />


## Workflow
1. Accessed IAM console and reviewed users and groups.  
2. Inspected policy permissions attached to groups.  
3. Assigned users to groups based on their roles.  
4. Logged in as each IAM user using the sign-in URL.  
5. Validated permissions by accessing AWS services.  


## Learning Outcomes
- Understood the role of IAM in AWS security.  
- Learned how IAM users, groups, and policies interact.  
- Gained practical experience implementing role-based access control.  
- Verified permission enforcement through real-time service testing.  


## Conclusion
This lab provided hands-on experience with AWS IAM by demonstrating how organizations manage secure access to cloud resources. Assigning users to groups with predefined policies simplified permission management and ensured role-based access control across AWS services.


## Author
**Name:** Your Name and (Reg No)
**Course:** Introduction to Cloud Computing  

