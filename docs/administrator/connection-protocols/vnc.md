---
title: VNC - Virtual network computing
description:
keywords:
---

Virtual network computing is a client to server protocol that enables desktop sharing. Virtual network computing is typically used to take control of a remote workstation or server. By default, VNC connections use port 5900.

## Before you begin

Before you begin, verify the following:

* You have specified the application name, display name, access type, and selected VNC as the application protocol as described in [Add private applications](../add-private-applications.md).
* You know the host and port number used by VNC clients and servers in your organization.
* You know if the application host is part of a private local area network.
* You know the connector that services the private network or the Splashtop Secure Workspace edge location to use if the application host isn't part of a private network.

## Add VNC general settings

To add an application that uses Virtual Network Computing:

1. Specify the application host by hostname or IP address.
2. Specify the port number the VNC server listens on, if you aren't using the default port 5900.
3. Select **Through Connector** and select the connector to use if the host is part of a private local area network (LAN).

   If the host is available on a public network, turn off **Through Connector** and select a Splashtop Secure Workspace edge location.
 
## Select VNC access groups and policies

To control access to the application you're adding:

1.  Select one or more groups that are entitled to use this application.
   For information about the default groups and adding new groups, see XXX.

1. (Optional) Select one or more application policies to apply to this application.
For information about creating application policies, see XXX.

## Set additional options

By default, dynamic credentials are turned off and session recording is turned on. There's also an advanced option to set the maximum number of seconds that a network session can stay open.
You can change the defaults if you want to use dynamic credentials, disable session recording for this application, or set a different maximum session duration time.

For information about dynamic credentials, see XXX.
For information about session recording, see XXX.

To change the maximum session duration:

1. Click **Advanced options**.
2. Set a new maximum network session duration in seconds.

## Save application settings 

To finish adding the application:

1. Review all of the VNC application settings.
1. Click **Save** to save the application.
