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


<h3>🔧EC2 Instance Setup</h3>

1. Logged in to the AWS Management Console.
2. Navigated to the EC2 Dashboard.
3. Clicked "Launch Instance".
4. Chose a Windows Amazon Machine Image.
5. Selected an Instance Type.
8. Added Tags for identification.
9. Configured Security Group.
10. Reviewed and launched the instance.
11. Selected an existing key pair to access the instance.
12. Launched the instance and verified it in the EC2 Dashboard.


<h3>Create Users, Groups and Reset passwords in Active Directory</h3>

✅ Creating a New User
1. Open Active Directory Users and Computers.
2. Navigate to the appropriate Organizational Unit.
3. Right-click the OU > Select New > User.
4. Enter First Name, Last Name, and User Logon Name.
5. Click Next and set a password (optionally require password change at next login).

✅ Creating a New Group
1. In ADUC, navigate to the desired OU.
2. Right-click > Select New > Group.
3. Enter a Group Name.
4. Choose Group Scope.
5. Click OK to create the group.

✅ Changing a User Password
1. In ADUC, right-click the user account.
2. Select Reset Password.
3. Enter the new password and confirm it.
4. Choose whether to require the user to change it at next login.
5. Click OK to apply.

Watch me Provision an Instance. ⬇️

https://www.loom.com/share/5331c375ecba468db9c423f684f0561d?sid=29500a94-af31-4ddf-9f60-f5b8e32c8516

Watch me Configure Active Directory, password, user and group. ⬇️

https://www.loom.com/share/e67cada0ea00477abc37b5b98bb465fc?sid=fa81eeb1-0bc2-4574-bf2d-97de19f1d7f3

---

<h2>Creating a Ticket in Service Now</h2>

1. Log in to the ServiceNow Portal.
2. Navigate to the Incidents section.
3. Click on "New" to create a new incident.
4. Fill out the Description field with details about the problem.
5. Submit the ticket to log the incident.

Watch me Create a Ticket in ServiceNow. ⬇️

https://www.loom.com/share/19b75c9b0d2f450da2e2482d8768d970?sid=abf69408-7804-44e0-b0ea-6c88e56f5f51




