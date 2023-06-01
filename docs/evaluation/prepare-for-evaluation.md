---
title: Prepare for evaluation
description:
keywords:
---

As a first look at Splashtop Secure Workspace, the [_Quick start_](../quickstart/index.md) provides an overview of the Splashtop Secure Workspace platform and shows you how to install the Splashtop Secure Workspace desktop client on a single local computer. 
However, the _Quick start_ doesn't represent a typical deployment.

To prepare for an evaluation that allows you to simulate your network infrastructure and test different types of access and device policies, you must have a physical or virtual network with representative servers, applications, and endpoints. 
Therefore, for the purposes of evaluation, the _Evaluator's Handbook_ assumes you have access to a small test environment and that you have administrative privileges for managing the test network.

## Review the architecture

You can get an overview of Splashtop Secure Workspace features and architecture in the following articles:

* [What is Splashtop Secure Workspace?](../welcome/what-is-ssw.md)
* [Basic concepts and component](../welcome/basic-concepts-and-components.md)
* [Organizations and roles](../welcome/organizations-and-roles.md)

At a minimum, you should be familiar with the following Splashtop Secure Workspace core components:

* The Splashtop Secure Workspace desktop client app
* The Splashtop Secure Workspace cloud service
* The Splashtop Secure Workspace network edge services
* Splashtop Secure Workspace connectors

## Set up a test network

You can use any method you like to set up the test network.
For example, you can use virtualization software to create a network of virtual Linux, macOS, and Windows virtual machines. 
If you have an Amazon Web Services (AWS) account, you can create a virtual network using an AWS instance.
If you have experience with Kubernetes, you can create the test network in a Kubernetes cluster.  

The simplest way to set up a test network is to deploy connectors on a few representative servers that host applications and that are configured to allow communication within your firewall.
For the evaluation scenarios described in this guide, the _Evaluator's handbook_ assumes that the evaluation test environment consists of the following physical or virtual machines:

* Two macOS computers
* One Ubuntu Server
* One Ubuntu Desktop

## Set up accounts

The evaluation scenarios in this guide assume that you have access to at least two accounts—an administrative account and a regular user account—for testing purposes.
You also might want to set up a test account for any external applications that you want to include in your own evaluation scenarios.

If your evaluation includes testing access to cloud-based applications or applications that are hosted on the public internet, you should collect information about how the external service provider handles authentication and authorization for user account. 
For example, you should know whether the service provider requires users to create a user name and password or sign in with an email address.

## Verify applications are available

If you have a virtual or physical network prepared for testing purposes, be sure the network includes representative applications that use one or more of the following standard connection protocols to support remote access:

- Hypertext Transfer Protocol (HTTP)
- Hypertext Transfer Protocol Secure (HTTPS)
- Remote Desktop Protocol (RDP)
- Virtual Network Connection (VNC)
- Splashtop Desktop Protocol (SDP)
- Secure Shell (SSH) or telnet
- Kubernetes client API

After you identify the computers in your test network that host applications that use these access protocols, you should take note of the host name, IP addresses, and ports numbers used.

## Verify remote access is allowed

You should also verify that the applications and computers in the test environment are configured to allow remote access or network sharing.
For example, on the macOS computers in the evaluation environment, you should turn on the following system settings:

* Screen sharing
* Printer sharing
* Remote login

Similarly, you should check that the computers you include in the test network allow remote access and host applications that you want to test access to. For example, if you include Ubuntu Desktop be sure that sharing is on and active.

## Next steps

After you have prepared an evaluation environment with a test network with computers that host applications that use remote access protocols, you're ready to start securing your infrastructure.