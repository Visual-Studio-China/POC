---
external help file: Microsoft.Azure.Commands.ResourceManager.Automation.dll-Help.xml
online version: .\Get-AzureRmAutomationAccount.md
schema: 2.0.0
ms.assetid: 3CE8492B-FB2E-43EB-A4F0-770A33E5A19E
updated_at: 10/19/2016 3:33 AM
ms.date: 10/19/2016
content_git_url: https://github.com/SummerSun/azure-docs-powershell-int/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v2.1.0/Get-AzureRmAutomationRegistrationInfo.md
gitcommit: https://github.com/SummerSun/azure-docs-powershell-int/blob/c0d1e448da01261236e9ece01ca5c2a98effbf31/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v2.1.0/Get-AzureRmAutomationRegistrationInfo.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
---

# Get-AzureRmAutomationRegistrationInfo

## SYNOPSIS
Gets registration information for onboarding a DSC node or hybrid worker to Automation.

## SYNTAX

```
Get-AzureRmAutomationRegistrationInfo [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmAutomationRegistrationInfo** cmdlet gets the endpoint and keys required to onboard a Desired State Configuration (DSC) node or hybrid worker into an Azure Automation account.

## EXAMPLES

### Example 1: Get registration information
```
PS C:\>Get-AzureRmAutomationRegistrationInfo -ResourceGroup "ResourceGroup01" -AutomationAccountName "AutomationAccount01"
```

This command gets the registration information for the Automation account named AutomationAccount01 in the Resource Group named ResourceGroup01.

## PARAMETERS

### -AutomationAccountName
Specifies the name of Automation account for which this cmdlet gets registration information.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of a resource group.
This cmdlet gets registration information for the resource group that this parameter specifies.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmAutomationAccount](.\Get-AzureRmAutomationAccount.md)

[Get-AzureRmAutomationDscNode](.\Get-AzureRmAutomationDscNode.md)

[New-AzureRmAutomationKey](.\New-AzureRmAutomationKey.md)

