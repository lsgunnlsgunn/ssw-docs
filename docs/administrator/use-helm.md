---
title: Add a connector using Helm
description:
keywords:
---

If you have a Kubernetes cluster and are familiar with Helm charts and Helm commands, you can add a connector by pulling the latest image and running a Helm command.
One of the advantages to adding a connector service using Helm is that it enables you to construct a command line that can then be used to automate the deployment on a remote server.

## Before you begin

Before you begin, verify the following:

- You have the user name and password for an account with the Org Admin or Super Admin role assigned.
- You have an account with administrative privileges for a Kubernetes cluster.
- You are familiar with the commands used to manage a Kubernetes cluster.
- You have Helm installed and are familiar with using Helm commands to deploy applications in pods and containers on Kubernetes cluster nodes.

## Configure connector settings

To add a connector using Docker:

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
   | Cluster mode |  Select this option if you want to install the connector on multiple nodes to form a cluster. For example, you can select this option to add and deploy multiple instances of the connector to make your network more resilient and to prevent service interruptions.  |
   | Scan interval | Set the frequency for the connector to check for changes to the applications. In most cases, the default interval of 20 minutes is appropriate. |
   | IP range | Set an IP range for discovering applications, if appropriate. You can use the Classless Inter-Domain Routing (CIDR) format—for example, 192.168.20.0/24—to specify the range. Alternatively, you can specify a static IP address or a range of addresses using the following format: 192.168.20.0-192.168.20.100 |
   | Protocols | Click **Select all** to scan for all application protocols. |
1. Select **Helm** as the deployment method.
   
   You should see a command line constructed for Helm that looks similar to the following example, but with a full token instead of the truncated token shown here:
   
   ```
   helm repo add connector-stage https://s3.us-west-2.amazonaws.com/splashlock-assets.splashshield.ai/helm-chart/ztw-connector-stage/ --force-update && helm upgrade --install -n connector stage-acme-lisaacme-montreal1 connector-stage/ztw-connector --set token="eyJhbGciOiJSUzI[...]" --create-namespace --wait
   ```
   
   If you are deploying on a cluster, click **Add Instance** to automatically construct the command line for each additional instance. A number is appended to the connector name for each instance you add. For example, if you set the the connector name to `montreal`, the first instance is named `montreal1`, the second instance is named `montreal2`, and so on.
3. Copy the command displayed and leave the deployment page open in the administrative portal.

## Install the connector

To install the connector using the Helm command:

1. Open a terminal shell on the computer where Helm is running.
2. Verify that the Helm process is installed by running the following command:

   ```
   helm version
   ```
   
4. Paste the command you copied from the administrative portal.
   After running the command, return to the administrative portal deployment page to verify the status of the connector is Connected.
1. Click **Done**.