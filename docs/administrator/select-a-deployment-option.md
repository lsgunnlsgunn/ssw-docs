---
title: Select a deployment option
description:
keywords:
---

Depending on your network topology and the applications that run on your internal networks, you can deploy as many or as few connectors as you need. You can also choose to use networks to group connectors based on whatever criteria best reflects your organization. 
After you identify where you need to deploy connectors to provide access to applications, you have a few different options for how you deploy them. The two primary options are: 

- Deploy directly from an application running locally on a macOS, Windows, or Linux computer using the Splashtop Secure Workspace desktop client app.
- Deploy indirectly from a remote repository using a deployment and orchestration service like Docker or Kubernetes and Helm.

Deploying directly from the Splashtop Secure Workspace desktop client is the simplest option because you can use a familiar graphical user interface to download, install, and run the software. 

Deploying from a remote repository requires you to run a fairly complex command in a terminal shell. However, you can use the Splashtop Secure Workspace administrative portal to construct the command for the platform you use. If you choose to deploy from the command line, you can also automate the process using scripts and other deployment tools.

You have three options for deploying from the command line:

- Docker
- Helm
- Linux

The specific commands you use are different, but the steps are the same for all three of these deployment options:

- You select the headless command-line interface option to indicate that you want to perform a service-based deployment.
- You configure the connector settings that are used to construct the correct command line.
- You configure application discovery settings for the connector to find applications on your network.
- You select the platform—Docker, Helm, or Linux—for deploying the connector service.
- You wait for the successful completion of the command and the deployment status to be Connected.

For more information about adding connectors using a specific deployment option, see the following topics:

- [Add a connector from the desktop client](./add-a-connector)
- [Add a connector using Docker](./use-docker)
- [Add a connector using Helm](./use-helm)
- [Add a connector from the command-line](./use-linux-cmd-line)