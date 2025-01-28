---
copyright:
  years: 2024, 2024
lastupdated: "2024-10-20"

subcollection: ibmi-managed-powervs
---

{{site.data.keyword.attribute-definition-list}}

# Provisioning
{: #provisioning}


## Provisoning through the IBM Cloud Catalog
{: #provisioning-through-ibm-cloud-catalog}

IBM i Managed on PowerVS instance(s) may be provisioned from the [IBM Cloud Catalog](https://test.cloud.ibm.com/catalog/services/managed-powervs). Plan and instance configuration parameters will need to be sepcified.


### Plan selection
{: #plan-selection}

IBM i Managed on PowerVS offers two plans:

1. **IBM i Managed**: Provides one virtual server instance with the IBM i operating system (OS) and associated networking.
2.  **IBM i Managed with HA**: Provides two virtual server instances with the IBM i operating system (OS) and associated networking. This plan provides high availability within the same region through the user of PowerHA.

A base management fee/component is required and is needed to support all instances regardless of the number of instances or plan types.
{: tip}

### Configure the instance
{: #resource-configuration}
 
Specify configuration values for the instance:

- **Service name**: The name can be any string and is the name that is used to identify the new deployment.
- **Resource group**: If you are organizing your services into [resource groups](https://cloud.ibm.com/docs/account?topic=account-account_setup), specify the resource group in this field. Otherwise, you can leave it as Default. For more information, see [Managing resource groups](https://cloud.ibm.com/docs/account?topic=account-rgs).
- **Additional Comments**: Provide any additional details or comments you would like shared with the provisioning team.

Select from a list of optional services if desired:
- **Disaster Recovery Environment**: Select if you would like the IBM i instance to be configured to replicate data to another IBM i instance (located in another region).
- **Multi-Factor Authentication**: Allows for additional authentication method when logging into an IBM i instance.
- **Network/Connectivity**: This service provides management of network connectivity to on-prem via private Direct Links.
- **FalconStor Backup**: Enhances backup operation by using FalconStor Backup.



After you select the appropriate settings, click **Create** to start the provisoning process. 
