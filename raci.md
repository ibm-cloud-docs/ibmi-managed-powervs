---
copyright:
  years: 2024, 2024
lastupdated: "2024-10-28"

subcollection: ibmi-managed-powervs
---

{{site.data.keyword.attribute-definition-list}}

# Roles and Responsibilities
{: #responsibilities}


In this section, learn about the responsibilities and terms and conditions that you have when you use IBM i Managed on PowerVS. The table below provides a list of operation management tasks and specific responsibilities for you and for IBM.

For a high-level view of the service types in IBM Cloud and the breakdown of responsibilities between the client and IBM for each type, see [Shared responsibilities for IBM Cloud offerings](/docs/overview?topic=overview-shared-responsibilities). For overall terms of use, see [IBM Cloud Terms and Notices](/docs/overview/terms-of-use?topic=overview-terms).




## Operations Management
{: #ops-mgmt-responsibilities}

| Task                                | IBM Responsibilities  | Your responsibilities |
| ------------------------------------| --------------------- | --------------------- |
| Updates/Patching | Apply fixes and updates (Cum, Group, and Hiper PTFs) to the IBM i operating system. | Apply updates to your applications and data. |
| Monitoring  | Monitor and resolve issues affecting availabilty of IBM i LPAR, including network connectivity.| Monitor application related messages in message queue. |
| Performance and Capacity Management | Monitor system health (CPU, Memory, Storage) and provide recommendations for improvement.  | Request appropiate sizing of CPU, disk, and memory to support application.<br><br>Application level performance tuning. |
| Security | Manage secure posture of environment which includes vulnerability scanning, integration with SIEM, and monitoring by SOC Team.<br><br>Privilege Access Management (PAM) within the IBM i environment for when users need to run privileged commands. | Secure application layer access.<br><br>Open a support ticket to associate an IBM i user profile with a PAM profile or to request PAM profile configuration changes.|
| Network Connectivity | Manage network connectivity and firewalls within the IBM Cloud, including IBM Cloud Direct Links. | Establish connectivity from on-prem to the IBM Cloud and maintain on-prem edge device firewall. |
| Backup and Restore | Responsible for automatic daily backups of IBM i LPARs, as well as monitoring the state of client backups. | Open a support ticket when backups need to be restored or when adhoc on-demand backups need to be performed. |
| Disaster Recovery (Optional Add-on) | Configure and manage replication of data from primary LPAR to DR LPAR (i.e. using Mimix). | BCDR planning and declaration of when a DR failover event needs to occur.<br><br>Perform application layer configuration and validate application failover is successful. |
{: caption="Operation responsibilities" caption-side="top"}
