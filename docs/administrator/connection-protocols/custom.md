---
title: Custom - TCP/IP protocols
description:
keywords:
---

Selecting Custom as the application protocol enables you to support access for any application or resource that can be located using its IP address and port number through the transmission control protocol (TCP) and internet protocol (IP). For example, you can set the application protocol to Custom to add printers or smart appliances that have an IP address and a port that they listen on.

## Before you begin

Before you begin, verify the following:

* You have specified the application name, display name, access type, and selected CUSTOM as the application protocol as described in [Add private applications](../add-private-applications.md).
* You know the host and port number used for access to the application or resource in your organization.
* You know the connector that services the application host in your private local area network.

## Add general settings

To add an application or resource that uses TCP/IP:

1. Specify the address for the application or resource using the hostname or IP address and a port number.

   For example, you can specify an address similar to the following:
   
   ```
   192.168.1.101:631
   ```
3. Select **Through Connector** and select the connector to use to access the application or resource address in the private local area network (LAN).
 
## Select access groups and policies

To control access to the application or resource you're adding:

1. Select one or more groups that are entitled to use this application or resource.
   For information about the default groups and adding new groups, see XXX.

1. (Optional) Select one or more application policies to apply to this application or resource.
   
   For information about creating application policies, see XXX.

## Save application settings 

To finish adding the application or resource:

1. Review all of the application or resource settings.

4. Click **Save** to save the application.
