<h1>Help Desk Emulation Project (Active Directory + ServiceNow)</h1>

This project documents the process of provisioning a virtual machine in AWS, which serves as the foundation for setting up Active Directory. The VM is configured to support core IT workflows, including:

- User account management

- Password resets

- Incident tracking and resolution

Additionally, this lab includes a hands-on ServiceNow environment, where I explore the platform’s features for IT Service Management (ITSM). This includes creating and managing incident tickets, tracking their lifecycle, and integrating workflows to simulate real-world support operations.

---

<h2>Project Overview</h2>

| Component     | Description                                                  |
|-------------------|--------------------------------------------------------------|
| Platform | AWS (EC2) |
| OS  | Windows Server 2025                     |
| Services       | Active Directory Domain Services, ServiceNow Developer                |
| Goal |  Simulate daily helpdesk operations in a lab setting          |
---

<h3>EC2 Instance Setup</h3>

1. Launched a Windows Server EC2 instance using AWS.
2. Enable RDP Access.
3. Install Active Directory Domain Services via Server Manager.
4. Promote the server to a Domain Controller and create a test domain.

https://www.loom.com/share/246a391ad0e4452ba9508e93b4410c5b?sid=6e22aaad-ed93-4b70-9f86-13d594ff05e4
---

<h3>Create Users, Groups and Reset passwords in Active Directory</h3>





