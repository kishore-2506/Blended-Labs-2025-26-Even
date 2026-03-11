# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**: KISHORE M
* **Register Number**: 212223040100
* **Date of Submission**: 27-02-2026
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

(Write the steps you followed in your own words)

First, I logged in to the AWS Management Console using my AWS account and navigated to the Amazon EC2 service dashboard to explore the available options like Instances, AMIs, Key Pairs, and Security Groups. Next, I clicked on Launch Instance, selected the Amazon Linux 2 AMI, and chose the t2.micro instance type under the free tier. I configured the instance name, created a new key pair, and downloaded the .pem file. Then, I configured the Security Group by allowing inbound rules for SSH (Port 22) from my IP address and HTTP (Port 80) from anywhere. After reviewing all configurations, I launched the EC2 instance. Once the instance was in the running state, I copied the Public IP address and connected to the instance using SSH through the terminal with the key pair file. After successful login, I verified the connection by running basic Linux commands. After testing the instance, I performed basic instance operations such as Stop, Start, and Reboot from the EC2 console and observed the status changes in the Monitoring tab. Finally, I terminated the instance to avoid unnecessary charges.

---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Dashboard / Instance List

<img width="1920" height="1200" alt="Screenshot (105)" src="https://github.com/user-attachments/assets/fc0b23f6-07e6-4d47-9d4f-f952ffe11fe4" />


---

### Screenshot 2: SSH Connection to Instance

<img width="1920" height="1200" alt="Screenshot (111)" src="https://github.com/user-attachments/assets/eed131d3-5c70-44e2-acfe-8f3d4325adea" />



### Screenshot 3: Instance Monitoring / Status

<img width="1920" height="1200" alt="Screenshot (112)" src="https://github.com/user-attachments/assets/d9dfa90f-0b26-4fcf-bce5-66f7a8ccaeca" />


## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.
