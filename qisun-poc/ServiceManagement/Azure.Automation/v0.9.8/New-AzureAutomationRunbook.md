---
external help file: Microsoft.Azure.Commands.Automation.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=397908
schema: 2.0.0
ms.assetid: 94F81587-D376-4499-B61A-7BEE999D7FBF
updated_at: 10/19/2016 3:33 AM
ms.date: 10/19/2016
content_git_url: https://github.com/SummerSun/azure-docs-powershell-int/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v0.9.8/New-AzureAutomationRunbook.md
gitcommit: https://github.com/SummerSun/azure-docs-powershell-int/blob/c0d1e448da01261236e9ece01ca5c2a98effbf31/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v0.9.8/New-AzureAutomationRunbook.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureAutomationRunbook

## SYNOPSIS
Creates a new runbook.

## SYNTAX

### ByRunbookName (Default)
```
New-AzureAutomationRunbook [-Name] <String> [-Description <String>] [-Tags <String[]>]
 [-AutomationAccountName] <String> [-Profile <AzureProfile>] [<CommonParameters>]
```

### ByPath
```
New-AzureAutomationRunbook [-Path] <String> [-Description <String>] [-Tags <String[]>]
 [-AutomationAccountName] <String> [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureAutomationRunbook** cmdlet creates a new, empty Microsoft Azure Automation runbook.
Specify a name to create a new runbook.

You can also specify the path to a Windows PowerShell ‚Â® script (.ps1 ) file to import a runbook.
The script to import must contain a single Windows PowerShell ‚Â® Workflow definition.
The name of this Windows PowerShell Workflow becomes the name of the runbook.

## EXAMPLES

### Example 1: Create a runbook
```
PS C:\> New-AzureAutomationRunbook -AutomationAccountName "Contoso17" -Name "Runbook02"
```

This command creates a new runbook named Runbook02 in the Azure Automation account named Contoso17.

## PARAMETERS

### -AutomationAccountName
@{Text=}

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

### -Description
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name for the runbook.

```yaml
Type: String
Parameter Sets: ByRunbookName
Aliases: RunbookName

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Path
@{Text=}

```yaml
Type: String
Parameter Sets: ByPath
Aliases: RunbookPath

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Tags
@{Text=}

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Tag

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
In-memory profile.```yaml
Type: AzureProfile
Parameter Sets: (All)
Aliases: 

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

### Microsoft.Azure.Commands.Automation.Model.Runbook

## NOTES

## RELATED LINKS

[Get-AzureAutomationRunbook](..\..\..\..\ResourceManager\AzureRM.Automation\v0.9.8\CmdletMDs\Get-AzureAutomationRunbook.md)

[Publish-AzureAutomationRunbook](..\..\..\..\ResourceManager\AzureRM.Automation\v0.9.8\CmdletMDs\Publish-AzureAutomationRunbook.md)

[Remove-AzureAutomationRunbook](..\..\..\..\ResourceManager\AzureRM.Automation\v0.9.8\CmdletMDs\Remove-AzureAutomationRunbook.md)

[Set-AzureAutomationRunbook](..\..\..\..\ResourceManager\AzureRM.Automation\v0.9.8\CmdletMDs\Set-AzureAutomationRunbook.md)

[Start-AzureAutomationRunbook](..\..\..\..\ResourceManager\AzureRM.Automation\v0.9.8\CmdletMDs\Start-AzureAutomationRunbook.md)

