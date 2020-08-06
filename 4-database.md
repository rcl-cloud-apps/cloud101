---
title: 4. Database
has_children: false
nav_order: 5
---

# Database

Databases store data for your web applications. In this section, we will create a database.

## Prerequisites

Before you proceed with this tutorial, you should have created a **Resource Group** in your Subscription

## Create a Database Server

A Database Server will host one or more databases. To create a database server, follow these instructions :

- In the 'RCL Web Apps + TLS/SSL' portal side menu click on 'Databases'

- Click on the 'Create a new Database Server' link

![Database](images/database-open.PNG)

- Create a new 'SQL Server' 

![Database](images/database-create.PNG)

- In the 'Database Servers List', you will see the new SQL Server

![Database](images/database-list.PNG)

if you don't see the new Database Server, wait a few minutes and click on the refresh link. Sometimes it may take a few minutes to create a new resource on Azure.

SQL Servers are used for ASP.NET web applications, eg. Orchard CMS, DNN, etc. If you intent to install a ASP.NET application, a SQL Server and Database are requirements for the installation.

## Create a Database

- In the 'Database Servers' list, click on 'Databases' in the Sever that you would like to create the database in

![Database](images/database-database-create.PNG)

- In the Databases page, click 'Create a new Database'

![Database](images/database-database-create2.PNG)

- Create a new 'Basic' database

![Database](images/database-database-create3.PNG)

- In the 'Database List', you will see the new SQL Database

![Database](images/database-database-list.PNG)

if you don't see the new Database, wait a few minutes and click on the refresh link. Sometimes it may take a few minutes to create a new resource on Azure.

## Add a Firewall Rule

You must add a firewall rule for web apps to connect to the Database Server.

- In the 'Database Server' list, click on the 'Firewall' link

![Database](images/database-firewall-open.PNG)

- In the 'Firewall Rules' page, click on 'Create a new Firewall Rule'

![Database](images/database-firewall-create.PNG)

Set the properties of the firewall

- Firewall name - AllowAllWebApps
- Start IP Address - 0.0.0.0
- End IP Address - 0.0.0.0

Click the 'Submit' button when you are done

![Database](images/database-firewall-create2.PNG)

The new firewall rule is shown below

![Database](images/database-firewall-created.PNG)

Now, all web apps in your subscription can access the database through the database server firewall.