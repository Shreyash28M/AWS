# EC2

## 🔹 what is ec2 
EC2 stands for Elastic Compute Cloud. It is a service in AWS that provides virtual servers in the cloud.

We use EC2 to run applications without managing physical hardware. It allows us to launch, stop, and scale servers as per requirement with a pay-as-you-go pricing model.

In DevOps, EC2 is commonly used to host applications, run CI/CD pipelines, and deploy containerized applications


## 🔹 What are the different types of EC2 instances?
“There are mainly five types of EC2 instance types based on use-case.

First is General Purpose, which provides a balance of CPU, memory, and networking. Example: t2.micro, m5.large.

Second is Compute Optimized, used for high CPU-intensive applications like batch processing. Example: c5 instances.

Third is Memory Optimized, used for high RAM applications like databases. Example: r5, x1 instances.

Fourth is Storage Optimized, used for high disk throughput like big data workloads. Example: i3 instances.

Fifth is Accelerated Computing, which uses GPUs for machine learning and graphics processing. Example: p3 instances.”


##    What is the difference between Security Group and NACL?
Security Group and NACL both are firewalls in AWS, but they work at different levels.

Security Group works at the instance level and is stateful, which means if inbound traffic is allowed, outbound is automatically allowed. It only supports allow rules.

NACL works at the subnet level and is stateless, which means we have to define both inbound and outbound rules separately. It supports both allow and deny rules.

So, Security Group provides instance-level security, while NACL provides subnet-level security.
| Feature | Security Group | NACL         |
| ------- | -------------- | ------------ |
| Level   | Instance       | Subnet       |
| Type    | Stateful       | Stateless    |
| Rules   | Allow only     | Allow & Deny |


##   What is AMI in EC2?
AMI stands for Amazon Machine Image. It is a pre-configured template used to launch EC2 instances.

It contains the operating system, application software, and required configurations.

In real-world DevOps, AMIs are used to quickly create multiple identical EC2 instances, which helps in scaling and maintaining consistency.


##   What is EBS in EC2 ?
EBS stands for Elastic Block Store. It is a block storage service in AWS used with EC2 instances.

It provides durable and high-performance storage that can be attached to EC2 instances like a hard disk.

The data in EBS persists even after the instance is stopped.

In real-world DevOps, it is used to store application data, databases, and logs.


## 
