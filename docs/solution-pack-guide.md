# Configuring Multi Tenancy Addons Solution Pack

1. Enable the remote execution flag for all the playbooks in *04-Actions (Remote)* collection on the Tenant systems by executing the **Enable Remote Execution Flag(Tenant Only)** playbook as follows:
    1. Open the FortiSOAR Tenant instance, and from the navigation panel, click the **Alerts** module.
    2. Click **Execute** and then select **Enable Remote Execution Flag (Tenant Only)**.  
       **Important**: Before you execute the "Enable Remote Execution Flag (Tenant Only)" playbook, ensure that there is no **Playbook Mappings** in **Remote Tenant Manager** under **Multitenancy Section** on the Master node.
        ![Remote Tenant Manager](media/remoteTenantMngr.png)  
    3. After the **Enable Remote Execution Flag (Tenant Only)** playbook is executed, **Playbook Mappings** is added in **Remote Tenant Manager** under **Multitenancy Section** on the Master node.  
        ![Manage Playbook Mapping](media/managePbMappings.png)

2. Map Aliases of remote actions playbooks on the Master node by executing the **Remote Alias Mapping (Master)** playbook as follows:
    1. From the navigation panel,click the **Alerts** module.
    2. Click **Execute** and then select **Remote Alias Mapping (Master Only)**.

3. Disable SLA Playbooks from the *"06 - IRP - Case Management"* collection on the Tenant (*SLA* keyword). This is required because, SLA operations on all records, i.e. records of Master or Tenant, get performed on the Master.
    ![Disabling SLA Playbooks](media/disableSLAPbs.png)

4. Define Tenant SLA by adding SLA records for the Tenant in the **SLA Templates** module on the Master instance.  
   ![Adding SLA Templates](media/addSLATemplates.png)
