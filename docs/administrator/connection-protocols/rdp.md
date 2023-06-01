---
title: RDP - Remote desktop protocol
description:
keywords:
---

The Remote Desktop Protocol is a client to server protocol that enables desktop sharing. Remote desktop connections are typically used to take control of a remote Windows workstation or server. By default, RDP connections use port 3389.

## Before you begin
Before you begin, verify the following:

* You have specified the application name, display name, access type, and selected RDP as the pplication protocol as described in [Add private applications](../add-applications.md).
* You know the host and port number used by RDP clients and servers in your organization.
* You know if the application host is part of a private local area network.
* You know the connector that services the private network or the Splashtop Secure Workspace edge location to use if the application host isn't part of a private network.

## Add RDP general settings

To add an application that uses Remote Desktop Protocol:

1. Specify the application host by hostname or IP address.
2. Specify the port number the RDP server listens on, if you aren't using the default port 3389.
3. Select **Through Connector** and select the connector to use if the host is part of a private local area network (LAN).

   If the host is available on a public network, turn off **Through Connector** and select a Splashtop Secure Workspace edge location.
 
## Select RDP access groups and policies

To control access to the application you're adding:

1.  Select one or more groups that are entitiled to use this application.
   For information about the default groups and adding new groups, see XXX.

1. (Optional) Select one or more application policies to apply to this application.
For information about creating application policies, see XXX.

## Set additional options

There are several additional options you can set for RDP applications. For most organization, the default settings for the additional options are fine, but you can change them if you need to.
The additional options are set as follows by default:

* Dynamic credentials are turned off.
* Security options are turned off.
* Server certificates are ignored.
* Session recording is turned on. 

There's also an advanced option to set the maximum number of seconds that a network session can remain open with a default of 28800 seconds.

You can change the default settings for any of these options. For example, you can turn on and configure dynamic credentials if you want to use them with this application.

For information about dynamic credentials, see XXX.
For information about session recording, see XXX.

To change the maximum session duration:

1. Click **Advanced options**.
2. Set a new maximum network session duration in seconds.

## Save application settings 

To finish adding the application:

1. Review all of the RDP application settings.

1. Click **Save** to save the application.
