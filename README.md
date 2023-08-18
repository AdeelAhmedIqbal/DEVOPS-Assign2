# DICE DEVOPS Assignment 2
## Part 1: Docker Networking
Verify that the "nginx" default page is accessible on your host machine at http://localhost:8080 
![image](https://github.com/AdeelAhmedIqbal/DEVOPS-Assign2/assets/62285793/b90deea9-268a-4698-a800-d876cb4572be)

Verify that the "httpd" default page is accessible on your host machine at http://localhost:8081.
![image](https://github.com/AdeelAhmedIqbal/DEVOPS-Assign2/assets/62285793/2cb2266f-b313-4a39-8327-2179cffb7915)

<hr>

## Docker Network Inspect Findings:
### Docker Network Information
- Name: my_network
- Id: d3158f9892e27c7d712c63265c8e7aa060b68284227c7b33492e4cc0fb010740
- Created: 2023-08-16T16:10:25.4454334+05:00
-	Scope: local
-	Driver: bridge
-	EnableIPv6: false
### IP Address Management (IPAM)
-	IPAM Driver: default
-	IPAM Options: (No specific options provided)
-	IPAM Config:
	- Subnet: 172.18.0.0/16
	- Gateway: 172.18.0.1
### Network Properties
-	Internal: false
-	Attachable: false
-	Ingress: false
-	ConfigFrom: Network configuration is not derived from another network.
-	ConfigOnly: false
### Containers Attached to the Network
1.	Container: **nginx_container**
-	Name: nginx_container
-	EndpointID: cb250ca031cf71de821bd24eb85946d8e7d7aaaa158715136ba552dcf503dda8
-	MacAddress: 02:42:ac:12:00:02
-	IPv4Address: 172.18.0.2/16
2.	Container: **httpd_container**
-	Name: httpd_container
-	EndpointID: 7ae0f7dfe40888dc5bd573dd95daa43b3c0a5a65fb66031e9cd46b5fb8d1e3e6
-	MacAddress: 02:42:ac:12:00:03
-	IPv4Address: 172.18.0.3/16

<hr>

**Docker Container ls** 
![image](https://github.com/AdeelAhmedIqbal/DEVOPS-Assign2/assets/62285793/c0d0362e-50ec-479e-b494-5eb74c457c76)

<hr>

# Part 2: Multi-Container Application Deployment using Docker Compose
### Docker compose up

Use the **docker-compose up** command to build and run the application. Verify that the web application is accessible from a web browser and that the database is running

![image](https://github.com/AdeelAhmedIqbal/DEVOPS-Assign2/assets/62285793/5821d79b-5571-4e27-94c8-daf4e2ac8a74)

![image](https://github.com/AdeelAhmedIqbal/DEVOPS-Assign2/assets/62285793/da1d853e-ded6-4fa8-a2f9-ff500ce92cde)

**Modify** the Docker file for the web application container to include a new feature

![image](https://github.com/AdeelAhmedIqbal/DEVOPS-Assign2/assets/62285793/b7f4d119-2ecb-4488-8cb9-2cd4a0a7591f)

### Implement a scaling strategy
![image](https://github.com/AdeelAhmedIqbal/DEVOPS-Assign2/assets/62285793/ac7cdcc3-bbda-4f7e-9bdb-d89c9e124207)

![image](https://github.com/AdeelAhmedIqbal/DEVOPS-Assign2/assets/62285793/bd6f7028-4647-4ebb-a8ff-b18e45d75e42)


