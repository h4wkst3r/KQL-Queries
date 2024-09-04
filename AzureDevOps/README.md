# Azure DevOps KQL Queries

The KQL queries in this folder can be used as part of threat hunting rules or scheduled analytic rules within Microsoft Sentinel.

## Persistence with ADOKit Detected

`ADOKitPersistence.kql`

This query will show when a PAT or SSH key has been created with [ADOKit](https://github.com/xforcered/ADOKit).

## ADOKit Usage Detected

`ADOKitUsage.kql`

This query will show when any auditable event is performed (e.g., adding user to group) with [ADOKit](https://github.com/xforcered/ADOKit).

## Azure DevOps Administrator Group Monitoring

`ADOAdminGroupAdditions.kql`

This is an update to [this Sentinel analytic rule logic](https://github.com/Azure/Azure-Sentinel/blob/master/Solutions/AzureDevOpsAuditing/Analytic%20Rules/AzDOAdminGroupAdditions.yaml). The update includes setting `MonitorAllProjects` to `true`, so that all projects are monitored for any additions to the `Project Administrators` group.

## Azure DevOps Personal Access Token (PAT) misuse

`ADOPATMisuse.kql`

This is an update to [this Sentinel analytic rule logic](https://github.com/Azure/Azure-Sentinel/blob/master/Solutions/AzureDevOpsAuditing/Analytic%20Rules/AzDOPatSessionMisuse.yaml). The update includes adding the authentication mechanism of `UserAuthToken`.

## Azure DevOps Persistence Technique Detected

`ADOPersistenceTechniqueDetected.kql`

This is a new KQL query to show when an SSH key or PAT has been created.

## New PA, PCA, or PCAS added to Azure DevOps

`NewPAPCAPCASaddedtoADO.kql`

This is an update to [this Sentinel analytic rule logic](https://github.com/Azure/Azure-Sentinel/blob/master/Solutions/AzureDevOpsAuditing/Analytic%20Rules/NewPAPCAPCASaddedtoADO.yaml). The update includes the addition of `Project Collection Build Administrators`, as well as fixing a bug in the detection when adding a user to the `Build Administrators` group.



