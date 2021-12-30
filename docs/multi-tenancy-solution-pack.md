# FortiSOAR Multi Tenancy Solution Pack – Out-of-the box Playbooks Collections

The FortiSOAR™ Incident Response Solution Pack (solution-pack-multi-tenancy) for Managed Security Service Providers (MSSPs). This solution pack enables users to experience the power and capability of FortiSOAR™ incident response in a multi-tenant architecture. 
This article provides a listing and brief description of the various types of playbook collections included in the Solution Pack. You can use the playbooks to perform various operations used to automate security processes across your organization.

## Remote Actions Playbook Collection

You can use the playbooks in the 05-Actions (Remote) collection to perform various operations or actions such as blocking or unblocking domains, URLs, hosts, etc on remote tenant.

Following is a table that lists the playbooks that are a part of the “05-Actions (Remote)” collection in the Solution Pack:

|**SN**|**Playbook Name**|**Description**|
| :- | :- | :- |
|1|Alias Mapping|Map alias with remote actions playbooks|
|2|Alias Mapping - Update Playbook|This is a subroutine playbook to update the playbook with alias|
|3|Enable Remote Execution Flag|Enable remote execution flag on all tenant actions playbooks|
|4|Remote Action - Domain - Block (Indicator)|Blocks the indicators of type 'Domain' on the firewall and marks the indicator as "Blocked" based on its block status on tenant.|
|5|Remote Action - Domain - Unblock (Indicator)|Unblocks the indicators of type 'Domain' on the firewall and marks the indicator as "Unblocked" based on its block status on tenant.|
|6|Remote Action - Email Address - Block (Indicator)|Blocks the indicators of type 'Email Address' on the firewall and marks indicator as "Blocked" based on its block status on Tenant.|
|7|Remote Action - Email Address - Unblock (Indicator)|Unblocks the indicators of type 'Email Address' on the firewall and mark indicator as "Unblocked" based on its block status on Tenant.|
|8|Remote Action - File - Block (Indicator)|Blocks the indicators of type 'File' on the firewall and marks the indicator as "Blocked" based on its block status on Tenant.|
|9|Remote Action - File MD5 - Block (Indicator)|Blocks the indicators of type 'Filehash' on the firewall and marks the indicator as "Blocked" based on its block status on Tenant.|
|10|Remote Action - File MD5- Unblock (Indicator)|Unblocks the indicators of type 'Filehash' on the firewall and marks the indicator as "Unblocked" based on its block status on Tenant.|
|11|Remote Action - File - Unblock (Indicator)|Unblocks the indicators of type 'File' on the firewall and marks the indicator as "Unblocked" based on its block status on Tenant.|
|12|Remote Action - Host - Block (Indicator)|Blocks indicators of type 'Host' on the firewall and marks the indicator as "Blocked" based on its block status on Tenant.|
|13|Remote Action - Host - Isolate Host|Isolates indicators of type 'Host' and marks the indicator as "Isolated" based on its block status on Tenant.|
|14|Remote Action - Host - Unblock (Indicator)|Unblocks indicators of type 'Host' on the firewall and marks the indicators as "Unblocked" based on their block status on Tenant.|
|15|Remote Action - IP Address - Block (Indicator)|Blocks indicators of type 'IP Address' on the firewall and marks the indicators as "Blocked" based on their block status on Tenant.|
|16|Remote Action - IP Address - Unblock (Indicator)|Unblocks indicators of type 'IP Address' on the firewall and marks the indicator as "Unblocked" based on their block status on Tenant.|
|17|Remote Action - URL - Block (Indicator)|Blocks indicators of type ‘URL’ on the firewall and marks the indicators as “Blocked” based on their block status on Tenant.|
|` `18|Remote Action - URL - Unblock (Indicator)|Unblocks indicators of type 'URL' on the firewall and marks the indicators as "Unblocked" based on their block status on Tenant.|

