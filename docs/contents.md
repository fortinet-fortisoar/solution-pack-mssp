| [Home](https://github.com/fortinet-fortisoar/solution-pack-multi-tenancy/blob/develop/README.md) |
|--------------------------------------------------------------------------------------------------|

# Contents

## Dashboards

- MSSP Overview
- Tenant Overview

## Reports
- Tenant Overdue Alerts Activities
- Tenant Overdue Incidents Activities
- Tenant Weekly Alert Report
- Tenant Weekly Incident Report

## Playbook Collection

|04 - Actions (Remote)|
|:--------------------|

| Playbook Name                                       | Description                                                                                                                            |
|:----------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------|
| Alias Mapping                                       | Map alias with remote actions playbooks                                                                                                |
| Alias Mapping - Update Playbook                     | This is a subroutine playbook to update the playbook with alias                                                                        |
| Enable Remote Execution Flag                        | Enable remote execution flag on all tenant actions playbooks                                                                           |
| Remote Action - Domain - Block (Indicator)          | Blocks the indicators of type 'Domain' on the firewall and marks the indicator as "Blocked" based on its block status on tenant.       |
| Remote Action - Domain - Unblock (Indicator)        | Unblocks the indicators of type 'Domain' on the firewall and marks the indicator as "Unblocked" based on its block status on tenant.   |
| Remote Action - Email Address - Block (Indicator)   | Blocks the indicators of type 'Email Address' on the firewall and marks indicator as "Blocked" based on its block status on Tenant.    |
| Remote Action - Email Address - Unblock (Indicator) | Unblocks the indicators of type 'Email Address' on the firewall and mark indicator as "Unblocked" based on its block status on Tenant. |
| Remote Action - File - Block (Indicator)            | Blocks the indicators of type 'File' on the firewall and marks the indicator as "Blocked" based on its block status on Tenant.         |
| Remote Action - File MD5 - Block (Indicator)        | Blocks the indicators of type 'Filehash' on the firewall and marks the indicator as "Blocked" based on its block status on Tenant.     |
| Remote Action - File MD5- Unblock (Indicator)       | Unblocks the indicators of type 'Filehash' on the firewall and marks the indicator as "Unblocked" based on its block status on Tenant. |
| Remote Action - File - Unblock (Indicator)          | Unblocks the indicators of type 'File' on the firewall and marks the indicator as "Unblocked" based on its block status on Tenant.     |
| Remote Action - Host - Block (Indicator)            | Blocks indicators of type 'Host' on the firewall and marks the indicator as "Blocked" based on its block status on Tenant.             |
| Remote Action - Host - Isolate Host                 | Isolates indicators of type 'Host' and marks the indicator as "Isolated" based on its block status on Tenant.                          |
| Remote Action - Host - Unblock (Indicator)          | Unblocks indicators of type 'Host' on the firewall and marks the indicators as "Unblocked" based on their block status on Tenant.      |
| Remote Action - IP Address - Block (Indicator)      | Blocks indicators of type 'IP Address' on the firewall and marks the indicators as "Blocked" based on their block status on Tenant.    |
| Remote Action - IP Address - Unblock (Indicator)    | Unblocks indicators of type 'IP Address' on the firewall and marks the indicator as "Unblocked" based on their block status on Tenant. |
| Remote Action - URL - Block (Indicator)             | Blocks indicators of type 'URL' on the firewall and marks the indicators as "Blocked" based on their block status on Tenant.           |
| Remote Action - URL - Unblock (Indicator)           | Unblocks indicators of type 'URL' on the firewall and marks the indicators as "Unblocked" based on their block status on Tenant.       |
