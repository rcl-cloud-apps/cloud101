---
title: Database
has_children: false
nav_order: 6
---

# Lesson: Database

Databases store data for your web applications. In this section, we will create a database server and a database.

## Prerequisites

- Before you proceed with this lesson, you should have created a [Resource Group](https://rcl-cloud-apps.github.io/cloud101/resource-groups.html) in your Subscription

## Create a Database Server

A Database Server will host one or more databases. To create a database server, follow these instructions :

- In the 'RCL Web Apps + TLS/SSL' portal side menu, click on 'Databases'

- Click on the 'Create a new Database Server' link

![Database](images/database-open.PNG)

- Create a new 'SQL Server' 

![Database](images/database-create.PNG)

- Ensure the Database Server Type is set to 'SQL Server'

- The 'Admin Password' should be at least 12 characters long. It must contain common letters, at least one capital letter, at least one number and at least one none alphanumeric character (#, !, $, %, etc.). Save the password in a safe place so that you will not forget it.

- Click the submit button when you are done

- The Database Server will be submitted to your cloud account for installation, you will need to wait for up to 15 minutes for the Database Server to be created

![Database](images/database-list.PNG)

- In the 'Database Servers List', you will see the new SQL Server

If you don't see the new Database Server, wait a few minutes and click on the refresh link.

SQL Servers are used for ASP.NET web applications, eg. Orchard CMS, DNN, nopCommerce, etc. If you intend to install an ASP.NET application, a SQL Server and Database are requirements for the installation.

## Create a Database

- In the 'Database Servers' list, click on 'Databases' in the Sever that you would like to create the database in

![Database](images/database-database-create.PNG)

- In the Databases page, click 'Create a new Database'

![Database](images/database-database-create2.PNG)

- Add a database name and create a new 'Basic' database. 

There are three SKU/Tiers based on storage size and compute power. The SKU/Tiers are as follows:

- Basic - Development and testing
- Standard S0 - Light workloads
- Standard S1 - Production workloads

![Database](images/database-database-create3.PNG)

- In the 'Database List', you will see the new SQL Database

![Database](images/database-database-list.PNG)

If you don't see the new Database, wait a few minutes and click on the refresh link. 

## Database Properties

The configuration and credentials to connect to the SQL Database is provided in the 'Properties' page.

- In the databases list, click on the 'Properties' link for the database

![Database](images/database-sqldb-properties.PNG)

- The properties page will provide you with the information to connect to the database

![Database](images/database-sqldb-properties2.PNG)

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

# Next Lesson

[Web App](https://rcl-cloud-apps.github.io/cloud101/webapp.html)