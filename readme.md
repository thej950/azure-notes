# Cloud Computing 

### ☁️ **Cloud Computing = Renting instead of owning**

## **Analogy:**

Think of **cloud computing like renting a house** instead of **building your own house**.

## 🔍 **Without Cloud (On-Premises):**

You **build your own house**:

* You buy land (servers)
* Build rooms (storage, compute)
* Maintain plumbing & electricity (network, power)
* Fix everything yourself (updates, hardware failures)

## ☁️ **With Cloud:**

You **rent a house or apartment**:

* You pay only for what you use
* No need to worry about construction or maintenance
* Someone else handles repairs, electricity, water, security
* You can upgrade or downgrade anytime

---

## ✔️ **In Tech Terms:**

* Instead of buying servers → you rent them from AWS/Azure/GCP
* Instead of managing hardware → cloud provider manages it
* You pay only for usage (like rent or electricity bill)

---

## 🎯 **Super Simple Summary**

➡️ **Cloud computing means using someone else’s computer (the cloud) over the internet instead of buying and maintaining your own.**

---

# Features of Cloud Computing

## **1. On-Demand Self-Service**

You can create servers, storage, or databases **whenever you want** without contacting support.
*Like ordering food from an app — no human needed.*

---

## **2. Broad Network Access**

Cloud services are accessible **from anywhere** using the internet — laptop, mobile, or tablet.
*Like Netflix works on any device.*

---

## **3. Resource Pooling**

Cloud providers use **shared resources** (servers/storage) for multiple customers while keeping data isolated.
*Like many people living in the same apartment building but in separate flats.*

---

## **4. Rapid Elasticity**

You can **scale up or down** resources instantly based on your needs.
*Like adding more chairs to a restaurant during rush hour.*

VMSS it is service here in Azure 

---

## **5. Measured Service (Pay-As-You-Go)**

You pay only for what you use — like electricity or mobile data.
*No upfront hardware cost.*

---

## **6. High Availability**

Cloud ensures systems stay up even if some components fail.
*Like having multiple backup generators in a building.*

---

## **7. Security**

Cloud offers built-in security tools — encryption, IAM, firewalls, monitoring.
*Much stronger than normal on-prem setups.*

---

## **8. Automation**

Cloud automatically handles patches, updates, autoscaling, backups, monitoring.
*Less manual work for DevOps teams.*

---

## **9. Global Reach**

Cloud providers have data centers all over the world.
*You can deploy your app in India, US, UK within minutes.*

---

## **10. Cost Efficiency**

## **11. Fault Tolerance** 

## **12. Scalability**
   - vertical scaling 
   - horizontal scaling  
![alt text](.images/image-8.png)

No need to buy physical servers; cloud reduces maintenance + operational cost.
*Pay only for usage.*

pricing calculator (estimate cost about resources)
TCO (total cost of ownership) it shows estimate of cost of onpremises costs and compare to cloud costs

---

## 🎯 **Interview Tip (Short Answer)**

Cloud computing provides **on-demand**, **scalable**, **pay-as-you-go** resources over the internet with features like **self-service**, **elasticity**, **resource pooling**, and **global access**.

---


# Platform Models 

![alt text](.images/image.png)

## ☁️ **1. IaaS – Infrastructure as a Service**

### **What it is:**

Cloud provider gives you **virtual machines, storage, networks**.
You manage OS, software, apps.

### **Simple analogy:**

*Like renting an empty house — you bring your own furniture.*

### **Examples:**

* Azure VM
* AWS EC2
* Google Compute Engine
* Azure Storage, VNet

---

## ☁️ **2. PaaS – Platform as a Service**

### **What it is:**

Cloud provides **runtime environment + OS + middleware**, you only deploy your **application code**.

### **Simple analogy:**

*Like renting a fully furnished apartment — you only live in it, no setup required.*

### **Examples:**

* Azure App Service
* Azure SQL Database
* AWS Elastic Beanstalk
* Google App Engine

---

## ☁️ **3. SaaS – Software as a Service**

### **What it is:**

Complete application delivered over the internet.
You don’t manage anything — just use it.

## **Simple analogy:**

*Like staying in a hotel — everything is ready, you just enjoy the service.*

### **Examples:**

* Microsoft 365
* Gmail
* Salesforce
* Zoom

---

## 🎯 **Super Simple Interview Answer**

**IaaS gives infrastructure, PaaS gives platform to run apps, and SaaS gives finished software to users.**

---

# shared responsibility 
![alt text](.images/image-1.png)

# Cloud Models 

![alt text](.images/image-2.png)

## ☁️ **1. Public Cloud**

### **What it is:**

Cloud services delivered over the internet and **shared among multiple organizations**.

### **Who owns it?**

A third-party provider like Azure, AWS, or GCP.

### **You pay for:**

Only what you use (pay-as-you-go).

### **Analogy:**

*Like using a public bus — anyone can use it, and you only pay for your trip.*

### **Examples:**

* Microsoft Azure
* Amazon AWS
* Google Cloud Platform

---

## 🏢 **2. Private Cloud**

### **What it is:**

Cloud infrastructure **used by a single organization only**, not shared with others.

### **Who owns it?**

Your company (on-premises) or hosted privately by a vendor.

### **Best for:**

Banks, government, or companies needing high security.

### **Analogy:**

*Like having your own personal car — only you can use it.*

### **Examples:**

* On-prem VMware cloud
* Azure Stack (private Azure)
* OpenStack private cloud

---

## 🔗 **3. Hybrid Cloud**

### **What it is:**

A combination of **private cloud + public cloud** working together.

### **Why use it?**

* Keep sensitive data privately
* Move scalable workloads to public cloud
* Best of both worlds

## **Analogy:**

*Like having your own car (private) but also using public buses when needed (public).*

### **Examples:**

* On-prem datacenter + Azure
* Azure Arc
* AWS Outposts

---

## 🎯 **Short Interview-Friendly Summary**

* **Public Cloud:** Shared infrastructure, internet-based, pay-as-you-go.
* **Private Cloud:** Dedicated to one organization, more control and security.
* **Hybrid Cloud:** Mix of both; sensitive data stays private, workloads can scale in public cloud.

---

# **Azure Hierarchy**

![alt text](.images/image-3.png)

## **1. Azure Account (Identity / Tenant Level)**

* When you create an Azure account, you get an **Azure AD tenant**.
* This tenant stores **users, groups, roles, and identity** information.
* It is the **top-level identity boundary**.

---

## **2. Subscription (Billing & Resource Boundary)**

* When the account is created, Azure gives you **one default subscription** (for billing).
* You can create multiple subscriptions like:

  * **Sales Subscription**
  * **IT Operations Subscription**
  * **Dev/Test Subscription**
  * **Production Subscription**
* A subscription is the **entry point to create Azure resources**.
* It also defines:

  * Billing
  * Access management (RBAC)
  * Resource limits

---

## **3. Resource Group (Logical Grouping)**

* Resource Groups (RGs) exist **inside a subscription**.
* They act as **logical containers** to organize resources.
* Companies usually group resources by:

  * **Environment** → dev, staging, prod
  * **Application** → web-app-rg, finance-api-rg
  * **Department** → HR-rg, Marketing-rg

---

## **4. Resources (Actual Services)**

* These are the actual services you create:

  * Virtual Machines
  * VNets
  * Storage Accounts
  * AKS clusters
  * Databases
* Resources must belong to **one resource group**.

---

## 📌 **Final Azure Hierarchy Order**

```
Azure Account (Tenant)
        ↓
   Subscription
        ↓
  Resource Group
        ↓
     Resources
```

---

## 🎯 **Interview Tip**

If asked to explain Azure hierarchy, say:

**“Azure uses a hierarchical structure:
Tenant → Subscription → Resource Groups → Resources.
Subscription handles billing, resource groups organize resources, and the tenant manages identities.”**

---


# Azure Management Group 

![alt text](.images/image-4.png) 

![alt text](.images/image-5.png)

---

## ⭐ **What is an Azure Management Group? (Simple Explanation)**

An **Azure Management Group** is a **container used to organize your subscriptions**.
It helps you apply **policies, RBAC roles, security rules, and governance** *across multiple subscriptions at once*.

---

## 🧠 **Think of it like this:**

### ✔️ **Management Group = Folder**

### ✔️ **Subscription = Files inside the folder**

So instead of managing each subscription separately, you manage the **folder (management group)** and everything inside follows those rules.

---

## 🔥 **Why do we use Management Groups?**

1. **Organize subscriptions** (HR, IT, Marketing, Production, Dev/Test)
2. Apply **policies** (like disallow public IPs, enforce tagging) at once
3. Apply **RBAC permissions** at a higher level
4. Manage **governance** for large organizations
5. Create **hierarchies** (Global → Departments → Projects → Subscriptions)

---

## 📌 **Azure Hierarchy (Including Management Groups)**

```
Tenant / Account
      ↓
Root Management Group
      ↓
Management Groups
      ↓
Subscriptions
      ↓
Resource Groups
      ↓
Resources
```

---

## 🧩 **Example using your pictures**

### ✔️ Root Management Group

Top-level container created automatically.

### ✔️ Department Management Groups

* Human Resources
* IT
* Marketing
* Geo Region 1
* Geo Region 2

### ✔️ Subscriptions under each

* EA Subscription
* Dev/Test Subscription
* Free Trial Subscription

### ✔️ Resource Groups → Resources

---

## 🎯 **Super Simple Interview Answer**

**“Management Groups in Azure are used to organize multiple subscriptions and apply policies and RBAC at scale. They sit above subscriptions in the Azure hierarchy.”**

---

# CloudShell 

**Cloud Shell** is a **browser-based command-line tool** provided by Azure.
You don’t need to install anything — it runs directly in the Azure Portal.

---

## ⭐ **Simple Definition**

**CloudShell is a pre-configured, browser-based shell in Azure that lets you run CLI commands (Azure CLI or PowerShell) without installing tools on your computer.**

---

## 🔧 **Key Features**

### ✔️ **Comes with Azure CLI & PowerShell preinstalled**

You can choose:

* Bash
* PowerShell

### ✔️ **Runs in the browser**

No setup required. Works directly from:
👉 portal.azure.com (top-right corner > CloudShell icon)

### ✔️ **Has a built-in storage (file share)**

It stores your scripts, files, SSH keys in a storage account.

### ✔️ **Always up-to-date**

Microsoft maintains and updates all tools automatically.

### ✔️ **Supports Development Tools**

Inside CloudShell you get:

* Terraform
* Git
* Kubectl
* Helm
* Python
* .NET tools
* Az CLI

### ✔️ **Great for managing Azure resources**

Run:

```bash
az group create
az vm create
kubectl get nodes
terraform init
```

---

### 🎯 **Super Simple Example**

If you want to create a VM in CloudShell:

```bash
az vm create --resource-group rg1 --name myVM --image UbuntuLTS
```

---

### 🌐 **Where to find it?**

In Azure Portal → Top bar → **Click the Shell icon**
(looks like >_ )

---

## 🎯 **Interview Tip**

“Cloud Shell is Azure’s built-in online command-line environment. It provides Bash or PowerShell with all Azure tools preinstalled so users can manage resources without installing anything locally.”

--- 

# Data Centers & Regions & Availability Zones 
![alt text](.images/image-7.png)

- collection of multiple datacenters are availability zones 
- in azure region having maximum 3 availability centers only 

# VM scale set (VMSS)
 - It is Autoscales vms when cpu utilization high it will create new VM and when Cpu utilization low reduce VM 

![alt text](.images/image-9.png)

![alt text](.images/image-10.png)

Project details 

Scale set details 

Orchestration

Instance details 

Administrative account 

# Azure Virtual Desktop 
- it is a type of managed vm that enables multiple users to access virtual desktops and applcations from anywhere, using any device 
 - azure virtual desktop is a desktop and application virtualization service that runs on the cloud 
 - it provides scalable and secure solution for remote work and desktop virtualization 
 - secure access through MFA and RBACs  

![alt text](.images/image-11.png)

# Virtualization 
 - virtualization means allow to run multiple OS instance  concurrently  in a single computer 

![alt text](.images/image-12.png)   |   ![alt text](.images/image-13.png)


![alt text](.images/image-14.png)   |   ![alt text](.images/image-15.png)

# Azure Contaner Instances 

![alt text](.images/image-16.png)

# Azure Function 
 - Azure Functions are event-driven and can trigger actions like sending emails when files are uploaded to Azure Blob Storage. They are cost-effective as they only charge for code execution and provide fast response times.
 - Unlike traditional virtual machines, Azure Functions eliminate the need for constant infrastructure management, significantly reducing operational costs. This serverless architecture is ideal for applications with intermittent usage patterns.
 - Azure Functions provide a scalable solution, capable of handling a large number of requests while being flexible enough to use different programming languages. This flexibility supports various application requirements.
 - event driven
    - executed based on events suppose if there is a file uploaded to azure blob storage then execute, it could be a http based, time based or message like that  
 - serverless
 - compute 
    - to run any function it is not required servers and compute usage 

features
 - cost efective
 - no of execution 
 - faster 
 - scalable
 - flexible
 
# Azure App services 
 - it is a Platform as a Service 
 - To build and host application in any programming laungauages 
   - web apps using azure webapps
   - Backround jobs using azure webJobs 
   - Mobile Backends using Mobile Apps 
   - Restful APIs using  API apps  
 - supports High availability, and automatic scaling
 - it supports linux and windows, so user focus on building app and maintance of application 
 - microsoft focus on infrastructher 

web Apps
 - full support of hosting web apps 
    ASP .NET Core 
    ASP .NET
    Java 
    Ruby 
    Node.js

API Apps 
 - Rest based web APIs by using choice of langauage and framework 
 - full swagger support 
 - ability to package and publish API in market place 
 - apps can be consumed from any http/https based clients  


webJobs
 - it simlar to cronjob 
 - scheduled / trigger 
 - use to run program (.exe, java, php or nodejs)
 - use script (.cmd, .bat, Powershellor bash )
 - Run backround jobs or task 

Mobile Apps
 - Build a backend for IOS/Android 
 - store app data in a coud based SQL database 
 - user authenticate using social providers 
 - send push notifications 
 - execute custome backend logic in c#/Nodejs

![alt text](.images/image-17.png)


# Azure VNET 

![alt text](.images/image-18.png)


# VNET Peering 

![alt text](.images/image-19.png)

# VPN 

![alt text](.images/image-20.png)

# Express route 

![alt text](.images/image-21.png)

# DNS

# Blobs Storage 

![alt text](.images/image-22.png)

- Serving images or documents directly to a browser (static web Hosting)
- Storing files for distrinuting access 
- Streaming video and audio 
- storing data for backup and restore, disater recovery and archiving 
- storing data for analysis by an on-premises or azure hosted service 

# File storage 
 - it works based on SMB/NFS protocol 
 - need to mount to vm after created, any number if vmcan be able to connect 
 - Azure file storage enables you to create files shares in the cloud and access these file share from anywhere with internet connection  
 - azure file storage exposes file shares using the server message Block 3.0 (SMB) protocol 
 - once you created a azure account, you can upload files to azure file storage using the azure portal, or tools such as the azZopy utility 
 - Attaching a network drive to multiple computers **Azure file storage performance tiers**
 - the standard tier uses hard disk based hardware in a daacenter 
 - premium tier uses solid-state disks, the premium tiers offers greater throughput but it is charged higher rate 

# Azure Queue Storage 

# Storage Account 

![alt text](.images/image-23.png)

# Azure Blob Storage: Access tiers 

![alt text](.images/image-24.png)  |  ![alt text](.images/image-25.png)

# Azure Storage Redundancy 

## Local Reduntdant 
![alt text](.images/image-26.png) 

## Zone Redunant Storage 

![alt text](.images/image-27.png)

## Geo Reduntdant Storage 

![alt text](.images/image-28.png)

# Azure Migrate 

![alt text](.images/image-29.png)

## Azure Data Box 

![alt text](.images/image-30.png) 

# Azure File Movement 

![alt text](.images/image-31.png)

# Azure Storage Explorer 

# Azure File Sync 

![alt text](.images/image-33.png)

# Identity, Authentication and Authorization 

![alt text](.images/image-32.png)

# Azure Active Directory 

![alt text](.images/image-34.png)

## Connect

![alt text](.images/image-35.png)

## Domain 

![alt text](.images/image-36.png)

# Role 

![alt text](.images/image-37.png)

![alt text](.images/image-38.png)

## Role Assignement

![alt text](.images/image-39.png)

## Conditional Access 

![alt text](.images/image-40.png)


# Cost Estimation in Azure 

![alt text](.images/image-41.png)

![alt text](.images/image-42.png)

# Azure Management and Governance 

![alt text](.images/image-43.png)

![alt text](.images/image-44.png)

# Resource Locks  
- Prevents resourced from being accidentally deleted or modified 
- Resource Locks are inherited 
- can be applied at multiple levels 


# Service Trust Portal 

# Tools for interact with Azure 

![alt text](.images/image-45.png)

# Azure Arc 

![alt text](.images/image-46.png)

# ARM Templates 
- ARM Template it is a Infrastrucher as service in azure 


# Monitoring Tools in Azure 

## Azure Advisor 

![alt text](.images/image-47.png)

## Azure Service Health 

![alt text](.images/image-48.png)

## Azure Monitor 

![alt text](.images/image-49.png)


