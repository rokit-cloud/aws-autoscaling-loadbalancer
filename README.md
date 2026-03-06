# 🚀 AWS Auto-Scaling Web Application with Load Balancer

## 📋 Project Overview
Deployed a highly available, self-healing web application on AWS using 
EC2, Application Load Balancer, and Auto Scaling Group inside 
Vocareum Sandbox environment.

---

## 🏗️ Architecture
```
Internet
    ↓
Application Load Balancer (ALB)
    ↓
Auto Scaling Group
    ↓
EC2 Instance 1 | EC2 Instance 2 | EC2 Instance N
```


## ⚙️ AWS Services Used
| Service | Purpose |
|---------|---------|
| EC2 (t2.micro) | Virtual servers running the web app |
| Application Load Balancer | Distributes traffic across EC2 instances |
| Auto Scaling Group | Auto adds/removes EC2 based on CPU load |
| Launch Template | Defines EC2 configuration |
| Security Groups | Controls inbound/outbound traffic |
| Target Group | Routes requests to healthy instances |

---

## 🛠️ Setup Steps
1. Created Launch Template with Amazon Linux 2023
2. Created Target Group with HTTP health checks
3. Created Application Load Balancer (Internet-facing)
4. Created Auto Scaling Group (Min:1 / Desired:2 / Max:4)
5. Tested via Load Balancer DNS — app live!
6. Terminated instances — AWS auto-replaced them ✅

---

## ✅ What I Demonstrated
- ✅ High Availability — app stays online always
- ✅ Auto Scaling — scales up/down based on CPU
- ✅ Self Healing — auto replaces terminated instances
- ✅ Load Balancing — traffic distributed evenly

---

## 🧪 Lab Environment
- Platform: Vocareum AWS Sandbox
- Region: us-west-2 (Oregon)
- Instance Type: t2.micro (Free Tier)

---

## 👨‍💻 Author
...Rokit S...
