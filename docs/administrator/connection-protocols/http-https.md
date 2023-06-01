---
title: HTTP and HTTPS – Hypertext transfer protocol
description:
keywords:
---

Both the hypertext transfer protocol (HTTP) and hypertext transfer protocol secure (HTTPS) are used to access web-based applications. Typically, these protocols enable unencrypted (HTTP) and encrypted (HTTPS) communication through a browser. By default, HTTP connections use port 80 and HTTPS connections use port 443.

## Before you begin

Before you begin, verify the following:

* You have specified the application name, display name, access type, and selected HTTP or HTTPS as the application protocol as described in [Add private applications](../add-private-applications.md).
* You know the host and port number used for access to applications in your organization.
* You know if the application host is part of a private local area network.
* You know the connector that services the private network or the Splashtop Secure Workspace edge location to use if the application host isn't part of a private network.

## Add HTTP general settings

To add an application that uses HTTP or HTTPS:

1. Specify the application host by hostname or IP address.
2. Specify the port number the HTTP or HTTPS server listens on, if you aren't using the default port.
3. Select **Through Connector** and select the connector to use if the host is part of a private local area network (LAN).

   If the host is available on a public network, turn off **Through Connector** and select a Splashtop Secure Workspace edge location.
 
## Select HTTP access groups and policies

To control access to the application you're adding:

1.  Select one or more groups that are entitiled to use this application.
   For information about the default groups and adding new groups, see XXX.

1. (Optional) Select one or more application policies to apply to this application.
For information about creating application policies, see XXX.

## Set additional options

By default, dynamic credentials are turned off and there's an advanced option to set the maximum number of seconds that a network session can remain open.
You can change the defaults if you want to use dynamic credentials or set a different maximum session duration time.

For information about dynamic credentials, see XXX.

To change the maximum session duration:

1. Click **Advanced options**.
2. Set a new maximum network session duration in seconds.

## Save application settings 

To finish adding the application:

1. Review all of the HTTP or HTTPS application settings.

1. Click **Save** to save the application.
