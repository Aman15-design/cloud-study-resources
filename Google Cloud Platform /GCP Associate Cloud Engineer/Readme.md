# Google Cloud Associate Cloud Engineer

## Introduction
GCP has 200+ services. This exam expects knowledge of 40+ services.
Exam expects in-depth knowledge about these services.
Exams test your decision making abilities like which services do you choose in which situation?

How about provisioning or renting resources when we need them and releasing them back when you do not need them?<br>
This is called on demand provisioning. <br> 
Here we are trading capital expense for variable expense. <br>
GCP provides 200+ services. This is the same infrastructure that power 8 services with over 1 billion users: Gmail, Google Search, YouTube etc.

## Table of Content
  1. Introduction to cloud and GCP
  2. Understanding regions and zones
  3. Understanding compute services 
  4. Optimizing usage and cost
  5. Command Line Utility 
  6. Instance group
  7. Load balancing
  8. Managed services 
  9. Compute Solution in google cloud 
  10. Container orchestration and kubernetes
  11. Google cloud function
  12. Google cloud run
  13. Encryption with cloud kms
  14. Block and file storage in google cloud platform
  15. Object storage
  16. Authentication and authorization
  17. Databases
  18. Asynchronous communications
  19. Private Network in Google cloud

## Regions and zones


a. Regions


Imagine setting up data centers in different regions around the world, would that be easy? <br>
Google provides 20+ regions around the world which are expanding every year. <br>
This would be lead to: <br>
  1. high availability as requests would be diverted to the nearest available region in case of unavailability due to any reason.
  2. Low latency as nearest available data center could be used to serve user request
  3. Global footprints, suppose a startup in Gurgaon wants to go global, it can be done easily by deploying the application in multiple regions.
  4. Adhere to government

<br> 
b. Zones
<br> 
<br> 
Zones allow us to achieve high availability in the same regions. Google cloud has at least 3 zones in the same region. This allows for increased availability and fault tolerance. <br>
Each zone has one or more discrete clusters ( that are housed in data centers). Zones in a region are connected with low latency links. <br>
<br>
<br>


| Region Code | Region                                | Zones | Zones List                  |
|-------------|---------------------------------------|-------|-----------------------------|
| us-west1    | The Dalles, Oregon, North America     | 3     | us-west1-a, us-west1-b, us-west1-c |




