---
title: Grant temporary privileged access
description:
keywords:
---

With Splashtop Secure Workspace, there are two ways you can share secret information to allow secure access to privileged credentials or sensitive information.
You saw the first method in [Manage secrets](manage-secrets.md) when you assigned the permissions defined in a secrets policy to a user or group. 

If you are the owner of a secret—or of a folder that contains multiple secrets—you can assign specific permissions to individual users or groups in your organization. With this type of sharing,
you can use the Details tab to share secrets with specific users or group, select the security policy to apply, and the specific read, write, or admin permission to grant for each user and group you are sharing secrets with.

The second way you can share secret information is called **link sharing**. With link sharing, you to share individual secrets with third parties or contractors who don't have a Splashtop Secure Workspace account. As the owner of a secret, you can generate a link and send it to the recipient. The recipient can then use the link to access and view the shared secret or store it in their own personal vault or Splashtop Secure Workspace.

To create a link for a secret:

1. Sign in with your administrative account to open the Splashtop Secure Workspace administrative portal.

1. Under Secrets Manager, click **Secrets**, then click the vault name—either **My Vault** or **ajuba**—to display the secrets list.

1. Find the specific secret that you want to share with an external party.

1. Select **Link Share** from the list of Actions for the secret.

1. Specify a title, the number of times the link was be used, allowed usage, and an expiration date.  

    You can also add an optional passphrase to secure the shared secret, so that only authorized individuals can access the shared secret. The optional passphrase provides an additional layer of protection against unauthorized access.

1. Click **Create**.

1. Copy the link to your clipboard, then click **OK**.

1. Send the link to the authorized external party.

One of the most common use cases for link sharing is to give an external party temporary administrative access or privilege elevation for a specific resource or application.
