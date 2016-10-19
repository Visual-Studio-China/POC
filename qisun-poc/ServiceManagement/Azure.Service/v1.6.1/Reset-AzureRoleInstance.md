---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: .\Set-AzureRole.md
schema: 2.0.0
ms.assetid: 688BE4C0-0390-4DB2-97B7-81E05E8D796B
updated_at: 10/19/2016 3:33 AM
ms.date: 10/19/2016
content_git_url: https://github.com/SummerSun/azure-docs-powershell-int/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/Reset-AzureRoleInstance.md
gitcommit: https://github.com/SummerSun/azure-docs-powershell-int/blob/c0d1e448da01261236e9ece01ca5c2a98effbf31/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/Reset-AzureRoleInstance.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Reset-AzureRoleInstance

## SYNOPSIS
Requests a reboot or reimage of a single role instance or all role instances of a specific role.

## SYNTAX

```
Reset-AzureRoleInstance [-ServiceName] <String> -Slot <String> -InstanceName <String> [-Reboot] [-Reimage]
 [-Profile <AzureSMProfile>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Reset-AzureRoleInstance** cmdlet requests a reboot or a reimage of a role instance that is running in a deployment.
This operation executes synchronously.
When you reboot a role instance, azure_2 takes the instance offline, restarts the underlying operating system for that instance, and brings the instance back online.
Any data that is written to the local disk persists across reboots.
Any data that is in-memory is lost.

Reimaging a role instance results in different behavior depending on the type of role.
For a web or worker role, when the role is reimaged, azure_2 takes the role offline and writes a fresh installation of the azure_2 guest operating system to the virtual machine.
The role is then brought back online.
For a VM role, when the role is reimaged, azure_2 takes the role offline, reapplies the custom image that you provided for it, and brings the role back online.

azure_2 attempts to maintain data in any local storage resources when the role is reimaged; however, in case of a transient hardware failure, the local storage resource may be lost.
If your application requires that data persist, writing to a durable data source, such as an azure_2 drive, is recommended.
Any data that is written to a local directory other than that defined by the local storage resource will be lost when the role is reimaged.

## EXAMPLES

### Example 1: Reboot a role instance
```
PS C:\>ReSet-AzureRoleInstance -ServiceName "MySvc01" -Slot "Staging" -InstanceName "MyWebRole_IN_0" -Reboot
```

This command reboots the role instance named MyWebRole_IN_0 in the staging deployment of the MySvc01 service.

### Example 2: Reimage a role instance
```
PS C:\>ReSet-AzureRoleInstance -ServiceName "MySvc01" -Slot "Staging" -Reimage
```

This command reimages the role instances in the staging deployment of the MySvc01 cloud service.

### Example 3: Reimage all role instances
```
PS C:\>ReSet-AzureRoleInstance -ServiceName "MySvc1" -Slot "Production" -Reimage
```

This command reimages all role instances in the production deployment of the MySvc01 service.

## PARAMETERS

### -ServiceName
Specifies the name of the service.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Slot
Specifies the deployment environment where the role instances run.
Valid values are: Production and Staging.
You can include either the *DeploymentName* or *Slot* parameter, but not both.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InstanceName
Specifies the name of the role instance to reimage or reboot.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Reboot
Specifies that this cmdlet reboots the specified role instance or, if none is specified, all role instances.
You must include either a *Reboot* or *Reimage* parameter, but not both.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Reimage
Specifies that this cmdlet reimages the specified role instance or, if none is specified, all role instances.
You must include either a *Reboot* or *Reimage* parameter, but not both.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
ps_azureprofile_description

```yaml
Type: AzureSMProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
@{Text=}```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
@{Text=}```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Set-AzureRole](.\Set-AzureRole.md)

