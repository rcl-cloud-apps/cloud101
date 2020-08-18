---
title: Access Control
has_children: false
nav_order: 3
---

# Lesson Access Control

**Personal Accounts and Microsoft Accounts are not supported in Access Control. Only Active Directory (also known as 'School or Work Accounts') are supported.**

The Azure Active Directory (AAD) organizational account that you use to login to the RCL Web Apps + TLS/SSL app must either be :

- An administrator to the subscription containing the web app
- Have a role of 'Owner' or 'Contributor' to the subscription containing the web app

## Subscription Administrator
 
You can determine if you are an administrator on the subscription by logging in to the Azure portal with the same AAD account that you use to login to to the RCL Web Apps + TLS/SSL app. 

- Navigate to the **Subscriptions** section 

![Access Control](images/access-control-subscriptions.PNG)

- Select a subscription. 

![Access Control](images/access-control-subscriptions2.PNG)


After you select a subscription, click on the 'My permissions' link for the subscription.

![Access Control](images/access-control-admin.PNG)

- Here you can determine if you AAD account is an administrator or not 

### Owner or Contributor roles

If your AAD account is not an administrator in the subscription, you should add the AAD account as an 'Owner' or 'Contributor' to the subscription.

You will do this in the **IAM** area of the Subscription section.

- Add a "Contributor' or 'Owner' role assignment to your subscription for your AAD account

![Access Control](images/access-control-create.PNG)

- You will see the new role assignment in the 'Role assignments' tab

![Access Control](images/access-control-list.PNG)