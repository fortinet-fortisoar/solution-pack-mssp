# Multi Tenancy Addons Solution Pack

## Release Information

- Solution Pack Version: 1.0.1
- Minimum Compatible FortiSOAR™ Version: 7.2.0
- Authored By: Fortinet
- Certified: Yes

## Overview

### Introduction

The FortiSOAR™ Multi Tenancy Addons Solution Pack (solution-pack-multi-tenancy) for Managed Security Service Providers (MSSPs). This solution pack enables users to experience the power and capability of FortiSOAR™ incident response in a multi-tenant architecture.

This solution pack provides a template of mitigation playbooks that can are agnostic of underneath tenants. You can configure these remotely executable playbooks to execute mitigation actions on the tenants from the master node. For example, if you require to block a domain on a tenant node from the master node, then you can use the remote executable playbooks that are part of this solution pack to achieve this action.

To use the remote executable playbooks, enable the Remote Execution Flag on the tenant node. This adds "Playbook Mappings" in the "Remote Tenant Manager" tab under the "Multitenancy Section" on the master node, and then Map Aliases of remote actions playbooks on the master node.

### Usage

More information about usage/Configuring of Multi Tenancy Addons Solution Pack [here](https://github.com/fortinet-fortisoar/solution-pack-multi-tenancy/blob/develop/docs/solution-pack-guide.md).

## Prerequisites

|**Solution Pack Name**|**Purpose**|**Doc Link**|
| :- | :- | :- |
|SOAR Framework 1.0.0|Require for Incident Response modules|[Click here](https://github.com/fortinet-fortisoar/solution-pack-soar-framework/blob/develop/README.md)|

  **Important**: You must install Multi Tenancy Addons solution pack on both the 'Master' and the 'Tenant' nodes.

## Contents

1. Dashboards (s)
    - MSSP Overview
    - Tenant Overview
2. Report(s)
    - Tenant Overdue Alerts Activities
    - Tenant Overdue Incidents Activities
    - Tenant Weekly Alert Report
    - Tenant Weekly Incident Report
3. Playbook Collection(s)
    - 04 - Actions (Remote) (18): You can use the playbooks in the 04-Actions (Remote) collection to perform various operations or actions such as blocking or unblocking domains, URLs, hosts, etc on remote tenant.

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
    |17|Remote Action - URL - Block (Indicator)|Blocks indicators of type 'URL' on the firewall and marks the indicators as "Blocked" based on their block status on Tenant.|
    |18|Remote Action - URL - Unblock (Indicator)|Unblocks indicators of type 'URL' on the firewall and marks the indicators as "Unblocked" based on their block status on Tenant.|
