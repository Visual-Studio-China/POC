---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 2F1DA4E0-4D7C-4726-85AA-2493B0A3FDA8
updated_at: 10/19/2016 3:31 AM
ms.date: 10/19/2016
content_git_url: https://github.com/SummerSun/azure-docs-powershell-azuread-int/blob/master/Azure%20AD%20Cmdlets/AzureADPreview/v2.0.0/Remove-AzureADGroupOwner.md
gitcommit: https://github.com/SummerSun/azure-docs-powershell-azuread-int/blob/6a895a73e21f1df9572197497237f3a825ebd518/Azure%20AD%20Cmdlets/AzureADPreview/v2.0.0/Remove-AzureADGroupOwner.md
ms.topic: reference
ms.prod: powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
open_to_public_contributors: false
ms.service: Azure PowerShell
---

# Remove-AzureADGroupOwner

## SYNOPSIS
Removes an owner from a group.

## SYNTAX

```
Remove-AzureADGroupOwner -ObjectId <String> -OwnerId <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
PS C:\>Remove-AzureADGroupOwner -ObjectId 62438306-7c37-4638-a72d-0ee8d9217680 -OwnerId 0a1068c0-dbb6-4537-9db3-b48f3e31dd76
```

## PARAMETERS

### -ObjectId
The unique identifier of a group in Azure Active Directory (ObjectId)

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -OwnerId
The unique identifier of the object specific Azure Active Directory object

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
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


