---
title: Add a connector from the desktop client
description:
keywords:
---

The most common way to add a connector is by downloading and installing the 
Splashtop Secure Workspace desktop client directly on a local macOS, Windows, or Linux computer that hosts internal applications. The steps are similar to the ones described in the _Quick start_ except that you are using the connector to discover network applications instead of a local application.

## Before you begin

Before you begin, verify the following:

* You have the user name and password for an account with the Org Admin or Super Admin role assigned.
* You have access to the applications on your internal network from the computer where you are installing the Splashtop Secure Workspace desktop client.
* You have sufficient permissions to download and install the Splashtop Secure Workspace desktop client on the local computer.

## Install the desktop client

To download and install the Splashtop Secure Workspace desktop client:

1. Sign in to your organization URL using your administrative account.
2. Click **Deployment**, then click **Connector** to display the list of connectors in your organization.
3. Click **Add connector**.
4. Select **With the SSW Desktop App**, then click **Next**.
5. Select your operating system and architecture.
6. Click the first step to download the connector for the operating system and architecture you selected.
7. Open the downloaded file and follow the installation instructions to install the software.

## Run the connector from the desktop client

To run the connector:

1. Open **Secure Workspace** on the computer where your installed the  Splashtop Secure Workspace desktop client, then click **Next step**.
   
   For example, if you installed the workspace client on macOS, go to **Applications** and open **Secure Workspace**.

1. Select the name of your organization from the list of recent organizations, then click **Launch**.

1. Type the Username and Password your administrative account, then click **Sign in**.

1. Click **Connector** in the sidebar.
   
   By default, the connector location is prepopulated using the point of presence closest to your current location.

1. Select **Allow Remote Control** if you want to manage the connector from the Splashtop Secure Workspace administrative portal.

1. Click Application Discovery if you want to customize the settings used to discover applications such as the scan interval, IP address range, or protocols to look for.

1. Click **Run Connector** to connect to the Splashtop Secure Workspace network edge.

### Discover applications

After the Splashtop Secure Workspace connector finds the closest point of presence and connects to the Splashtop Secure Workspace network edge, you can discover applications in your private network matching the application criteria you specify.

To discover applications:

1. Verify the status of the connector is Connected.
2. Click **Discover applications**.
3. Select one or more discovered applications, then click **Add**.
