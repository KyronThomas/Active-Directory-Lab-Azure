# osTicket - Prerequisites and Installation
![68747470733a2f2f692e696d6775722e636f6d2f436c7a6a3758732e706e67](https://github.com/user-attachments/assets/a0c657b7-4216-433d-9b63-86a1028dc666)


This guide outlines the prerequisites and installation steps for setting up the open-source help desk ticketing system **osTicket**.

---

## 📺 Video Demonstration

**YouTube:** [How To Install osTicket with Prerequisites](https://www.youtube.com/watch?v=pKBDk7v1zmg)

---

## 🖥️ Environments and Technologies Used

- **Microsoft Azure** – Virtual Machines / Compute Resources
- **Remote Desktop** – For VM access  
- **Internet Information Services (IIS)** – Web server configuration  
- **Operating System:** Windows 10 (21H2)

---

## 📋 Prerequisites

Ensure the following components are installed or prepared before beginning:

1. Windows 10 machine or Azure VM (21H2 or later)
2. Internet Information Services (IIS) with required modules enabled  
3. PHP (version compatible with osTicket)  
4. MySQL or MariaDB database setup  
5. osTicket installation files (download from [osTicket.com](https://osticket.com))  


---

## 🛠️ Installation Steps

1. **Download osTicket**
   - Visit [https://osticket.com](https://osticket.com) to download the latest version.

2. **Configure IIS**
   - Enable necessary components like CGI, ISAPI, and Static Content.
   - Set up a new site in IIS pointing to the osTicket root directory.  

3. **Install and Configure PHP**
   - Install PHP (compatible version).
   - Configure PHP in IIS (set handler mappings, PHP.ini adjustments).  

4. **Database Configuration**
   - Install MySQL or MariaDB.
   - Create a new database (e.g., `osticket_db`) and user (with full permissions).

5. **Run osTicket Web Installer**
   - Access `http://localhost/your-osticket-folder/setup/`
   - Follow the setup wizard to complete the installation.  

6. **Configure File Permissions**
   - Grant write access to:
     - `/include/ost-config.php`
     - `/attachments/`
     - `/logs/`  
   ![Permissions Screenshot](/path/to/file-permissions.png)

---

## 🧼 Disk Sanitization Steps

Use these steps to sanitize disks before repurposing virtual machines:

> Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.  
> Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.  
> Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.

(Add your organization's actual disk sanitization policy and tools here.)  
![Disk Wipe Tool Screenshot](/path/to/disk-wipe.png)


