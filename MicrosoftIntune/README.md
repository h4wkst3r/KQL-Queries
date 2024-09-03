# Microsoft Intune KQL Queries

The KQL queries in this folder can be used as part of threat hunting rules or scheduled analytic rules within Microsoft Sentinel.

## User created PowerShell script or Windows application

`CreatedPSScriptOrWindowsApp.kql`

This query will show when a new application or PowerShell script has been created in Microsoft Intune.

## User created and deleted PowerShell script

`CreatedAndDeletedPSScript.kql`

This query will show when a user has created and then deleted a PowerShell script in Intune within a 24 hour period. This can be evident of misuse or abuse by a threat actor to cover their tracks.

## User created and deleted Windows application

`CreatedAndDeletedWindowsApp.kql`

This query will show when a user has created and then deleted a Windows app in Intune within a 24 hour period. This can be evident of misuse or abuse by a threat actor to cover their tracks.

## User created PowerShell script or Windows application and forced a device restart

`CreatedPSScriptOrWindowsAppForcedRestart.kql`

This query will show when a user has created a PowerShell script or Windows app in Intune, and has also initiated a device restart for a device within 24 hours. This can be evident of misuse or abuse by a threat actor to force a device to run a script or application.

## User created PowerShell script or Windows application and forced a device sync

`CreatedPSScriptOrWindowsAppForcedSync.kql`

This query will show when a user has created a PowerShell script or Windows app in Intune, and has also initiated a device sync for a device within 24 hours. This can be evident of misuse or abuse by a threat actor to force a device to run a script or application.
