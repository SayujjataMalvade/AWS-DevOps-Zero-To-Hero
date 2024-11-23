# Elastic Cloud Compute (EC2)

EC2 is used to create a virtual server on a public platform, which is elastic in nature, meaning it can scale up or down depending on your requirements. It contains CPU, RAM, and Disk.

---

## Why Use EC2 Instances?

There are three main reasons to use EC2 instances:

1. **Management**: AWS takes care of upgrading the server.
2. **Security**: AWS handles server security issues.
3. **Cost**: You are only charged while the instance is running. If you stop your EC2 instance, you are not charged, but you must still pay for associated resources like Elastic IP and attached volumes.

Additionally, EC2 is a region-specific service.

---

## Types of EC2 Instances

1. **General Purpose**  
   Suitable for a variety of workloads, balancing compute, memory, and network resources.

2. **Compute Optimized**  
   Instances that provide a higher ratio of compute power compared to other instance types.

3. **Memory Optimized**  
   Instances designed for fast performance of memory-intensive operations, offering high memory capacity.

4. **Storage Optimized**  
   Instances designed for workloads that require high, sequential read and write access to large data sets on local storage.

5. **Accelerated Compute**  
   Instances designed for applications that require hardware accelerators, such as GPUs or FPGAs.

---

## Regions

Regions are geographical areas where AWS has its data centers.

---

## Availability Zones (AZs)

Availability Zones are discrete data centers within a region, offering high availability and fault tolerance.
