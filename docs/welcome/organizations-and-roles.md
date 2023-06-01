---
title: Organizations and roles
description:
keywords:
---

In Splashtop Secure Workspace, an organization represents the top-level entity that you manage security for. 
For example, an organization might be a global business, a school district, or a regional government agency.

However, organizations aren't defined by their size. 
Organization are defined by the scope of what they contain. 
Each organization is an independent entity with its own users, groups, applications, network topology, and policies. 
For example, an enterprise with multiple divisions might have separate organizations for engineering and sales because engineering and sales have very different sets of users and applications to manage and share very little infrastructure.

It's important to keep this separation in mind because each organization is managed completely independent from all other organizations. 
Users in one organization don't have access to resources in any other organization.

## Roles and privileges

In Splashtop Secure Workspace, roles define what users can do. 
Roles are predefined as part of Splashtop Secure Workspace. 
Roles aren't defined by organizations or tenants.
Each predefined role has specific privileges and restrictions. You can't modify role privileges and restrictions or add new roles to the predefined set.

Roles control the features that different classes of users can access. Each user you add to an organization you manage must be assigned one of the following predefined roles:

- **User** is the most restricted role with the fewest privileges. People assigned the User role can access and use an organization’s applications, manage their own secrets, and monitor their own Splashtop Secure Workspace activities. This predefined role is the role most often assigned to new Splashtop Secure Workspace users.

- **Analyzer** has the same privileges as the User role, but can also monitor the Splashtop Secure Workspace activities of other users within the organization. For example, you might assign the Analyzer role to members of the IT staff to allow them to check other users' actions or to a compliance manager who wants to monitor activity for possible security risks.

- **Manager** has the same privileges as the Analyzer role, but can also add and modify access to applications within an organization. For example, you might assign the Manager role to an application owner in a specific department or to an IT manager working under the senior-level IT administrator.

- **Org Admin** has all administrative privileges within a single organization. Accounts that are assigned the Org Admin role can use all Splashtop Secure Workspace features, including creating user accounts, setting device configuration and posture checks, and much more.

- **Super Admin** has all administrative privileges, but is not restricted to a single organization. Accounts that are assigned the Super Admin role have access to all organizations in their tenant instance and can add, modify, and delete organizations in their instance. This role is associated with a Splashtop Secure Workspace service account. Users who sign in with a service account can choose to work with any of their organizations, but they can only make changes to any one of those organizations at a time.

- **Auditor** has the read-only privileges to view any Splashtop Secure Workspace information, including configuration settings, event logs, user activity, and anything that a Super Admin might see. Users in the Auditor role can’t perform any administrative actions.

## Groups

Unlike the predefined roles, organization administrators can use groups to define sets of users that share common privileges or requirements. For example, you can use groups for users who access the same set of applications or to apply access policies for users in the same location. 
Groups allow you to implement privileges and restrictions for multiple users at a time based on the criteria you define.

## Guests

Guests are application users who don't have Splashtop Secure Workspace accounts. 
Guests aren’t part of the organization you manage, but might periodically or regularly need access to resources in the organization. 
For example, you might have an outside party—a partner, vendor, contractor, or temporary employee—who requires short-term or temporary access to a server or application. 
In this scenario, you want to grant limited access without adding the outside party as a Splashtop Secure Workspace user with an account in the organization you manage.

You can give guests temporary access to applications by sending them a URL and credentials. 
The guest uses the URL to present the credentials you provided and is granted access to the application through Splashtop Secure Workspace without seeing or using any of Splashtop Secure Workspace features.