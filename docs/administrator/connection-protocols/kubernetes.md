---
title: Kubernetes – Kubernetes API
description:
keywords:
---

Kubernetes is container and cluster orchestration platform with multiple components and services for automating software deployment, scaling, and application management. Selecting Kubernetes as the application protocol enables communication with the Kubernetes API server and—through the API—between and across all of the components in a Kubernetes configuration. By default, the Kubernetes API server listens on port 6443.

## Before you begin

Before you begin, verify the following:

* You have specified the application name, display name, access type, and selected KUBERNETES as the application protocol as described in [Add private applications](/v1/docs/add-private-applications).
* You know the host and port number used for access to applications in your organization.
* You know if the application host is part of a private local area network.
* You know the connector that services the private network or the Splashtop Secure Workspace edge location to use if the application host isn't part of a private network.

## Add Kubernetes general settings

To add an application that uses Kubernetes:

1. Specify the application host by hostname or IP address.
2. Specify the port number the Kubernetes API server listens on, if you aren't using the default port.
3. Select **Through Connector** and select the connector to use if the host is part of a private local area network (LAN).

   If the host is available on a public network, turn off **Through Connector** and select a Splashtop Secure Workspace edge location.
 
## Select Kubernetes access groups and policies

To control access to the application you're adding:

1.  Select one or more groups that are entitiled to use this application.
   For information about the default groups and adding new groups, see XXX.

1. (Optional) Select one or more application policies to apply to this application.
For information about creating application policies, see XXX.

## Set additional options

By default, dynamic credentials are turned off for Kubernetes applications.
You can change the defaults if you want to use dynamic credentials.

For information about dynamic credentials, see XXX.

## Save application settings 

To finish adding the application:

1. Review all of the Kubernetes application settings.

1. Click **Save** to save the application.
