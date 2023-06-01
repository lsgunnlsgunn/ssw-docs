---
title: Add private applications
description:
keywords:
---

In addition to discovered applications, you can use the Splashtop Secure Workspace administrative portal to add private applications and resources manually. For example, you can add printers or smart appliances to your network to simplify access and remote management of those devices.

Adding applications manually to Splashtop Secure Workspace requires you to provide information about how users access the application, including the access method, the application protocol, and the host name or IP address that users connect to. All of this information is highly dependent on the private application or resource you're adding. Therefore, the following instructions provide a simplified example that you can use as a general model.

To add a private application:

1. Sign in to your organization URL using your administrative account.

2. Open **Applications**, then click **Applications**.

3. Click **Add Applications**, then select **Private Application**.

4. Type the **Application name** and the **Display name** to use for the application.

6. Select the type of access that can be used to connect to the application:
   
   * Select **All** to allow any type of access.
   * Select **Network** to allow access over a private network using a network-based client.
   * Select **Browser** to allow access to the application from a browser.
   
7. Select the protocol used to connect to the application or resource.
   
   After you select one of the following protocols, click the link to continue adding the application or resource of the selected type:

   * **[VNC](./connection-protocols/vnc.md)** if the application uses Virtual Network Computing.

   * **[RDP](./connection-protocols/rdp.md)** if the application uses Remote Desktop Protocol.

   * **[SSH](./connection-protocols/ssh.md)** if the application uses Secure Shell protocol.

   * **[HTTP](./connection-protocols/http-https.md)** if the application uses Hypertext Transfer Protocol.

   * **[HTTPS](./connection-protocols/http-https.md)** if the application uses secure Hypertext Transfer Protocol.

   * **[Telnet](./connection-protocols/telnet.md)** if the application uses the Telnet protocol.

   * **[Kubernetes](./connection-protocols/kubernetes.md)** if the application uses the Kubernetes API.

   * **[Splashtop](./connection-protocols/sdp.md)** if the application uses the Splashtop Desktop Protocol.

   * **[Custom](./connection-protocols/custom.md)** to connect to any application or resource using Transmission Control Protocol (TCP) and Internet Protocol (IP).
   
Regardless of the protocol you select, you must provide at least the following information:

* Application host by hostname or IP address.
* Port number used to access the application.
* Splashtop Secure Workspace connector or the Splashtop Secure Workspace edge location to use for the application.

For more information about adding a specific type of application, click the connection protocol link.