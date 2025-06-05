<h1>Help Desk Emulation Project (Active Directory + ServiceNow)</h1>

This project documents the process of provisioning a virtual machine in AWS, which serves as the foundation for setting up Active Directory. The VM is configured to support core IT workflows, including User account management, password resets as well as incident tracking and resolution. Additionally, this lab includes a hands-on ServiceNow environment, where I create a ticket in ServiceNow.

---

<h2>Project Overview</h2>

| Component     | Description                                                  |
|-------------------|--------------------------------------------------------------|
| Platform | AWS (EC2) |
| OS  | Windows Server 2025                     |
| Services       | Active Directory Domain Services, ServiceNow Developer                |
| Goal |  Simulate daily helpdesk operations in a lab setting          |


<h3>EC2 Instance Setup</h3>

1. Launched a Windows Server EC2 instance using AWS.
2. Enable RDP Access.
3. Install Active Directory Domain Services via Server Manager.
4. Promote the server to a Domain Controller and create a test domain.


<h3>Create Users, Groups and Reset passwords in Active Directory</h3>



Watch me Provision an Instance 
https://www.loom.com/share/5331c375ecba468db9c423f684f0561d?sid=29500a94-af31-4ddf-9f60-f5b8e32c8516

Watch me Configure Active Directory, Password/User/Group
https://www.loom.com/share/e67cada0ea00477abc37b5b98bb465fc?sid=fa81eeb1-0bc2-4574-bf2d-97de19f1d7f3

---

<h2>Creating a Ticket in Service Now</h2>

1. Log in to the ServiceNow Portal.
2. Navigate to the Incidents section.
3. Click on "New" to create a new incident.
4. Fill out the Description field with details about the problem.
5. Submit the ticket to log the incident.

Watch me Create a Ticket in ServiceNow.




