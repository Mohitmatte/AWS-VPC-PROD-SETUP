# 🚀 Production-Ready AWS Infrastructure Deployment

This project showcases a **highly available and secure AWS infrastructure** setup using the AWS Management Console (UI). The infrastructure follows industry best practices for scalability, fault tolerance, and security, making it suitable for production environments.

## 🧱 Architecture Overview

The deployment includes:

- 🏗️ A **Virtual Private Cloud (VPC)** with:
  - Public and Private Subnets
  - Two Availability Zones (AZs) for high availability

- 🖥️ **EC2 Instances** in private subnets (no public IPs)

- ⚖️ **Application Load Balancer (ALB)** to distribute traffic across instances

- 🔁 **Auto Scaling Group (ASG)** to handle varying loads and ensure availability

- 🌐 **NAT Gateway** in each AZ to allow instances in private subnets to access the internet securely

- 🔐 Proper use of **Security Groups** and **Route Tables**

## 📊 Architecture Diagram

![AWS Infrastructure Diagram](https://github.com/Mohitmatte/AWS-VPC-PROD-SETUP/blob/main/VPC_.png)

## 🛡️ Security Considerations

- All EC2 instances are in private subnets with no direct internet exposure
- Internet access provided only through NAT Gateways
- ALB handles external requests and routes traffic to instances
- Custom security groups restrict inbound/outbound traffic

## 🛠 Technologies Used

- Amazon VPC
- EC2 Instances
- Application Load Balancer
- Auto Scaling Groups
- NAT Gateways
- Subnets, Route Tables, Internet Gateway
- AWS Management Console (UI)

---

## 💡 Future Improvements

- Migrate this setup to Infrastructure as Code (Terraform / CloudFormation)
- Enable CloudWatch monitoring and logging
- Add Bastion Host for secure SSH access to private instances

---

## 🙋‍♂️ Author

**Mohit Dushyant Matte**  
Fresher DevOps & Cloud Engineer | Data Science & Python Developer Intern    
