---
title: Administrator's guide
description:
keywords:
---

As discussed in [Organizations and roles](../welcome/organizations-and-roles.md), Splashtop Secure Workspace provides two administrative roles: the **Org Admin** role and the **Super Admin** role.

If you are assigned the **Org Admin** role, you can perform all administrative tasks and use all Splashtop Secure Workspace features within a single organization. For example, you can create user and groups, manage device configuration requirements, add and manage secret information, and monitor network activity. 

In this role, your first tasks typically involve setting up the Splashtop Secure Workspace infrastructure by deploying connectors and adding applications. See the following topics to get started:

* [Deploy connectors](./deploy-connectors.md)
* [Add application](./add-applications.md)

If you are assigned the **Super Admin** role, you can perform all of the same administrative tasks as an organization administrator, but you're not restricted to a single organization. Accounts that are assigned the Super Admin role have full access to a tenant instance and can add, modify, and delete organizations in the instance. The Super Admin role is associated with a Splashtop Secure Workspace **service account** and you must sign in with the service account to work with the organizations you manage, but you can only make changes to any one organizations at a time. 

In this role, your first step is create one or more organizations in your tenant. See [Manage organizations](./manage-organizations.md) to get started, then select an organization and begin deploying the Splashtop Secure Workspace infrastructure for that organization.

