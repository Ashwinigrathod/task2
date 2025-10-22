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

### 3️⃣ Connect to EC2 via SSH

Obtained the Public IPv4 of the EC2 instance.

Connected using SSH:

# Ubuntu
ssh -i "your-key-file.pem" ubuntu@<EC2-PUBLIC-IP>

Typed yes if prompted to confirm host authenticity.


4️⃣ Verify Connection

Ran basic commands to confirm connectivity:

whoami
uname -a
ls -l

🧰 AWS Services Used

Amazon EC2 (Elastic Compute Cloud)

AWS Management Console


💡 Key Learnings

How to launch and configure an EC2 instance.

How to set secure key permissions for SSH.

How to connect to Linux/Ubuntu EC2 instances using ssh

Basic terminal commands to verify connectivity and manage the instance.


🧹 Cleanup (to avoid charges)

Terminated the EC2 instance after testing.

Deleted associated key pair and security group if not needed.


✅ Project Outcome

Successfully launched an AWS EC2 instance and connected via SSH terminal, verifying secure access.


👩‍💻 Author

Ashwini G. Rathod
Simplilearn Certified Cloud Architect | AWS & Azure Learner
📧 [ashwinirathod701@gmail.com]
🔗 [https://github.com/Ashwinigrathod/task2]


