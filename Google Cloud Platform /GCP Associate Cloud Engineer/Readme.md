# **Google Cloud Associate Cloud Engineer**

## **Introduction**
GCP offers **200+ services**, and this exam expects knowledge of **40+ services** in detail. It evaluates your decision-making abilities, such as selecting the appropriate service for specific situations.

Imagine provisioning or renting resources only when needed and releasing them when they’re no longer required.  
This concept is called **on-demand provisioning**, where we trade **capital expense** for **variable expense**.  

GCP provides over **200 services**, running on the same infrastructure that powers products with over **1 billion users** like Gmail, Google Search, and YouTube.

---

## **Table of Content**
1. Introduction to cloud and GCP  
2. Understanding regions and zones  
3. Understanding compute services  
4. Optimizing usage and cost  
5. Command Line Utility  
6. Instance group  
7. Load balancing  
8. Managed services  
9. Compute solution in Google Cloud  
10. Container orchestration and Kubernetes  
11. Google Cloud Function  
12. Google Cloud Run  
13. Encryption with Cloud KMS  
14. Block and file storage in Google Cloud Platform  
15. Object storage  
16. Authentication and authorization  
17. Databases  
18. Asynchronous communications  
19. Private Network in Google Cloud  

---

## **Regions and Zones**

### **a. Regions**
Imagine setting up data centers in different regions worldwide—this is made simple with **Google Cloud’s 20+ regions**, expanding annually.  
Benefits include:  
1. **High availability:** Requests are redirected to the nearest available region in case of unavailability.  
2. **Low latency:** User requests are served by the nearest available data center.  
3. **Global footprint:** For example, a startup in Gurgaon can easily go global by deploying its application in multiple regions.  
4. **Adherence to government regulations.**

---

### **b. Zones**
Zones allow for **high availability** within the same region.  
- Google Cloud provides at least **3 zones per region**, ensuring **fault tolerance**.  
- Each zone consists of one or more discrete clusters housed in data centers.  
- Zones within a region are connected by **low-latency links**.

---

### **Region and Zone Details**

| Region Code | Region                                | Zones | Zones List                         |
|-------------|---------------------------------------|-------|-------------------------------------|
| us-west1    | The Dalles, Oregon, North America     | 3     | us-west1-a, us-west1-b, us-west1-c |


---

## **Google Compute Engine**

Whenever we want to deploy applications, we need servers and whenever we want to deploy applications on cloud, we need virtual servers. That is what google compute engine enables us to provision.
In corporate data centers, applications are deployed on physical servers.
Where do we deploy applications in the cloud?
1. Rent virtual servers.
2. Virtual Machines - Virtual Servers in GCP.
3. **Google Compute Engine (GCE)** - Provision and manage virtual machine.

Google Compute Engine allows us to:

1. Create and manage the lifecycle of Virtual Machine instances.
2. Load balancing and auto-scaling for multiple VM instances.
3. Attach storage to your VM instances.
4. Manage network connectivity and configuration for your VM instances.

### Create Instance

### Steps to Create a New VM Instance:
- Specify **names**, **labels**, and **regions**.
- Choose machine configurations (hardware configurations), including **machine families** that suit your requirements.
- Select an **operating system image**.
- Configure the firewall based on your requirements.

### Key Considerations for Hardware:
When configuring hardware, we need to account for two main factors:  
1. **Machine Family**  
2. **Machine Type**

### Compute Engine Machine Families:
Different machine families are available based on varying requirements:

1. **General Purpose (E2, N2, N2D, N1):**
   - Best in terms of price-performance ratio.
   - Suitable for:
     - Web and application servers.
     - Small-to-medium databases.
     - Development environments.

2. **Memory Optimized (M2, M1):**
   - Ultra high memory workloads.
   - Suitable for:
     - Large in-memory databases.
     - In-memory analytics.

3. **Compute Optimized (C2):**
   - Compute-intensive workloads.
   - Suitable for:
     - Gaming applications.

### Choosing Machine Types:
After selecting the machine family, the next step is to choose the specific **machine type** based on your workload.

![Google Compute Engine Machine Types](https://github.com/Aman15-design/cloud-study-resources/blob/0d69d589a8f4dd218cf63ba194b06bcd950763cb/Google%20Cloud%20Platform%20/Resources/Google-Compute-Engine-Machine-Types.JPG "Google Compute Engine Machine Types")


### Image
**What operating system and software do you want on the instance?**  

#### Types of Images:
1. **Public Images**:
   - Provided and maintained by Google, open-source communities, or third-party vendors.
   
2. **Custom Images**:
   - Created by you for your specific project.

## Setting up an HTTP Server

### Commands:
```bash
sudo su -
#! /bin/bash
sudo su
apt update
apt -y install apache2
sudo service apache2 start
sudo update-rc.d apache2 enable
echo "Hello World" > /var/www/html/index.html
echo "Hello world from $(hostname) $(hostname -I)" > /var/www/html/index.html



