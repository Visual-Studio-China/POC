---
external help file: Microsoft.Azure.Commands.TrafficManager.dll-Help.xml
online version: .\Disable-AzureRmTrafficManagerProfile.md
schema: 2.0.0
ms.assetid: F2233F68-3DF3-4E2E-9626-1ED063FC6C92
updated_at: 10/19/2016 3:33 AM
ms.date: 10/19/2016
content_git_url: https://github.com/SummerSun/azure-docs-powershell-int/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.TrafficManager/v1.0/Enable-AzureRmTrafficManagerProfile.md
gitcommit: https://github.com/SummerSun/azure-docs-powershell-int/blob/c0d1e448da01261236e9ece01ca5c2a98effbf31/azureps-cmdlets-docs/ResourceManager/AzureRM.TrafficManager/v1.0/Enable-AzureRmTrafficManagerProfile.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
---

# Enable-AzureRmTrafficManagerProfile

## SYNOPSIS
Enables a Traffic Manager profile.

## SYNTAX

### Fields
```
Enable-AzureRmTrafficManagerProfile -Name <String> -ResourceGroupName <String> [<CommonParameters>]
```

### Object
```
Enable-AzureRmTrafficManagerProfile -TrafficManagerProfile <TrafficManagerProfile> [<CommonParameters>]
```

## DESCRIPTION
The **Enable-AzureRmTrafficManagerProfile** cmdlet enables an azure_2 Traffic Manager profile.
You can specify the profile object by using the pipeline or as a parameter value.
Alternatively, you can specify the profile by using the *Name* and *ResourceGroupName* parameters.

## EXAMPLES

### Example 1: Enable a profile specified by name
```
PS C:\>Enable-AzureRmTrafficManagerProfile -Name "ContosoProfile" -ResourceGroupName "ResourceGroup11"
```

This command enables the profile named ContosoProfile in ResourceGroup11.

### Example 2: Enable a profile by using the pipeline
```
PS C:\>Get-AzureRmTrafficManagerProfile -Name "ContosoProfile" -ResourceGroupName "ResourceGroup11" | Enable-AzureRmTrafficManagerProfile
```

This command gets the profile named ContosoProfile in ResourceGroup11.
The command then passes that profile to the **Enable-AzureRmTrafficManagerProfile** cmdlet by using the pipeline operator.
That cmdlet enables that profile.

## PARAMETERS

### -Name
Specifies the name of the Traffic Manager profile that this cmdlet enables.

```yaml
Type: String
Parameter Sets: Fields
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of a resource group.
This cmdlet enables a Traffic Manager profile in the group that this parameter specifies.

```yaml
Type: String
Parameter Sets: Fields
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TrafficManagerProfile
Specifies a **TrafficManagerProfile** object to enable.
To obtain a **TrafficManagerProfile** object, use the Get-AzureRmTrafficManagerProfile cmdlet.

```yaml
Type: TrafficManagerProfile
Parameter Sets: Object
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.Commands.Network.TrafficManagerProfile
This cmdlet accepts a **TrafficManagerProfile** object.

## OUTPUTS

## NOTES

## RELATED LINKS

[Disable-AzureRmTrafficManagerProfile](.\Disable-AzureRmTrafficManagerProfile.md)

[Get-AzureRmTrafficManagerProfile](.\Get-AzureRmTrafficManagerProfile.md)

[New-AzureRmTrafficManagerProfile](.\New-AzureRmTrafficManagerProfile.md)

[Remove-AzureRmTrafficManagerProfile](.\Remove-AzureRmTrafficManagerProfile.md)

[Set-AzureRmTrafficManagerProfile](.\Set-AzureRmTrafficManagerProfile.md)

