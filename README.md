# post-install-config<p align="center">
![image](https://github.com/user-attachments/assets/b857fd0b-d292-4ce2-924e-4db2a6835e86)
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>Configuration Steps</h2>

Login to osTicket using the "adminuser" and "Password1".
![image](https://github.com/user-attachments/assets/30abd196-498d-4816-9848-d13441574a07)

To Configure rolls go to admin panel in the top right next to your name in orange. Then Agents, and Roles. Add a new roll on the top right name it Supreme Admin then in the Premissions tab check all the boxes in Ticets, Tasks, Knowledgebase and add the role.
![image](https://github.com/user-attachments/assets/1f1df5e5-1ce3-4da1-950b-bfd6c859af8f)
![image](https://github.com/user-attachments/assets/4aee6050-a182-414c-8e10-9805a810ac48)
![image](https://github.com/user-attachments/assets/a2d9b029-6aec-4c93-828f-8879397c4e14)
![image](https://github.com/user-attachments/assets/2a284ab1-3f5e-47aa-9f10-1a495dea89b9)

Next we will set up departments. Under Agents select the Departments tab, click on Add New Deparment. For the name we will name it SysAdmins. Then hit create.
![image](https://github.com/user-attachments/assets/4d7c6e95-96bc-48d3-8ca4-67591bfe2ba0)

Our next step is to setup Teams. On the Agents tab we are going to select Teams then Add New Team. We will name it "Online Banking" and hit Create Team.
![image](https://github.com/user-attachments/assets/555f8ac8-2a8f-494c-b28d-3096cbc428a3)

To allow anyone to create tickets we have to go to Settings on the top row. Then Users and Make sure the Registration Required box is not checked. If it is uncheck it.
![image](https://github.com/user-attachments/assets/cde721cf-78df-4925-8bc9-a8259c28e480)
![image](https://github.com/user-attachments/assets/eaaa5b90-25e8-4ce6-9f13-c7ec02dbe0fd)

Now to configure our agents head back over to the Agents tab and add new agents. We will be using Jane and John Doe with the password set as Password1. Uncheck the "Send the agent a password reset eamil" and the "Require password change next login".
![image](https://github.com/user-attachments/assets/60d4d247-cd5a-49e1-8e0f-63016903ca01)
![image](https://github.com/user-attachments/assets/0abe505d-d013-4211-9fec-08bdf928eef4)

On the Access tab Jane will get the "SysAdmins" Department and Supreme Admin Role. Then on the Teams tab add Jane to the Online Banking team.
![image](https://github.com/user-attachments/assets/cac6bdfc-16b8-4374-8b5d-e488c13f812a)
![image](https://github.com/user-attachments/assets/7e3d4757-fde1-4a73-aec3-c33e796adaa3)

Now to get John setup. On the Agents tab make a new agent and give the name John Doe and Password1. On the Access tab John will get the Support Department and View Only Role and then Create.
![image](https://github.com/user-attachments/assets/0b380786-134a-49d7-90d1-f19db457863c)
![image](https://github.com/user-attachments/assets/2fa87ed9-e470-4919-b658-243df7724851)

Now to make a User. Swap to the Agent panel go to Users and Add User. We will make the name Ken.
![image](https://github.com/user-attachments/assets/9277b2fd-f56f-4f4d-9d56-a26c7447aa74)

Next we have to setup SLAs (Service Level Agreement). Go back to the Admin Panel. Go to Manage tab and then SLA.
![image](https://github.com/user-attachments/assets/e7687f95-0e11-4ed3-a284-84375d6be5f7)

We will now add new SLAs. We will repeat this process for all 3. Sev-A (Grace Period: 1 hour, Schedule: 24/7), Sev-B (Grace Period: 4 hours, Schedule: 24/7), Sev-C (Grace Period: 8 hours, Business Hours)
![image](https://github.com/user-attachments/assets/ee2f8bce-7d02-47d6-89a4-d50f6d57679f)
![image](https://github.com/user-attachments/assets/56796c8c-8a19-435a-b7d9-8a8913dddfa6)
![image](https://github.com/user-attachments/assets/35b26bda-3e41-488b-8682-efb9e1c21a67)

Lastly we will set up Help Topics. On the Help Topics page click Add New Help Topic. The topic will be "Business Critical Outage". We will also make Personal Computer Issues, Equipment Request, Password Reset and Other using all the same steps.
![image](https://github.com/user-attachments/assets/398539d7-b294-4577-b285-6ef2458783d2)


osTicket setup is complete. We have successfully set up agents along with their departments, roles, and permissions. As well as configured SLAs (Service Level Agreements), help topics, and users. osTicket is now setup for the next project where we will create and work different tickets using multiple agents and users.
