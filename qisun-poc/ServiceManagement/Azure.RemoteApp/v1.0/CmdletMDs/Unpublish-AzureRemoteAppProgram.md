---
external help file: Microsoft.WindowsAzure.Commands.RemoteApp.dll-Help.xml
online version: .\Get-AzureRemoteAppProgram.md
schema: 2.0.0
content_git_url: https://github.com/SummerSun/azure-docs-powershell-int/projects/azure-docs-powershell-int/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v1.0/CmdletMDs/Unpublish-AzureRemoteAppProgram.md
gitcommit: https://github.com/SummerSun/azure-docs-powershell-int/projects/azure-docs-powershell-int/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v1.0/CmdletMDs/Unpublish-AzureRemoteAppProgram.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, content
manager: visual-studio-china
---

# Unpublish-AzureRemoteAppProgram

## SYNOPSIS
Unpublishes an azure_2 RemoteApp program.

## SYNTAX

```
Unpublish-AzureRemoteAppProgram [-CollectionName] <String> [[-Alias] <String[]>] [-Profile <AzureSMProfile>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Unpublish-AzureRemoteAppProgram** cmdlet unpublishes an azure_2 RemoteApp program.
After you unpublish a program, it is no longer available to the users of an azure_2 RemoteApp collection.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -Alias
Specifies an array of aliases of the programs to unpublish.
Use Get-AzureRemoteAppProgram to retrieve the alias of a program to unpublish.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -CollectionName
Specifies the name of the azure_2 RemoteApp collection.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Name

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Confirm
psdx_confirmdesc

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
psdx_whatifdesc

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRemoteAppProgram](.\Get-AzureRemoteAppProgram.md)

[Publish-AzureRemoteAppProgram](.\Publish-AzureRemoteAppProgram.md)
