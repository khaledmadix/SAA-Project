

![3 tier app](https://github.com/user-attachments/assets/641dd6dc-a5b6-48fc-be2d-d93ff83cc4a4)






# SAA-Project
🛠️ 3-Tier Highly Available Architecture for an E-Commerce Store (AWS)

# ✅ Overview
This diagram represents a highly available and scalable 3-tier architecture hosted on AWS, ideal for running an e-commerce web application.

# 🧱 Architecture Components
🔹 Tier 1: Web (Presentation Layer)

Amazon Route 53 – DNS routing for user traffic.

Amazon CloudFront – Content delivery network (CDN) for caching static assets.

Amazon S3 – Hosts a static site used for maintenance or basic information.

Application Load Balancer (ALB) – Distributes traffic to EC2 instances.

# 🔹 Tier 2: Application Layer

Amazon EC2 (Auto Scaling Group) – Web servers running Apache and PHP.

Amazon EFS – Shared file system across EC2 instances in different AZs.

Multi-AZ Deployment – EC2 instances are deployed in two Availability Zones for high availability.

# 🔹 Tier 3: Data Layer

Amazon RDS (MariaDB) – Relational database deployed in private subnets (multi-AZ).

Amazon ElastiCache (Memcached) – In-memory cache to improve read performance and reduce DB load.

# 🔐 Security & Network
Private and Public Subnets spread across multiple Availability Zones.

Databases and caches are isolated in private subnets for enhanced security.

EC2 instances and ALB are in public subnets for user accessibility.

# 📈 High Availability Features
Redundant setup across Availability Zone 1 & 2.    

Auto Scaling ensures the app scales up/down based on demand.

All tiers are fault-tolerant and scalable.


# Manara AWS SAA Project
Done by Khaled Madi 
khaledmadi40@gmail.com
