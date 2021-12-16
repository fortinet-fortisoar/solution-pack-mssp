# Multi-tenancy Incident Response Solution Pack 7.0.2

## Overview

This article describes the FortiSOAR™ Incident Response Solution Pack (solution-pack-multi-tenancy) for Managed Security Service Providers (MSSPs). This solution pack enables users to experience the power and capability of FortiSOAR™ incident response in a multi-tenant architecture.

## Deploying MSSP IR Solution Pack

**Important**: Before you deploy the solution pack, ensure that you have deployed the FortiSOAR™ Incident Response Solution Pack ([solution-pack-incident-response](https://github.com/fortinet-fortisoar/solution-pack-incident-response)) and there are no records such as alerts, indicators, incidents, etc., in your FortiSOAR™ system.

1. Log onto the Solution Pack GIT repo ([https://github.com/fortinet-fortisoar/solution-pack-multi-tenancy](https://github.com/fortinet-fortisoar/solution-pack-multi-tenancy)) using your credentials.
2. Click the **Code** button and select the **Download ZIP** option.  
   ![Fortinet-FortiSOAR GIT branch > Code >Download the solution pack zip](media/MSSPSolutionPackZip.png)
3. Log into your FortiSOAR instance, and on the left-navigation, click **Import Wizard**.  
   ![Import Wizard](media/importWizard.png)
4. On the `Import Wizard` page, click **Import From File** and selected the solution pack zip that you have downloaded, and navigate through the Import Wizard.  
   ![Importing the IR Solution Pack zip file](media/importIRCP.png)  
    **Note**: It is recommended not the change any configurations or options of the imported solution pack zip file.  
   Once the import is successfully completed, you can use the MSSP IR solution pack.



Once you have completed installing the MSSP IR Solution Pack, you can choose to import other Solution Packs (using the same steps mentioned above) based on your requirements:

- [solution-pack-mitre-attack](https://github.com/fortinet-fortisoar/solution-pack-mitre-attack)
- [solution-pack-symantec-solutions](https://github.com/fortinet-fortisoar/solution-pack-symantec-solutions)
- [solution-pack-knowledge-base](https://github.com/fortinet-fortisoar/solution-pack-knowledge-base)
- [solution-pack-vulnerability-management](https://github.com/fortinet-fortisoar/solution-pack-vulnerability-management)
- [solution-pack-soc-simulator](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator)

## Configuring MSSP IR Solution Pack

1. Enable the remote execution flag for all the playbooks in *05-Actions (Remote)* collection on the Tenant systems by executing the “Enable Remote Execution Flag(Tenant Only)” playbook as follows:
    1. Open the FortiSOAR Tenant instance,and from the navigation panel, click the **Alerts** module.
    2. Click **Execute** and then select **Enable Remote Execution Flag (Tenant Only)**.  
       **Important**: Before you execute the “Enable Remote Execution Flag (Tenant Only)” playbook, ensure that there is no “Playbook Mappings” in “Remote Tenant Manager” under “Multitenancy Section” on the Master node.   
        ![Remote Tenant Manager](media/remoteTenantMngr.png)  
       After the “Enable Remote Execution Flag (Tenant Only)” playbook is executed, you will notice that “Playbook Mappings” is added in “Remote Tenant Manager” under “Multitenancy Section” on the Master node.  
        ![Manage Playbook Mapping](media/managePbMappings.png)

2. Map Aliases of remote actions playbooks on the Master node by executing the “Remote Alias Mapping (Master)” playbook as follows:
    1. From the navigation panel,click the **Alerts** module.
    2. Click **Execute** and then select **Remote Alias Mapping (Master Only)**.

3. Disable SLA Playbooks from the *08 - Case Management* collection on the Tenant (“SLA” keyword). This is required because, SLA operations on all records, i.e. records of Master or Tenant, get performed on the Master only.  

      ![Disabling SLA Playbooks](media/disbaleSLAPbs.png)

4. Define Tenant SLA by adding SLA records for the Tenant in the “SLA Templates” module on the Master.  
   ![Adding SLA Templates](media/addSLATemplates.png)