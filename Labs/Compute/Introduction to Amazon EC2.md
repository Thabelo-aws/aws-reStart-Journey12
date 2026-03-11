<b>Introduction to Amazon EC2<b>
Overview

<b>Amazon Elastic Compute Cloud (Amazon EC2)<b> is a web service that provides resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers.

Topics covered:
Launch a web server with termination protection enabled
Monitored the EC2 instance
Modified the security group that my web server is using to allow HTTP access

<img width="419,75" height="164,75" alt="image" src="https://github.com/user-attachments/assets/286bfa2b-1030-411e-9ec5-5ee6ce6b606e"/>

To launch my EC2 instance, I start by choosing an Amazon Machine Image (AMI). The AMI includes everything my instance needs to run, such as the operating system and default settings. I keep the default Amazon Linux 2023 AMI since it’s already selected for me. Next, I choose the instance type. I select a t3.micro instance, which gives me 2 virtual CPUs and 1 GiB of memory—perfect for this lab.
Because I won’t be logging into the instance, I continue without a key pair. Then I move on to the network settings. I select the Lab VPC, and I create a security group called Web Server security group with a description for my web server. Since I won’t be using SSH, I remove the default SSH rule to make the instance more secure.
For storage, I keep the default 8 GiB root volume. In the advanced settings, I enable termination protection to prevent accidental deletion. I also paste a user data script that automatically installs and starts an Apache web server and creates a simple “Hello From Your Web Server!” webpage.
Once all settings are configured, I launch the instance and view it in the console. The instance first shows as Pending, and after a short while it changes to Running. I wait until the status checks show 3/3 passed, confirming that my web server is successfully up and running.

<img width="374.5" height="295.5" alt="image" src="https://github.com/user-attachments/assets/e840478b-5c6e-4214-8654-9fb058403183" />

I can’t access my web server right now because my security group isn’t allowing inbound traffic on port 80, which is the port used for HTTP requests. This shows how a security group works like a firewall by controlling what network traffic can go in and out of my instance.

![Uploading image.png…]()
redcrffvgt hgbudchyugb dhrbfcyueryugb 
