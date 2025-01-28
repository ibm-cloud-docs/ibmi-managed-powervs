---
copyright:
  years: 2024, 2025
lastupdated: "2025-01-28"

subcollection: ibmi-managed-powervs
---

{{site.data.keyword.attribute-definition-list}}

# Managing Access
{: #access}


Access to IBM i Managed on PowerVS instances for users is controlled by IBM Cloud Identity and Access Management (IAM). Privileged Access Management (PAM) and Multi-Factor Authentication is also provided by the offering to manage access within an IBM i server.

## IBM Cloud IAM
{: #cloud-iam}

IBM Cloud IAM provides two types of roles: 

* [**Platform management roles**](/docs/account?topic=account-userroles#platformroles) allow varying levels of permissions for performing platform actions within the account such as creating, deleting, editing, and viewing service instances. 

* [**Service management roles**](/docs/account?topic=account-userroles#service_access_roles) enable user access to APIs and features WITHIN a provisioned service instance.


### Platform management roles
{: #platform-roles}

In order to create an IBM i Managed on PowerVS instance from the IBM Cloud Catalog, view the details of a provisioned instance, update the configuration, and/or delete an existing instance, a user must be assigned to the required platform management role. Review the following table which outlines the different types of roles and the task(s) they allow.


| Platform role | Description of actions                                                                                                                |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| Viewer        | Can view service instances, but can't modify them.                                                                            |
| Operator      | Perform platform actions that are required to configure and operate service instances, such as viewing a service dashboard.   |
| Editor        | Perform all platform actions except for managing the account and assigning access policies.                                   |
| Administrator | Perform all platform actions based on the resource this role is assigned, including assigning access policies to other users. |
{: caption="Platform management roles for service" caption-side="bottom"}


### Service management roles
{: #service-roles}

Service management roles are NOT applicable to IBM i Managed on PowerVS. 
{: note}

The actions a user may peprform within an IBM i instance (i.e. after logging into the system) is managed by the [IBM i OS](https://www.ibm.com/docs/en/i/7.5?topic=reference-designing-security) and not via IBM Cloud IAM. There are different options for how user profiles will be maintained (i.e. leveraging an existing SSO solution, existing IAM team within your enterprise, etc), and will be covered as part of the onboarding process.



## Privileged Access Management 
{: #pam}

The ensure the security of the environment, user profiles within the IBM i OS will not have privileged rights directly assigned to them.  However, Privileged Access Management (PAM) is part of the base offering and is used to allow specified users to gain privileged access to run certain commands (via swap profile). To request the creation of a PAM Profile and/or to add or remove users to a profile, a [support case](/docs/ibmi-managed-powervs?topic=ibmi-managed-powervs-getting-support) needs to be created. When opening a support case, please include the following information:

* LPAR/Server name(s) this applies to
* Original profile name and the privileged profile to switch to
* Specify if this should be allowed 24x7 or only during certain time periods


## Multi-Factor Authentication 
{: #mfa}

As an additional level of security, multi-factor authentication is an [optional add-on](/docs/ibmi-managed-powervs?topic=ibmi-managed-powervs-overview#offering-optional) of this offering which may be used when a user logins to a server and/or performs a swap profile to gain privileged access.

To request changes to your MFA configuration (i.e. enabling a user for MFA), a [support case](/docs/ibmi-managed-powervs?topic=ibmi-managed-powervs-getting-support) needs to be created. When opening a support case, please include the following information:

* LPAR/Server name(s) this applies to
* User full name
* Email address
* IBM i profile name
* When to enable MFA (options: user login, profile swap)
