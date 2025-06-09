# 🧰 Help Desk Emulation Project  
**Technologies Used: Active Directory, ServiceNow, Spiceworks, AWS EC2**

This project demonstrates a full emulation of help desk workflows in a controlled lab environment. It covers the deployment of a Windows Server VM on AWS, configuration of Active Directory for user and group management, and simulates common IT support tasks including password resets. As well as ticket creation using ServiceNow and Spiceworks.

---

## 📌 Project Overview

| **Component** | **Description** |
|---------------|------------------|
| **Platform**  | AWS (EC2) |
| **OS**        | Windows Server 2025 |
| **Services**  | Active Directory Domain Services, ServiceNow Developer Instance, Spiceworks Cloud Help Desk |
| **Goal**      | Simulate daily help desk operations in a lab environment |

---

## 🚀 EC2 Instance Setup

1. Logged into the AWS Management Console.
2. Navigated to the EC2 Dashboard and selected **Launch Instance**.
3. Chose a **Windows Server Amazon Machine Image**.
4. Selected instance type and configured tags.
5. Set up a security group and chose an existing key pair.
6. Launched the instance and verified its availability.

🎥 [Watch me provision an EC2 instance](https://www.loom.com/share/5331c375ecba468db9c423f684f0561d?sid=29500a94-af31-4ddf-9f60-f5b8e32c8516)

---

## 🛠️ Configuring Active Directory on AWS (Windows Server VM)

This section outlines the step-by-step process of installing and configuring **Active Directory Domain Services (AD DS)** on a Windows Server virtual machine hosted on AWS.

### 📋 Steps to Install Active Directory

1. Click the **Windows icon** and open **Server Manager**.
2. In the **Configure this local server** panel, click **Add roles and features**.
3. In the **Add Roles and Features Wizard**, click **Next** until you reach the **Installation Type** screen.
4. Ensure **Role-based or feature-based installation** is selected, then click **Next**.
5. On the **Server Selection** tab, confirm **Select a server from the server pool** is selected, and click **Next**.
6. On the **Select server roles** screen, check the box for **Active Directory Domain Services**.
7. A dialog will appear asking to install required features—click **Add Features**, then click **Next** twice.
8. On the **AD DS** overview screen, click **Next**.
9. In the **Confirmation** tab, click **Install**.

### ⚙️ Promoting the Server to a Domain Controller

10. After installation, click the **flag icon** in the upper-right corner and select **Promote this server to a domain controller**.
11. Under **Deployment Configuration**, choose **Add a new forest**.
12. Enter your root domain name:  
    **`learn.local`**, then click **Next**.
13. In the **Domain Controller Options** tab:
    - Set a **Directory Services Restore Mode (DSRM) password**
    - Click **Next**
14. Leave default settings in the **DNS Options** tab and click **Next**.
15. The wizard will auto-generate a **NetBIOS domain name** based on your root domain—click **Next**.
16. In the **Paths** tab, accept the defaults and click **Next**.
17. Review your configuration and click **Next**.
18. On the final screen, click **Install**.

🔄 The server will automatically restart upon completion of the configuration.

✅ **Result**: Your AWS-hosted Windows Server is now configured as a Domain Controller with Active Directory installed and running under the domain `learn.local`.


## 👥 Active Directory: User, Group & Password Management

### ✅ Creating a New User
- Open **Active Directory Users and Computers (ADUC)**.
- Navigate to the appropriate Organizational Unit (OU).
- Right-click → **New → User**.
- Fill in user details and assign a password.

### ✅ Creating a New Group
- In ADUC, navigate to the target OU.
- Right-click → **New → Group**.
- Enter the group name, select the scope, and create the group.

### ✅ Resetting a User Password
- Right-click on the user → **Reset Password**.
- Enter a new password and confirm.
- Optional: Require password change at next login.

🎥 [Watch me configure AD, create a user, group, and reset a password](https://www.loom.com/share/e67cada0ea00477abc37b5b98bb465fc?sid=fa81eeb1-0bc2-4574-bf2d-97de19f1d7f3)

---

## 🛠️ Creating a Ticket in ServiceNow

1. Log into the **ServiceNow Developer Portal**.
2. Navigate to **Incidents** > **Create New**.
3. Fill out the **Short Description** and details of the issue.
4. Submit the form to create the incident ticket.

🎥 [Watch me create a ticket in ServiceNow](https://www.loom.com/share/19b75c9b0d2f450da2e2482d8768d970?sid=abf69408-7804-44e0-b0ea-6c88e56f5f51)

---

## 📝 Creating a Ticket in Spiceworks

1. Log into the **Spiceworks Cloud Help Desk**.
2. Navigate to **IT Tools > Cloud Help Desk**.
3. Click **Try Cloud Help Desk** and then **+ New Ticket**.
4. Enter ticket details and submit.

🎥 [Watch me create a ticket in Spiceworks](https://www.loom.com/share/a0d169587fd04f93b40de49d96c5b34d?sid=33540ae7-d7c5-4218-a113-5044e675b3fb)

---

## 📂 Purpose of This Repository

This repository showcases hands-on experience simulating real-world IT support scenarios. It highlights the deployment and use of essential tools like Active Directory, ServiceNow, and Spiceworks to manage IT operations in a help desk setting.

