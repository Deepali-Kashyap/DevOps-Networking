# 🛡️ AWS EC2 Security Groups: A Step-by-Step Guide

## 📌 What is a Security Group?

In AWS, a **Security Group** acts as a **virtual firewall** for your EC2 instance to control **inbound and outbound traffic**. It defines **who can access your instance** and **how they can connect** (e.g., via SSH, HTTP, etc.).

---

## 🚀 Step 1: Launch an EC2 Instance (Free Tier)

1. Go to the [AWS Console](https://console.aws.amazon.com).
2. Navigate to **EC2 > Instances**.
3. Click **Launch Instance**.
4. Choose **Amazon Linux 2023 AMI** (Free Tier Eligible).
5. Select **t2.micro** instance type (Free Tier).
6. Click **Next: Configure Security Group**.

---

## 🔐 Step 2: Create a New Security Group

You can either **create a new security group** or use an **existing one**.

- **Name:** `MyWebServerSG`
- **Description:** `Security group for web server access`
- **VPC:** Leave the default (unless you’ve created custom VPCs)

---

## ✅ Step 3: Add Inbound Rules

Here’s how to allow traffic **into** your EC2 instance:

| Type     | Protocol | Port Range | Source        | Purpose                    |
|----------|----------|------------|---------------|----------------------------|
| SSH      | TCP      | 22         | My IP         | Remote login from your IP  |
| HTTP     | TCP      | 80         | 0.0.0.0/0     | Web traffic (insecure)     |
| HTTPS    | TCP      | 443        | 0.0.0.0/0     | Secure web traffic         |

> 🔒 **Note:** Only allow **SSH (port 22)** from **your own IP**, not `0.0.0.0/0`, for security.

---

## 📤 Step 4: Configure Outbound Rules (Default OK)

By default, **all outbound traffic is allowed** — which is usually fine unless you want to restrict external access.

---

## 🟢 Step 5: Launch the Instance

1. Click **Review and Launch**.
2. Choose or create a key pair (for SSH access).
3. Click **Launch**.

---

## 🛠️ Step 6: Verify Security Group

After the instance is running:

- Go to **EC2 > Instances**
- Select your instance
- Scroll down to the **Security Groups** section
- Click on the Security Group to view or edit rules

---

## 🧠 Why Security Groups Matter in DevOps

- **Access Control:** Restrict access to services (like only allowing SSH from specific IPs).
- **Microservices:** Secure communication between EC2 instances/services.
- **Automation:** Easily configure rules using Terraform, AWS CLI, or CloudFormation.
- **Security Audits:** Keep your cloud infrastructure compliant and protected.

---

## 🔄 Common Tips

- Use **"My IP"** for safe SSH access.
- Never open **port 22 (SSH)** to the public (`0.0.0.0/0`) unless absolutely necessary.
- Use **tags** to organize security groups by environment (e.g., `Dev`, `Prod`).
- Combine with **IAM roles** and **CloudWatch** for better control and monitoring.

---

## 📚 Resources

- [AWS EC2 Documentation](https://docs.aws.amazon.com/ec2/)
- [Security Groups Overview](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html)

---
