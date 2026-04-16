# Cloud_Computing_Practicals

Cloud computing delivers services like storage, servers, and software over the internet instead of local systems. Platforms like Amazon Web Services provide scalable, cost-effective resources. It enables remote access, flexibility, and easy data management for users and businesses.

Cloud Computing Practicals

This repository contains a comprehensive set of practical exercises designed to build hands-on experience with leading cloud platforms such as Amazon Web Services, Microsoft Azure, and Google Cloud Platform. These practicals cover essential cloud concepts including compute services, storage, networking, scaling, monitoring, and private cloud setup.

The goal of this project is to provide real-world exposure to cloud infrastructure and prepare students for academic exams, certifications, and industry-level work.


---

Table of Contents

1. Introduction to Cloud Platforms


2. Launching an Amazon EC2 Instance


3. Virtual Private Cloud (VPC) Setup


4. Auto Scaling and Load Balancing


5. Static Website Deployment


6. Monitoring with CloudWatch


7. OpenStack Installation




---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

 1. Introduction to Cloud Platforms

Objective

To understand the basic structure and interface of modern cloud platforms.

Description

Cloud platforms provide on-demand computing services such as virtual machines, databases, and storage systems. Each platform has its own dashboard and service naming but follows similar core concepts.

Steps

Create free-tier accounts on:

AWS

Azure

GCP


Explore dashboards and identify key services:

Compute: EC2, Virtual Machines, Compute Engine

Storage: S3, Blob Storage, Cloud Storage

Networking: VPC, Virtual Network


Study pricing calculators to understand cost estimation


--Outcome

Familiarity with cloud dashboards

Understanding of service categories



---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

2. Launch Your First Amazon EC2 Instance

Objective

To deploy and connect to a virtual machine in the cloud.

Description

Amazon EC2 (Elastic Compute Cloud) allows users to create virtual servers in minutes.

Steps

Go to AWS Management Console

Launch a new EC2 instance

Select AMI (Amazon Linux 2)

Choose instance type (t2.micro – free tier)

Configure Security Group:

Allow SSH (port 22)


Download key pair

Connect using SSH:

ssh -i key.pem ec2-user@your-public-ip


--Outcome

Successfully deployed VM

Remote server access using SSH



---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

3. Set Up a Virtual Private Cloud (VPC)

Objective

To create a secure and isolated cloud network.

Description

A VPC allows you to define your own network configuration, including IP ranges, subnets, and routing.

Steps

Create a custom VPC

Create:

Public subnet (for internet access)

Private subnet (for secure resources)


Launch EC2 instances in both subnets

Attach Internet Gateway to VPC

Configure route table for public subnet

Create NAT Gateway for private subnet

Update private subnet route table


--Outcome

Understanding of cloud networking

Secure architecture implementation



---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

4. Configure Auto Scaling and Load Balancing

Objective

To handle traffic dynamically and ensure high availability.

Description

Auto Scaling automatically adjusts the number of instances based on demand, while Load Balancer distributes incoming traffic.

Steps

Create Launch Template

Create Auto Scaling Group

Set:

Minimum instances: 1

Maximum instances: 3


Configure scaling policy:

Scale up when CPU > 70%


Deploy Application Load Balancer (ALB)

Register instances with target group

Simulate traffic using stress tools


--Outcome

Improved fault tolerance

Dynamic scaling based on load

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

5. Deploying a Static Website

Objective

To host a static website using cloud storage.

Description

Static websites consist of HTML, CSS, and JavaScript files and can be hosted using storage services.

Steps

Choose platform:

AWS S3

Azure Blob Storage

GCP Cloud Storage


Create storage bucket

Upload index.html file

Enable static website hosting

Set permissions for public access

Access website via public URL


--Outcome

Live website hosted on cloud

Understanding of storage-based hosting

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

6. Monitor Resources Using CloudWatch

Objective

To track performance and set alerts.

Description

Cloud monitoring tools help track usage, performance, and system health.

Steps

Open CloudWatch dashboard

Monitor EC2 metrics:

CPU utilization

Network usage


Create Alarm:

Trigger when CPU > threshold


Configure SNS topic:

Add email notifications


Test by increasing CPU load


--Outcome

Real-time monitoring

Alert system setup

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

7. Install OpenStack (Local Cloud)

Objective

To set up a private cloud environment.

Description

OpenStack is an open-source platform used to build private and public clouds.

Steps:

Install prerequisites (Linux system)

Clone DevStack repository

Create local.conf file

Run installation:

./stack.sh

Wait 20–40 minutes

Access dashboard:

http://localhost/dashboard

Login:

Username: admin

Password: admin



--Outcome

Hands-on private cloud setup

Understanding of cloud internals



--Technologies Used

AWS (EC2, S3, VPC, CloudWatch)

Azure Cloud

GCP

OpenStack


--Learning Outcomes

After completing this project, you will:
Understand cloud computing fundamentals
Deploy and manage virtual machines
Design secure network architectures
Implement auto scaling and load balancing
Host websites on cloud storage
Monitor and optimize cloud resources
Work with both public and private cloud environments

 --Conclusion
This practical guide provides a strong foundation in cloud computing by combining theory with real-world implementation. It is ideal for students, beginners, and professionals preparing for cloud certifications or technical interviews.
