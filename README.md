# 🛡️ Configuring Active Directory in Azure Virtual Machines

This repository demonstrates my experience setting up and configuring **Active Directory Domain Services (AD DS)** within a Windows Server Virtual Machine hosted in **Microsoft Azure**.

##  Tools & Technologies Used

-  Microsoft Azure
- 🖥 Windows Server 2019 Datacenter (VM)
-  Active Directory Domain Services (AD DS)
-  DNS Server
-  Group Policy Management Console (GPMC)
-  Remote Desktop Protocol (RDP)

---

## ⚙️ Lab Objectives

- Deploy a Windows Server VM in Azure
- Install and configure Active Directory Domain Services
- Promote the server to a Domain Controller
- Configure DNS for domain resolution
- Join a client VM to the domain
- Manage users and OUs via ADUC
- Apply and test Group Policies (GPOs)

---

## 🧾 Step-by-Step Breakdown

### 1. Set Up Azure Resources
- Create a **Resource Group**
- Deploy two VMs:
  - `DC-1`: Domain Controller (Windows Server 2019)
  - `Client-1`: Domain-joined client (Windows 10 or Server)

### 2. Configure DC-1
- Rename VM to `DC-1`
- Assign a static private IP
- Install the **Active Directory Domain Services** role
- Promote to a Domain Controller:
  - Domain Name: `mydomain.local`

### 3. Configure DNS
- Ensure DNS service is installed and pointing to DC-1's static IP
- Confirm domain resolution from Client-1

### 4. Join Client-1 to Domain
- Point DNS on `Client-1` to `DC-1`'s IP
- Join `mydomain.local`
- Restart and log in using domain credentials

### 5. Manage Active Directory
- Create Organizational Units (OUs)
- Create Users and Security Groups
- Apply basic Group Policies (e.g., desktop background, password policies)


## 📌 Key Concepts Demonstrated

- Domain Controllers and Active Directory structure
- DNS integration with AD DS
- VM networking and private IP management in Azure
- User and OU management
- Group Policy basics

---

## 🔒 Security Best Practices (Bonus)

- Disable RDP access from public internet
- Enable NSGs for VM subnet isolation
- Use complex passwords and domain lockout policies

---

## ✅ Summary

This lab demonstrates the foundational setup and configuration of **Active Directory in a cloud-hosted environment**, including domain setup, DNS configuration, domain joins, and user policy management. It highlights essential skills in system administration and cloud networking.
