---
title: Manage unified policies
description:
keywords:
---

With a unified policy, you can combine different types of access controls and the conditions to evaluate for those controls in a single policy definition. 
A unified policy can simplify policy management because you can create one policy to control the following: 

* User authentication
* Application access
* Network access
* Permission to Read secrets
* Permission to Write secrets
* Permission to Update secrets

For each control, you can specify conditions that allow access, require multifactor authentication, or deny access.
The flexibility of being able to combine multiple controls and conditions in one policy can be powerful, especially for controls that you want broadly applied across the organization.
However, combining multiple controls in one policy can also lead to complexity in keeping track of all the conditions to be evaluated. 

In general, you should use a unified policy to consolidate controls that you want to enforce across your organization infrastructure.
You can then use specialized policies to provide more targeted controls for specific applications, secrets, or groups.

## Defining multiple unified policies

Although you can define one unified policy that includes all of the access controls, it's often useful to define multiple unified policies.
For example, you might want to define one unified policy focused on basic user authentication and a second unified policy focused on restricting network access to a specific subnet address range. 
In some cases, the clarity of separating the purpose of each policy outweighs the overhead of managing two unified policies instead of one.

## Actions, events, and conditions

Every control in a unified policy has a default action to take when a triggering event—such as an authentication request or an attempt to access the network—occurs.
For any control, you can change the default action or set conditions to be evaluated that can result in a change to the action taken.
For example, if the default action is to deny access and you don't define any conditions that allow access or that allow access with multifactor authentication, all access requests are denied.
You can define one or more conditions that must be met to all access or to  allow access with multifactor authentication. 
If none of the conditions are satisfied, the default action to deny access is enforced.

## Groups and policy evaluation

Unified policies are always applied based on group membership.
When you create a unified policy, you must specify one or more groups where the policy applies.
When members of a group where the policy is applied attempt to sign in, access applications, or read secrets, the policy conditions are evaluated to determine whether the user should be allowed access, allowed access with multifactor authentication of denied access. 

## Create a unified policy

You must be assigned the Super Admin or Org Admin role to define unified policies.

To create a unified policy:

1. Sign in with your administrative account to open the Splashtop Secure Workspace administrative portal.

2. Click **Access**, then click **Policies**. 

3. Click **Add Policy**.

1. Type a descriptive name for the new unified policy that indicates the purpose or scope of the policy.

1. Select the groups where the policy should apply.
    
    All of the members of the groups you select are subject to the policy controls.
    For example, select **All User** to apply this policy to all users with access to Splashtop Secure Workspace.

1. (Optional) Specify specify one or more tags to categorize the policy for filtering and searching.

1. Click **Add Control**, then select the type of control you want to enforce with this policy.
    
    * Select **Secret Read** to control read access to secrets.
    * Select **Secret Write** to control write access to secrets.
    * Select **Secret Admin** to control administrative permissions for secrets.
    * Select **Application Access** to control access to applications.
    * Select **User Authentication** to control authentication request handling.
    * Select **Network Access** to control access to network resources.
    
    For each control, you can specify a default action to take if none of the conditions you specify is met.
    If you aren't defining any conditions, you should select **Allow** to allow access or **Allow_MFA** to allow access with multifactor authentication.
    
    If you have previously defined conditions, you can select the condition to evaluate and the action to take based on the result of the evaluation.
    To define a condition for the control you're adding, click **Choose conditions**, select **Create new condition**, then follow the steps in [Create a new condition]().

    You can add multiple controls and conditions to this policy.
    When you are finished adding controls and conditions for each control, continue to the next step.

1. Click **Save** to save the unified policy.
    
    After you click Save, the policy is added to the list of policies.
    By default, the policy is enabled and begins enforcing access controls immediately. 
    
1. Click the **Enabled** toggle to turn enforcement of the policy off temporarily or if you want to delay deployment.

    After a policy is enabled and actively enforcing the access controls, you should monitor the effect of policy settings on user activity and access to applications and network resources within the Group and make adjustments, if necessary.

## Modify a unified policy

## Delete a unified policy
