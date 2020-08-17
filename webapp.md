---
title: Web App
has_children: false
nav_order: 6
---

# Lesson Web App

You can install and use many popular open source web applications for your organization. In this lesson, you will learn how to install an e-Commerce web application.

## Prerequisites

- Before you proceed with this lesson, you should have created a [Resource Group](https://rcl-cloud-apps.github.io/cloud101/2-resource-groups.html) in your Subscription

- You should have created a [Plan](https://rcl-cloud-apps.github.io/cloud101/3-plan.html) to host your web app

- You should have created a [Database](https://rcl-cloud-apps.github.io/cloud101/4-database.html) to store the data for your web app

## Create a Web Application

- In the 'RCL Web Apps + TLS/SSL' portal, click on 'Web Apps' in the side menu, then click 'My Apps' in the sub menu. Click on 'Create a new Web App'

![webapp](images/webapp-open.PNG)

- Click on the 'Install' button in the 'nopCommerce' web application

![webapp](images/webapp-create.PNG)

This application is an ASP.NET + SQL Server application. It requires a **SQL Server database** for installation.

- Select the **Resource Group** and **Plan** for the web app

![webapp](images/webapp-create2.PNG)

- Select the **Database Server**, enter the username and password. Select the **Database**

![webapp](images/webapp-create3.PNG)

- In the 'Web Apps' list you will see the new web app. 

![webapp](images/webapp-admin.PNG)

if you don't see the new web app, wait a few minutes and click on the refresh link. Sometimes, it may take a few minutes to create a new resource on Azure.

- Wait for 5 minutes and click on the 'Admin' link.

- When you create a new site and try to access it, you may see that the site is unavailable. Wait for a few minutes and refresh the page

![webapp](images/webapp-site-unavailable.PNG)

- When the site is being provisioned, you will see the 'Azure Web App' placeholder page. You will need to wait a few minutes until the provisioning is complete and then refresh the page

![webapp](images/webapp-place-holder.PNG)

- After provisioning, your site will be constructed. You will see an 'Under Construction' title in your browser. Wait a few minutes and refresh the page

![webapp](images/webapp-site-under-construction.PNG)

- After the site is constructed, install nopCommerce. Add admin email and password

![webapp](images/webapp-nop-install.PNG)

- Add SQL Server name, Database name, SQL Server username and password. You will get the SQL Server name on the Database Server **Properties** page.

- Click the 'Install' button when you are done

![webapp](images/webapp-nop-install2.PNG)

- You can login to the admin portal of nopCommerce and add product content to build your e-Commerce site

![webapp](images/webapp-nop-site.PNG)

# Next Lesson

[Lesson 6 DNS](https://rcl-cloud-apps.github.io/cloud101/6-dns.html)