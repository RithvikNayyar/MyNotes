What is cloud computing?
Cloud computing is a delivery model for services like storage, compute power, analytics, networking and much more. 

What is scalability?
scalability means ability of the system to scale on different work loads. It is a process of allocating and deallocating of resources.
**FIG - 0.1**
![[Azure Fundamentals - Recap-20240823170206298.webp|692]]
What is agility?
Agility is to react quickly, that is Agility is to allocate and de-allocate resources quickly.

What is Elasticity?
Elasticity is a way to scale dynamically. Check fig 0.1 right side graph as the load increases the resources are automatically allocated and when the load is reduced then the resources are also reduced so that there is absolutely no wastage.

What is Reliability?
Reliability is the ability of the system to recover from failures and continue to function. It is also one of the pillars of the Microsoft Azure well architected framework.

What is Fault tolerance?
The ability to remain up and running and running even after failure of the resources or components or services.

Cloud uses consumption based model which is multiple pricing components per service and very granular usage measurement.

THINGS WE NEED IN OWN INFRASTURCTURE: 
* OS - WINDOWS, LINUX
* MIDDLEWARE - HARDWARE - RAM, ROM, MOTHERBOARD, CPU, ETC.
* RUNTIME - DOCKER
* APPLICATION DATA - APPS
* NETWORKING -  ROUTER AND INTERNET
* STORAGE - HARD DRIVE OR SSD
* VIRTULIZATION - VMWARE 
* ELECTRICITY 

WHAT IS PUBLIC CLOUD?
PUBLIC CLOUD is where everything we run is on the cloud providers computer. ex: Azure, aws, oracle cloud. No local hardware. some services share hardware with other costumers.

WHAT IS PRIVATE CLOUD?
PRIVATE CLOUD is where you have the hardware and you host the system so that you can use the hardware from anywhere and is only limited to you and no one else.

WHAT IS HYBRID CLOUD?
HYBRID CLOUD is where you have both public and private cloud and use both simultaneously for your work. Like you store your personal things in private cloud and for extra compute work you use public cloud.

WHAT IS DATA CENTER?
A **data center** is a facility that houses computer systems and related components, such as telecommunications and storage systems. It provides the infrastructure needed for IT operations, including servers, data storage, and networking equipment. Data centers ensure the continuous operation of these systems with backup power supplies, cooling systems, and security measures.

➜ A Group of data centers that are connected with each other with high end throughput connectivity is called regions.
➜ Regions is a geographical area on the planet.
➜Microsoft has many data centers.
➜ Usually more than 2 datacenter's are connected with each other with ultra low latency.
➜ Each location has its own equipment like for some region has a particular tool and some do not. some of them do not even require regional based services like IAM service.

WHAT IS AVAILIBILITY ZONE?
**Availability zones** are isolated locations within a cloud provider’s region, each with its own power, cooling, and networking. They minimize the risk of simultaneous failures and enhance reliability by distributing applications and data across multiple zones.
➜ Microsoft has multiple AV's in a single region like US - EAST 1, US - EAST 2, ETC.
➜ This makes cloud highly available to everyone as if one of the AV's is down then the other are availability.
➜ A zone has multiple data center's and more than 3 zones are required to call it a region.
➜ Not all regions have availability zone as they have zone redundant storage.
➜ Each region is at least 300 miles away from each other so if any problem arises this comes in handy and if a region goes down then regional pair takes place of it.

**RESOURSE MANAGEMENT:**

**Azure Resource Manager (ARM)** is the deployment and management service for Azure. It provides a management layer that enables you to create, update, and delete resources in your Azure account. Key features include:

1. **Consistent Management Layer**: ARM handles all requests through the same API, ensuring consistent results across different tools like the Azure portal, PowerShell, Azure CLI, REST APIs, and client SDKs.
2. **Resource Groups**: Resources in Azure are organized into resource groups, which act as containers for related resources. This organization helps manage resources as a group based on their lifecycle.
3. **Access Control**: ARM allows you to manage access to resources using role-based access control (RBAC). This ensures that only authorized users can perform actions on resources.
4. **Resource Locks**: You can apply locks to prevent accidental deletion or modification of critical resources.
5. **Tags**: Tags are used to organize resources by applying metadata to them. This helps in categorizing and managing resources based on different criteria.
6. **Templates**: ARM templates (JSON files) and Bicep files provide a declarative syntax to define the infrastructure to deploy to Azure. These templates help automate the deployment and management of resources.
7. **Deployment**: Resources can be deployed to a resource group using ARM templates. The Azure portal provides a user-friendly interface to manage these deployments.
8. **Monitoring and Alerts**: ARM integrates with Azure Monitor to provide insights into resource performance and health. You can set up alerts to notify you of critical conditions.
9. **Cost Management**: ARM helps track and manage costs associated with resources, providing insights into spending and helping optimize resource usage.
















