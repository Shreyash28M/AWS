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


##  🔹  What is the difference between Security Group and NACL?
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


## 🔹  What is EBS in EC2 ?
EBS stands for Elastic Block Store. It is a block storage service in AWS used with EC2 instances.

It provides durable and high-performance storage that can be attached to EC2 instances like a hard disk.

The data in EBS persists even after the instance is stopped.

In real-world DevOps, it is used to store application data, databases, and logs.


##  🔹 What is an EC2 Instance? And what are its main components?

An EC2 instance is a virtual server in AWS used to run applications. It is created from an Amazon Machine Image (AMI) and runs in the cloud instead of physical hardware. Each EC2 instance has components like CPU, memory, storage, operating system, and networking configuration.


##  🔹 What is AMI in EC2? Why is it used?
How to answer: \
1.What is AMI \
2.What it contains \
3.Why we use it (real use case) 


AMI (Amazon Machine Image) is a pre-configured template used to launch EC2 instances. It contains the operating system, application software, and required configurations. AMIs are used to quickly create instances with the same setup, which helps in automation, scalability, and consistency across environments.

##  🔹  Important Points You Should Know
### An AMI includes:
OS (Linux/Windows) \
Pre-installed software (like Nginx, Docker, etc.) \
EBS snapshot (storage) \
Configuration settings


##  🔹 What is the difference between EBS and Instance Store?
$${\color{#FFD700}Notes}$$   
🔹 EBS (Elastic Block Store)

<img width="450" height="450" alt="image" src="https://github.com/user-attachments/assets/99092b71-bed4-4f03-afc7-93b8321fd186" />
<img width="500" height="450" alt="image" src="https://github.com/user-attachments/assets/b6e8997b-ada1-4af8-b280-70f87c472aca" />

Network-attached storage (like external hard disk) \
Persistent → data stays even if instance stops/terminates \
Used for:
Databases \
Production apps \
Important data

### 🔹 Instance Store


<img width="500" height="450" alt="image" src="https://github.com/user-attachments/assets/121479bc-51e7-4e3a-837b-4b280ab7573d" />

Temporary storage (inside the server) \
Not persistent → data lost when instance stops/terminates \
     Used for: \
Cache \
Temporary files \
Buffers 


 EBS is a persistent block storage that remains even after the EC2 instance is stopped or terminated, making it suitable for databases and critical applications. Instance Store is temporary storage attached to the instance, and its data is lost when the instance stops or terminates, so it is mainly used for cache or temporary data.

##   

