# task2
AWS EC2 SSH Connection Project

## 🎯 Objective
To launch an AWS EC2 instance, connect to it using SSH via terminal, and verify the connection.

---

## 🧭 Steps Followed

### 1️⃣ Launch an EC2 Instance
- Logged in to the AWS Management Console.
- Navigated to *EC2 → Instances → Launch Instances*.
- Selected an AMI (e.g., **Ubuntu 22.04*).
- Chose an instance type (e.g., t2.micro for free tier).
- Configured security group: allowed *SSH (port 22)* from my IP.
- Created or selected an existing key pair and downloaded the .pem file.
- Clicked *Launch Instance*.

### 2️⃣ Set Permissions for the Key File
- Opened terminal and navigated to the directory containing the .pem file:
```bash
cd /path/to/keyfile

