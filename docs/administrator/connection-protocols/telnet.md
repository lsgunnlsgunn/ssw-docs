---
title: Telnet - Telnet protocol
description:
keywords:
---

Telnet is a client to server protocol that enables access to remote servers and workstations. Telent sessions are often used to execute command-line programs on remote systems.  However, telnet connections aren't secure. With telnet, communication over the network is in plain text, so it is only used on local area networks. By default, telnet connections use port 23.

## Before you begin
Before you begin, verify the following:

* You have specified the application name, display name, access type, and selected TELNET as the application protocol as described in [Add private applications](../add-private-applications.md).
* You know the host and port number used for access to applications in your organization.
* You know the local area network that hosts the application.
* You know the connector that services the local are network.

## Add Telnet general settings

To add an application that uses Telnet:

1. Specify the application host by hostname or IP address.
2. Specify the port number the Telnet server listens on, if you aren't using the default port.
3. Select **Through Connector** and select the connector to use for the host in the local area network (LAN).
 
## Select Telnet access groups and policies

To control access to the application you're adding:

1.  Select one or more groups that are entitled to use this application.
   For information about the default groups and adding new groups, see XXX.

1. (Optional) Select one or more application policies to apply to this application.
For information about creating application policies, see XXX.

## Set additional options

By default, dynamic credentials are turned off for Telnet applications.
You can change the defaults if you want to use dynamic credentials.

For information about dynamic credentials, see XXX.

## Save application settings 

To finish adding the application:

1. Review all of the Telnet application settings.

1. Click **Save** to save the application.