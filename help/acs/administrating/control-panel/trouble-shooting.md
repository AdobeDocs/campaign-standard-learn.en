---
title: Trouble Shooting the Control Panel
seo-title: Trouble Shooting the Control Panel
description: The Control Panel allows you to monitor and manage your SFTP storage by instance and whitelist IP addresses.
seo-description: The Control Panel allows you to monitor and manage your SFTP storage by instance and whitelist IP addresses.
uuid: e73e2288-85e2-45f4-9f13-2f1e89d30cca
discoiquuid: 700ba7da-6734-450b-a054-e547454f706e
feature: Control Panel
topics: Control Panel
kt: KT-2938
doc-type: article
activity: use
team: PM
---

# Trouble Shooting the Control Panel

## Login and Homepage

### Symptom: Unable to login to Experience Cloud

**What to do:**
The user needs to locate their IMS Org ID (xxx). The Administrator needs to add the user to the Product Profile “Campaign-xxx-Admins”  for each instance that they would like to manage. If the user is an admin of all instances they still might need to add themselves as “users” 

### Symptom: Links in the Experience Cloud Home to access Control Panel do not appear for a user 

**Cause:**
Users won’t see the links until they are added as users to Product Profile “Campaign-xxx-Administrators/Admin”

**What to do:**
The Administrator needs to add the user to the Product Profile “Campaign-xxx-Admins”  for each instance that they would like to manage. If the user is an admin of all instances they still might need to add themselves as “users. 

### Symptom: An Instance is not listed in the Control Panel

**Cause:**
Most likely user needs to be added as a “user” Product Profile “Campaign-xxx-Administrators/Admin” for the instance that is missing

**What to do:** 
The Administrator needs to add the user to the Product Profile “Campaign-xxx-Admins”  for each instance that they would like to manage. If the user is an admin of all instances they still might need to add themselves as “users”.

### Helpful videos

>[!VIDEO](https://video.tv.adobe.com/v/27183?quality=12)
*Check IMS Org ID (00:26 min)*

>[!VIDEO](https://video.tv.adobe.com/v/27147?quality=12)
*How to add an administrator to the product profile "administrators" to be able to use Control panel (01:03 min)*

### Helpful Documentation

* [Discover the Control Panel](https://helpx.adobe.com/campaign/kb/control-panel-overview.html)
* [Managing permissions to the Control Panel](https://helpx.adobe.com/campaign/kb/control-panel-access.html)

## Establishing Connection to SFTP Server (Client or API)

Connecting to SFTP servers requires:

* Whitelisting the IP address from which you are connecting to the SFTP server  
* Private/public key pair that needs to be registered with Adobe Campaign
* If connecting to the SFTP server directly you will also need SFTP client software

### Helpful Documentation

* [Logging into your SFTP server](https://helpx.adobe.com/campaign/kb/control-panel-sftp.html#LoggingintoyourSFTPserver)
  