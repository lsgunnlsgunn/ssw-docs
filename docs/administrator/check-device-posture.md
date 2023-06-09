---
title: Check device posture
description:
keywords:
---

Splashtop Secure Workspace includes several important devices management features to ensure that devices that connect to organization resources meet the security requirements you want to enforce.
For example, you can create security posture profiles to check that desktop and mobile devices meet specific security standards before they connect to private applications or remote resources in the organization and periodically during active sessions to verify the device remains compliant after the initial connection is established. 
You can create multiple security posture profiles to tailor the security requirements for different types of devices, different operating systems, and different groups.

## Create a security posture profile

With a security posture profile, you can define a set of conditions to check for a set of devices and the scheudle for how frequently the conditions should be evaluated.

To create a security posture profile:

1. Sign in with your administrative account to open the Splashtop Secure Workspace administrative portal.

2. Click **Devices**, then click **Posture Check**.

1. Click **Add Profile**.

1. Type a descriptive name for the profile.
    
    For example, if the profile is intended for mobile devices used by members of the Sales team, you might type a description such as `Android-Sales-NA`.

1. Select a group to a group where this profile applies.
    
    For example, if the profile is intended for mobile devices used by members of the Sales team, you might select a group such as `Sales-NA`.

1. Select a schedule for this profile to run.
    
    * Select **Prior to Connection and**, then select an interval to check the device periodically after a successful connection.
    * Select **Prior to Connection Only** if you only want to check the security posture before allowing a connection to applications or organization resources.

1. 

## 


## 