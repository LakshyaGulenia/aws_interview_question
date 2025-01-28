
# AWS VPC Interview Questions

### 1. How does VPC peering work?
VPC peering connects two VPCs for communication using private IPs. Traffic stays within AWS without transiting the internet.

---

### 2. What are route tables, and why are they important?
Route tables define paths for traffic within a VPC and to external destinations (e.g., Internet Gateway, NAT Gateway).

---

### 3. Internet Gateway vs. NAT Gateway:
- **Internet Gateway (IGW):** Enables internet access for public subnet instances.
- **NAT Gateway:** Provides outbound internet access for private subnet instances.

---

### 4. Purpose of Security Groups and NACLs:
- **Security Groups:** Instance-level rules for inbound/outbound traffic.
- **NACLs (Network Access Control Lists):** Subnet-level, stateless rules for traffic filtering.

---

### 5. Restricting traffic between subnets:
Use NACLs or security group rules to limit access based on IP ranges or ports.

---

### 6. Designing a multi-region VPC architecture:
- Use Transit Gateway or VPC peering for inter-region connectivity.
- Ensure redundancy, low latency, and compliance with regulations.

---

### 7. AWS Transit Gateway vs. VPC Peering:
- **Transit Gateway:** Central hub for connecting multiple VPCs and on-premises networks.
- **VPC Peering:** One-to-one connection between VPCs.

---

### 8. Elastic Load Balancer (ELB) with VPC:
Distributes incoming traffic across instances in subnets and enhances scalability and fault tolerance.

---

### 9. Ensuring high availability in a VPC design:
- Deploy resources across multiple Availability Zones.
- Use redundant Internet Gateways, NAT Gateways, and load balancers.

---

### 10. VPC limits:
- **Default limits:** 5 VPCs per region, 200 subnets per VPC.
- Limits can be increased via AWS Support.



# AWS Interview Questions for Freshers

## 1. What is AWS?
AWS (Amazon Web Services) is a secure cloud services platform offering compute power, database storage, content delivery, and other functionalities to help businesses scale and grow.

---

## 2. What are the main components of AWS?
The main components of AWS include:
- **EC2**: Virtual servers in the cloud.
- **S3**: Scalable storage in the cloud.
- **RDS**: Managed relational database service.
- **Lambda**: Serverless compute service.
- **VPC**: Virtual Private Cloud for network isolation.

---

## 3. Explain the difference between S3 and EBS.
- **S3 (Simple Storage Service)**: Object storage for storing and retrieving data, suitable for static assets.
- **EBS (Elastic Block Store)**: Persistent block storage for use with EC2 instances, suitable for databases and file systems.

---

## 4. What is the difference between a public and a private subnet?
- **Public Subnet**: Resources can access the internet via an Internet Gateway.
- **Private Subnet**: Resources do not have direct internet access and are typically used for backend services.

---

## 5. What is an IAM role?
An IAM role is an AWS identity with specific permissions that can be assumed by trusted entities, such as AWS services, users, or applications, to access AWS resources securely.

---

## 6. What is Auto Scaling in AWS?
Auto Scaling is a service that automatically adjusts the number of EC2 instances in a group based on predefined conditions, ensuring high availability and cost efficiency.

---

## 7. What is the difference between horizontal and vertical scaling?
- **Horizontal Scaling**: Adding more instances to distribute the load (scaling out).
- **Vertical Scaling**: Increasing the capacity of a single instance (scaling up).

---

## 8. What are security groups and NACLs?
- **Security Groups**: Virtual firewalls for EC2 instances, controlling inbound and outbound traffic at the instance level.
- **NACLs (Network Access Control Lists)**: Stateless firewalls at the subnet level, controlling inbound and outbound traffic for subnets.

---

## 9. What is CloudFront?
CloudFront is a content delivery network (CDN) service that delivers content with low latency by caching copies in edge locations worldwide.

---

## 10. How does AWS Lambda work?
AWS Lambda is a serverless compute service that lets you run code in response to events. You upload your code, set triggers, and Lambda automatically manages the compute resources.

---

## 11. What is an Elastic Load Balancer (ELB)?
An Elastic Load Balancer distributes incoming traffic across multiple targets (e.g., EC2 instances) to ensure high availability and fault tolerance.

---

## 12. What is the purpose of Route 53?
Route 53 is a scalable DNS and domain name registration service that routes users to AWS resources or external websites based on routing policies.

---

## 13. What is the Shared Responsibility Model in AWS?
The Shared Responsibility Model defines AWS's and the customer's responsibilities:
- **AWS**: Responsible for the security of the cloud (infrastructure, hardware).
- **Customer**: Responsible for security in the cloud (data, applications, identity management).

---

## 14. What are AWS Availability Zones and Regions?
- **Availability Zones**: Data centers within a region, isolated but interconnected.
- **Regions**: Geographical areas with multiple Availability Zones, allowing redundancy and disaster recovery.

---

## 15. What is a VPC?
A VPC (Virtual Private Cloud) is a logically isolated network in AWS where you can launch AWS resources and define networking configurations, including subnets, route tables, and gateways.

---

## 16. Explain AWS EC2 pricing models.
- **On-Demand**: Pay-as-you-go.
- **Reserved Instances**: Significant discounts for long-term commitments.
- **Spot Instances**: Low-cost option for flexible workloads.
- **Savings Plans**: Flexible pricing for consistent usage.

---

## 17. What is a NAT Gateway?
A NAT Gateway allows instances in a private subnet to connect to the internet for outgoing traffic while keeping them unreachable from the internet.

---

## 18. How can you secure your data in AWS?
- Use **IAM roles** and policies for access control.
- Enable **encryption** (S3, EBS, RDS).
- Use **CloudTrail** and **CloudWatch** for monitoring.
- Implement **security groups** and **NACLs**.

---

## 19. What is the AWS Free Tier?
The AWS Free Tier provides limited, free access to AWS services for 12 months, including 750 hours of EC2 usage, 5GB of S3 storage, and more.

---

## 20. What is the difference between RDS and DynamoDB?
- **RDS**: Managed relational database service supporting SQL-based databases.
- **DynamoDB**: NoSQL database service designed for key-value and document-based applications.
