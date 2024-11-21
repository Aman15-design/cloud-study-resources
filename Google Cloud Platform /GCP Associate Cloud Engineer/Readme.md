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
