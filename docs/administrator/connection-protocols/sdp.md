---
title: Splashtop - Splashtop desktop protocol
description:
keywords:
---

Splashtop desktop protocol (SDP) provides the low-level interfaces for the suite of Splashtop products that enable remote workers to securely access and control their office computers. By default, the Splashtop server listens on port 6783.

## Before you begin

Before you begin, verify the following:

* You have specified the application name, display name, access type, and selected SPLASHTOP as the application protocol as described in [Add private applications](../add-private-applications.md).
* You know the host and port number used for access to applications in your organization.
* You know if the application host is part of a private local area network.
* You know the connector that services the private network or the Splashtop Secure Workspace edge location to use if the application host isn't part of a private network.

## Add Splashtop general settings

To add an application that uses Splashtop:

1. Specify the application host by hostname or IP address.
2. Specify the port number the Kubernetes API server listens on, if you aren't using the default port.
3. Select **Through Connector** and select the connector to use if the host is part of a private local area network (LAN).

   If the host is available on a public network, turn off **Through Connector** and select a Splashtop Secure Workspace edge location.
 
## Select Splashtop access groups and policies

To control access to the application you're adding:

1.  Select one or more groups that are entitled to use this application.
   For information about the default groups and adding new groups, see XXX.

1. (Optional) Select one or more application policies to apply to this application.
For information about creating application policies, see XXX.

## Set additional options

By default, authentication is turned off for Splashtop applications.
If the Splashtop application you are adding requires a six-digit security code to sign in, you can store the code in the application settings. 

To store the authentication security code for a Splashtop application, turn on **Authentication**, then type the security code in the field displayed. After you set the security code, you don't need to provide it in when you use the Splashtop application you are adding.

For more information about using a security code to sign in, see [How can I set up the security code for my computer](https://support-splashtopbusiness.splashtop.com/hc/en-us/articles/212724883-How-can-I-set-up-the-Security-Code-for-my-computer-).

## Save application settings 

To finish adding the application:

1. Review all of the Splashtop application settings.

1. Click **Save** to save the application.