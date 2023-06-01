---
title: Add a connector from the command line
description:
keywords:
---

If you want to add a connector on a computer or virtual machine with a Linux distribution and you aren't using Docker or Helm, you can add a connector by running a script in a terminal.
One of the advantages to adding a connector service using the script and the command line that Splashtop Secure Workspace constructs for you is that you can copy and run the script to automate the deployment on a remote server.

## Before you begin

Before you begin, verify the following:

* You have the user name and password for an account with the Org Admin or Super Admin role assigned.
* You have an account with `sudo` administrative privileges on the Linux computer.
* You have an internet connection with network access to the Linux computer.
* You are generally familiar with how to run commands in a terminal.

## Configure connector settings

To add a connector by running a script in a terminal:

1. Sign in to your organization URL using your administrative account.
2. Click **Deployment**, then click **Connector** to display the connectors currently deployed for your organization.
3. Click **Add Connector**. 
4. Click **Headless / CLI**, then click **Next**.
5. Configure the settings for the connector and application discovery, then click **Next**.
   
   | For this | Do this |
   | :--- | :--- |
   | Connector name | Type a name for the connector process to use. You should avoid including spaces or special characters. |
   | Display name | Type the name you want displayed in the administrative portal for the connector. |
   | Network | Verify the network displayed is the correct organization. Optionally, you can add a new network identifier for the connector instead of using your organization. For more information about adding networks, see [Add a network identifier](./network-identifier). |
   | Edge location | Select an appropriate edge location. |
   | Auto bandwidth detection | Select this option to allow the connector to monitor bandwidth changes to ensure the best performance for the connector. | 
   | Cluster mode | Select this option if you want to install the connector on multiple nodes to form a cluster. For example, you can select this option to add and deploy multiple instances of the connector to make your network more resilient and to prevent service interruptions. |
   | Scan interval | Set the frequency for the connector to check for changes to the applications. In most cases, the default interval of 20 minutes is appropriate. |
   | IP range | Set an IP range for discovering applications, if appropriate. You can use the Classless Inter-Domain Routing (CIDR) format—for example, 192.168.20.0/24—to specify the range. Alternatively, you can specify a static IP address or a range of addresses using the following format: 192.168.20.0-192.168.20.100 |
   | Protocols | Click **Select all** to scan for all application protocols. |
1. Select **Linux** as the deployment method.

   You should see a command line that looks similar to the following example, but with a full token instead of the truncated token shown here:
   
   ```
   export ZTW_CONNECTOR=connector-stage-acme-lisaacme-sanfrancisco && curl "https://s3.us-west-2.amazonaws.com/splashlock-assets.splashshield.ai/connector/stage/setup.sh" | sudo bash -s $ZTW_CONNECTOR && sudo $ZTW_CONNECTOR -install -configPath /etc/$ZTW_CONNECTOR -conf eyJhbGciOiJSUzI[...]  && sudo systemctl start $ZTW_CONNECTOR
   ```
   
   If you are deploying on a cluster, click **Add Instance** to automatically construct the command line for each additional instance. A number is appended to the connector name for each instance you add. For example, if you set the the connector name to `sanfrancisco`, the first instance is named `sanfrancisco1`, the second instance is named `sanfrancisco2`, and so on.
3. Copy the command displayed and leave the deployment page open in the administrative portal.

## Install the connector

To install the connector from the command line:

1. Open a terminal shell on the Linux computer.
2. Verify that you have sudo permission by running the following command:

   ```
   sudo --list
   ```
   
4. Paste the command you copied from the administrative portal.
   
   The command line sets an environment variable, downloads the connector setup script, executes the setup script using the environment variable, and starts the connector. Between downloading the script and executing it, you might be prompted to provide your password to run the command using your `sudo` privileges.
   
   After running the command, return to the administrative portal deployment page to verify the status of the connector is Connected.
1. Click **Done**.